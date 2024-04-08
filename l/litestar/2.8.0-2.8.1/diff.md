# Comparing `tmp/litestar-2.8.0.tar.gz` & `tmp/litestar-2.8.1.tar.gz`

## Comparing `litestar-2.8.0.tar` & `litestar-2.8.1.tar`

### file list

```diff
@@ -1,713 +1,713 @@
--rw-r--r--   0        0        0     6672 2020-02-02 00:00:00.000000 litestar-2.8.0/Makefile
--rw-r--r--   0        0        0    19851 2020-02-02 00:00:00.000000 litestar-2.8.0/docs/PYPI_README.md
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/__init__.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/__main__.py
--rw-r--r--   0        0        0     6000 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_multipart.py
--rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_parsers.py
--rw-r--r--   0        0        0    39616 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/app.py
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/background_tasks.py
--rw-r--r--   0        0        0     3367 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/concurrency.py
--rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/constants.py
--rw-r--r--   0        0        0    11032 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/controller.py
--rw-r--r--   0        0        0    17681 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/data_extractors.py
--rw-r--r--   0        0        0     4282 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/di.py
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/enums.py
--rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/file_system.py
--rw-r--r--   0        0        0    11029 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/pagination.py
--rw-r--r--   0        0        0    15965 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/params.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/py.typed
--rw-r--r--   0        0        0    16702 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/router.py
--rw-r--r--   0        0        0     8973 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/status_codes.py
--rw-r--r--   0        0        0    25972 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/typing.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_asgi/__init__.py
--rw-r--r--   0        0        0     6526 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_asgi/asgi_router.py
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_asgi/utils.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_asgi/routing_trie/__init__.py
--rw-r--r--   0        0        0     8059 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_asgi/routing_trie/mapping.py
--rw-r--r--   0        0        0     5995 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_asgi/routing_trie/traversal.py
--rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_asgi/routing_trie/types.py
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_asgi/routing_trie/validate.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_kwargs/__init__.py
--rw-r--r--   0        0        0     3846 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_kwargs/cleanup.py
--rw-r--r--   0        0        0     4195 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_kwargs/dependencies.py
--rw-r--r--   0        0        0    16651 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_kwargs/extractors.py
--rw-r--r--   0        0        0    20472 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_kwargs/kwargs_model.py
--rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_kwargs/parameter_definition.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_layers/__init__.py
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_layers/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_openapi/__init__.py
--rw-r--r--   0        0        0     6577 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_openapi/datastructures.py
--rw-r--r--   0        0        0    10647 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_openapi/parameters.py
--rw-r--r--   0        0        0     6839 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_openapi/path_item.py
--rw-r--r--   0        0        0     7836 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_openapi/plugin.py
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_openapi/request_body.py
--rw-r--r--   0        0        0    13607 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_openapi/responses.py
--rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_openapi/utils.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_openapi/schema_generation/__init__.py
--rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_openapi/schema_generation/constrained_fields.py
--rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_openapi/schema_generation/examples.py
--rw-r--r--   0        0        0    25613 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_openapi/schema_generation/schema.py
--rw-r--r--   0        0        0     3842 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_openapi/schema_generation/utils.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_openapi/schema_generation/plugins/__init__.py
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_openapi/schema_generation/plugins/dataclass.py
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_openapi/schema_generation/plugins/pagination.py
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_openapi/schema_generation/plugins/struct.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_openapi/schema_generation/plugins/typed_dict.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_openapi/typescript_converter/__init__.py
--rw-r--r--   0        0        0    10909 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_openapi/typescript_converter/converter.py
--rw-r--r--   0        0        0     5212 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_openapi/typescript_converter/schema_parsing.py
--rw-r--r--   0        0        0     7664 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_openapi/typescript_converter/types.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_signature/__init__.py
--rw-r--r--   0        0        0    11710 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_signature/model.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_signature/types.py
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/_signature/utils.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/channels/__init__.py
--rw-r--r--   0        0        0    15848 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/channels/plugin.py
--rw-r--r--   0        0        0     4711 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/channels/subscriber.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/channels/backends/__init__.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/channels/backends/_redis_flushall_streams.lua
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/channels/backends/_redis_pubsub_publish.lua
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/channels/backends/_redis_xadd_expire.lua
--rw-r--r--   0        0        0     3435 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/channels/backends/asyncpg.py
--rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/channels/backends/base.py
--rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/channels/backends/memory.py
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/channels/backends/psycopg.py
--rw-r--r--   0        0        0    11422 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/channels/backends/redis.py
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/cli/__init__.py
--rw-r--r--   0        0        0    20230 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/cli/_utils.py
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/cli/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/cli/commands/__init__.py
--rw-r--r--   0        0        0    12215 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/cli/commands/core.py
--rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/cli/commands/schema.py
--rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/cli/commands/sessions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/config/__init__.py
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/config/allowed_hosts.py
--rw-r--r--   0        0        0    12477 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/config/app.py
--rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/config/compression.py
--rw-r--r--   0        0        0     5178 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/config/cors.py
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/config/csrf.py
--rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/config/response_cache.py
--rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/connection/__init__.py
--rw-r--r--   0        0        0    11536 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/connection/base.py
--rw-r--r--   0        0        0     9482 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/connection/request.py
--rw-r--r--   0        0        0    11331 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/connection/websocket.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/__init__.py
--rw-r--r--   0        0        0     3998 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/jinja.py
--rw-r--r--   0        0        0     5451 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/mako.py
--rw-r--r--   0        0        0     7831 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/minijinja.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/minijnja.py
--rw-r--r--   0        0        0     3839 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/piccolo.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/attrs/__init__.py
--rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/attrs/attrs_schema_plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/htmx/__init__.py
--rw-r--r--   0        0        0     4800 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/htmx/_utils.py
--rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/htmx/request.py
--rw-r--r--   0        0        0     6408 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/htmx/response.py
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/htmx/types.py
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/jwt/__init__.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/jwt/jwt_auth.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/jwt/jwt_token.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/jwt/middleware.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/opentelemetry/__init__.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/opentelemetry/_utils.py
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/opentelemetry/config.py
--rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/opentelemetry/middleware.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/prometheus/__init__.py
--rw-r--r--   0        0        0     2768 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/prometheus/config.py
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/prometheus/controller.py
--rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/prometheus/middleware.py
--rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/pydantic/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/pydantic/config.py
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/pydantic/pydantic_di_plugin.py
--rw-r--r--   0        0        0     5955 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/pydantic/pydantic_dto_factory.py
--rw-r--r--   0        0        0     6706 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/pydantic/pydantic_init_plugin.py
--rw-r--r--   0        0        0    13051 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/pydantic/pydantic_schema_plugin.py
--rw-r--r--   0        0        0     7667 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/pydantic/utils.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/repository/__init__.py
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/repository/exceptions.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/repository/filters.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/repository/handlers.py
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/repository/testing.py
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/repository/abc/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/sqlalchemy/__init__.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/sqlalchemy/base.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/sqlalchemy/dto.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/sqlalchemy/types.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/sqlalchemy/plugins/__init__.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/sqlalchemy/plugins/serialization.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/sqlalchemy/plugins/init/__init__.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/sqlalchemy/plugins/init/plugin.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/sqlalchemy/plugins/init/config/__init__.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/sqlalchemy/plugins/init/config/asyncio.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/sqlalchemy/plugins/init/config/common.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/sqlalchemy/plugins/init/config/compat.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/sqlalchemy/plugins/init/config/engine.py
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/sqlalchemy/plugins/init/config/sync.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/sqlalchemy/repository/__init__.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/sqlalchemy/repository/_async.py
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/sqlalchemy/repository/_sync.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/sqlalchemy/repository/_util.py
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/contrib/sqlalchemy/repository/types.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/datastructures/__init__.py
--rw-r--r--   0        0        0     3770 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/datastructures/cookie.py
--rw-r--r--   0        0        0    17475 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/datastructures/headers.py
--rw-r--r--   0        0        0     3301 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/datastructures/multi_dicts.py
--rw-r--r--   0        0        0     5027 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/datastructures/response_header.py
--rw-r--r--   0        0        0     9699 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/datastructures/state.py
--rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/datastructures/upload_file.py
--rw-r--r--   0        0        0     7351 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/datastructures/url.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/dto/__init__.py
--rw-r--r--   0        0        0    33807 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/dto/_backend.py
--rw-r--r--   0        0        0    22848 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/dto/_codegen_backend.py
--rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/dto/_types.py
--rw-r--r--   0        0        0    12845 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/dto/base_dto.py
--rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/dto/config.py
--rw-r--r--   0        0        0     3906 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/dto/data_structures.py
--rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/dto/dataclass_dto.py
--rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/dto/field.py
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/dto/msgspec_dto.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/dto/types.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/events/__init__.py
--rw-r--r--   0        0        0     4530 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/events/emitter.py
--rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/events/listener.py
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/exceptions/__init__.py
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/exceptions/base_exceptions.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/exceptions/dto_exceptions.py
--rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/exceptions/http_exceptions.py
--rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/exceptions/websocket_exceptions.py
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/handlers/__init__.py
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/handlers/asgi_handlers.py
--rw-r--r--   0        0        0    23116 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/handlers/base.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/handlers/http_handlers/__init__.py
--rw-r--r--   0        0        0     6976 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/handlers/http_handlers/_utils.py
--rw-r--r--   0        0        0    29363 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/handlers/http_handlers/base.py
--rw-r--r--   0        0        0    65669 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/handlers/http_handlers/decorators.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/handlers/websocket_handlers/__init__.py
--rw-r--r--   0        0        0     6182 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/handlers/websocket_handlers/_utils.py
--rw-r--r--   0        0        0    18815 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/handlers/websocket_handlers/listener.py
--rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/handlers/websocket_handlers/route_handler.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/logging/__init__.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/logging/_utils.py
--rw-r--r--   0        0        0    18040 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/logging/config.py
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/logging/picologging.py
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/logging/standard.py
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/middleware/__init__.py
--rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/middleware/_utils.py
--rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/middleware/allowed_hosts.py
--rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/middleware/authentication.py
--rw-r--r--   0        0        0     5283 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/middleware/base.py
--rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/middleware/cors.py
--rw-r--r--   0        0        0     6539 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/middleware/csrf.py
--rw-r--r--   0        0        0    13235 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/middleware/logging.py
--rw-r--r--   0        0        0    10725 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/middleware/rate_limit.py
--rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/middleware/response_cache.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/middleware/compression/__init__.py
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/middleware/compression/brotli_facade.py
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/middleware/compression/facade.py
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/middleware/compression/gzip_facade.py
--rw-r--r--   0        0        0     6653 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/middleware/compression/middleware.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/middleware/exceptions/__init__.py
--rw-r--r--   0        0        0     7964 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/middleware/exceptions/_debug_response.py
--rw-r--r--   0        0        0    11666 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/middleware/exceptions/middleware.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/middleware/exceptions/templates/body.html
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/middleware/exceptions/templates/frame.html
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/middleware/exceptions/templates/scripts.js
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/middleware/exceptions/templates/styles.css
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/middleware/session/__init__.py
--rw-r--r--   0        0        0     8487 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/middleware/session/base.py
--rw-r--r--   0        0        0    10895 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/middleware/session/client_side.py
--rw-r--r--   0        0        0     9387 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/middleware/session/server_side.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/__init__.py
--rw-r--r--   0        0        0    10629 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/config.py
--rw-r--r--   0        0        0    23018 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/controller.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/datastructures.py
--rw-r--r--   0        0        0    23249 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/plugins.py
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/__init__.py
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/base.py
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/callback.py
--rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/components.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/contact.py
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/discriminator.py
--rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/encoding.py
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/enums.py
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/example.py
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/external_documentation.py
--rw-r--r--   0        0        0     5669 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/header.py
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/info.py
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/license.py
--rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/link.py
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/media_type.py
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/oauth_flow.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/oauth_flows.py
--rw-r--r--   0        0        0     4046 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/open_api.py
--rw-r--r--   0        0        0     4842 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/operation.py
--rw-r--r--   0        0        0     6254 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/parameter.py
--rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/path_item.py
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/paths.py
--rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/reference.py
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/request_body.py
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/response.py
--rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/responses.py
--rw-r--r--   0        0        0    33872 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/schema.py
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/security_requirement.py
--rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/security_scheme.py
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/server.py
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/server_variable.py
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/tag.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/openapi/spec/xml.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/plugins/__init__.py
--rw-r--r--   0        0        0    10975 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/plugins/base.py
--rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/plugins/core.py
--rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/plugins/flash.py
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/plugins/sqlalchemy.py
--rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/plugins/structlog.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/repository/__init__.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/repository/_exceptions.py
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/repository/_filters.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/repository/exceptions.py
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/repository/filters.py
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/repository/handlers.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/repository/abc/__init__.py
--rw-r--r--   0        0        0    10228 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/repository/abc/_async.py
--rw-r--r--   0        0        0    10232 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/repository/abc/_sync.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/repository/testing/__init__.py
--rw-r--r--   0        0        0    28346 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/repository/testing/generic_mock_repository.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/response/__init__.py
--rw-r--r--   0        0        0    16726 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/response/base.py
--rw-r--r--   0        0        0    15271 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/response/file.py
--rw-r--r--   0        0        0     6423 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/response/redirect.py
--rw-r--r--   0        0        0     7135 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/response/sse.py
--rw-r--r--   0        0        0     9650 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/response/streaming.py
--rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/response/template.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/routes/__init__.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/routes/asgi.py
--rw-r--r--   0        0        0     6680 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/routes/base.py
--rw-r--r--   0        0        0    12878 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/routes/http.py
--rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/routes/websocket.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/security/__init__.py
--rw-r--r--   0        0        0     7431 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/security/base.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/security/jwt/__init__.py
--rw-r--r--   0        0        0    30453 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/security/jwt/auth.py
--rw-r--r--   0        0        0     7595 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/security/jwt/middleware.py
--rw-r--r--   0        0        0     4373 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/security/jwt/token.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/security/session_auth/__init__.py
--rw-r--r--   0        0        0     5912 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/security/session_auth/auth.py
--rw-r--r--   0        0        0     5257 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/security/session_auth/middleware.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/serialization/__init__.py
--rw-r--r--   0        0        0     7788 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/serialization/msgspec_hooks.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/static_files/__init__.py
--rw-r--r--   0        0        0     5688 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/static_files/base.py
--rw-r--r--   0        0        0     8666 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/static_files/config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/stores/__init__.py
--rw-r--r--   0        0        0     4738 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/stores/base.py
--rw-r--r--   0        0        0     5469 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/stores/file.py
--rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/stores/memory.py
--rw-r--r--   0        0        0     7277 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/stores/redis.py
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/stores/registry.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/template/__init__.py
--rw-r--r--   0        0        0     5942 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/template/base.py
--rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/template/config.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/testing/__init__.py
--rw-r--r--   0        0        0    31457 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/testing/helpers.py
--rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/testing/life_span_handler.py
--rw-r--r--   0        0        0    22930 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/testing/request_factory.py
--rw-r--r--   0        0        0     7980 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/testing/transport.py
--rw-r--r--   0        0        0     8563 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/testing/websocket_test_session.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/testing/client/__init__.py
--rw-r--r--   0        0        0    17874 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/testing/client/async_client.py
--rw-r--r--   0        0        0     6443 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/testing/client/base.py
--rw-r--r--   0        0        0    19967 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/testing/client/sync_client.py
--rw-r--r--   0        0        0     4136 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/types/__init__.py
--rw-r--r--   0        0        0     8978 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/types/asgi_types.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/types/builtin_types.py
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/types/callable_types.py
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/types/composite_types.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/types/empty.py
--rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/types/file_types.py
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/types/helper_types.py
--rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/types/internal_types.py
--rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/types/protocols.py
--rw-r--r--   0        0        0     2067 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/types/serialization.py
--rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/utils/__init__.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/utils/compat.py
--rw-r--r--   0        0        0     3763 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/utils/dataclass.py
--rw-r--r--   0        0        0     3553 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/utils/deprecation.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/utils/empty.py
--rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/utils/helpers.py
--rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/utils/module_loader.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/utils/path.py
--rw-r--r--   0        0        0     9211 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/utils/predicates.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/utils/sequence.py
--rw-r--r--   0        0        0     9670 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/utils/signature.py
--rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/utils/sync.py
--rw-r--r--   0        0        0     9984 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/utils/typing.py
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/utils/version.py
--rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/utils/warnings.py
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/utils/scope/__init__.py
--rw-r--r--   0        0        0     4831 2020-02-02 00:00:00.000000 litestar-2.8.0/litestar/utils/scope/state.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/__init__.py
--rw-r--r--   0        0        0    10120 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/conftest.py
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/docker-compose.yml
--rw-r--r--   0        0        0     4211 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/docker_service_fixtures.py
--rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/helpers.py
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/e2e/__init__.py
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/e2e/test_advanced_alchemy.py
--rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/e2e/test_exception_handlers.py
--rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/e2e/test_option_requests.py
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/e2e/test_pydantic.py
--rw-r--r--   0        0        0    11523 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/e2e/test_response_caching.py
--rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/e2e/test_router_registration.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/e2e/test_starlette_responses.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/e2e/test_dependency_injection/__init__.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/e2e/test_dependency_injection/test_dependency_validation.py
--rw-r--r--   0        0        0     3397 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/e2e/test_dependency_injection/test_http_handler_dependency_injection.py
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/e2e/test_dependency_injection/test_injection_of_classes.py
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/e2e/test_dependency_injection/test_injection_of_generic_models.py
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/e2e/test_dependency_injection/test_inter_dependencies.py
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/e2e/test_dependency_injection/test_request_local_caching.py
--rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/e2e/test_dependency_injection/test_websocket_handler_dependency_injection.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/e2e/test_life_cycle_hooks/__init__.py
--rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/e2e/test_life_cycle_hooks/test_after_request.py
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/e2e/test_life_cycle_hooks/test_after_response.py
--rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/e2e/test_life_cycle_hooks/test_before_request.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/e2e/test_routing/__init__.py
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/e2e/test_routing/conftest.py
--rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/e2e/test_routing/test_asset_url_path.py
--rw-r--r--   0        0        0     4936 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/e2e/test_routing/test_path_mounting.py
--rw-r--r--   0        0        0    12716 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/e2e/test_routing/test_path_resolution.py
--rw-r--r--   0        0        0     4798 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/e2e/test_routing/test_route_indexing.py
--rw-r--r--   0        0        0     4039 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/e2e/test_routing/test_route_reverse.py
--rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/e2e/test_routing/test_validations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/__init__.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/conftest.py
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_cache_control_headers.py
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_exceptions.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_hello_world.py
--rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_lifecycle_hooks.py
--rw-r--r--   0        0        0     4447 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_request_data.py
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_routing.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_signature_namespace.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_startup_and_shutdown.py
--rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_static_files.py
--rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_stores.py
--rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_todo_app.py
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_using_session_auth.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_websockets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_application_hooks/__init__.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_application_hooks/test_application_after_exception_hook.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_application_hooks/test_application_before_send.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_application_hooks/test_lifespan_manager.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_application_hooks/test_on_app_init.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_application_state/__init__.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_application_state/test_passing_initial_state.py
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_application_state/test_using_application_state.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_application_state/test_using_custom_state.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_application_state/test_using_immutable_state.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_contrib/__init__.py
--rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_contrib/test_piccolo_orm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_contrib/prometheus/__init__.py
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_contrib/prometheus/test_prometheus_exporter_example.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_contrib/prometheus/test_prometheus_exporter_example_with_extra_config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_contrib/test_sqlalchemy/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_contrib/test_sqlalchemy/plugins/__init__.py
--rw-r--r--   0        0        0     5889 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_contrib/test_sqlalchemy/plugins/test_example_apps.py
--rw-r--r--   0        0        0     2480 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_contrib/test_sqlalchemy/plugins/test_tutorial_example_apps.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_dependency_injection/__init__.py
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_dependency_injection/test_dependency_default_value_no_dependency_fn.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_dependency_injection/test_dependency_default_value_with_dependency_fn.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_dependency_injection/test_dependency_skip_validation.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_dependency_injection/test_dependency_validation_error.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_dependency_injection/tests_dependency_non_optional_not_provided.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_dto/__init__.py
--rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_dto/test_example_apps.py
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_dto/test_tutorial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_middleware/__init__.py
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_middleware/test_abstract_middleware.py
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_middleware/test_call_order.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_middleware/test_logging_middleware.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_middleware/test_rate_limit_middleware.py
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_middleware/test_session_middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_openapi/__init__.py
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_openapi/test_openapi.py
--rw-r--r--   0        0        0     4267 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_openapi/test_plugins.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_pagination/__init__.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_pagination/test_using_classic_pagination.py
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_pagination/test_using_cursor_pagination.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_pagination/test_using_offset_pagination.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_parameters/__init__.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_parameters/test_header_and_cookies_parameters.py
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_parameters/test_layered_parameters.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_parameters/test_path_parameters.py
--rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_parameters/test_query_parameters.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_plugins/__init__.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_plugins/test_di_plugin.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_plugins/test_example_apps.py
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_plugins/test_sqlalchemy_init_plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_responses/__init__.py
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_responses/test_background_tasks.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_responses/test_custom_responses.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_responses/test_json_suffix_responses.py
--rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_responses/test_response_cookies.py
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_responses/test_response_headers.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_responses/test_returning_responses.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_responses/test_sse_responses.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_security/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_security/test_jwt/__init__.py
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_security/test_jwt/test_using_jwt_auth.py
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_security/test_jwt/test_using_jwt_cookie_auth.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_security/test_jwt/test_using_oauth2_password_bearer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_templating/__init__.py
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_templating/test_engine_instance.py
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_templating/test_returning_templates.py
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/examples/test_templating/test_template_functions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/__init__.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/conftest.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/piccolo_conf.py
--rw-r--r--   0        0        0    15242 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_app.py
--rw-r--r--   0        0        0     6321 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_asgi_router.py
--rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_background_tasks.py
--rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_concurrency.py
--rw-r--r--   0        0        0     3854 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_controller.py
--rw-r--r--   0        0        0     6006 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_data_extractors.py
--rw-r--r--   0        0        0     4933 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_deprecations.py
--rw-r--r--   0        0        0     4606 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_di.py
--rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_events.py
--rw-r--r--   0        0        0     8341 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_exceptions.py
--rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_file_system.py
--rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_guards.py
--rw-r--r--   0        0        0    11592 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_pagination.py
--rw-r--r--   0        0        0    11015 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_params.py
--rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_parsers.py
--rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_request_class_resolution.py
--rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_response_class_resolution.py
--rw-r--r--   0        0        0    13025 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_stores.py
--rw-r--r--   0        0        0    17322 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_typing.py
--rw-r--r--   0        0        0     4516 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_websocket_class_resolution.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_channels/__init__.py
--rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_channels/conftest.py
--rw-r--r--   0        0        0     8672 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_channels/test_backends.py
--rw-r--r--   0        0        0    16493 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_channels/test_plugin.py
--rw-r--r--   0        0        0     3542 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_channels/test_subscriber.py
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_channels/util.py
--rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_cli/__init__.py
--rw-r--r--   0        0        0     4932 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_cli/conftest.py
--rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_cli/test_cli.py
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_cli/test_cli_plugin.py
--rw-r--r--   0        0        0    23147 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_cli/test_core_commands.py
--rw-r--r--   0        0        0     4294 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_cli/test_env_resolution.py
--rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_cli/test_schema_commands.py
--rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_cli/test_session_commands.py
--rw-r--r--   0        0        0     9784 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_cli/test_ssl.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_connection/__init__.py
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_connection/test_base.py
--rw-r--r--   0        0        0     7225 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_connection/test_connection_caching.py
--rw-r--r--   0        0        0    19442 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_connection/test_request.py
--rw-r--r--   0        0        0    14929 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_connection/test_websocket.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/__init__.py
--rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/conftest.py
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_minijinja.py
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_msgspec.py
--rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_opentelemetry.py
--rw-r--r--   0        0        0     7545 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_prometheus.py
--rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_repository.py
--rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_sqlalchemy.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_attrs/__init__.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_attrs/test_inject_attrs_class.py
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_attrs/test_schema_plugin.py
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_attrs/test_schema_spec_generation.py
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_attrs/test_signature.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_htmx/__init__.py
--rw-r--r--   0        0        0    10431 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_htmx/test_htmx_request.py
--rw-r--r--   0        0        0    13872 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_htmx/test_htmx_response.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_piccolo_orm/__init__.py
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_piccolo_orm/endpoints.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_piccolo_orm/piccolo_app.py
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_piccolo_orm/tables.py
--rw-r--r--   0        0        0     6298 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_piccolo_orm/test_piccolo_orm_dto.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_pydantic/__init__.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_pydantic/conftest.py
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_pydantic/models.py
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_pydantic/test_beanie_integration.py
--rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_pydantic/test_dto.py
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_pydantic/test_inject_pydantic.py
--rw-r--r--   0        0        0    11001 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_pydantic/test_integration.py
--rw-r--r--   0        0        0    29005 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_pydantic/test_openapi.py
--rw-r--r--   0        0        0     9126 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_pydantic/test_plugin_serialization.py
--rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_pydantic/test_pydantic_dto_factory.py
--rw-r--r--   0        0        0     5138 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_pydantic/test_schema_plugin.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_contrib/test_pydantic/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_datastructures/__init_.py
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_datastructures/test_cookie.py
--rw-r--r--   0        0        0    13358 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_datastructures/test_headers.py
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_datastructures/test_multi_dicts.py
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_datastructures/test_response_header.py
--rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_datastructures/test_state.py
--rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_datastructures/test_upload_file.py
--rw-r--r--   0        0        0     3672 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_datastructures/test_url.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_dto/__init__.py
--rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_dto/conftest.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_dto/test_config.py
--rw-r--r--   0        0        0     5943 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_dto/test_integration.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_dto/test_interface.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_dto/test_factory/__init__.py
--rw-r--r--   0        0        0     5259 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_dto/test_factory/test_base_dto.py
--rw-r--r--   0        0        0     4464 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_dto/test_factory/test_dataclass_dto.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_dto/test_factory/test_field.py
--rw-r--r--   0        0        0    30290 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_dto/test_factory/test_integration.py
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_dto/test_factory/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_dto/test_factory/test_backends/__init__.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_dto/test_factory/test_backends/conftest.py
--rw-r--r--   0        0        0    16326 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_dto/test_factory/test_backends/test_backends.py
--rw-r--r--   0        0        0    10244 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_dto/test_factory/test_backends/test_base_dto.py
--rw-r--r--   0        0        0     7630 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_dto/test_factory/test_backends/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_handlers/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_handlers/test_asgi_handlers/__init__.py
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_handlers/test_asgi_handlers/test_handle_asgi.py
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_handlers/test_asgi_handlers/test_handle_asgi_with_future_annotations.py
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_handlers/test_asgi_handlers/test_validations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_handlers/test_base_handlers/__init__.py
--rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_handlers/test_base_handlers/test_opt.py
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_handlers/test_base_handlers/test_resolution.py
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_handlers/test_base_handlers/test_validations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_handlers/test_http_handlers/__init__.py
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_handlers/test_http_handlers/test_defaults.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_handlers/test_http_handlers/test_delete.py
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_handlers/test_http_handlers/test_head.py
--rw-r--r--   0        0        0     3165 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_handlers/test_http_handlers/test_kwarg_handling.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_handlers/test_http_handlers/test_media_type.py
--rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_handlers/test_http_handlers/test_signature_namespace.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_handlers/test_http_handlers/test_sync.py
--rw-r--r--   0        0        0     4437 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_handlers/test_http_handlers/test_validations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_handlers/test_websocket_handlers/__init__.py
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_handlers/test_websocket_handlers/test_handle_websocket.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_handlers/test_websocket_handlers/test_handle_websocket_with_future_annotations.py
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_handlers/test_websocket_handlers/test_kwarg_handling.py
--rw-r--r--   0        0        0    14396 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_handlers/test_websocket_handlers/test_listeners.py
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_handlers/test_websocket_handlers/test_validations.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_kwargs/__init__.py
--rw-r--r--   0        0        0    72895 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_kwargs/flower.jpeg
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_kwargs/test_cleanup_group.py
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_kwargs/test_cookie_params.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_kwargs/test_defaults.py
--rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_kwargs/test_dependency_batches.py
--rw-r--r--   0        0        0     7259 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_kwargs/test_generator_dependencies.py
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_kwargs/test_header_params.py
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_kwargs/test_json_data.py
--rw-r--r--   0        0        0     8662 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_kwargs/test_layered_params.py
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_kwargs/test_msgpack_data.py
--rw-r--r--   0        0        0    21924 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_kwargs/test_multipart_data.py
--rw-r--r--   0        0        0     6592 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_kwargs/test_path_params.py
--rw-r--r--   0        0        0     6666 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_kwargs/test_query_params.py
--rw-r--r--   0        0        0     9794 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_kwargs/test_reserved_kwargs_injection.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_kwargs/test_url_encoded_data.py
--rw-r--r--   0        0        0     4372 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_kwargs/test_validations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_logging/__init__.py
--rw-r--r--   0        0        0     9198 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_logging/test_logging_config.py
--rw-r--r--   0        0        0     7083 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_logging/test_structlog_config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_middleware/__init__.py
--rw-r--r--   0        0        0     5873 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_middleware/test_allowed_hosts_middleware.py
--rw-r--r--   0        0        0     8644 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_middleware/test_base_authentication_middleware.py
--rw-r--r--   0        0        0     5095 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_middleware/test_base_middleware.py
--rw-r--r--   0        0        0    11412 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_middleware/test_compression_middleware.py
--rw-r--r--   0        0        0     5506 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_middleware/test_cors_middleware.py
--rw-r--r--   0        0        0     9446 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_middleware/test_csrf_middleware.py
--rw-r--r--   0        0        0    14919 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_middleware/test_exception_handler_middleware.py
--rw-r--r--   0        0        0    12163 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_middleware/test_logging_middleware.py
--rw-r--r--   0        0        0     5821 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_middleware/test_middleware_handling.py
--rw-r--r--   0        0        0     7846 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_middleware/test_rate_limit_middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_middleware/test_session/__init__.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_middleware/test_session/conftest.py
--rw-r--r--   0        0        0     8354 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_middleware/test_session/test_client_side_backend.py
--rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_middleware/test_session/test_integration.py
--rw-r--r--   0        0        0     8726 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_middleware/test_session/test_middleware.py
--rw-r--r--   0        0        0     5444 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_middleware/test_session/test_server_side_backend.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_openapi/__init__.py
--rw-r--r--   0        0        0     5595 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_openapi/conftest.py
--rw-r--r--   0        0        0     4373 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_openapi/test_config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_openapi/test_constrained_fields.py
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_openapi/test_datastructures.py
--rw-r--r--   0        0        0    20213 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_openapi/test_endpoints.py
--rw-r--r--   0        0        0    19008 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_openapi/test_integration.py
--rw-r--r--   0        0        0    13925 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_openapi/test_parameters.py
--rw-r--r--   0        0        0     9934 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_openapi/test_path_item.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_openapi/test_render_plugins.py
--rw-r--r--   0        0        0     6233 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_openapi/test_request_body.py
--rw-r--r--   0        0        0    20422 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_openapi/test_responses.py
--rw-r--r--   0        0        0    22306 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_openapi/test_schema.py
--rw-r--r--   0        0        0     4561 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_openapi/test_security_schemes.py
--rw-r--r--   0        0        0     6434 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_openapi/test_spec_generation.py
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_openapi/test_tags.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_openapi/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_openapi/test_typescript_converter/__init__.py
--rw-r--r--   0        0        0     8625 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_openapi/test_typescript_converter/test_converter.py
--rw-r--r--   0        0        0     3176 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_openapi/test_typescript_converter/test_schema_parsing.py
--rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_openapi/test_typescript_converter/test_typescript_types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_plugins/__init__.py
--rw-r--r--   0        0        0     5114 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_plugins/test_base.py
--rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_plugins/test_flash.py
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_plugins/test_sqlalchemy.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_repository/__init__.py
--rw-r--r--   0        0        0     4732 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_repository/models_bigint.py
--rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_repository/models_uuid.py
--rw-r--r--   0        0        0    18932 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_repository/test_generic_mock_repository.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_response/__init__.py
--rw-r--r--   0        0        0     7676 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_response/test_base_response.py
--rw-r--r--   0        0        0    11238 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_response/test_file_response.py
--rw-r--r--   0        0        0     4418 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_response/test_redirect_response.py
--rw-r--r--   0        0        0     5170 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_response/test_response_cookies.py
--rw-r--r--   0        0        0     6433 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_response/test_response_headers.py
--rw-r--r--   0        0        0    16365 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_response/test_response_to_asgi_response.py
--rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_response/test_serialization.py
--rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_response/test_sse.py
--rw-r--r--   0        0        0     6247 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_response/test_streaming_response.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_response/test_type_decoders.py
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_response/test_type_encoders.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_security/__init__.py
--rw-r--r--   0        0        0     7076 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_security/test_security.py
--rw-r--r--   0        0        0     3728 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_security/test_session_auth.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_security/test_jwt/__init__.py
--rw-r--r--   0        0        0    18293 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_security/test_jwt/test_auth.py
--rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_security/test_jwt/test_integration.py
--rw-r--r--   0        0        0     5443 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_security/test_jwt/test_token.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_signature/__init__.py
--rw-r--r--   0        0        0     6896 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_signature/test_parsing.py
--rw-r--r--   0        0        0     9475 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_signature/test_validation.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_static_files/__init__.py
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_static_files/conftest.py
--rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_static_files/test_create_static_router.py
--rw-r--r--   0        0        0    11768 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_static_files/test_file_serving_resolution.py
--rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_static_files/test_html_mode.py
--rw-r--r--   0        0        0     4186 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_static_files/test_static_files_validation.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_template/__init__.py
--rw-r--r--   0        0        0     6440 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_template/test_built_in.py
--rw-r--r--   0        0        0    11615 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_template/test_builtin_functions.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_template/test_config.py
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_template/test_context.py
--rw-r--r--   0        0        0     2634 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_template/test_csrf_token.py
--rw-r--r--   0        0        0     7401 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_template/test_template.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_testing/__init__.py
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_testing/test_lifespan_handler.py
--rw-r--r--   0        0        0     7205 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_testing/test_request_factory.py
--rw-r--r--   0        0        0     9945 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_testing/test_test_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_types/__init__.py
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_types/test_protocols.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_utils/__init__.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_utils/test_compat.py
--rw-r--r--   0        0        0     4367 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_utils/test_dataclass.py
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_utils/test_deprecation.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_utils/test_helpers.py
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_utils/test_module_loader.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_utils/test_path.py
--rw-r--r--   0        0        0     7229 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_utils/test_predicates.py
--rw-r--r--   0        0        0     2750 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_utils/test_scope.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_utils/test_sequence.py
--rw-r--r--   0        0        0     7921 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_utils/test_signature.py
--rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_utils/test_sync.py
--rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_utils/test_typing.py
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 litestar-2.8.0/tests/unit/test_utils/test_version.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 litestar-2.8.0/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 litestar-2.8.0/LICENSE
--rw-r--r--   0        0        0    92575 2020-02-02 00:00:00.000000 litestar-2.8.0/README.md
--rw-r--r--   0        0        0    12698 2020-02-02 00:00:00.000000 litestar-2.8.0/pyproject.toml
--rw-r--r--   0        0        0    97593 2020-02-02 00:00:00.000000 litestar-2.8.0/PKG-INFO
+-rw-r--r--   0        0        0     6672 2020-02-02 00:00:00.000000 litestar-2.8.1/Makefile
+-rw-r--r--   0        0        0    19851 2020-02-02 00:00:00.000000 litestar-2.8.1/docs/PYPI_README.md
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/__init__.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/__main__.py
+-rw-r--r--   0        0        0     6000 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/_multipart.py
+-rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/_parsers.py
+-rw-r--r--   0        0        0    39586 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/app.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/background_tasks.py
+-rw-r--r--   0        0        0     3367 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/concurrency.py
+-rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/constants.py
+-rw-r--r--   0        0        0    11032 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/controller.py
+-rw-r--r--   0        0        0    17681 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/data_extractors.py
+-rw-r--r--   0        0        0     4282 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/di.py
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/enums.py
+-rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/file_system.py
+-rw-r--r--   0        0        0    11029 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/pagination.py
+-rw-r--r--   0        0        0    15965 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/params.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/py.typed
+-rw-r--r--   0        0        0    16702 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/router.py
+-rw-r--r--   0        0        0     8973 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/status_codes.py
+-rw-r--r--   0        0        0    25972 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/typing.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/_asgi/__init__.py
+-rw-r--r--   0        0        0     6530 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/_asgi/asgi_router.py
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/_asgi/utils.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/_asgi/routing_trie/__init__.py
+-rw-r--r--   0        0        0     8107 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/_asgi/routing_trie/mapping.py
+-rw-r--r--   0        0        0     5995 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/_asgi/routing_trie/traversal.py
+-rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/_asgi/routing_trie/types.py
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/_asgi/routing_trie/validate.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/_kwargs/__init__.py
+-rw-r--r--   0        0        0     3846 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/_kwargs/cleanup.py
+-rw-r--r--   0        0        0     4195 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/_kwargs/dependencies.py
+-rw-r--r--   0        0        0    16651 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/_kwargs/extractors.py
+-rw-r--r--   0        0        0    20472 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/_kwargs/kwargs_model.py
+-rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/_kwargs/parameter_definition.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/_layers/__init__.py
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/_layers/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/_openapi/__init__.py
+-rw-r--r--   0        0        0     6577 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/_openapi/datastructures.py
+-rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/_openapi/parameters.py
+-rw-r--r--   0        0        0     6839 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/_openapi/path_item.py
+-rw-r--r--   0        0        0     7836 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/_openapi/plugin.py
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/_openapi/request_body.py
+-rw-r--r--   0        0        0    13607 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/_openapi/responses.py
+-rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/_openapi/utils.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/_openapi/schema_generation/__init__.py
+-rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/_openapi/schema_generation/constrained_fields.py
+-rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/_openapi/schema_generation/examples.py
+-rw-r--r--   0        0        0    25613 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/_openapi/schema_generation/schema.py
+-rw-r--r--   0        0        0     3842 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/_openapi/schema_generation/utils.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/_openapi/schema_generation/plugins/__init__.py
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/_openapi/schema_generation/plugins/dataclass.py
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/_openapi/schema_generation/plugins/pagination.py
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/_openapi/schema_generation/plugins/struct.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/_openapi/schema_generation/plugins/typed_dict.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/_openapi/typescript_converter/__init__.py
+-rw-r--r--   0        0        0    10909 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/_openapi/typescript_converter/converter.py
+-rw-r--r--   0        0        0     5212 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/_openapi/typescript_converter/schema_parsing.py
+-rw-r--r--   0        0        0     7664 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/_openapi/typescript_converter/types.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/_signature/__init__.py
+-rw-r--r--   0        0        0    11710 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/_signature/model.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/_signature/types.py
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/_signature/utils.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/channels/__init__.py
+-rw-r--r--   0        0        0    15848 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/channels/plugin.py
+-rw-r--r--   0        0        0     4711 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/channels/subscriber.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/channels/backends/__init__.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/channels/backends/_redis_flushall_streams.lua
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/channels/backends/_redis_pubsub_publish.lua
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/channels/backends/_redis_xadd_expire.lua
+-rw-r--r--   0        0        0     3435 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/channels/backends/asyncpg.py
+-rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/channels/backends/base.py
+-rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/channels/backends/memory.py
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/channels/backends/psycopg.py
+-rw-r--r--   0        0        0    11422 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/channels/backends/redis.py
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/cli/__init__.py
+-rw-r--r--   0        0        0    20230 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/cli/_utils.py
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/cli/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/cli/commands/__init__.py
+-rw-r--r--   0        0        0    12215 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/cli/commands/core.py
+-rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/cli/commands/schema.py
+-rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/cli/commands/sessions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/config/__init__.py
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/config/allowed_hosts.py
+-rw-r--r--   0        0        0    12477 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/config/app.py
+-rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/config/compression.py
+-rw-r--r--   0        0        0     5178 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/config/cors.py
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/config/csrf.py
+-rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/config/response_cache.py
+-rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/connection/__init__.py
+-rw-r--r--   0        0        0    11536 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/connection/base.py
+-rw-r--r--   0        0        0     9482 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/connection/request.py
+-rw-r--r--   0        0        0    11331 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/connection/websocket.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/contrib/__init__.py
+-rw-r--r--   0        0        0     3998 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/contrib/jinja.py
+-rw-r--r--   0        0        0     5451 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/contrib/mako.py
+-rw-r--r--   0        0        0     7831 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/contrib/minijinja.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/contrib/minijnja.py
+-rw-r--r--   0        0        0     3839 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/contrib/piccolo.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/contrib/attrs/__init__.py
+-rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/contrib/attrs/attrs_schema_plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/contrib/htmx/__init__.py
+-rw-r--r--   0        0        0     4800 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/contrib/htmx/_utils.py
+-rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/contrib/htmx/request.py
+-rw-r--r--   0        0        0     6408 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/contrib/htmx/response.py
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/contrib/htmx/types.py
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/contrib/jwt/__init__.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/contrib/jwt/jwt_auth.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/contrib/jwt/jwt_token.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/contrib/jwt/middleware.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/contrib/opentelemetry/__init__.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/contrib/opentelemetry/_utils.py
+-rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/contrib/opentelemetry/config.py
+-rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/contrib/opentelemetry/middleware.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/contrib/prometheus/__init__.py
+-rw-r--r--   0        0        0     2768 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/contrib/prometheus/config.py
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/contrib/prometheus/controller.py
+-rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/contrib/prometheus/middleware.py
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/contrib/pydantic/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/contrib/pydantic/config.py
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/contrib/pydantic/pydantic_di_plugin.py
+-rw-r--r--   0        0        0     6147 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/contrib/pydantic/pydantic_dto_factory.py
+-rw-r--r--   0        0        0     6706 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/contrib/pydantic/pydantic_init_plugin.py
+-rw-r--r--   0        0        0    13051 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/contrib/pydantic/pydantic_schema_plugin.py
+-rw-r--r--   0        0        0     7667 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/contrib/pydantic/utils.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/contrib/repository/__init__.py
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/contrib/repository/exceptions.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/contrib/repository/filters.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/contrib/repository/handlers.py
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/contrib/repository/testing.py
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/contrib/repository/abc/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/contrib/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/contrib/sqlalchemy/base.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/contrib/sqlalchemy/dto.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/contrib/sqlalchemy/types.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/contrib/sqlalchemy/plugins/__init__.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/contrib/sqlalchemy/plugins/serialization.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/contrib/sqlalchemy/plugins/init/__init__.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/contrib/sqlalchemy/plugins/init/plugin.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/contrib/sqlalchemy/plugins/init/config/__init__.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/contrib/sqlalchemy/plugins/init/config/asyncio.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/contrib/sqlalchemy/plugins/init/config/common.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/contrib/sqlalchemy/plugins/init/config/compat.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/contrib/sqlalchemy/plugins/init/config/engine.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/contrib/sqlalchemy/plugins/init/config/sync.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/contrib/sqlalchemy/repository/__init__.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/contrib/sqlalchemy/repository/_async.py
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/contrib/sqlalchemy/repository/_sync.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/contrib/sqlalchemy/repository/_util.py
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/contrib/sqlalchemy/repository/types.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/datastructures/__init__.py
+-rw-r--r--   0        0        0     3770 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/datastructures/cookie.py
+-rw-r--r--   0        0        0    17475 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/datastructures/headers.py
+-rw-r--r--   0        0        0     3301 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/datastructures/multi_dicts.py
+-rw-r--r--   0        0        0     5027 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/datastructures/response_header.py
+-rw-r--r--   0        0        0     9699 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/datastructures/state.py
+-rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/datastructures/upload_file.py
+-rw-r--r--   0        0        0     7351 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/datastructures/url.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/dto/__init__.py
+-rw-r--r--   0        0        0    33807 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/dto/_backend.py
+-rw-r--r--   0        0        0    22848 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/dto/_codegen_backend.py
+-rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/dto/_types.py
+-rw-r--r--   0        0        0    12845 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/dto/base_dto.py
+-rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/dto/config.py
+-rw-r--r--   0        0        0     3906 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/dto/data_structures.py
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/dto/dataclass_dto.py
+-rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/dto/field.py
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/dto/msgspec_dto.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/dto/types.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/events/__init__.py
+-rw-r--r--   0        0        0     4530 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/events/emitter.py
+-rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/events/listener.py
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/exceptions/__init__.py
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/exceptions/base_exceptions.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/exceptions/dto_exceptions.py
+-rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/exceptions/http_exceptions.py
+-rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/exceptions/websocket_exceptions.py
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/handlers/__init__.py
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/handlers/asgi_handlers.py
+-rw-r--r--   0        0        0    23819 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/handlers/base.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/handlers/http_handlers/__init__.py
+-rw-r--r--   0        0        0     6976 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/handlers/http_handlers/_utils.py
+-rw-r--r--   0        0        0    29363 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/handlers/http_handlers/base.py
+-rw-r--r--   0        0        0    65669 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/handlers/http_handlers/decorators.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/handlers/websocket_handlers/__init__.py
+-rw-r--r--   0        0        0     6182 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/handlers/websocket_handlers/_utils.py
+-rw-r--r--   0        0        0    18815 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/handlers/websocket_handlers/listener.py
+-rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/handlers/websocket_handlers/route_handler.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/logging/__init__.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/logging/_utils.py
+-rw-r--r--   0        0        0    18040 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/logging/config.py
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/logging/picologging.py
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/logging/standard.py
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/middleware/__init__.py
+-rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/middleware/_utils.py
+-rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/middleware/allowed_hosts.py
+-rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/middleware/authentication.py
+-rw-r--r--   0        0        0     5283 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/middleware/base.py
+-rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/middleware/cors.py
+-rw-r--r--   0        0        0     6539 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/middleware/csrf.py
+-rw-r--r--   0        0        0    13235 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/middleware/logging.py
+-rw-r--r--   0        0        0    10725 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/middleware/rate_limit.py
+-rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/middleware/response_cache.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/middleware/compression/__init__.py
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/middleware/compression/brotli_facade.py
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/middleware/compression/facade.py
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/middleware/compression/gzip_facade.py
+-rw-r--r--   0        0        0     6653 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/middleware/compression/middleware.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/middleware/exceptions/__init__.py
+-rw-r--r--   0        0        0     7964 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/middleware/exceptions/_debug_response.py
+-rw-r--r--   0        0        0    11666 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/middleware/exceptions/middleware.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/middleware/exceptions/templates/body.html
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/middleware/exceptions/templates/frame.html
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/middleware/exceptions/templates/scripts.js
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/middleware/exceptions/templates/styles.css
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/middleware/session/__init__.py
+-rw-r--r--   0        0        0     8487 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/middleware/session/base.py
+-rw-r--r--   0        0        0    10895 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/middleware/session/client_side.py
+-rw-r--r--   0        0        0     9387 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/middleware/session/server_side.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/openapi/__init__.py
+-rw-r--r--   0        0        0    10629 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/openapi/config.py
+-rw-r--r--   0        0        0    23353 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/openapi/controller.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/openapi/datastructures.py
+-rw-r--r--   0        0        0    23249 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/openapi/plugins.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/openapi/spec/__init__.py
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/openapi/spec/base.py
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/openapi/spec/callback.py
+-rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/openapi/spec/components.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/openapi/spec/contact.py
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/openapi/spec/discriminator.py
+-rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/openapi/spec/encoding.py
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/openapi/spec/enums.py
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/openapi/spec/example.py
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/openapi/spec/external_documentation.py
+-rw-r--r--   0        0        0     5669 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/openapi/spec/header.py
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/openapi/spec/info.py
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/openapi/spec/license.py
+-rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/openapi/spec/link.py
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/openapi/spec/media_type.py
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/openapi/spec/oauth_flow.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/openapi/spec/oauth_flows.py
+-rw-r--r--   0        0        0     4046 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/openapi/spec/open_api.py
+-rw-r--r--   0        0        0     4842 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/openapi/spec/operation.py
+-rw-r--r--   0        0        0     6254 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/openapi/spec/parameter.py
+-rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/openapi/spec/path_item.py
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/openapi/spec/paths.py
+-rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/openapi/spec/reference.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/openapi/spec/request_body.py
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/openapi/spec/response.py
+-rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/openapi/spec/responses.py
+-rw-r--r--   0        0        0    33872 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/openapi/spec/schema.py
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/openapi/spec/security_requirement.py
+-rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/openapi/spec/security_scheme.py
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/openapi/spec/server.py
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/openapi/spec/server_variable.py
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/openapi/spec/tag.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/openapi/spec/xml.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/plugins/__init__.py
+-rw-r--r--   0        0        0    10975 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/plugins/base.py
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/plugins/core.py
+-rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/plugins/flash.py
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/plugins/sqlalchemy.py
+-rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/plugins/structlog.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/repository/__init__.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/repository/_exceptions.py
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/repository/_filters.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/repository/exceptions.py
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/repository/filters.py
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/repository/handlers.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/repository/abc/__init__.py
+-rw-r--r--   0        0        0    10228 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/repository/abc/_async.py
+-rw-r--r--   0        0        0    10232 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/repository/abc/_sync.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/repository/testing/__init__.py
+-rw-r--r--   0        0        0    28346 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/repository/testing/generic_mock_repository.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/response/__init__.py
+-rw-r--r--   0        0        0    16726 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/response/base.py
+-rw-r--r--   0        0        0    15271 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/response/file.py
+-rw-r--r--   0        0        0     6423 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/response/redirect.py
+-rw-r--r--   0        0        0     7135 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/response/sse.py
+-rw-r--r--   0        0        0     9650 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/response/streaming.py
+-rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/response/template.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/routes/__init__.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/routes/asgi.py
+-rw-r--r--   0        0        0     5974 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/routes/base.py
+-rw-r--r--   0        0        0    12888 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/routes/http.py
+-rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/routes/websocket.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/security/__init__.py
+-rw-r--r--   0        0        0     7431 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/security/base.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/security/jwt/__init__.py
+-rw-r--r--   0        0        0    30453 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/security/jwt/auth.py
+-rw-r--r--   0        0        0     7595 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/security/jwt/middleware.py
+-rw-r--r--   0        0        0     4373 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/security/jwt/token.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/security/session_auth/__init__.py
+-rw-r--r--   0        0        0     5912 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/security/session_auth/auth.py
+-rw-r--r--   0        0        0     5257 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/security/session_auth/middleware.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/serialization/__init__.py
+-rw-r--r--   0        0        0     7788 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/serialization/msgspec_hooks.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/static_files/__init__.py
+-rw-r--r--   0        0        0     5688 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/static_files/base.py
+-rw-r--r--   0        0        0     8666 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/static_files/config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/stores/__init__.py
+-rw-r--r--   0        0        0     4738 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/stores/base.py
+-rw-r--r--   0        0        0     5469 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/stores/file.py
+-rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/stores/memory.py
+-rw-r--r--   0        0        0     7277 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/stores/redis.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/stores/registry.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/template/__init__.py
+-rw-r--r--   0        0        0     5942 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/template/base.py
+-rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/template/config.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/testing/__init__.py
+-rw-r--r--   0        0        0    31457 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/testing/helpers.py
+-rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/testing/life_span_handler.py
+-rw-r--r--   0        0        0    22930 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/testing/request_factory.py
+-rw-r--r--   0        0        0     7980 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/testing/transport.py
+-rw-r--r--   0        0        0     8563 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/testing/websocket_test_session.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/testing/client/__init__.py
+-rw-r--r--   0        0        0    17874 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/testing/client/async_client.py
+-rw-r--r--   0        0        0     6443 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/testing/client/base.py
+-rw-r--r--   0        0        0    19967 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/testing/client/sync_client.py
+-rw-r--r--   0        0        0     4136 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/types/__init__.py
+-rw-r--r--   0        0        0     8978 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/types/asgi_types.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/types/builtin_types.py
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/types/callable_types.py
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/types/composite_types.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/types/empty.py
+-rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/types/file_types.py
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/types/helper_types.py
+-rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/types/internal_types.py
+-rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/types/protocols.py
+-rw-r--r--   0        0        0     2067 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/types/serialization.py
+-rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/utils/__init__.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/utils/compat.py
+-rw-r--r--   0        0        0     3763 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/utils/dataclass.py
+-rw-r--r--   0        0        0     3553 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/utils/deprecation.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/utils/empty.py
+-rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/utils/helpers.py
+-rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/utils/module_loader.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/utils/path.py
+-rw-r--r--   0        0        0     9211 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/utils/predicates.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/utils/sequence.py
+-rw-r--r--   0        0        0     9670 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/utils/signature.py
+-rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/utils/sync.py
+-rw-r--r--   0        0        0     9984 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/utils/typing.py
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/utils/version.py
+-rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/utils/warnings.py
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/utils/scope/__init__.py
+-rw-r--r--   0        0        0     4831 2020-02-02 00:00:00.000000 litestar-2.8.1/litestar/utils/scope/state.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/__init__.py
+-rw-r--r--   0        0        0    10120 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/conftest.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/docker-compose.yml
+-rw-r--r--   0        0        0     4211 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/docker_service_fixtures.py
+-rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/helpers.py
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/e2e/__init__.py
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/e2e/test_advanced_alchemy.py
+-rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/e2e/test_exception_handlers.py
+-rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/e2e/test_option_requests.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/e2e/test_pydantic.py
+-rw-r--r--   0        0        0    11523 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/e2e/test_response_caching.py
+-rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/e2e/test_router_registration.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/e2e/test_starlette_responses.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/e2e/test_dependency_injection/__init__.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/e2e/test_dependency_injection/test_dependency_validation.py
+-rw-r--r--   0        0        0     3397 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/e2e/test_dependency_injection/test_http_handler_dependency_injection.py
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/e2e/test_dependency_injection/test_injection_of_classes.py
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/e2e/test_dependency_injection/test_injection_of_generic_models.py
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/e2e/test_dependency_injection/test_inter_dependencies.py
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/e2e/test_dependency_injection/test_request_local_caching.py
+-rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/e2e/test_dependency_injection/test_websocket_handler_dependency_injection.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/e2e/test_life_cycle_hooks/__init__.py
+-rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/e2e/test_life_cycle_hooks/test_after_request.py
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/e2e/test_life_cycle_hooks/test_after_response.py
+-rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/e2e/test_life_cycle_hooks/test_before_request.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/e2e/test_routing/__init__.py
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/e2e/test_routing/conftest.py
+-rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/e2e/test_routing/test_asset_url_path.py
+-rw-r--r--   0        0        0     4936 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/e2e/test_routing/test_path_mounting.py
+-rw-r--r--   0        0        0    12716 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/e2e/test_routing/test_path_resolution.py
+-rw-r--r--   0        0        0     4798 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/e2e/test_routing/test_route_indexing.py
+-rw-r--r--   0        0        0     4039 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/e2e/test_routing/test_route_reverse.py
+-rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/e2e/test_routing/test_validations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/__init__.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/conftest.py
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_cache_control_headers.py
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_exceptions.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_hello_world.py
+-rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_lifecycle_hooks.py
+-rw-r--r--   0        0        0     4447 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_request_data.py
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_routing.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_signature_namespace.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_startup_and_shutdown.py
+-rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_static_files.py
+-rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_stores.py
+-rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_todo_app.py
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_using_session_auth.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_websockets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_application_hooks/__init__.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_application_hooks/test_application_after_exception_hook.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_application_hooks/test_application_before_send.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_application_hooks/test_lifespan_manager.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_application_hooks/test_on_app_init.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_application_state/__init__.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_application_state/test_passing_initial_state.py
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_application_state/test_using_application_state.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_application_state/test_using_custom_state.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_application_state/test_using_immutable_state.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_contrib/__init__.py
+-rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_contrib/test_piccolo_orm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_contrib/prometheus/__init__.py
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_contrib/prometheus/test_prometheus_exporter_example.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_contrib/prometheus/test_prometheus_exporter_example_with_extra_config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_contrib/test_sqlalchemy/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_contrib/test_sqlalchemy/plugins/__init__.py
+-rw-r--r--   0        0        0     5889 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_contrib/test_sqlalchemy/plugins/test_example_apps.py
+-rw-r--r--   0        0        0     2480 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_contrib/test_sqlalchemy/plugins/test_tutorial_example_apps.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_dependency_injection/__init__.py
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_dependency_injection/test_dependency_default_value_no_dependency_fn.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_dependency_injection/test_dependency_default_value_with_dependency_fn.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_dependency_injection/test_dependency_skip_validation.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_dependency_injection/test_dependency_validation_error.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_dependency_injection/tests_dependency_non_optional_not_provided.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_dto/__init__.py
+-rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_dto/test_example_apps.py
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_dto/test_tutorial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_middleware/__init__.py
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_middleware/test_abstract_middleware.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_middleware/test_call_order.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_middleware/test_logging_middleware.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_middleware/test_rate_limit_middleware.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_middleware/test_session_middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_openapi/__init__.py
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_openapi/test_openapi.py
+-rw-r--r--   0        0        0     4267 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_openapi/test_plugins.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_pagination/__init__.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_pagination/test_using_classic_pagination.py
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_pagination/test_using_cursor_pagination.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_pagination/test_using_offset_pagination.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_parameters/__init__.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_parameters/test_header_and_cookies_parameters.py
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_parameters/test_layered_parameters.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_parameters/test_path_parameters.py
+-rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_parameters/test_query_parameters.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_plugins/__init__.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_plugins/test_di_plugin.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_plugins/test_example_apps.py
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_plugins/test_sqlalchemy_init_plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_responses/__init__.py
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_responses/test_background_tasks.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_responses/test_custom_responses.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_responses/test_json_suffix_responses.py
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_responses/test_response_cookies.py
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_responses/test_response_headers.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_responses/test_returning_responses.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_responses/test_sse_responses.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_security/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_security/test_jwt/__init__.py
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_security/test_jwt/test_using_jwt_auth.py
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_security/test_jwt/test_using_jwt_cookie_auth.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_security/test_jwt/test_using_oauth2_password_bearer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_templating/__init__.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_templating/test_engine_instance.py
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_templating/test_returning_templates.py
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/examples/test_templating/test_template_functions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/__init__.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/conftest.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/piccolo_conf.py
+-rw-r--r--   0        0        0    15242 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_app.py
+-rw-r--r--   0        0        0     7296 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_asgi_router.py
+-rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_background_tasks.py
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_concurrency.py
+-rw-r--r--   0        0        0     3854 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_controller.py
+-rw-r--r--   0        0        0     6006 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_data_extractors.py
+-rw-r--r--   0        0        0     4933 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_deprecations.py
+-rw-r--r--   0        0        0     4606 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_di.py
+-rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_events.py
+-rw-r--r--   0        0        0     8341 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_exceptions.py
+-rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_file_system.py
+-rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_guards.py
+-rw-r--r--   0        0        0    11592 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_pagination.py
+-rw-r--r--   0        0        0    11015 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_params.py
+-rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_parsers.py
+-rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_request_class_resolution.py
+-rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_response_class_resolution.py
+-rw-r--r--   0        0        0    13025 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_stores.py
+-rw-r--r--   0        0        0    17322 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_typing.py
+-rw-r--r--   0        0        0     4516 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_websocket_class_resolution.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_channels/__init__.py
+-rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_channels/conftest.py
+-rw-r--r--   0        0        0     8672 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_channels/test_backends.py
+-rw-r--r--   0        0        0    16493 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_channels/test_plugin.py
+-rw-r--r--   0        0        0     3542 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_channels/test_subscriber.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_channels/util.py
+-rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_cli/__init__.py
+-rw-r--r--   0        0        0     4932 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_cli/conftest.py
+-rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_cli/test_cli.py
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_cli/test_cli_plugin.py
+-rw-r--r--   0        0        0    23147 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_cli/test_core_commands.py
+-rw-r--r--   0        0        0     4294 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_cli/test_env_resolution.py
+-rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_cli/test_schema_commands.py
+-rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_cli/test_session_commands.py
+-rw-r--r--   0        0        0     9784 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_cli/test_ssl.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_connection/__init__.py
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_connection/test_base.py
+-rw-r--r--   0        0        0     7225 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_connection/test_connection_caching.py
+-rw-r--r--   0        0        0    19442 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_connection/test_request.py
+-rw-r--r--   0        0        0    14929 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_connection/test_websocket.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_contrib/__init__.py
+-rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_contrib/conftest.py
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_contrib/test_minijinja.py
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_contrib/test_msgspec.py
+-rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_contrib/test_opentelemetry.py
+-rw-r--r--   0        0        0     7545 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_contrib/test_prometheus.py
+-rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_contrib/test_repository.py
+-rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_contrib/test_sqlalchemy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_contrib/test_attrs/__init__.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_contrib/test_attrs/test_inject_attrs_class.py
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_contrib/test_attrs/test_schema_plugin.py
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_contrib/test_attrs/test_schema_spec_generation.py
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_contrib/test_attrs/test_signature.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_contrib/test_htmx/__init__.py
+-rw-r--r--   0        0        0    10431 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_contrib/test_htmx/test_htmx_request.py
+-rw-r--r--   0        0        0    13872 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_contrib/test_htmx/test_htmx_response.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_contrib/test_piccolo_orm/__init__.py
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_contrib/test_piccolo_orm/endpoints.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_contrib/test_piccolo_orm/piccolo_app.py
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_contrib/test_piccolo_orm/tables.py
+-rw-r--r--   0        0        0     6298 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_contrib/test_piccolo_orm/test_piccolo_orm_dto.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_contrib/test_pydantic/__init__.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_contrib/test_pydantic/conftest.py
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_contrib/test_pydantic/models.py
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_contrib/test_pydantic/test_beanie_integration.py
+-rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_contrib/test_pydantic/test_dto.py
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_contrib/test_pydantic/test_inject_pydantic.py
+-rw-r--r--   0        0        0    11001 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_contrib/test_pydantic/test_integration.py
+-rw-r--r--   0        0        0    29005 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_contrib/test_pydantic/test_openapi.py
+-rw-r--r--   0        0        0     9126 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_contrib/test_pydantic/test_plugin_serialization.py
+-rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_contrib/test_pydantic/test_pydantic_dto_factory.py
+-rw-r--r--   0        0        0     5138 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_contrib/test_pydantic/test_schema_plugin.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_contrib/test_pydantic/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_datastructures/__init_.py
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_datastructures/test_cookie.py
+-rw-r--r--   0        0        0    13358 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_datastructures/test_headers.py
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_datastructures/test_multi_dicts.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_datastructures/test_response_header.py
+-rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_datastructures/test_state.py
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_datastructures/test_upload_file.py
+-rw-r--r--   0        0        0     3672 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_datastructures/test_url.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_dto/__init__.py
+-rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_dto/conftest.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_dto/test_config.py
+-rw-r--r--   0        0        0     5943 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_dto/test_integration.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_dto/test_interface.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_dto/test_factory/__init__.py
+-rw-r--r--   0        0        0     5259 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_dto/test_factory/test_base_dto.py
+-rw-r--r--   0        0        0     4464 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_dto/test_factory/test_dataclass_dto.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_dto/test_factory/test_field.py
+-rw-r--r--   0        0        0    30290 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_dto/test_factory/test_integration.py
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_dto/test_factory/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_dto/test_factory/test_backends/__init__.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_dto/test_factory/test_backends/conftest.py
+-rw-r--r--   0        0        0    16326 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_dto/test_factory/test_backends/test_backends.py
+-rw-r--r--   0        0        0    10244 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_dto/test_factory/test_backends/test_base_dto.py
+-rw-r--r--   0        0        0     7630 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_dto/test_factory/test_backends/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_handlers/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_handlers/test_asgi_handlers/__init__.py
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_handlers/test_asgi_handlers/test_handle_asgi.py
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_handlers/test_asgi_handlers/test_handle_asgi_with_future_annotations.py
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_handlers/test_asgi_handlers/test_validations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_handlers/test_base_handlers/__init__.py
+-rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_handlers/test_base_handlers/test_opt.py
+-rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_handlers/test_base_handlers/test_resolution.py
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_handlers/test_base_handlers/test_validations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_handlers/test_http_handlers/__init__.py
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_handlers/test_http_handlers/test_defaults.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_handlers/test_http_handlers/test_delete.py
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_handlers/test_http_handlers/test_head.py
+-rw-r--r--   0        0        0     3165 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_handlers/test_http_handlers/test_kwarg_handling.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_handlers/test_http_handlers/test_media_type.py
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_handlers/test_http_handlers/test_signature_namespace.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_handlers/test_http_handlers/test_sync.py
+-rw-r--r--   0        0        0     4437 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_handlers/test_http_handlers/test_validations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_handlers/test_websocket_handlers/__init__.py
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_handlers/test_websocket_handlers/test_handle_websocket.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_handlers/test_websocket_handlers/test_handle_websocket_with_future_annotations.py
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_handlers/test_websocket_handlers/test_kwarg_handling.py
+-rw-r--r--   0        0        0    14396 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_handlers/test_websocket_handlers/test_listeners.py
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_handlers/test_websocket_handlers/test_validations.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_kwargs/__init__.py
+-rw-r--r--   0        0        0    72895 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_kwargs/flower.jpeg
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_kwargs/test_cleanup_group.py
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_kwargs/test_cookie_params.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_kwargs/test_defaults.py
+-rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_kwargs/test_dependency_batches.py
+-rw-r--r--   0        0        0     7259 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_kwargs/test_generator_dependencies.py
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_kwargs/test_header_params.py
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_kwargs/test_json_data.py
+-rw-r--r--   0        0        0     8662 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_kwargs/test_layered_params.py
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_kwargs/test_msgpack_data.py
+-rw-r--r--   0        0        0    21924 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_kwargs/test_multipart_data.py
+-rw-r--r--   0        0        0     6592 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_kwargs/test_path_params.py
+-rw-r--r--   0        0        0     6666 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_kwargs/test_query_params.py
+-rw-r--r--   0        0        0     9794 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_kwargs/test_reserved_kwargs_injection.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_kwargs/test_url_encoded_data.py
+-rw-r--r--   0        0        0     4372 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_kwargs/test_validations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_logging/__init__.py
+-rw-r--r--   0        0        0     9198 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_logging/test_logging_config.py
+-rw-r--r--   0        0        0     7083 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_logging/test_structlog_config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_middleware/__init__.py
+-rw-r--r--   0        0        0     5873 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_middleware/test_allowed_hosts_middleware.py
+-rw-r--r--   0        0        0     8644 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_middleware/test_base_authentication_middleware.py
+-rw-r--r--   0        0        0     5095 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_middleware/test_base_middleware.py
+-rw-r--r--   0        0        0    11412 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_middleware/test_compression_middleware.py
+-rw-r--r--   0        0        0     5506 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_middleware/test_cors_middleware.py
+-rw-r--r--   0        0        0     9446 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_middleware/test_csrf_middleware.py
+-rw-r--r--   0        0        0    14919 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_middleware/test_exception_handler_middleware.py
+-rw-r--r--   0        0        0    12163 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_middleware/test_logging_middleware.py
+-rw-r--r--   0        0        0     5821 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_middleware/test_middleware_handling.py
+-rw-r--r--   0        0        0     7846 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_middleware/test_rate_limit_middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_middleware/test_session/__init__.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_middleware/test_session/conftest.py
+-rw-r--r--   0        0        0     8354 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_middleware/test_session/test_client_side_backend.py
+-rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_middleware/test_session/test_integration.py
+-rw-r--r--   0        0        0     8726 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_middleware/test_session/test_middleware.py
+-rw-r--r--   0        0        0     5444 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_middleware/test_session/test_server_side_backend.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_openapi/__init__.py
+-rw-r--r--   0        0        0     5595 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_openapi/conftest.py
+-rw-r--r--   0        0        0     4373 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_openapi/test_config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_openapi/test_constrained_fields.py
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_openapi/test_datastructures.py
+-rw-r--r--   0        0        0    20213 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_openapi/test_endpoints.py
+-rw-r--r--   0        0        0    20582 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_openapi/test_integration.py
+-rw-r--r--   0        0        0    13925 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_openapi/test_parameters.py
+-rw-r--r--   0        0        0     9934 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_openapi/test_path_item.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_openapi/test_render_plugins.py
+-rw-r--r--   0        0        0     6233 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_openapi/test_request_body.py
+-rw-r--r--   0        0        0    20422 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_openapi/test_responses.py
+-rw-r--r--   0        0        0    22306 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_openapi/test_schema.py
+-rw-r--r--   0        0        0     4561 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_openapi/test_security_schemes.py
+-rw-r--r--   0        0        0     6434 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_openapi/test_spec_generation.py
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_openapi/test_tags.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_openapi/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_openapi/test_typescript_converter/__init__.py
+-rw-r--r--   0        0        0     8625 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_openapi/test_typescript_converter/test_converter.py
+-rw-r--r--   0        0        0     3176 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_openapi/test_typescript_converter/test_schema_parsing.py
+-rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_openapi/test_typescript_converter/test_typescript_types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_plugins/__init__.py
+-rw-r--r--   0        0        0     5114 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_plugins/test_base.py
+-rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_plugins/test_flash.py
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_plugins/test_sqlalchemy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_repository/__init__.py
+-rw-r--r--   0        0        0     4732 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_repository/models_bigint.py
+-rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_repository/models_uuid.py
+-rw-r--r--   0        0        0    18932 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_repository/test_generic_mock_repository.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_response/__init__.py
+-rw-r--r--   0        0        0     7676 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_response/test_base_response.py
+-rw-r--r--   0        0        0    11238 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_response/test_file_response.py
+-rw-r--r--   0        0        0     4418 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_response/test_redirect_response.py
+-rw-r--r--   0        0        0     5170 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_response/test_response_cookies.py
+-rw-r--r--   0        0        0     6433 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_response/test_response_headers.py
+-rw-r--r--   0        0        0    16365 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_response/test_response_to_asgi_response.py
+-rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_response/test_serialization.py
+-rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_response/test_sse.py
+-rw-r--r--   0        0        0     6247 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_response/test_streaming_response.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_response/test_type_decoders.py
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_response/test_type_encoders.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_security/__init__.py
+-rw-r--r--   0        0        0     7076 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_security/test_security.py
+-rw-r--r--   0        0        0     3728 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_security/test_session_auth.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_security/test_jwt/__init__.py
+-rw-r--r--   0        0        0    18293 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_security/test_jwt/test_auth.py
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_security/test_jwt/test_integration.py
+-rw-r--r--   0        0        0     5443 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_security/test_jwt/test_token.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_signature/__init__.py
+-rw-r--r--   0        0        0     6896 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_signature/test_parsing.py
+-rw-r--r--   0        0        0     9475 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_signature/test_validation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_static_files/__init__.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_static_files/conftest.py
+-rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_static_files/test_create_static_router.py
+-rw-r--r--   0        0        0    11768 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_static_files/test_file_serving_resolution.py
+-rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_static_files/test_html_mode.py
+-rw-r--r--   0        0        0     4186 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_static_files/test_static_files_validation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_template/__init__.py
+-rw-r--r--   0        0        0     6440 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_template/test_built_in.py
+-rw-r--r--   0        0        0    11615 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_template/test_builtin_functions.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_template/test_config.py
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_template/test_context.py
+-rw-r--r--   0        0        0     2634 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_template/test_csrf_token.py
+-rw-r--r--   0        0        0     7401 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_template/test_template.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_testing/__init__.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_testing/test_lifespan_handler.py
+-rw-r--r--   0        0        0     7205 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_testing/test_request_factory.py
+-rw-r--r--   0        0        0     9945 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_testing/test_test_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_types/__init__.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_types/test_protocols.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_utils/__init__.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_utils/test_compat.py
+-rw-r--r--   0        0        0     4367 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_utils/test_dataclass.py
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_utils/test_deprecation.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_utils/test_helpers.py
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_utils/test_module_loader.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_utils/test_path.py
+-rw-r--r--   0        0        0     7229 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_utils/test_predicates.py
+-rw-r--r--   0        0        0     2750 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_utils/test_scope.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_utils/test_sequence.py
+-rw-r--r--   0        0        0     7921 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_utils/test_signature.py
+-rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_utils/test_sync.py
+-rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_utils/test_typing.py
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 litestar-2.8.1/tests/unit/test_utils/test_version.py
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 litestar-2.8.1/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 litestar-2.8.1/LICENSE
+-rw-r--r--   0        0        0    92575 2020-02-02 00:00:00.000000 litestar-2.8.1/README.md
+-rw-r--r--   0        0        0    12698 2020-02-02 00:00:00.000000 litestar-2.8.1/pyproject.toml
+-rw-r--r--   0        0        0    97593 2020-02-02 00:00:00.000000 litestar-2.8.1/PKG-INFO
```

### Comparing `litestar-2.8.0/Makefile` & `litestar-2.8.1/Makefile`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/docs/PYPI_README.md` & `litestar-2.8.1/docs/PYPI_README.md`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/__init__.py` & `litestar-2.8.1/litestar/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/_multipart.py` & `litestar-2.8.1/litestar/_multipart.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/_parsers.py` & `litestar-2.8.1/litestar/_parsers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/app.py` & `litestar-2.8.1/litestar/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -666,15 +666,16 @@
             for route_handler in route_handlers:
                 route_handler.on_registration(self)
 
             if isinstance(route, HTTPRoute):
                 route.create_handler_map()
 
             elif isinstance(route, WebSocketRoute):
-                route.handler_parameter_model = route.create_handler_kwargs_model(route.route_handler)
+                handler = route.route_handler
+                route.handler_parameter_model = handler.create_kwargs_model(path_parameters=route.path_parameters)
 
             for plugin in self.plugins.receive_route:
                 plugin.receive_route(route)
 
         self.asgi_router.construct_routing_trie()
 
     def get_handler_index_by_name(self, name: str) -> HandlerIndex | None:
@@ -755,19 +756,15 @@
             self.asgi_router.route_mapping[handler_index["identifier"]],
             key=lambda r: len(r.path_parameters),
             reverse=True,
         )
         passed_parameters = set(path_parameters.keys())
 
         selected_route = next(
-            (
-                route
-                for route in routes
-                if passed_parameters.issuperset({param.name for param in route.path_parameters})
-            ),
+            (route for route in routes if passed_parameters.issuperset(route.path_parameters)),
             routes[-1],
         )
         output: list[str] = []
         for component in selected_route.path_components:
             if isinstance(component, PathParameterDefinition):
                 val = path_parameters.get(component.name)
                 if not isinstance(val, component.type) and (
```

### Comparing `litestar-2.8.0/litestar/background_tasks.py` & `litestar-2.8.1/litestar/background_tasks.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/concurrency.py` & `litestar-2.8.1/litestar/concurrency.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/constants.py` & `litestar-2.8.1/litestar/constants.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/controller.py` & `litestar-2.8.1/litestar/controller.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/data_extractors.py` & `litestar-2.8.1/litestar/data_extractors.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/di.py` & `litestar-2.8.1/litestar/di.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/enums.py` & `litestar-2.8.1/litestar/enums.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/file_system.py` & `litestar-2.8.1/litestar/file_system.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/pagination.py` & `litestar-2.8.1/litestar/pagination.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/params.py` & `litestar-2.8.1/litestar/params.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/router.py` & `litestar-2.8.1/litestar/router.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/status_codes.py` & `litestar-2.8.1/litestar/status_codes.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/typing.py` & `litestar-2.8.1/litestar/typing.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/_asgi/asgi_router.py` & `litestar-2.8.1/litestar/_asgi/asgi_router.py`

 * *Files 8% similar despite different names*

```diff
@@ -154,31 +154,32 @@
         Args:
             receive: The ASGI receive function.
             send: The ASGI send function.
 
         Returns:
             None.
         """
-
-        message = await receive()
         shutdown_event: LifeSpanShutdownCompleteEvent = {"type": "lifespan.shutdown.complete"}
         startup_event: LifeSpanStartupCompleteEvent = {"type": "lifespan.startup.complete"}
 
+        await receive()
+
+        started = False
         try:
             async with self.app.lifespan():
                 await send(startup_event)
-                message = await receive()
+                started = True
+                await receive()
 
         except BaseException as e:
             formatted_exception = format_exc()
             failure_message: LifeSpanStartupFailedEvent | LifeSpanShutdownFailedEvent
 
-            if message["type"] == "lifespan.startup":
-                failure_message = {"type": "lifespan.startup.failed", "message": formatted_exception}
-            else:
+            if started:
                 failure_message = {"type": "lifespan.shutdown.failed", "message": formatted_exception}
+            else:
+                failure_message = {"type": "lifespan.startup.failed", "message": formatted_exception}
 
             await send(failure_message)
-
             raise e
 
         await send(shutdown_event)
```

### Comparing `litestar-2.8.0/litestar/_asgi/utils.py` & `litestar-2.8.1/litestar/_asgi/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/_asgi/routing_trie/mapping.py` & `litestar-2.8.1/litestar/_asgi/routing_trie/mapping.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,29 +146,29 @@
     if isinstance(route, HTTPRoute):
         for method, handler_mapping in route.route_handler_map.items():
             handler, _ = handler_mapping
             node.asgi_handlers[method] = ASGIHandlerTuple(
                 asgi_app=build_route_middleware_stack(app=app, route=route, route_handler=handler),
                 handler=handler,
             )
-            node.path_parameters[method] = route.path_parameters
+            node.path_parameters[method] = tuple(route.path_parameters.values())
 
     elif isinstance(route, WebSocketRoute):
         node.asgi_handlers["websocket"] = ASGIHandlerTuple(
             asgi_app=build_route_middleware_stack(app=app, route=route, route_handler=route.route_handler),
             handler=route.route_handler,
         )
-        node.path_parameters["websocket"] = route.path_parameters
+        node.path_parameters["websocket"] = tuple(route.path_parameters.values())
 
     else:
         node.asgi_handlers["asgi"] = ASGIHandlerTuple(
             asgi_app=build_route_middleware_stack(app=app, route=route, route_handler=route.route_handler),
             handler=route.route_handler,
         )
-        node.path_parameters["asgi"] = route.path_parameters
+        node.path_parameters["asgi"] = tuple(route.path_parameters.values())
         node.is_asgi = True
 
 
 def build_route_middleware_stack(
     app: Litestar,
     route: HTTPRoute | WebSocketRoute | ASGIRoute,
     route_handler: RouteHandlerType,
```

### Comparing `litestar-2.8.0/litestar/_asgi/routing_trie/traversal.py` & `litestar-2.8.1/litestar/_asgi/routing_trie/traversal.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/_asgi/routing_trie/types.py` & `litestar-2.8.1/litestar/_asgi/routing_trie/types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/_asgi/routing_trie/validate.py` & `litestar-2.8.1/litestar/_asgi/routing_trie/validate.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/_kwargs/cleanup.py` & `litestar-2.8.1/litestar/_kwargs/cleanup.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/_kwargs/dependencies.py` & `litestar-2.8.1/litestar/_kwargs/dependencies.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/_kwargs/extractors.py` & `litestar-2.8.1/litestar/_kwargs/extractors.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/_kwargs/kwargs_model.py` & `litestar-2.8.1/litestar/_kwargs/kwargs_model.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/_kwargs/parameter_definition.py` & `litestar-2.8.1/litestar/_kwargs/parameter_definition.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/_layers/utils.py` & `litestar-2.8.1/litestar/_layers/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/_openapi/datastructures.py` & `litestar-2.8.1/litestar/_openapi/datastructures.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/_openapi/parameters.py` & `litestar-2.8.1/litestar/_openapi/parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,30 +77,30 @@
 class ParameterFactory:
     """Factory for creating OpenAPI Parameters for a given route handler."""
 
     def __init__(
         self,
         context: OpenAPIContext,
         route_handler: BaseRouteHandler,
-        path_parameters: tuple[PathParameterDefinition, ...],
+        path_parameters: dict[str, PathParameterDefinition],
     ) -> None:
         """Initialize ParameterFactory.
 
         Args:
             context: The OpenAPI context.
             route_handler: The route handler.
             path_parameters: The path parameters for the route.
         """
         self.context = context
         self.schema_creator = SchemaCreator.from_openapi_context(self.context, prefer_alias=True)
         self.route_handler = route_handler
         self.parameters = ParameterCollection(route_handler)
         self.dependency_providers = route_handler.resolve_dependencies()
         self.layered_parameters = route_handler.resolve_layered_parameters()
-        self.path_parameters: dict[str, PathParameterDefinition] = {p.name: p for p in path_parameters}
+        self.path_parameters = path_parameters
 
     def create_parameter(self, field_definition: FieldDefinition, parameter_name: str) -> Parameter:
         """Create an OpenAPI Parameter instance for a field definition.
 
         Args:
             field_definition: The field definition.
             parameter_name: The name of the parameter.
@@ -229,15 +229,15 @@
         self.create_parameters_for_field_definitions(handler_fields)
         return self.parameters.list()
 
 
 def create_parameters_for_handler(
     context: OpenAPIContext,
     route_handler: BaseRouteHandler,
-    path_parameters: tuple[PathParameterDefinition, ...],
+    path_parameters: dict[str, PathParameterDefinition],
 ) -> list[Parameter]:
     """Create a list of path/query/header Parameter models for the given PathHandler."""
     factory = ParameterFactory(
         context=context,
         route_handler=route_handler,
         path_parameters=path_parameters,
     )
```

### Comparing `litestar-2.8.0/litestar/_openapi/path_item.py` & `litestar-2.8.1/litestar/_openapi/path_item.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/_openapi/plugin.py` & `litestar-2.8.1/litestar/_openapi/plugin.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/_openapi/request_body.py` & `litestar-2.8.1/litestar/_openapi/request_body.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/_openapi/responses.py` & `litestar-2.8.1/litestar/_openapi/responses.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/_openapi/utils.py` & `litestar-2.8.1/litestar/_openapi/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/_openapi/schema_generation/constrained_fields.py` & `litestar-2.8.1/litestar/_openapi/schema_generation/constrained_fields.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/_openapi/schema_generation/examples.py` & `litestar-2.8.1/litestar/_openapi/schema_generation/examples.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/_openapi/schema_generation/schema.py` & `litestar-2.8.1/litestar/_openapi/schema_generation/schema.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/_openapi/schema_generation/utils.py` & `litestar-2.8.1/litestar/_openapi/schema_generation/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/_openapi/schema_generation/plugins/__init__.py` & `litestar-2.8.1/litestar/_openapi/schema_generation/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/_openapi/schema_generation/plugins/dataclass.py` & `litestar-2.8.1/litestar/_openapi/schema_generation/plugins/dataclass.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/_openapi/schema_generation/plugins/pagination.py` & `litestar-2.8.1/litestar/_openapi/schema_generation/plugins/pagination.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/_openapi/schema_generation/plugins/struct.py` & `litestar-2.8.1/litestar/_openapi/schema_generation/plugins/struct.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/_openapi/schema_generation/plugins/typed_dict.py` & `litestar-2.8.1/litestar/_openapi/schema_generation/plugins/typed_dict.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/_openapi/typescript_converter/converter.py` & `litestar-2.8.1/litestar/_openapi/typescript_converter/converter.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/_openapi/typescript_converter/schema_parsing.py` & `litestar-2.8.1/litestar/_openapi/typescript_converter/schema_parsing.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/_openapi/typescript_converter/types.py` & `litestar-2.8.1/litestar/_openapi/typescript_converter/types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/_signature/model.py` & `litestar-2.8.1/litestar/_signature/model.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/_signature/utils.py` & `litestar-2.8.1/litestar/_signature/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/channels/plugin.py` & `litestar-2.8.1/litestar/channels/plugin.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/channels/subscriber.py` & `litestar-2.8.1/litestar/channels/subscriber.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/channels/backends/asyncpg.py` & `litestar-2.8.1/litestar/channels/backends/asyncpg.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/channels/backends/base.py` & `litestar-2.8.1/litestar/channels/backends/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/channels/backends/memory.py` & `litestar-2.8.1/litestar/channels/backends/memory.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/channels/backends/psycopg.py` & `litestar-2.8.1/litestar/channels/backends/psycopg.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/channels/backends/redis.py` & `litestar-2.8.1/litestar/channels/backends/redis.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/cli/__init__.py` & `litestar-2.8.1/litestar/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/cli/_utils.py` & `litestar-2.8.1/litestar/cli/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/cli/main.py` & `litestar-2.8.1/litestar/cli/main.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/cli/commands/core.py` & `litestar-2.8.1/litestar/cli/commands/core.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/cli/commands/schema.py` & `litestar-2.8.1/litestar/cli/commands/schema.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/cli/commands/sessions.py` & `litestar-2.8.1/litestar/cli/commands/sessions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/config/allowed_hosts.py` & `litestar-2.8.1/litestar/config/allowed_hosts.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/config/app.py` & `litestar-2.8.1/litestar/config/app.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/config/compression.py` & `litestar-2.8.1/litestar/config/compression.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/config/cors.py` & `litestar-2.8.1/litestar/config/cors.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/config/csrf.py` & `litestar-2.8.1/litestar/config/csrf.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/config/response_cache.py` & `litestar-2.8.1/litestar/config/response_cache.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/connection/__init__.py` & `litestar-2.8.1/litestar/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/connection/base.py` & `litestar-2.8.1/litestar/connection/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/connection/request.py` & `litestar-2.8.1/litestar/connection/request.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/connection/websocket.py` & `litestar-2.8.1/litestar/connection/websocket.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/contrib/jinja.py` & `litestar-2.8.1/litestar/contrib/jinja.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/contrib/mako.py` & `litestar-2.8.1/litestar/contrib/mako.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/contrib/minijinja.py` & `litestar-2.8.1/litestar/contrib/minijinja.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/contrib/piccolo.py` & `litestar-2.8.1/litestar/contrib/piccolo.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/contrib/attrs/attrs_schema_plugin.py` & `litestar-2.8.1/litestar/contrib/attrs/attrs_schema_plugin.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/contrib/htmx/_utils.py` & `litestar-2.8.1/litestar/contrib/htmx/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/contrib/htmx/request.py` & `litestar-2.8.1/litestar/contrib/htmx/request.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/contrib/htmx/response.py` & `litestar-2.8.1/litestar/contrib/htmx/response.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/contrib/htmx/types.py` & `litestar-2.8.1/litestar/contrib/htmx/types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/contrib/jwt/__init__.py` & `litestar-2.8.1/litestar/contrib/jwt/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/contrib/opentelemetry/_utils.py` & `litestar-2.8.1/litestar/contrib/opentelemetry/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/contrib/opentelemetry/config.py` & `litestar-2.8.1/litestar/contrib/opentelemetry/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/contrib/opentelemetry/middleware.py` & `litestar-2.8.1/litestar/contrib/opentelemetry/middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/contrib/prometheus/config.py` & `litestar-2.8.1/litestar/contrib/prometheus/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/contrib/prometheus/controller.py` & `litestar-2.8.1/litestar/contrib/prometheus/controller.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/contrib/prometheus/middleware.py` & `litestar-2.8.1/litestar/contrib/prometheus/middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/contrib/pydantic/__init__.py` & `litestar-2.8.1/litestar/contrib/pydantic/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/contrib/pydantic/pydantic_di_plugin.py` & `litestar-2.8.1/litestar/contrib/pydantic/pydantic_di_plugin.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/contrib/pydantic/pydantic_dto_factory.py` & `litestar-2.8.1/litestar/contrib/pydantic/pydantic_dto_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,26 +42,32 @@
 
 
 T = TypeVar("T", bound="ModelType | Collection[ModelType]")
 
 
 __all__ = ("PydanticDTO",)
 
-_down_types = {
-    pydantic_v2.JsonValue: Any,
+_down_types: dict[Any, Any] = {
     pydantic_v1.EmailStr: str,
-    pydantic_v2.EmailStr: str,
     pydantic_v1.IPvAnyAddress: str,
-    pydantic_v2.IPvAnyAddress: str,
     pydantic_v1.IPvAnyInterface: str,
-    pydantic_v2.IPvAnyInterface: str,
     pydantic_v1.IPvAnyNetwork: str,
-    pydantic_v2.IPvAnyNetwork: str,
 }
 
+if pydantic_v2 is not Empty:  # type: ignore[comparison-overlap]  # pragma: no cover
+    _down_types.update(
+        {
+            pydantic_v2.JsonValue: Any,
+            pydantic_v2.EmailStr: str,
+            pydantic_v2.IPvAnyAddress: str,
+            pydantic_v2.IPvAnyInterface: str,
+            pydantic_v2.IPvAnyNetwork: str,
+        }
+    )
+
 
 def convert_validation_error(validation_error: ValidationErrorV1 | ValidationErrorV2) -> list[dict[str, Any]]:
     error_list = validation_error.errors()
     for error in error_list:
         if isinstance(exception := error.get("ctx", {}).get("error"), Exception):
             error["ctx"]["error"] = type(exception).__name__
     return error_list  # type: ignore[return-value]
```

### Comparing `litestar-2.8.0/litestar/contrib/pydantic/pydantic_init_plugin.py` & `litestar-2.8.1/litestar/contrib/pydantic/pydantic_init_plugin.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/contrib/pydantic/pydantic_schema_plugin.py` & `litestar-2.8.1/litestar/contrib/pydantic/pydantic_schema_plugin.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/contrib/pydantic/utils.py` & `litestar-2.8.1/litestar/contrib/pydantic/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/contrib/repository/__init__.py` & `litestar-2.8.1/litestar/contrib/repository/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/contrib/repository/exceptions.py` & `litestar-2.8.1/litestar/contrib/repository/exceptions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/contrib/repository/filters.py` & `litestar-2.8.1/litestar/contrib/repository/filters.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/contrib/repository/handlers.py` & `litestar-2.8.1/litestar/contrib/repository/handlers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/contrib/repository/testing.py` & `litestar-2.8.1/litestar/contrib/repository/testing.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/contrib/repository/abc/__init__.py` & `litestar-2.8.1/litestar/contrib/repository/abc/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/contrib/sqlalchemy/base.py` & `litestar-2.8.1/litestar/contrib/sqlalchemy/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/contrib/sqlalchemy/plugins/__init__.py` & `litestar-2.8.1/litestar/contrib/sqlalchemy/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/contrib/sqlalchemy/plugins/init/config/asyncio.py` & `litestar-2.8.1/litestar/contrib/sqlalchemy/plugins/init/config/asyncio.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/contrib/sqlalchemy/plugins/init/config/compat.py` & `litestar-2.8.1/litestar/contrib/sqlalchemy/plugins/init/config/compat.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/contrib/sqlalchemy/plugins/init/config/sync.py` & `litestar-2.8.1/litestar/contrib/sqlalchemy/plugins/init/config/sync.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/datastructures/__init__.py` & `litestar-2.8.1/litestar/datastructures/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/datastructures/cookie.py` & `litestar-2.8.1/litestar/datastructures/cookie.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/datastructures/headers.py` & `litestar-2.8.1/litestar/datastructures/headers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/datastructures/multi_dicts.py` & `litestar-2.8.1/litestar/datastructures/multi_dicts.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/datastructures/response_header.py` & `litestar-2.8.1/litestar/datastructures/response_header.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/datastructures/state.py` & `litestar-2.8.1/litestar/datastructures/state.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/datastructures/upload_file.py` & `litestar-2.8.1/litestar/datastructures/upload_file.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/datastructures/url.py` & `litestar-2.8.1/litestar/datastructures/url.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/dto/_backend.py` & `litestar-2.8.1/litestar/dto/_backend.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/dto/_codegen_backend.py` & `litestar-2.8.1/litestar/dto/_codegen_backend.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/dto/_types.py` & `litestar-2.8.1/litestar/dto/_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/dto/base_dto.py` & `litestar-2.8.1/litestar/dto/base_dto.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/dto/config.py` & `litestar-2.8.1/litestar/dto/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/dto/data_structures.py` & `litestar-2.8.1/litestar/dto/data_structures.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/dto/dataclass_dto.py` & `litestar-2.8.1/litestar/dto/dataclass_dto.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/dto/field.py` & `litestar-2.8.1/litestar/dto/field.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/dto/msgspec_dto.py` & `litestar-2.8.1/litestar/dto/msgspec_dto.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/events/emitter.py` & `litestar-2.8.1/litestar/events/emitter.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/events/listener.py` & `litestar-2.8.1/litestar/events/listener.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/exceptions/__init__.py` & `litestar-2.8.1/litestar/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/exceptions/base_exceptions.py` & `litestar-2.8.1/litestar/exceptions/base_exceptions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/exceptions/http_exceptions.py` & `litestar-2.8.1/litestar/exceptions/http_exceptions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/exceptions/websocket_exceptions.py` & `litestar-2.8.1/litestar/exceptions/websocket_exceptions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/handlers/__init__.py` & `litestar-2.8.1/litestar/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/handlers/asgi_handlers.py` & `litestar-2.8.1/litestar/handlers/asgi_handlers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/handlers/base.py` & `litestar-2.8.1/litestar/handlers/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,22 +23,24 @@
 from litestar.utils import ensure_async_callable, get_name, normalize_path
 from litestar.utils.helpers import unwrap_partial
 from litestar.utils.signature import ParsedSignature, add_types_to_signature_namespace
 
 if TYPE_CHECKING:
     from typing_extensions import Self
 
+    from litestar._kwargs import KwargsModel
     from litestar.app import Litestar
     from litestar.connection import ASGIConnection
     from litestar.controller import Controller
     from litestar.dto import AbstractDTO
     from litestar.params import ParameterKwarg
     from litestar.router import Router
     from litestar.types import AnyCallable, AsyncAnyCallable, ExceptionHandler
     from litestar.types.empty import EmptyType
+    from litestar.types.internal_types import PathParameterDefinition
 
 __all__ = ("BaseRouteHandler",)
 
 
 class BaseRouteHandler:
     """Base route handler.
 
@@ -560,7 +562,22 @@
             A string
         """
         target: type[AsyncAnyCallable] | AsyncAnyCallable  # pyright: ignore
         target = unwrap_partial(self.fn)
         if not hasattr(target, "__qualname__"):
             target = type(target)
         return f"{target.__module__}.{target.__qualname__}"
+
+    def create_kwargs_model(
+        self,
+        path_parameters: dict[str, PathParameterDefinition],
+    ) -> KwargsModel:
+        """Create a `KwargsModel` for a given route handler."""
+        from litestar._kwargs import KwargsModel
+
+        return KwargsModel.create_for_signature_model(
+            signature_model=self.signature_model,
+            parsed_signature=self.parsed_fn_signature,
+            dependencies=self.resolve_dependencies(),
+            path_parameters=set(path_parameters.keys()),
+            layered_parameters=self.resolve_layered_parameters(),
+        )
```

### Comparing `litestar-2.8.0/litestar/handlers/http_handlers/_utils.py` & `litestar-2.8.1/litestar/handlers/http_handlers/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/handlers/http_handlers/base.py` & `litestar-2.8.1/litestar/handlers/http_handlers/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/handlers/http_handlers/decorators.py` & `litestar-2.8.1/litestar/handlers/http_handlers/decorators.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/handlers/websocket_handlers/_utils.py` & `litestar-2.8.1/litestar/handlers/websocket_handlers/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/handlers/websocket_handlers/listener.py` & `litestar-2.8.1/litestar/handlers/websocket_handlers/listener.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/handlers/websocket_handlers/route_handler.py` & `litestar-2.8.1/litestar/handlers/websocket_handlers/route_handler.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/logging/_utils.py` & `litestar-2.8.1/litestar/logging/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/logging/config.py` & `litestar-2.8.1/litestar/logging/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/logging/picologging.py` & `litestar-2.8.1/litestar/logging/picologging.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/logging/standard.py` & `litestar-2.8.1/litestar/logging/standard.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/middleware/_utils.py` & `litestar-2.8.1/litestar/middleware/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/middleware/allowed_hosts.py` & `litestar-2.8.1/litestar/middleware/allowed_hosts.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/middleware/authentication.py` & `litestar-2.8.1/litestar/middleware/authentication.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/middleware/base.py` & `litestar-2.8.1/litestar/middleware/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/middleware/cors.py` & `litestar-2.8.1/litestar/middleware/cors.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/middleware/csrf.py` & `litestar-2.8.1/litestar/middleware/csrf.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/middleware/logging.py` & `litestar-2.8.1/litestar/middleware/logging.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/middleware/rate_limit.py` & `litestar-2.8.1/litestar/middleware/rate_limit.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/middleware/response_cache.py` & `litestar-2.8.1/litestar/middleware/response_cache.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/middleware/compression/brotli_facade.py` & `litestar-2.8.1/litestar/middleware/compression/brotli_facade.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/middleware/compression/facade.py` & `litestar-2.8.1/litestar/middleware/compression/facade.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/middleware/compression/gzip_facade.py` & `litestar-2.8.1/litestar/middleware/compression/gzip_facade.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/middleware/compression/middleware.py` & `litestar-2.8.1/litestar/middleware/compression/middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/middleware/exceptions/_debug_response.py` & `litestar-2.8.1/litestar/middleware/exceptions/_debug_response.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/middleware/exceptions/middleware.py` & `litestar-2.8.1/litestar/middleware/exceptions/middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/middleware/exceptions/templates/scripts.js` & `litestar-2.8.1/litestar/middleware/exceptions/templates/scripts.js`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/middleware/exceptions/templates/styles.css` & `litestar-2.8.1/litestar/middleware/exceptions/templates/styles.css`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/middleware/session/base.py` & `litestar-2.8.1/litestar/middleware/session/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/middleware/session/client_side.py` & `litestar-2.8.1/litestar/middleware/session/client_side.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/middleware/session/server_side.py` & `litestar-2.8.1/litestar/middleware/session/server_side.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/openapi/config.py` & `litestar-2.8.1/litestar/openapi/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/openapi/controller.py` & `litestar-2.8.1/litestar/openapi/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 from __future__ import annotations
 
 from functools import cached_property
-from typing import TYPE_CHECKING, Any, Callable, Literal
+from typing import TYPE_CHECKING, Any, Callable, Final, Literal
+from uuid import uuid4
 
-from litestar.constants import OPENAPI_JSON_HANDLER_NAME, OPENAPI_NOT_INITIALIZED
+from litestar.constants import OPENAPI_NOT_INITIALIZED
 from litestar.controller import Controller
 from litestar.enums import MediaType, OpenAPIMediaType
 from litestar.exceptions import ImproperlyConfiguredException
 from litestar.handlers import get
 from litestar.openapi.config import _DEFAULT_SCHEMA_SITE
 from litestar.response.base import ASGIResponse
 from litestar.serialization import encode_json
 from litestar.serialization.msgspec_hooks import decode_json
 from litestar.status_codes import HTTP_404_NOT_FOUND
 
-__all__ = ("OpenAPIController",)
-
-
 if TYPE_CHECKING:
     from litestar.connection.request import Request
     from litestar.openapi.spec.open_api import OpenAPI
 
+__all__ = ("OpenAPIController",)
+
+# NOTE: We are explicitly using a different name to the one defined in litestar.constants so that an openapi
+#   controller can be added to a router on the same application as the openapi router.
+#   See: https://github.com/litestar-org/litestar/issues/3337
+OPENAPI_JSON_HANDLER_NAME: Final = f"{uuid4().hex}_litestar_openapi_json"
+
 
 class OpenAPIController(Controller):
     """Controller for OpenAPI endpoints."""
 
     path: str = "/schema"
     """Base path for the OpenAPI documentation endpoints."""
     style: str = "body { margin: 0; padding: 0 }"
```

### Comparing `litestar-2.8.0/litestar/openapi/datastructures.py` & `litestar-2.8.1/litestar/openapi/datastructures.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/openapi/plugins.py` & `litestar-2.8.1/litestar/openapi/plugins.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/openapi/spec/__init__.py` & `litestar-2.8.1/litestar/openapi/spec/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/openapi/spec/base.py` & `litestar-2.8.1/litestar/openapi/spec/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/openapi/spec/callback.py` & `litestar-2.8.1/litestar/openapi/spec/callback.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/openapi/spec/components.py` & `litestar-2.8.1/litestar/openapi/spec/components.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/openapi/spec/contact.py` & `litestar-2.8.1/litestar/openapi/spec/contact.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/openapi/spec/discriminator.py` & `litestar-2.8.1/litestar/openapi/spec/discriminator.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/openapi/spec/encoding.py` & `litestar-2.8.1/litestar/openapi/spec/encoding.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/openapi/spec/enums.py` & `litestar-2.8.1/litestar/openapi/spec/enums.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/openapi/spec/example.py` & `litestar-2.8.1/litestar/openapi/spec/example.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/openapi/spec/external_documentation.py` & `litestar-2.8.1/litestar/openapi/spec/external_documentation.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/openapi/spec/header.py` & `litestar-2.8.1/litestar/openapi/spec/header.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/openapi/spec/info.py` & `litestar-2.8.1/litestar/openapi/spec/info.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/openapi/spec/license.py` & `litestar-2.8.1/litestar/openapi/spec/license.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/openapi/spec/link.py` & `litestar-2.8.1/litestar/openapi/spec/link.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/openapi/spec/media_type.py` & `litestar-2.8.1/litestar/openapi/spec/media_type.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/openapi/spec/oauth_flow.py` & `litestar-2.8.1/litestar/openapi/spec/oauth_flow.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/openapi/spec/oauth_flows.py` & `litestar-2.8.1/litestar/openapi/spec/oauth_flows.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/openapi/spec/open_api.py` & `litestar-2.8.1/litestar/openapi/spec/open_api.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/openapi/spec/operation.py` & `litestar-2.8.1/litestar/openapi/spec/operation.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/openapi/spec/parameter.py` & `litestar-2.8.1/litestar/openapi/spec/parameter.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/openapi/spec/path_item.py` & `litestar-2.8.1/litestar/openapi/spec/path_item.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/openapi/spec/paths.py` & `litestar-2.8.1/litestar/openapi/spec/paths.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/openapi/spec/reference.py` & `litestar-2.8.1/litestar/openapi/spec/reference.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/openapi/spec/request_body.py` & `litestar-2.8.1/litestar/openapi/spec/request_body.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/openapi/spec/response.py` & `litestar-2.8.1/litestar/openapi/spec/response.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/openapi/spec/responses.py` & `litestar-2.8.1/litestar/openapi/spec/responses.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/openapi/spec/schema.py` & `litestar-2.8.1/litestar/openapi/spec/schema.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/openapi/spec/security_requirement.py` & `litestar-2.8.1/litestar/openapi/spec/security_requirement.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/openapi/spec/security_scheme.py` & `litestar-2.8.1/litestar/openapi/spec/security_scheme.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/openapi/spec/server.py` & `litestar-2.8.1/litestar/openapi/spec/server.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/openapi/spec/server_variable.py` & `litestar-2.8.1/litestar/openapi/spec/server_variable.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/openapi/spec/tag.py` & `litestar-2.8.1/litestar/openapi/spec/tag.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/openapi/spec/xml.py` & `litestar-2.8.1/litestar/openapi/spec/xml.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/plugins/base.py` & `litestar-2.8.1/litestar/plugins/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/plugins/core.py` & `litestar-2.8.1/litestar/plugins/core.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/plugins/flash.py` & `litestar-2.8.1/litestar/plugins/flash.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/plugins/sqlalchemy.py` & `litestar-2.8.1/litestar/plugins/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/plugins/structlog.py` & `litestar-2.8.1/litestar/plugins/structlog.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/repository/_filters.py` & `litestar-2.8.1/litestar/repository/_filters.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/repository/filters.py` & `litestar-2.8.1/litestar/repository/filters.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/repository/handlers.py` & `litestar-2.8.1/litestar/repository/handlers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/repository/abc/_async.py` & `litestar-2.8.1/litestar/repository/abc/_async.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/repository/abc/_sync.py` & `litestar-2.8.1/litestar/repository/abc/_sync.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/repository/testing/generic_mock_repository.py` & `litestar-2.8.1/litestar/repository/testing/generic_mock_repository.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/response/base.py` & `litestar-2.8.1/litestar/response/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/response/file.py` & `litestar-2.8.1/litestar/response/file.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/response/redirect.py` & `litestar-2.8.1/litestar/response/redirect.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/response/sse.py` & `litestar-2.8.1/litestar/response/sse.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/response/streaming.py` & `litestar-2.8.1/litestar/response/streaming.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/response/template.py` & `litestar-2.8.1/litestar/response/template.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/routes/asgi.py` & `litestar-2.8.1/litestar/routes/asgi.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/routes/base.py` & `litestar-2.8.1/litestar/routes/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,22 +6,20 @@
 from decimal import Decimal
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Callable
 from uuid import UUID
 
 import msgspec
 
-from litestar._kwargs import KwargsModel
 from litestar.exceptions import ImproperlyConfiguredException
 from litestar.types.internal_types import PathParameterDefinition
 from litestar.utils import join_paths, normalize_path
 
 if TYPE_CHECKING:
     from litestar.enums import ScopeType
-    from litestar.handlers.base import BaseRouteHandler
     from litestar.types import Method, Receive, Scope, Send
 
 
 def _parse_datetime(value: str) -> datetime:
     return msgspec.convert(value, datetime)
 
 
@@ -97,18 +95,15 @@
 
         Args:
             handler_names: Names of the associated handler functions
             path: Base path of the route
             scope_type: Type of the ASGI scope
             methods: Supported methods
         """
-        self.path, self.path_format, self.path_components = self._parse_path(path)
-        self.path_parameters: tuple[PathParameterDefinition, ...] = tuple(
-            component for component in self.path_components if isinstance(component, PathParameterDefinition)
-        )
+        self.path, self.path_format, self.path_components, self.path_parameters = self._parse_path(path)
         self.handler_names = handler_names
         self.scope_type = scope_type
         self.methods = set(methods or [])
 
     @abstractmethod
     async def handle(self, scope: Scope, receive: Receive, send: Send) -> None:
         """ASGI App of the route.
@@ -119,31 +114,14 @@
             send: The ASGI send function.
 
         Returns:
             None
         """
         raise NotImplementedError("Route subclasses must implement handle which serves as the ASGI app entry point")
 
-    def create_handler_kwargs_model(self, route_handler: BaseRouteHandler) -> KwargsModel:
-        """Create a `KwargsModel` for a given route handler."""
-
-        path_parameters = set()
-        for param in self.path_parameters:
-            if param.name in path_parameters:
-                raise ImproperlyConfiguredException(f"Duplicate parameter '{param.name}' detected in '{self.path}'.")
-            path_parameters.add(param.name)
-
-        return KwargsModel.create_for_signature_model(
-            signature_model=route_handler.signature_model,
-            parsed_signature=route_handler.parsed_fn_signature,
-            dependencies=route_handler.resolve_dependencies(),
-            path_parameters=path_parameters,
-            layered_parameters=route_handler.resolve_layered_parameters(),
-        )
-
     @staticmethod
     def _validate_path_parameter(param: str, path: str) -> None:
         """Validate that a path parameter adheres to the required format and datatypes.
 
         Raises:
             ImproperlyConfiguredException: If the parameter has an invalid format.
         """
@@ -156,40 +134,45 @@
             raise ImproperlyConfiguredException("Path parameter names should be of length greater than zero")
         if param_type not in param_type_map:
             raise ImproperlyConfiguredException(
                 f"Path parameters should be declared with an allowed type, i.e. one of {', '.join(param_type_map.keys())} in path: '{path}'"
             )
 
     @classmethod
-    def _parse_path(cls, path: str) -> tuple[str, str, list[str | PathParameterDefinition]]:
+    def _parse_path(
+        cls, path: str
+    ) -> tuple[str, str, list[str | PathParameterDefinition], dict[str, PathParameterDefinition]]:
         """Normalize and parse a path.
 
         Splits the path into a list of components, parsing any that are path parameters. Also builds the OpenAPI
         compatible path, which does not include the type of the path parameters.
 
         Returns:
             A 3-tuple of the normalized path, the OpenAPI formatted path, and the list of parsed components.
         """
         path = normalize_path(path)
 
         parsed_components: list[str | PathParameterDefinition] = []
         path_format_components = []
+        path_parameters: dict[str, PathParameterDefinition] = {}
 
         components = [component for component in path.split("/") if component]
         for component in components:
             if param_match := param_match_regex.fullmatch(component):
                 param = param_match.group(1)
                 cls._validate_path_parameter(param, path)
                 param_name, param_type = (p.strip() for p in param.split(":"))
                 type_class = param_type_map[param_type]
                 parser = parsers_map[type_class] if type_class not in {str, Path} else None
-                parsed_components.append(
-                    PathParameterDefinition(name=param_name, type=type_class, full=param, parser=parser)
-                )
+                if param_name in path_parameters:
+                    raise ImproperlyConfiguredException(f"Duplicate parameter '{param_name}' detected in '{path}'.")
+                param_definition = PathParameterDefinition(name=param_name, type=type_class, full=param, parser=parser)
+                parsed_components.append(param_definition)
+                path_parameters[param_name] = param_definition
                 path_format_components.append("{" + param_name + "}")
             else:
                 parsed_components.append(component)
                 path_format_components.append(component)
 
         path_format = join_paths(path_format_components)
 
-        return path, path_format, parsed_components
+        return path, path_format, parsed_components, path_parameters
```

### Comparing `litestar-2.8.0/litestar/routes/http.py` & `litestar-2.8.1/litestar/routes/http.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
             await self._cleanup_temporary_files(form_data=cast("dict[str, Any]", form_data))
 
     def create_handler_map(self) -> None:
         """Parse the ``router_handlers`` of this route and return a mapping of
         http- methods and route handlers.
         """
         for route_handler in self.route_handlers:
-            kwargs_model = self.create_handler_kwargs_model(route_handler=route_handler)
+            kwargs_model = route_handler.create_kwargs_model(path_parameters=self.path_parameters)
             for http_method in route_handler.http_methods:
                 if self.route_handler_map.get(http_method):
                     raise ImproperlyConfiguredException(
                         f"Handler already registered for path {self.path!r} and http method {http_method}"
                     )
                 self.route_handler_map[http_method] = (route_handler, kwargs_model)
```

### Comparing `litestar-2.8.0/litestar/routes/websocket.py` & `litestar-2.8.1/litestar/routes/websocket.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/security/base.py` & `litestar-2.8.1/litestar/security/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/security/jwt/__init__.py` & `litestar-2.8.1/litestar/security/jwt/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/security/jwt/auth.py` & `litestar-2.8.1/litestar/security/jwt/auth.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/security/jwt/middleware.py` & `litestar-2.8.1/litestar/security/jwt/middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/security/jwt/token.py` & `litestar-2.8.1/litestar/security/jwt/token.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/security/session_auth/auth.py` & `litestar-2.8.1/litestar/security/session_auth/auth.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/security/session_auth/middleware.py` & `litestar-2.8.1/litestar/security/session_auth/middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/serialization/msgspec_hooks.py` & `litestar-2.8.1/litestar/serialization/msgspec_hooks.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/static_files/base.py` & `litestar-2.8.1/litestar/static_files/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/static_files/config.py` & `litestar-2.8.1/litestar/static_files/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/stores/base.py` & `litestar-2.8.1/litestar/stores/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/stores/file.py` & `litestar-2.8.1/litestar/stores/file.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/stores/memory.py` & `litestar-2.8.1/litestar/stores/memory.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/stores/redis.py` & `litestar-2.8.1/litestar/stores/redis.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/stores/registry.py` & `litestar-2.8.1/litestar/stores/registry.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/template/base.py` & `litestar-2.8.1/litestar/template/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/template/config.py` & `litestar-2.8.1/litestar/template/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/testing/__init__.py` & `litestar-2.8.1/litestar/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/testing/helpers.py` & `litestar-2.8.1/litestar/testing/helpers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/testing/life_span_handler.py` & `litestar-2.8.1/litestar/testing/life_span_handler.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/testing/request_factory.py` & `litestar-2.8.1/litestar/testing/request_factory.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/testing/transport.py` & `litestar-2.8.1/litestar/testing/transport.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/testing/websocket_test_session.py` & `litestar-2.8.1/litestar/testing/websocket_test_session.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/testing/client/__init__.py` & `litestar-2.8.1/litestar/testing/client/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/testing/client/async_client.py` & `litestar-2.8.1/litestar/testing/client/async_client.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/testing/client/base.py` & `litestar-2.8.1/litestar/testing/client/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/testing/client/sync_client.py` & `litestar-2.8.1/litestar/testing/client/sync_client.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/types/__init__.py` & `litestar-2.8.1/litestar/types/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/types/asgi_types.py` & `litestar-2.8.1/litestar/types/asgi_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/types/builtin_types.py` & `litestar-2.8.1/litestar/types/builtin_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/types/callable_types.py` & `litestar-2.8.1/litestar/types/callable_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/types/composite_types.py` & `litestar-2.8.1/litestar/types/composite_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/types/file_types.py` & `litestar-2.8.1/litestar/types/file_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/types/helper_types.py` & `litestar-2.8.1/litestar/types/helper_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/types/internal_types.py` & `litestar-2.8.1/litestar/types/internal_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/types/protocols.py` & `litestar-2.8.1/litestar/types/protocols.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/types/serialization.py` & `litestar-2.8.1/litestar/types/serialization.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/utils/__init__.py` & `litestar-2.8.1/litestar/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/utils/compat.py` & `litestar-2.8.1/litestar/utils/compat.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/utils/dataclass.py` & `litestar-2.8.1/litestar/utils/dataclass.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/utils/deprecation.py` & `litestar-2.8.1/litestar/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/utils/empty.py` & `litestar-2.8.1/litestar/utils/empty.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/utils/helpers.py` & `litestar-2.8.1/litestar/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/utils/module_loader.py` & `litestar-2.8.1/litestar/utils/module_loader.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/utils/path.py` & `litestar-2.8.1/litestar/utils/path.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/utils/predicates.py` & `litestar-2.8.1/litestar/utils/predicates.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/utils/sequence.py` & `litestar-2.8.1/litestar/utils/sequence.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/utils/signature.py` & `litestar-2.8.1/litestar/utils/signature.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/utils/sync.py` & `litestar-2.8.1/litestar/utils/sync.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/utils/typing.py` & `litestar-2.8.1/litestar/utils/typing.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/utils/version.py` & `litestar-2.8.1/litestar/utils/version.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/utils/warnings.py` & `litestar-2.8.1/litestar/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/utils/scope/__init__.py` & `litestar-2.8.1/litestar/utils/scope/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/litestar/utils/scope/state.py` & `litestar-2.8.1/litestar/utils/scope/state.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/conftest.py` & `litestar-2.8.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/docker_service_fixtures.py` & `litestar-2.8.1/tests/docker_service_fixtures.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/helpers.py` & `litestar-2.8.1/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/models.py` & `litestar-2.8.1/tests/models.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/e2e/test_advanced_alchemy.py` & `litestar-2.8.1/tests/e2e/test_advanced_alchemy.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/e2e/test_exception_handlers.py` & `litestar-2.8.1/tests/e2e/test_exception_handlers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/e2e/test_option_requests.py` & `litestar-2.8.1/tests/e2e/test_option_requests.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/e2e/test_pydantic.py` & `litestar-2.8.1/tests/e2e/test_pydantic.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/e2e/test_response_caching.py` & `litestar-2.8.1/tests/e2e/test_response_caching.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/e2e/test_router_registration.py` & `litestar-2.8.1/tests/e2e/test_router_registration.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/e2e/test_starlette_responses.py` & `litestar-2.8.1/tests/e2e/test_starlette_responses.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/e2e/test_dependency_injection/test_dependency_validation.py` & `litestar-2.8.1/tests/e2e/test_dependency_injection/test_dependency_validation.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/e2e/test_dependency_injection/test_http_handler_dependency_injection.py` & `litestar-2.8.1/tests/e2e/test_dependency_injection/test_http_handler_dependency_injection.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/e2e/test_dependency_injection/test_injection_of_classes.py` & `litestar-2.8.1/tests/e2e/test_dependency_injection/test_injection_of_classes.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/e2e/test_dependency_injection/test_injection_of_generic_models.py` & `litestar-2.8.1/tests/e2e/test_dependency_injection/test_injection_of_generic_models.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/e2e/test_dependency_injection/test_inter_dependencies.py` & `litestar-2.8.1/tests/e2e/test_dependency_injection/test_inter_dependencies.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/e2e/test_dependency_injection/test_request_local_caching.py` & `litestar-2.8.1/tests/e2e/test_dependency_injection/test_request_local_caching.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/e2e/test_dependency_injection/test_websocket_handler_dependency_injection.py` & `litestar-2.8.1/tests/e2e/test_dependency_injection/test_websocket_handler_dependency_injection.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/e2e/test_life_cycle_hooks/test_after_request.py` & `litestar-2.8.1/tests/e2e/test_life_cycle_hooks/test_after_request.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/e2e/test_life_cycle_hooks/test_after_response.py` & `litestar-2.8.1/tests/e2e/test_life_cycle_hooks/test_after_response.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/e2e/test_life_cycle_hooks/test_before_request.py` & `litestar-2.8.1/tests/e2e/test_life_cycle_hooks/test_before_request.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/e2e/test_routing/conftest.py` & `litestar-2.8.1/tests/e2e/test_routing/conftest.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/e2e/test_routing/test_asset_url_path.py` & `litestar-2.8.1/tests/e2e/test_routing/test_asset_url_path.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/e2e/test_routing/test_path_mounting.py` & `litestar-2.8.1/tests/e2e/test_routing/test_path_mounting.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/e2e/test_routing/test_path_resolution.py` & `litestar-2.8.1/tests/e2e/test_routing/test_path_resolution.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/e2e/test_routing/test_route_indexing.py` & `litestar-2.8.1/tests/e2e/test_routing/test_route_indexing.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/e2e/test_routing/test_route_reverse.py` & `litestar-2.8.1/tests/e2e/test_routing/test_route_reverse.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/e2e/test_routing/test_validations.py` & `litestar-2.8.1/tests/e2e/test_routing/test_validations.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/examples/test_cache_control_headers.py` & `litestar-2.8.1/tests/examples/test_cache_control_headers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/examples/test_exceptions.py` & `litestar-2.8.1/tests/examples/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/examples/test_lifecycle_hooks.py` & `litestar-2.8.1/tests/examples/test_lifecycle_hooks.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/examples/test_request_data.py` & `litestar-2.8.1/tests/examples/test_request_data.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/examples/test_routing.py` & `litestar-2.8.1/tests/examples/test_routing.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/examples/test_startup_and_shutdown.py` & `litestar-2.8.1/tests/examples/test_startup_and_shutdown.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/examples/test_static_files.py` & `litestar-2.8.1/tests/examples/test_static_files.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/examples/test_stores.py` & `litestar-2.8.1/tests/examples/test_stores.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/examples/test_todo_app.py` & `litestar-2.8.1/tests/examples/test_todo_app.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/examples/test_using_session_auth.py` & `litestar-2.8.1/tests/examples/test_using_session_auth.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/examples/test_application_hooks/test_application_after_exception_hook.py` & `litestar-2.8.1/tests/examples/test_application_hooks/test_application_after_exception_hook.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/examples/test_application_hooks/test_lifespan_manager.py` & `litestar-2.8.1/tests/examples/test_application_hooks/test_lifespan_manager.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/examples/test_application_state/test_using_application_state.py` & `litestar-2.8.1/tests/examples/test_application_state/test_using_application_state.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/examples/test_contrib/test_piccolo_orm.py` & `litestar-2.8.1/tests/examples/test_contrib/test_piccolo_orm.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/examples/test_contrib/prometheus/test_prometheus_exporter_example.py` & `litestar-2.8.1/tests/examples/test_contrib/prometheus/test_prometheus_exporter_example.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/examples/test_contrib/prometheus/test_prometheus_exporter_example_with_extra_config.py` & `litestar-2.8.1/tests/examples/test_contrib/prometheus/test_prometheus_exporter_example_with_extra_config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/examples/test_contrib/test_sqlalchemy/plugins/test_example_apps.py` & `litestar-2.8.1/tests/examples/test_contrib/test_sqlalchemy/plugins/test_example_apps.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/examples/test_contrib/test_sqlalchemy/plugins/test_tutorial_example_apps.py` & `litestar-2.8.1/tests/examples/test_contrib/test_sqlalchemy/plugins/test_tutorial_example_apps.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/examples/test_dto/test_example_apps.py` & `litestar-2.8.1/tests/examples/test_dto/test_example_apps.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/examples/test_dto/test_tutorial.py` & `litestar-2.8.1/tests/examples/test_dto/test_tutorial.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/examples/test_middleware/test_abstract_middleware.py` & `litestar-2.8.1/tests/examples/test_middleware/test_abstract_middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/examples/test_middleware/test_logging_middleware.py` & `litestar-2.8.1/tests/examples/test_middleware/test_logging_middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/examples/test_middleware/test_session_middleware.py` & `litestar-2.8.1/tests/examples/test_middleware/test_session_middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/examples/test_openapi/test_openapi.py` & `litestar-2.8.1/tests/examples/test_openapi/test_openapi.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/examples/test_openapi/test_plugins.py` & `litestar-2.8.1/tests/examples/test_openapi/test_plugins.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/examples/test_pagination/test_using_classic_pagination.py` & `litestar-2.8.1/tests/examples/test_pagination/test_using_classic_pagination.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/examples/test_pagination/test_using_cursor_pagination.py` & `litestar-2.8.1/tests/examples/test_pagination/test_using_cursor_pagination.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/examples/test_pagination/test_using_offset_pagination.py` & `litestar-2.8.1/tests/examples/test_pagination/test_using_offset_pagination.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/examples/test_parameters/test_header_and_cookies_parameters.py` & `litestar-2.8.1/tests/examples/test_parameters/test_header_and_cookies_parameters.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/examples/test_parameters/test_layered_parameters.py` & `litestar-2.8.1/tests/examples/test_parameters/test_layered_parameters.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/examples/test_parameters/test_path_parameters.py` & `litestar-2.8.1/tests/examples/test_parameters/test_path_parameters.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/examples/test_parameters/test_query_parameters.py` & `litestar-2.8.1/tests/examples/test_parameters/test_query_parameters.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/examples/test_plugins/test_sqlalchemy_init_plugin.py` & `litestar-2.8.1/tests/examples/test_plugins/test_sqlalchemy_init_plugin.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/examples/test_responses/test_background_tasks.py` & `litestar-2.8.1/tests/examples/test_responses/test_background_tasks.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/examples/test_responses/test_response_cookies.py` & `litestar-2.8.1/tests/examples/test_responses/test_response_cookies.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/examples/test_responses/test_response_headers.py` & `litestar-2.8.1/tests/examples/test_responses/test_response_headers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/examples/test_responses/test_sse_responses.py` & `litestar-2.8.1/tests/examples/test_responses/test_sse_responses.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/examples/test_security/test_jwt/test_using_jwt_auth.py` & `litestar-2.8.1/tests/examples/test_security/test_jwt/test_using_jwt_auth.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/examples/test_security/test_jwt/test_using_jwt_cookie_auth.py` & `litestar-2.8.1/tests/examples/test_security/test_jwt/test_using_jwt_cookie_auth.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/examples/test_security/test_jwt/test_using_oauth2_password_bearer.py` & `litestar-2.8.1/tests/examples/test_security/test_jwt/test_using_oauth2_password_bearer.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/examples/test_templating/test_engine_instance.py` & `litestar-2.8.1/tests/examples/test_templating/test_engine_instance.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/examples/test_templating/test_returning_templates.py` & `litestar-2.8.1/tests/examples/test_templating/test_returning_templates.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/examples/test_templating/test_template_functions.py` & `litestar-2.8.1/tests/examples/test_templating/test_template_functions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/conftest.py` & `litestar-2.8.1/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_app.py` & `litestar-2.8.1/tests/unit/test_app.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_asgi_router.py` & `litestar-2.8.1/tests/unit/test_asgi_router.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 from contextlib import asynccontextmanager
 from typing import TYPE_CHECKING, AsyncGenerator, Callable
-from unittest.mock import AsyncMock, MagicMock
+from unittest.mock import AsyncMock, MagicMock, call
 
+import anyio
 import pytest
 from pytest_mock import MockerFixture
 
 from litestar import Litestar, asgi
 from litestar._asgi.asgi_router import ASGIRouter
 from litestar.exceptions import ImproperlyConfiguredException
 from litestar.testing import TestClient, create_test_client
@@ -190,7 +191,37 @@
     router = ASGIRouter(app=Litestar(on_shutdown=[on_shutdown]))
 
     with pytest.raises(ValueError):
         await router.lifespan(receive, send)
 
     assert send.call_count == 2
     assert send.call_args_list[1][0][0] == {"type": "lifespan.shutdown.failed", "message": mock_format_exc.return_value}
+
+
+async def test_lifespan_context_exception_after_startup(mock_format_exc: MagicMock) -> None:
+    receive = AsyncMock()
+    receive.return_value = {"type": "lifespan.startup"}
+    send = AsyncMock()
+    mock_format_exc.return_value = "foo"
+
+    async def sleep_and_raise() -> None:
+        await anyio.sleep(0)
+        raise RuntimeError("An error occurred")
+
+    @asynccontextmanager
+    async def lifespan(_: Litestar) -> AsyncGenerator[None, None]:
+        async with anyio.create_task_group() as tg:
+            tg.start_soon(sleep_and_raise)
+            yield
+
+    router = ASGIRouter(app=Litestar(lifespan=[lifespan]))
+
+    with pytest.raises(_ExceptionGroup):
+        await router.lifespan(receive, send)
+
+    assert receive.call_count == 2
+    send.assert_has_calls(
+        [
+            call({"type": "lifespan.startup.complete"}),
+            call({"type": "lifespan.shutdown.failed", "message": mock_format_exc.return_value}),
+        ]
+    )
```

### Comparing `litestar-2.8.0/tests/unit/test_background_tasks.py` & `litestar-2.8.1/tests/unit/test_background_tasks.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_concurrency.py` & `litestar-2.8.1/tests/unit/test_concurrency.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_controller.py` & `litestar-2.8.1/tests/unit/test_controller.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_data_extractors.py` & `litestar-2.8.1/tests/unit/test_data_extractors.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_deprecations.py` & `litestar-2.8.1/tests/unit/test_deprecations.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_di.py` & `litestar-2.8.1/tests/unit/test_di.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_events.py` & `litestar-2.8.1/tests/unit/test_events.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_exceptions.py` & `litestar-2.8.1/tests/unit/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_file_system.py` & `litestar-2.8.1/tests/unit/test_file_system.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_guards.py` & `litestar-2.8.1/tests/unit/test_guards.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_pagination.py` & `litestar-2.8.1/tests/unit/test_pagination.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_params.py` & `litestar-2.8.1/tests/unit/test_params.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_parsers.py` & `litestar-2.8.1/tests/unit/test_parsers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_request_class_resolution.py` & `litestar-2.8.1/tests/unit/test_request_class_resolution.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_response_class_resolution.py` & `litestar-2.8.1/tests/unit/test_response_class_resolution.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_stores.py` & `litestar-2.8.1/tests/unit/test_stores.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_typing.py` & `litestar-2.8.1/tests/unit/test_typing.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_websocket_class_resolution.py` & `litestar-2.8.1/tests/unit/test_websocket_class_resolution.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_channels/conftest.py` & `litestar-2.8.1/tests/unit/test_channels/conftest.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_channels/test_backends.py` & `litestar-2.8.1/tests/unit/test_channels/test_backends.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_channels/test_plugin.py` & `litestar-2.8.1/tests/unit/test_channels/test_plugin.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_channels/test_subscriber.py` & `litestar-2.8.1/tests/unit/test_channels/test_subscriber.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_cli/__init__.py` & `litestar-2.8.1/tests/unit/test_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_cli/conftest.py` & `litestar-2.8.1/tests/unit/test_cli/conftest.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_cli/test_cli.py` & `litestar-2.8.1/tests/unit/test_cli/test_cli.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_cli/test_cli_plugin.py` & `litestar-2.8.1/tests/unit/test_cli/test_cli_plugin.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_cli/test_core_commands.py` & `litestar-2.8.1/tests/unit/test_cli/test_core_commands.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_cli/test_env_resolution.py` & `litestar-2.8.1/tests/unit/test_cli/test_env_resolution.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_cli/test_schema_commands.py` & `litestar-2.8.1/tests/unit/test_cli/test_schema_commands.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_cli/test_session_commands.py` & `litestar-2.8.1/tests/unit/test_cli/test_session_commands.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_cli/test_ssl.py` & `litestar-2.8.1/tests/unit/test_cli/test_ssl.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_connection/test_base.py` & `litestar-2.8.1/tests/unit/test_connection/test_base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_connection/test_connection_caching.py` & `litestar-2.8.1/tests/unit/test_connection/test_connection_caching.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_connection/test_request.py` & `litestar-2.8.1/tests/unit/test_connection/test_request.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_connection/test_websocket.py` & `litestar-2.8.1/tests/unit/test_connection/test_websocket.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_contrib/conftest.py` & `litestar-2.8.1/tests/unit/test_contrib/conftest.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_contrib/test_minijinja.py` & `litestar-2.8.1/tests/unit/test_contrib/test_minijinja.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_contrib/test_msgspec.py` & `litestar-2.8.1/tests/unit/test_contrib/test_msgspec.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_contrib/test_opentelemetry.py` & `litestar-2.8.1/tests/unit/test_contrib/test_opentelemetry.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_contrib/test_prometheus.py` & `litestar-2.8.1/tests/unit/test_contrib/test_prometheus.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_contrib/test_repository.py` & `litestar-2.8.1/tests/unit/test_contrib/test_repository.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_contrib/test_sqlalchemy.py` & `litestar-2.8.1/tests/unit/test_contrib/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_contrib/test_attrs/test_inject_attrs_class.py` & `litestar-2.8.1/tests/unit/test_contrib/test_attrs/test_inject_attrs_class.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_contrib/test_attrs/test_schema_plugin.py` & `litestar-2.8.1/tests/unit/test_contrib/test_attrs/test_schema_plugin.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_contrib/test_attrs/test_schema_spec_generation.py` & `litestar-2.8.1/tests/unit/test_contrib/test_attrs/test_schema_spec_generation.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_contrib/test_attrs/test_signature.py` & `litestar-2.8.1/tests/unit/test_contrib/test_attrs/test_signature.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_contrib/test_htmx/test_htmx_request.py` & `litestar-2.8.1/tests/unit/test_contrib/test_htmx/test_htmx_request.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_contrib/test_htmx/test_htmx_response.py` & `litestar-2.8.1/tests/unit/test_contrib/test_htmx/test_htmx_response.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_contrib/test_piccolo_orm/endpoints.py` & `litestar-2.8.1/tests/unit/test_contrib/test_piccolo_orm/endpoints.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_contrib/test_piccolo_orm/piccolo_app.py` & `litestar-2.8.1/tests/unit/test_contrib/test_piccolo_orm/piccolo_app.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_contrib/test_piccolo_orm/tables.py` & `litestar-2.8.1/tests/unit/test_contrib/test_piccolo_orm/tables.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_contrib/test_piccolo_orm/test_piccolo_orm_dto.py` & `litestar-2.8.1/tests/unit/test_contrib/test_piccolo_orm/test_piccolo_orm_dto.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_contrib/test_pydantic/conftest.py` & `litestar-2.8.1/tests/unit/test_contrib/test_pydantic/conftest.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_contrib/test_pydantic/models.py` & `litestar-2.8.1/tests/unit/test_contrib/test_pydantic/models.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_contrib/test_pydantic/test_beanie_integration.py` & `litestar-2.8.1/tests/unit/test_contrib/test_pydantic/test_beanie_integration.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_contrib/test_pydantic/test_dto.py` & `litestar-2.8.1/tests/unit/test_contrib/test_pydantic/test_dto.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_contrib/test_pydantic/test_inject_pydantic.py` & `litestar-2.8.1/tests/unit/test_contrib/test_pydantic/test_inject_pydantic.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_contrib/test_pydantic/test_integration.py` & `litestar-2.8.1/tests/unit/test_contrib/test_pydantic/test_integration.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_contrib/test_pydantic/test_openapi.py` & `litestar-2.8.1/tests/unit/test_contrib/test_pydantic/test_openapi.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_contrib/test_pydantic/test_plugin_serialization.py` & `litestar-2.8.1/tests/unit/test_contrib/test_pydantic/test_plugin_serialization.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_contrib/test_pydantic/test_pydantic_dto_factory.py` & `litestar-2.8.1/tests/unit/test_contrib/test_pydantic/test_pydantic_dto_factory.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_contrib/test_pydantic/test_schema_plugin.py` & `litestar-2.8.1/tests/unit/test_contrib/test_pydantic/test_schema_plugin.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_contrib/test_pydantic/test_utils.py` & `litestar-2.8.1/tests/unit/test_contrib/test_pydantic/test_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_datastructures/test_cookie.py` & `litestar-2.8.1/tests/unit/test_datastructures/test_cookie.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_datastructures/test_headers.py` & `litestar-2.8.1/tests/unit/test_datastructures/test_headers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_datastructures/test_multi_dicts.py` & `litestar-2.8.1/tests/unit/test_datastructures/test_multi_dicts.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_datastructures/test_state.py` & `litestar-2.8.1/tests/unit/test_datastructures/test_state.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_datastructures/test_upload_file.py` & `litestar-2.8.1/tests/unit/test_datastructures/test_upload_file.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_datastructures/test_url.py` & `litestar-2.8.1/tests/unit/test_datastructures/test_url.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_dto/conftest.py` & `litestar-2.8.1/tests/unit/test_dto/conftest.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_dto/test_integration.py` & `litestar-2.8.1/tests/unit/test_dto/test_integration.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_dto/test_factory/test_base_dto.py` & `litestar-2.8.1/tests/unit/test_dto/test_factory/test_base_dto.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_dto/test_factory/test_dataclass_dto.py` & `litestar-2.8.1/tests/unit/test_dto/test_factory/test_dataclass_dto.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_dto/test_factory/test_integration.py` & `litestar-2.8.1/tests/unit/test_dto/test_factory/test_integration.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_dto/test_factory/test_utils.py` & `litestar-2.8.1/tests/unit/test_dto/test_factory/test_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_dto/test_factory/test_backends/test_backends.py` & `litestar-2.8.1/tests/unit/test_dto/test_factory/test_backends/test_backends.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_dto/test_factory/test_backends/test_base_dto.py` & `litestar-2.8.1/tests/unit/test_dto/test_factory/test_backends/test_base_dto.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_dto/test_factory/test_backends/test_utils.py` & `litestar-2.8.1/tests/unit/test_dto/test_factory/test_backends/test_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_handlers/test_asgi_handlers/test_handle_asgi.py` & `litestar-2.8.1/tests/unit/test_handlers/test_asgi_handlers/test_handle_asgi.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_handlers/test_asgi_handlers/test_handle_asgi_with_future_annotations.py` & `litestar-2.8.1/tests/unit/test_handlers/test_asgi_handlers/test_handle_asgi_with_future_annotations.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_handlers/test_asgi_handlers/test_validations.py` & `litestar-2.8.1/tests/unit/test_handlers/test_asgi_handlers/test_validations.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_handlers/test_base_handlers/test_opt.py` & `litestar-2.8.1/tests/unit/test_handlers/test_base_handlers/test_opt.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_handlers/test_base_handlers/test_resolution.py` & `litestar-2.8.1/tests/unit/test_handlers/test_base_handlers/test_resolution.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_handlers/test_base_handlers/test_validations.py` & `litestar-2.8.1/tests/unit/test_handlers/test_base_handlers/test_validations.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_handlers/test_http_handlers/test_defaults.py` & `litestar-2.8.1/tests/unit/test_handlers/test_http_handlers/test_defaults.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_handlers/test_http_handlers/test_head.py` & `litestar-2.8.1/tests/unit/test_handlers/test_http_handlers/test_head.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_handlers/test_http_handlers/test_kwarg_handling.py` & `litestar-2.8.1/tests/unit/test_handlers/test_http_handlers/test_kwarg_handling.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_handlers/test_http_handlers/test_media_type.py` & `litestar-2.8.1/tests/unit/test_handlers/test_http_handlers/test_media_type.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_handlers/test_http_handlers/test_signature_namespace.py` & `litestar-2.8.1/tests/unit/test_handlers/test_http_handlers/test_signature_namespace.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_handlers/test_http_handlers/test_sync.py` & `litestar-2.8.1/tests/unit/test_handlers/test_http_handlers/test_sync.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_handlers/test_http_handlers/test_validations.py` & `litestar-2.8.1/tests/unit/test_handlers/test_http_handlers/test_validations.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_handlers/test_websocket_handlers/test_handle_websocket.py` & `litestar-2.8.1/tests/unit/test_handlers/test_websocket_handlers/test_handle_websocket.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_handlers/test_websocket_handlers/test_handle_websocket_with_future_annotations.py` & `litestar-2.8.1/tests/unit/test_handlers/test_websocket_handlers/test_handle_websocket_with_future_annotations.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_handlers/test_websocket_handlers/test_kwarg_handling.py` & `litestar-2.8.1/tests/unit/test_handlers/test_websocket_handlers/test_kwarg_handling.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_handlers/test_websocket_handlers/test_listeners.py` & `litestar-2.8.1/tests/unit/test_handlers/test_websocket_handlers/test_listeners.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_handlers/test_websocket_handlers/test_validations.py` & `litestar-2.8.1/tests/unit/test_handlers/test_websocket_handlers/test_validations.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_kwargs/flower.jpeg` & `litestar-2.8.1/tests/unit/test_kwargs/flower.jpeg`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_kwargs/test_cleanup_group.py` & `litestar-2.8.1/tests/unit/test_kwargs/test_cleanup_group.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_kwargs/test_cookie_params.py` & `litestar-2.8.1/tests/unit/test_kwargs/test_cookie_params.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_kwargs/test_defaults.py` & `litestar-2.8.1/tests/unit/test_kwargs/test_defaults.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_kwargs/test_dependency_batches.py` & `litestar-2.8.1/tests/unit/test_kwargs/test_dependency_batches.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_kwargs/test_generator_dependencies.py` & `litestar-2.8.1/tests/unit/test_kwargs/test_generator_dependencies.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_kwargs/test_header_params.py` & `litestar-2.8.1/tests/unit/test_kwargs/test_header_params.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_kwargs/test_json_data.py` & `litestar-2.8.1/tests/unit/test_kwargs/test_json_data.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_kwargs/test_layered_params.py` & `litestar-2.8.1/tests/unit/test_kwargs/test_layered_params.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_kwargs/test_msgpack_data.py` & `litestar-2.8.1/tests/unit/test_kwargs/test_msgpack_data.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_kwargs/test_multipart_data.py` & `litestar-2.8.1/tests/unit/test_kwargs/test_multipart_data.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_kwargs/test_path_params.py` & `litestar-2.8.1/tests/unit/test_kwargs/test_path_params.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_kwargs/test_query_params.py` & `litestar-2.8.1/tests/unit/test_kwargs/test_query_params.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_kwargs/test_reserved_kwargs_injection.py` & `litestar-2.8.1/tests/unit/test_kwargs/test_reserved_kwargs_injection.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_kwargs/test_url_encoded_data.py` & `litestar-2.8.1/tests/unit/test_kwargs/test_url_encoded_data.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_kwargs/test_validations.py` & `litestar-2.8.1/tests/unit/test_kwargs/test_validations.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_logging/test_logging_config.py` & `litestar-2.8.1/tests/unit/test_logging/test_logging_config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_logging/test_structlog_config.py` & `litestar-2.8.1/tests/unit/test_logging/test_structlog_config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_middleware/test_allowed_hosts_middleware.py` & `litestar-2.8.1/tests/unit/test_middleware/test_allowed_hosts_middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_middleware/test_base_authentication_middleware.py` & `litestar-2.8.1/tests/unit/test_middleware/test_base_authentication_middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_middleware/test_base_middleware.py` & `litestar-2.8.1/tests/unit/test_middleware/test_base_middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_middleware/test_compression_middleware.py` & `litestar-2.8.1/tests/unit/test_middleware/test_compression_middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_middleware/test_cors_middleware.py` & `litestar-2.8.1/tests/unit/test_middleware/test_cors_middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_middleware/test_csrf_middleware.py` & `litestar-2.8.1/tests/unit/test_middleware/test_csrf_middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_middleware/test_exception_handler_middleware.py` & `litestar-2.8.1/tests/unit/test_middleware/test_exception_handler_middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_middleware/test_logging_middleware.py` & `litestar-2.8.1/tests/unit/test_middleware/test_logging_middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_middleware/test_middleware_handling.py` & `litestar-2.8.1/tests/unit/test_middleware/test_middleware_handling.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_middleware/test_rate_limit_middleware.py` & `litestar-2.8.1/tests/unit/test_middleware/test_rate_limit_middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_middleware/test_session/conftest.py` & `litestar-2.8.1/tests/unit/test_middleware/test_session/conftest.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_middleware/test_session/test_client_side_backend.py` & `litestar-2.8.1/tests/unit/test_middleware/test_session/test_client_side_backend.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_middleware/test_session/test_integration.py` & `litestar-2.8.1/tests/unit/test_middleware/test_session/test_integration.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_middleware/test_session/test_middleware.py` & `litestar-2.8.1/tests/unit/test_middleware/test_session/test_middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_middleware/test_session/test_server_side_backend.py` & `litestar-2.8.1/tests/unit/test_middleware/test_session/test_server_side_backend.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_openapi/conftest.py` & `litestar-2.8.1/tests/unit/test_openapi/conftest.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_openapi/test_config.py` & `litestar-2.8.1/tests/unit/test_openapi/test_config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_openapi/test_datastructures.py` & `litestar-2.8.1/tests/unit/test_openapi/test_datastructures.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_openapi/test_endpoints.py` & `litestar-2.8.1/tests/unit/test_openapi/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_openapi/test_integration.py` & `litestar-2.8.1/tests/unit/test_openapi/test_integration.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import Callable, Generic, Optional, TypeVar, cast
 
 import msgspec
 import pytest
 import yaml
 from typing_extensions import Annotated
 
-from litestar import Controller, Litestar, delete, get, patch, post
+from litestar import Controller, Litestar, Router, delete, get, patch, post
 from litestar._openapi.plugin import OpenAPIPlugin
 from litestar.enums import MediaType, OpenAPIMediaType, ParamType
 from litestar.openapi import OpenAPIConfig, OpenAPIController
 from litestar.openapi.spec import Parameter as OpenAPIParameter
 from litestar.params import Parameter
 from litestar.serialization.msgspec_hooks import decode_json, encode_json, get_serializer
 from litestar.status_codes import HTTP_200_OK, HTTP_404_NOT_FOUND
@@ -499,7 +499,44 @@
 
     expected_keys = [
         "test_components_schemas_in_alphabetical_order.A",
         "test_components_schemas_in_alphabetical_order.B",
         "test_components_schemas_in_alphabetical_order.C",
     ]
     assert list(openapi.components.schemas.keys()) == expected_keys
+
+
+def test_openapi_controller_and_openapi_router_on_same_app() -> None:
+    """Test that OpenAPIController and OpenAPIRouter can coexist on the same app.
+
+    As part of backward compatibility with new plugin-based OpenAPI router approach, we did not consider
+    the case where an OpenAPIController is registered on the application by means other than via the
+    OpenAPIConfig object. This is an approach that has been used to serve the openapi both under the
+    `/schema` and `/some-prefix/schema` paths. This test ensures that the OpenAPIController and OpenAPIRouter
+    can coexist on the same app.
+
+    See: https://github.com/litestar-org/litestar/issues/3337
+    """
+    router = Router(path="/abc", route_handlers=[OpenAPIController])
+    openapi_config = OpenAPIConfig("Litestar", "v0.0.1")  # no openapi_controller specified means we use the router
+    app = Litestar([router], openapi_config=openapi_config)
+    assert sorted(r.path for r in app.routes) == [
+        "/abc/schema",
+        "/abc/schema/elements",
+        "/abc/schema/oauth2-redirect.html",
+        "/abc/schema/openapi.json",
+        "/abc/schema/openapi.yaml",
+        "/abc/schema/openapi.yml",
+        "/abc/schema/rapidoc",
+        "/abc/schema/redoc",
+        "/abc/schema/swagger",
+        "/schema",
+        "/schema/elements",
+        "/schema/oauth2-redirect.html",
+        "/schema/openapi.json",
+        "/schema/openapi.yaml",
+        "/schema/openapi.yml",
+        "/schema/rapidoc",
+        "/schema/redoc",
+        "/schema/swagger",
+        "/schema/{path:str}",
+    ]
```

### Comparing `litestar-2.8.0/tests/unit/test_openapi/test_parameters.py` & `litestar-2.8.1/tests/unit/test_openapi/test_parameters.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_openapi/test_path_item.py` & `litestar-2.8.1/tests/unit/test_openapi/test_path_item.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_openapi/test_request_body.py` & `litestar-2.8.1/tests/unit/test_openapi/test_request_body.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_openapi/test_responses.py` & `litestar-2.8.1/tests/unit/test_openapi/test_responses.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_openapi/test_schema.py` & `litestar-2.8.1/tests/unit/test_openapi/test_schema.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_openapi/test_security_schemes.py` & `litestar-2.8.1/tests/unit/test_openapi/test_security_schemes.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_openapi/test_spec_generation.py` & `litestar-2.8.1/tests/unit/test_openapi/test_spec_generation.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_openapi/test_tags.py` & `litestar-2.8.1/tests/unit/test_openapi/test_tags.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_openapi/test_typescript_converter/test_converter.py` & `litestar-2.8.1/tests/unit/test_openapi/test_typescript_converter/test_converter.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_openapi/test_typescript_converter/test_schema_parsing.py` & `litestar-2.8.1/tests/unit/test_openapi/test_typescript_converter/test_schema_parsing.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_openapi/test_typescript_converter/test_typescript_types.py` & `litestar-2.8.1/tests/unit/test_openapi/test_typescript_converter/test_typescript_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_plugins/test_base.py` & `litestar-2.8.1/tests/unit/test_plugins/test_base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_plugins/test_flash.py` & `litestar-2.8.1/tests/unit/test_plugins/test_flash.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_plugins/test_sqlalchemy.py` & `litestar-2.8.1/tests/unit/test_plugins/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_repository/models_bigint.py` & `litestar-2.8.1/tests/unit/test_repository/models_bigint.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_repository/models_uuid.py` & `litestar-2.8.1/tests/unit/test_repository/models_uuid.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_repository/test_generic_mock_repository.py` & `litestar-2.8.1/tests/unit/test_repository/test_generic_mock_repository.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_response/test_base_response.py` & `litestar-2.8.1/tests/unit/test_response/test_base_response.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_response/test_file_response.py` & `litestar-2.8.1/tests/unit/test_response/test_file_response.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_response/test_redirect_response.py` & `litestar-2.8.1/tests/unit/test_response/test_redirect_response.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_response/test_response_cookies.py` & `litestar-2.8.1/tests/unit/test_response/test_response_cookies.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_response/test_response_headers.py` & `litestar-2.8.1/tests/unit/test_response/test_response_headers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_response/test_response_to_asgi_response.py` & `litestar-2.8.1/tests/unit/test_response/test_response_to_asgi_response.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_response/test_serialization.py` & `litestar-2.8.1/tests/unit/test_response/test_serialization.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_response/test_sse.py` & `litestar-2.8.1/tests/unit/test_response/test_sse.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_response/test_streaming_response.py` & `litestar-2.8.1/tests/unit/test_response/test_streaming_response.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_response/test_type_decoders.py` & `litestar-2.8.1/tests/unit/test_response/test_type_decoders.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_response/test_type_encoders.py` & `litestar-2.8.1/tests/unit/test_response/test_type_encoders.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_security/test_security.py` & `litestar-2.8.1/tests/unit/test_security/test_security.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_security/test_session_auth.py` & `litestar-2.8.1/tests/unit/test_security/test_session_auth.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_security/test_jwt/test_auth.py` & `litestar-2.8.1/tests/unit/test_security/test_jwt/test_auth.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_security/test_jwt/test_integration.py` & `litestar-2.8.1/tests/unit/test_security/test_jwt/test_integration.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_security/test_jwt/test_token.py` & `litestar-2.8.1/tests/unit/test_security/test_jwt/test_token.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_signature/test_parsing.py` & `litestar-2.8.1/tests/unit/test_signature/test_parsing.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_signature/test_validation.py` & `litestar-2.8.1/tests/unit/test_signature/test_validation.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_static_files/conftest.py` & `litestar-2.8.1/tests/unit/test_static_files/conftest.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_static_files/test_create_static_router.py` & `litestar-2.8.1/tests/unit/test_static_files/test_create_static_router.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_static_files/test_file_serving_resolution.py` & `litestar-2.8.1/tests/unit/test_static_files/test_file_serving_resolution.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_static_files/test_html_mode.py` & `litestar-2.8.1/tests/unit/test_static_files/test_html_mode.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_static_files/test_static_files_validation.py` & `litestar-2.8.1/tests/unit/test_static_files/test_static_files_validation.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_template/test_built_in.py` & `litestar-2.8.1/tests/unit/test_template/test_built_in.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_template/test_builtin_functions.py` & `litestar-2.8.1/tests/unit/test_template/test_builtin_functions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_template/test_context.py` & `litestar-2.8.1/tests/unit/test_template/test_context.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_template/test_csrf_token.py` & `litestar-2.8.1/tests/unit/test_template/test_csrf_token.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_template/test_template.py` & `litestar-2.8.1/tests/unit/test_template/test_template.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_testing/test_lifespan_handler.py` & `litestar-2.8.1/tests/unit/test_testing/test_lifespan_handler.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_testing/test_request_factory.py` & `litestar-2.8.1/tests/unit/test_testing/test_request_factory.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_testing/test_test_client.py` & `litestar-2.8.1/tests/unit/test_testing/test_test_client.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_types/test_protocols.py` & `litestar-2.8.1/tests/unit/test_types/test_protocols.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_utils/test_dataclass.py` & `litestar-2.8.1/tests/unit/test_utils/test_dataclass.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_utils/test_deprecation.py` & `litestar-2.8.1/tests/unit/test_utils/test_deprecation.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_utils/test_helpers.py` & `litestar-2.8.1/tests/unit/test_utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_utils/test_module_loader.py` & `litestar-2.8.1/tests/unit/test_utils/test_module_loader.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_utils/test_path.py` & `litestar-2.8.1/tests/unit/test_utils/test_path.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_utils/test_predicates.py` & `litestar-2.8.1/tests/unit/test_utils/test_predicates.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_utils/test_scope.py` & `litestar-2.8.1/tests/unit/test_utils/test_scope.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_utils/test_sequence.py` & `litestar-2.8.1/tests/unit/test_utils/test_sequence.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_utils/test_signature.py` & `litestar-2.8.1/tests/unit/test_utils/test_signature.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_utils/test_sync.py` & `litestar-2.8.1/tests/unit/test_utils/test_sync.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_utils/test_typing.py` & `litestar-2.8.1/tests/unit/test_utils/test_typing.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/tests/unit/test_utils/test_version.py` & `litestar-2.8.1/tests/unit/test_utils/test_version.py`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/LICENSE` & `litestar-2.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/README.md` & `litestar-2.8.1/README.md`

 * *Files identical despite different names*

### Comparing `litestar-2.8.0/pyproject.toml` & `litestar-2.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
   {name = "Peter Schutt", email = "peter@litestar.dev"},
   {name = "Visakh Unnikrishnan", email = "guacs@litestar.dev"},
   {name = "Alc", email = "alc@litestar.dev"}
 ]
 name = "litestar"
 readme = "README.md"
 requires-python = ">=3.8,<4.0"
-version = "2.8.0"
+version = "2.8.1"
 
 [project.urls]
 Blog = "https://blog.litestar.dev"
 Changelog = "https://github.com/litestar-org/litestar/releases/"
 Discord = "https://discord.gg/litestar-919193495116337154"
 Documentation = "https://docs.litestar.dev/"
 Homepage = "https://litestar.dev/"
```

### Comparing `litestar-2.8.0/PKG-INFO` & `litestar-2.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: litestar
-Version: 2.8.0
+Version: 2.8.1
 Summary: Litestar - A production-ready, highly performant, extensible ASGI API Framework
 Project-URL: Blog, https://blog.litestar.dev
 Project-URL: Changelog, https://github.com/litestar-org/litestar/releases/
 Project-URL: Discord, https://discord.gg/litestar-919193495116337154
 Project-URL: Documentation, https://docs.litestar.dev/
 Project-URL: Homepage, https://litestar.dev/
 Project-URL: Issue Tracker, https://github.com/litestar-org/litestar/issues?q=is%3Aissue+is%3Aopen+sort%3Aupdated-desc
```

