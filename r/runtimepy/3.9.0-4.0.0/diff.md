# Comparing `tmp/runtimepy-3.9.0.tar.gz` & `tmp/runtimepy-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runtimepy-3.9.0.tar", last modified: Mon Feb 26 03:24:13 2024, max compression
+gzip compressed data, was "runtimepy-4.0.0.tar", last modified: Mon Apr  8 19:05:49 2024, max compression
```

## Comparing `runtimepy-3.9.0.tar` & `runtimepy-4.0.0.tar`

### file list

```diff
@@ -1,219 +1,290 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.596395 runtimepy-3.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-02-26 03:21:58.000000 runtimepy-3.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6941 2024-02-26 03:24:13.592395 runtimepy-3.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-02-26 03:21:58.000000 runtimepy-3.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-02-26 03:21:58.000000 runtimepy-3.9.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.568395 runtimepy-3.9.0/runtimepy/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.572395 runtimepy-3.9.0/runtimepy/channel/
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/channel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.572395 runtimepy-3.9.0/runtimepy/channel/environment/
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/channel/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/channel/environment/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     8916 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/channel/environment/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.572395 runtimepy-3.9.0/runtimepy/channel/environment/command/
--rw-r--r--   0 runner    (1001) docker     (127)     8144 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/channel/environment/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/channel/environment/command/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5662 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/channel/environment/command/processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/channel/environment/command/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     5004 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/channel/environment/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     7034 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/channel/environment/file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.572395 runtimepy-3.9.0/runtimepy/channel/event/
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/channel/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/channel/event/header.py
--rw-r--r--   0 runner    (1001) docker     (127)     5703 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/channel/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.572395 runtimepy-3.9.0/runtimepy/codec/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/codec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.572395 runtimepy-3.9.0/runtimepy/codec/protocol/
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/codec/protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9041 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/codec/protocol/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/codec/protocol/json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.572395 runtimepy-3.9.0/runtimepy/codec/system/
--rw-r--r--   0 runner    (1001) docker     (127)     6950 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/codec/system/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.572395 runtimepy-3.9.0/runtimepy/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/commands/arbiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/commands/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3813 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/commands/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/commands/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/commands/tui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.572395 runtimepy-3.9.0/runtimepy/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/data/factories.yaml
--rw-r--r--   0 runner    (1001) docker     (127)   362870 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/data/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.576395 runtimepy-3.9.0/runtimepy/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/data/schemas/BitFields.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/data/schemas/Channel.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/data/schemas/ChannelCommand.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/data/schemas/ChannelRegistry.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/data/schemas/ClientConnectionConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/data/schemas/ConnectionArbiterConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/data/schemas/EnumRegistry.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/data/schemas/FindFile.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/data/schemas/RuntimeEnum.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/data/schemas/ServerConnectionConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/data/schemas/TaskConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/data/schemas/has_factory.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/data/schemas/has_name.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/data/schemas/has_request_flag.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.576395 runtimepy-3.9.0/runtimepy/enum/
--rw-r--r--   0 runner    (1001) docker     (127)     5599 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/enum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/enum/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/enum/type.py
--rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.576395 runtimepy-3.9.0/runtimepy/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/metrics/channel.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/metrics/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/metrics/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.580395 runtimepy-3.9.0/runtimepy/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/mixins/async_command.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/mixins/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/mixins/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/mixins/finalize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/mixins/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/mixins/regex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.580395 runtimepy-3.9.0/runtimepy/net/
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.580395 runtimepy-3.9.0/runtimepy/net/apps/
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.580395 runtimepy-3.9.0/runtimepy/net/arbiter/
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/arbiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11954 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/arbiter/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8457 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/arbiter/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.580395 runtimepy-3.9.0/runtimepy/net/arbiter/factory/
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/arbiter/factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/arbiter/factory/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/arbiter/factory/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.580395 runtimepy-3.9.0/runtimepy/net/arbiter/housekeeping/
--rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/arbiter/housekeeping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/arbiter/imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     5539 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/arbiter/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/arbiter/result.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/arbiter/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.580395 runtimepy-3.9.0/runtimepy/net/arbiter/tcp/
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/arbiter/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/arbiter/tcp/json.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/arbiter/udp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/arbiter/websocket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/backoff.py
--rw-r--r--   0 runner    (1001) docker     (127)    11292 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.580395 runtimepy-3.9.0/runtimepy/net/factories/
--rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/factories/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.584395 runtimepy-3.9.0/runtimepy/net/http/
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/http/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/http/header.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/http/request_target.py
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/http/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/http/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/http/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4140 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.584395 runtimepy-3.9.0/runtimepy/net/server/
--rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/server/html.py
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/server/json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.584395 runtimepy-3.9.0/runtimepy/net/stream/
--rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/stream/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.584395 runtimepy-3.9.0/runtimepy/net/stream/json/
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/stream/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11353 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/stream/json/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/stream/json/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/stream/json/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/stream/string.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.584395 runtimepy-3.9.0/runtimepy/net/tcp/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6911 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/tcp/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/tcp/create.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.584395 runtimepy-3.9.0/runtimepy/net/tcp/http/
--rw-r--r--   0 runner    (1001) docker     (127)     5185 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/tcp/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/tcp/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.584395 runtimepy-3.9.0/runtimepy/net/tcp/telnet/
--rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/tcp/telnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/tcp/telnet/codes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.584395 runtimepy-3.9.0/runtimepy/net/udp/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/udp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/udp/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/udp/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/udp/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.588395 runtimepy-3.9.0/runtimepy/net/websocket/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8143 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/websocket/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.588395 runtimepy-3.9.0/runtimepy/primitives/
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/primitives/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.588395 runtimepy-3.9.0/runtimepy/primitives/array/
--rw-r--r--   0 runner    (1001) docker     (127)     8311 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/primitives/array/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7561 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/primitives/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/primitives/bool.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/primitives/byte_order.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.588395 runtimepy-3.9.0/runtimepy/primitives/field/
--rw-r--r--   0 runner    (1001) docker     (127)     4138 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/primitives/field/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6620 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/primitives/field/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.588395 runtimepy-3.9.0/runtimepy/primitives/field/manager/
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/primitives/field/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/primitives/field/manager/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/primitives/float.py
--rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/primitives/int.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/primitives/scaling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.588395 runtimepy-3.9.0/runtimepy/primitives/serializable/
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/primitives/serializable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/primitives/serializable/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/primitives/serializable/fixed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/primitives/serializable/prefixed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/primitives/string.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.588395 runtimepy-3.9.0/runtimepy/primitives/type/
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/primitives/type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/primitives/type/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/primitives/type/bool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/primitives/type/bounds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/primitives/type/float.py
--rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/primitives/type/int.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.592395 runtimepy-3.9.0/runtimepy/registry/
--rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/registry/bool.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/registry/item.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/registry/name.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.592395 runtimepy-3.9.0/runtimepy/task/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5947 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/task/asynchronous.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.592395 runtimepy-3.9.0/runtimepy/task/basic/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/task/basic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/task/basic/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6169 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/task/basic/periodic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.592395 runtimepy-3.9.0/runtimepy/task/trig/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/task/trig/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.592395 runtimepy-3.9.0/runtimepy/telemetry/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/telemetry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.592395 runtimepy-3.9.0/runtimepy/tui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/tui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.592395 runtimepy-3.9.0/runtimepy/tui/channels/
--rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/tui/channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/tui/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/tui/mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/tui/mock.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/tui/task.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.592395 runtimepy-3.9.0/runtimepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6941 2024-02-26 03:24:13.000000 runtimepy-3.9.0/runtimepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5491 2024-02-26 03:24:13.000000 runtimepy-3.9.0/runtimepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 03:24:13.000000 runtimepy-3.9.0/runtimepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-26 03:24:13.000000 runtimepy-3.9.0/runtimepy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-02-26 03:24:13.000000 runtimepy-3.9.0/runtimepy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-26 03:24:13.000000 runtimepy-3.9.0/runtimepy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-26 03:24:13.596395 runtimepy-3.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-02-26 03:21:58.000000 runtimepy-3.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.592395 runtimepy-3.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-02-26 03:21:58.000000 runtimepy-3.9.0/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-02-26 03:21:58.000000 runtimepy-3.9.0/tests/test_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-02-26 03:21:58.000000 runtimepy-3.9.0/tests/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.532973 runtimepy-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-08 19:03:43.000000 runtimepy-4.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6988 2024-04-08 19:05:49.532973 runtimepy-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-04-08 19:03:43.000000 runtimepy-4.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-08 19:03:43.000000 runtimepy-4.0.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.496972 runtimepy-4.0.0/runtimepy/
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.500972 runtimepy-4.0.0/runtimepy/channel/
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/channel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.500972 runtimepy-4.0.0/runtimepy/channel/environment/
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/channel/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/channel/environment/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8984 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/channel/environment/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.500972 runtimepy-4.0.0/runtimepy/channel/environment/command/
+-rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/channel/environment/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/channel/environment/command/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5669 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/channel/environment/command/processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/channel/environment/command/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/channel/environment/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6949 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/channel/environment/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/channel/environment/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.500972 runtimepy-4.0.0/runtimepy/channel/event/
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/channel/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/channel/event/header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5774 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/channel/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.500972 runtimepy-4.0.0/runtimepy/codec/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/codec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.500972 runtimepy-4.0.0/runtimepy/codec/protocol/
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/codec/protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/codec/protocol/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/codec/protocol/json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.500972 runtimepy-4.0.0/runtimepy/codec/system/
+-rw-r--r--   0 runner    (1001) docker     (127)     6939 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/codec/system/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.504972 runtimepy-4.0.0/runtimepy/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/commands/arbiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/commands/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/commands/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/commands/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/commands/tui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.504972 runtimepy-4.0.0/runtimepy/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.504972 runtimepy-4.0.0/runtimepy/data/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/data/css/bootstrap_extra.css
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/data/css/main.css
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/data/dummy_load.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/data/factories.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)   362870 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/data/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.504972 runtimepy-4.0.0/runtimepy/data/js/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/data/js/DataConnection.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/data/js/JsonConnection.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/data/js/audio.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.508972 runtimepy-4.0.0/runtimepy/data/js/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/data/js/classes/App.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/data/js/classes/ChannelTable.js
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/data/js/classes/DataConnection.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/data/js/classes/JsonConnection.js
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/data/js/classes/Plot.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/data/js/classes/PlotManager.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/data/js/classes/TabFilter.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/data/js/classes/TabInterface.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/data/js/classes/WindowHashManager.js
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/data/js/classes/WorkerInterface.js
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/data/js/init.js
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/data/js/main.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.508972 runtimepy-4.0.0/runtimepy/data/js/tab/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/data/js/tab/env.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/data/js/tab/sound.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.508972 runtimepy-4.0.0/runtimepy/data/js/unused/
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/data/js/unused/pyodide.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/data/js/util.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/data/js/worker.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.508972 runtimepy-4.0.0/runtimepy/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/data/schemas/BitFields.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/data/schemas/Channel.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/data/schemas/ChannelCommand.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/data/schemas/ChannelRegistry.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/data/schemas/ClientConnectionConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/data/schemas/ConnectionArbiterConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/data/schemas/EnumRegistry.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/data/schemas/FindFile.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/data/schemas/RuntimeEnum.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/data/schemas/ServerConnectionConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/data/schemas/StructConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/data/schemas/TaskConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/data/schemas/has_factory.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/data/schemas/has_name.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/data/schemas/has_request_flag.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/data/server.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/data/server_base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/data/server_dev.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.508972 runtimepy-4.0.0/runtimepy/enum/
+-rw-r--r--   0 runner    (1001) docker     (127)     5819 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/enum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/enum/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/enum/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.512972 runtimepy-4.0.0/runtimepy/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/metrics/channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/metrics/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/metrics/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.512972 runtimepy-4.0.0/runtimepy/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/mixins/async_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/mixins/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/mixins/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/mixins/finalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/mixins/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/mixins/regex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.512972 runtimepy-4.0.0/runtimepy/net/
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.512972 runtimepy-4.0.0/runtimepy/net/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.512972 runtimepy-4.0.0/runtimepy/net/arbiter/
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/arbiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13412 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/arbiter/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.516972 runtimepy-4.0.0/runtimepy/net/arbiter/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     6873 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/arbiter/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/arbiter/config/codec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/arbiter/config/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.516972 runtimepy-4.0.0/runtimepy/net/arbiter/factory/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/arbiter/factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/arbiter/factory/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/arbiter/factory/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.516972 runtimepy-4.0.0/runtimepy/net/arbiter/housekeeping/
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/arbiter/housekeeping/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.516972 runtimepy-4.0.0/runtimepy/net/arbiter/imports/
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/arbiter/imports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/arbiter/imports/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/arbiter/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/arbiter/result.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.516972 runtimepy-4.0.0/runtimepy/net/arbiter/struct/
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/arbiter/struct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/arbiter/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.516972 runtimepy-4.0.0/runtimepy/net/arbiter/tcp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/arbiter/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/arbiter/tcp/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/arbiter/udp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/arbiter/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/backoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11766 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.516972 runtimepy-4.0.0/runtimepy/net/factories/
+-rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/factories/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.516972 runtimepy-4.0.0/runtimepy/net/http/
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/http/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/http/header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/http/request_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/http/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/http/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/http/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.516972 runtimepy-4.0.0/runtimepy/net/server/
+-rw-r--r--   0 runner    (1001) docker     (127)     5178 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.520973 runtimepy-4.0.0/runtimepy/net/server/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/server/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/server/app/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.520973 runtimepy-4.0.0/runtimepy/net/server/app/bootstrap/
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/server/app/bootstrap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/server/app/bootstrap/elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3794 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/server/app/bootstrap/tabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/server/app/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/server/app/elements.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.520973 runtimepy-4.0.0/runtimepy/net/server/app/env/
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/server/app/env/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/server/app/env/modal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.520973 runtimepy-4.0.0/runtimepy/net/server/app/env/tab/
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/server/app/env/tab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/server/app/env/tab/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7098 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/server/app/env/tab/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/server/app/env/tab/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4893 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/server/app/env/tab/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/server/app/env/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/server/app/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/server/app/placeholder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/server/app/pyodide.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/server/app/sound.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/server/app/tab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/server/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/server/json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.520973 runtimepy-4.0.0/runtimepy/net/server/struct/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/server/struct/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.520973 runtimepy-4.0.0/runtimepy/net/server/websocket/
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/server/websocket/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.520973 runtimepy-4.0.0/runtimepy/net/stream/
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/stream/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.520973 runtimepy-4.0.0/runtimepy/net/stream/json/
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/stream/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11453 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/stream/json/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/stream/json/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/stream/json/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/stream/string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.524973 runtimepy-4.0.0/runtimepy/net/tcp/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7377 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/tcp/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/tcp/create.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.524973 runtimepy-4.0.0/runtimepy/net/tcp/http/
+-rw-r--r--   0 runner    (1001) docker     (127)     5236 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/tcp/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/tcp/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.524973 runtimepy-4.0.0/runtimepy/net/tcp/telnet/
+-rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/tcp/telnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/tcp/telnet/codes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.524973 runtimepy-4.0.0/runtimepy/net/udp/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/udp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7485 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/udp/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/udp/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/udp/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.524973 runtimepy-4.0.0/runtimepy/net/websocket/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8068 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/net/websocket/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.524973 runtimepy-4.0.0/runtimepy/primitives/
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/primitives/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.524973 runtimepy-4.0.0/runtimepy/primitives/array/
+-rw-r--r--   0 runner    (1001) docker     (127)     8239 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/primitives/array/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7494 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/primitives/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/primitives/bool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/primitives/byte_order.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.524973 runtimepy-4.0.0/runtimepy/primitives/field/
+-rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/primitives/field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/primitives/field/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.528972 runtimepy-4.0.0/runtimepy/primitives/field/manager/
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/primitives/field/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/primitives/field/manager/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/primitives/float.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/primitives/int.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/primitives/scaling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.528972 runtimepy-4.0.0/runtimepy/primitives/serializable/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/primitives/serializable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/primitives/serializable/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/primitives/serializable/fixed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/primitives/serializable/prefixed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/primitives/string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.528972 runtimepy-4.0.0/runtimepy/primitives/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/primitives/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/primitives/types/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/primitives/types/bool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/primitives/types/bounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/primitives/types/float.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/primitives/types/int.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.528972 runtimepy-4.0.0/runtimepy/registry/
+-rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/registry/bool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/registry/item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/registry/name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.528972 runtimepy-4.0.0/runtimepy/struct/
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/struct/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.528972 runtimepy-4.0.0/runtimepy/task/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5947 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/task/asynchronous.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.528972 runtimepy-4.0.0/runtimepy/task/basic/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/task/basic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/task/basic/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6385 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/task/basic/periodic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/task/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.528972 runtimepy-4.0.0/runtimepy/task/trig/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/task/trig/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.528972 runtimepy-4.0.0/runtimepy/telemetry/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/telemetry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.532973 runtimepy-4.0.0/runtimepy/tui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/tui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.532973 runtimepy-4.0.0/runtimepy/tui/channels/
+-rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/tui/channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/tui/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/tui/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/tui/mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/tui/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-08 19:03:43.000000 runtimepy-4.0.0/runtimepy/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.532973 runtimepy-4.0.0/runtimepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6988 2024-04-08 19:05:49.000000 runtimepy-4.0.0/runtimepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7576 2024-04-08 19:05:49.000000 runtimepy-4.0.0/runtimepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 19:05:49.000000 runtimepy-4.0.0/runtimepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-08 19:05:49.000000 runtimepy-4.0.0/runtimepy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-08 19:05:49.000000 runtimepy-4.0.0/runtimepy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-08 19:05:49.000000 runtimepy-4.0.0/runtimepy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 19:05:49.532973 runtimepy-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-08 19:03:43.000000 runtimepy-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:05:49.532973 runtimepy-4.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-08 19:03:43.000000 runtimepy-4.0.0/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-08 19:03:43.000000 runtimepy-4.0.0/tests/test_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-08 19:03:43.000000 runtimepy-4.0.0/tests/test_resources.py
```

### Comparing `runtimepy-3.9.0/LICENSE` & `runtimepy-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `runtimepy-3.9.0/PKG-INFO` & `runtimepy-4.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runtimepy
-Version: 3.9.0
+Version: 4.0.0
 Summary: A framework for implementing Python services.
 Home-page: https://github.com/vkottler/runtimepy
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -13,43 +13,44 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: svgen>=0.5.0
-Requires-Dist: vcorelib>=3.2.0
 Requires-Dist: websockets
+Requires-Dist: vcorelib>=3.2.2
+Requires-Dist: svgen>=0.6.5
 Provides-Extra: test
 Requires-Dist: pylint; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: black; extra == "test"
 Requires-Dist: ruff; extra == "test"
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: isort; extra == "test"
 Requires-Dist: yamllint; extra == "test"
 Requires-Dist: yambs; extra == "test"
 Requires-Dist: vmklib; extra == "test"
 Requires-Dist: sphinx; extra == "test"
 Requires-Dist: sphinx-book-theme; extra == "test"
 Requires-Dist: pytest-asyncio; extra == "test"
+Requires-Dist: pytest-timeout; extra == "test"
 Requires-Dist: setuptools-wrapper; extra == "test"
 Requires-Dist: types-setuptools; extra == "test"
 Requires-Dist: uvloop; (sys_platform != "win32" and sys_platform != "cygwin") and extra == "test"
 
 <!--
     =====================================
     generator=datazen
     version=3.1.4
-    hash=c7bfaabcb235afbdae1921e1defa2f1a
+    hash=66a0cf61a6081296df95d09b170cf551
     =====================================
 -->
 
-# runtimepy ([3.9.0](https://pypi.org/project/runtimepy/))
+# runtimepy ([4.0.0](https://pypi.org/project/runtimepy/))
 
 [![python](https://img.shields.io/pypi/pyversions/runtimepy.svg)](https://pypi.org/project/runtimepy/)
 ![Build Status](https://github.com/vkottler/runtimepy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/runtimepy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/runtimepy)
 ![PyPI - Status](https://img.shields.io/pypi/status/runtimepy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/runtimepy)
 
@@ -80,15 +81,15 @@
 * `windows-latest`
 
 # Introduction
 
 # Command-line Options
 
 ```
-$ ./venv3.11/bin/runtimepy -h
+$ ./venv3.12/bin/runtimepy -h
 
 usage: runtimepy [-h] [--version] [-v] [-q] [--curses] [--no-uvloop] [-C DIR]
                  {arbiter,server,task,tui,noop} ...
 
 A framework for implementing Python services.
 
 options:
@@ -112,15 +113,15 @@
 ```
 
 ## Sub-command Options
 
 ### `arbiter`
 
 ```
-$ ./venv3.11/bin/runtimepy arbiter -h
+$ ./venv3.12/bin/runtimepy arbiter -h
 
 usage: runtimepy arbiter [-h] [-i] [-w] configs [configs ...]
 
 positional arguments:
   configs               the configuration to load
 
 options:
@@ -132,15 +133,15 @@
                         run last
 
 ```
 
 ### `server`
 
 ```
-$ ./venv3.11/bin/runtimepy server -h
+$ ./venv3.12/bin/runtimepy server -h
 
 usage: runtimepy server [-h] [-i] [-w] [--host HOST] [-p PORT] [-u] [-l]
                         factory [configs ...]
 
 positional arguments:
   factory               name of connection factory to create server for
   configs               the configuration to load
@@ -159,15 +160,15 @@
   -l, --loopback        if true a client of the same connection type is added
 
 ```
 
 ### `task`
 
 ```
-$ ./venv3.11/bin/runtimepy task -h
+$ ./venv3.12/bin/runtimepy task -h
 
 usage: runtimepy task [-h] [-i] [-w] [-r RATE] factory [configs ...]
 
 positional arguments:
   factory               name of task factory to create task with
   configs               the configuration to load
 
@@ -181,15 +182,15 @@
   -r RATE, --rate RATE  rate (in Hz) that the task should run (default: 10)
 
 ```
 
 ### `tui`
 
 ```
-$ ./venv3.11/bin/runtimepy tui -h
+$ ./venv3.12/bin/runtimepy tui -h
 
 usage: runtimepy tui [-h] [-i ITERATIONS] [-r RATE]
 
 options:
   -h, --help            show this help message and exit
   -i ITERATIONS, --iterations ITERATIONS
                         maximum number of program iterations (if greater than
```

### Comparing `runtimepy-3.9.0/README.md` & `runtimepy-4.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.4
-    hash=c7bfaabcb235afbdae1921e1defa2f1a
+    hash=66a0cf61a6081296df95d09b170cf551
     =====================================
 -->
 
-# runtimepy ([3.9.0](https://pypi.org/project/runtimepy/))
+# runtimepy ([4.0.0](https://pypi.org/project/runtimepy/))
 
 [![python](https://img.shields.io/pypi/pyversions/runtimepy.svg)](https://pypi.org/project/runtimepy/)
 ![Build Status](https://github.com/vkottler/runtimepy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/runtimepy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/runtimepy)
 ![PyPI - Status](https://img.shields.io/pypi/status/runtimepy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/runtimepy)
 
@@ -41,15 +41,15 @@
 * `windows-latest`
 
 # Introduction
 
 # Command-line Options
 
 ```
-$ ./venv3.11/bin/runtimepy -h
+$ ./venv3.12/bin/runtimepy -h
 
 usage: runtimepy [-h] [--version] [-v] [-q] [--curses] [--no-uvloop] [-C DIR]
                  {arbiter,server,task,tui,noop} ...
 
 A framework for implementing Python services.
 
 options:
@@ -73,15 +73,15 @@
 ```
 
 ## Sub-command Options
 
 ### `arbiter`
 
 ```
-$ ./venv3.11/bin/runtimepy arbiter -h
+$ ./venv3.12/bin/runtimepy arbiter -h
 
 usage: runtimepy arbiter [-h] [-i] [-w] configs [configs ...]
 
 positional arguments:
   configs               the configuration to load
 
 options:
@@ -93,15 +93,15 @@
                         run last
 
 ```
 
 ### `server`
 
 ```
-$ ./venv3.11/bin/runtimepy server -h
+$ ./venv3.12/bin/runtimepy server -h
 
 usage: runtimepy server [-h] [-i] [-w] [--host HOST] [-p PORT] [-u] [-l]
                         factory [configs ...]
 
 positional arguments:
   factory               name of connection factory to create server for
   configs               the configuration to load
@@ -120,15 +120,15 @@
   -l, --loopback        if true a client of the same connection type is added
 
 ```
 
 ### `task`
 
 ```
-$ ./venv3.11/bin/runtimepy task -h
+$ ./venv3.12/bin/runtimepy task -h
 
 usage: runtimepy task [-h] [-i] [-w] [-r RATE] factory [configs ...]
 
 positional arguments:
   factory               name of task factory to create task with
   configs               the configuration to load
 
@@ -142,15 +142,15 @@
   -r RATE, --rate RATE  rate (in Hz) that the task should run (default: 10)
 
 ```
 
 ### `tui`
 
 ```
-$ ./venv3.11/bin/runtimepy tui -h
+$ ./venv3.12/bin/runtimepy tui -h
 
 usage: runtimepy tui [-h] [-i ITERATIONS] [-r RATE]
 
 options:
   -h, --help            show this help message and exit
   -i ITERATIONS, --iterations ITERATIONS
                         maximum number of program iterations (if greater than
```

### Comparing `runtimepy-3.9.0/pyproject.toml` & `runtimepy-4.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "runtimepy"
-version = "3.9.0"
+version = "4.0.0"
 description = "A framework for implementing Python services."
 readme = "README.md"
 requires-python = ">=3.11"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
@@ -36,14 +36,15 @@
   "isort",
   "yamllint",
   "yambs",
   "vmklib",
   "sphinx",
   "sphinx-book-theme",
   "pytest-asyncio",
+  "pytest-timeout",
   "setuptools-wrapper",
   "types-setuptools",
   "uvloop; sys_platform != 'win32' and sys_platform != 'cygwin'"
 ]
 
 [project.scripts]
 runtimepy = "runtimepy.entry:main"
```

### Comparing `runtimepy-3.9.0/runtimepy/app.py` & `runtimepy-4.0.0/runtimepy/app.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.9.0/runtimepy/channel/__init__.py` & `runtimepy-4.0.0/runtimepy/channel/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 A module implementing a basic channel interface.
 """
 
 # built-in
 from typing import Generic as _Generic
+from typing import Optional as _Optional
 from typing import Union as _Union
 from typing import cast as _cast
 
 # third-party
 from vcorelib.io.types import JsonObject as _JsonObject
 
 # internal
@@ -22,15 +23,15 @@
 from runtimepy.primitives.int import Int16 as _Int16
 from runtimepy.primitives.int import Int32 as _Int32
 from runtimepy.primitives.int import Int64 as _Int64
 from runtimepy.primitives.int import Uint8 as _Uint8
 from runtimepy.primitives.int import Uint16 as _Uint16
 from runtimepy.primitives.int import Uint32 as _Uint32
 from runtimepy.primitives.int import Uint64 as _Uint64
-from runtimepy.primitives.type import AnyPrimitiveType as _AnyPrimitiveType
+from runtimepy.primitives.types import AnyPrimitiveType as _AnyPrimitiveType
 from runtimepy.registry.item import RegistryItem as _RegistryItem
 
 
 class Channel(_RegistryItem, _EnumMixin, _Generic[_T]):
     """An interface for an individual channel."""
 
     def __str__(self) -> str:
@@ -56,27 +57,34 @@
 
         # Whether or not this channel should accept commands.
         self.commandable: bool = _cast(bool, data["commandable"])
 
         # A key to this channel's enumeration in the enumeration registry.
         self._enum = _cast(str, data.get("enum"))
 
+        self.description: _Optional[str] = _cast(str, data.get("description"))
+
         # An event-streaming interface.
         self.event = PrimitiveEvent(self.raw, self.id)
 
     def asdict(self) -> _JsonObject:
         """Obtain a dictionary representing this instance."""
 
         result = {
             "id": self.id,
             "type": str(self.type),
             "commandable": self.commandable,
         }
+
         if self._enum is not None:
             result["enum"] = self._enum
+
+        if self.description:
+            result["description"] = self.description
+
         return _cast(_JsonObject, result)
 
 
 # Convenient type definitions.
 IntChannel = _Union[
     Channel[_Int8],
     Channel[_Int16],
```

### Comparing `runtimepy-3.9.0/runtimepy/channel/environment/__init__.py` & `runtimepy-4.0.0/runtimepy/channel/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.9.0/runtimepy/channel/environment/array.py` & `runtimepy-4.0.0/runtimepy/channel/environment/array.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 """
 A channel-environment extension for creating arrays of primitives.
 """
 
 # built-in
 from typing import Iterable as _Iterable
-from typing import List as _List
 from typing import NamedTuple
 from typing import Optional as _Optional
-from typing import Set as _Set
 
 # internal
 from runtimepy.channel.environment.base import (
     BaseChannelEnvironment as _BaseChannelEnvironment,
 )
 from runtimepy.primitives.array import PrimitiveArray as _PrimitiveArray
 from runtimepy.primitives.field.fields import BitFields as _BitFields
 from runtimepy.registry.name import RegistryKey as _RegistryKey
 
 
 class ChannelArray(NamedTuple):
     """A class for managing an array of channels and bit-fields."""
 
-    names: _List[str]
+    names: list[str]
     array: _PrimitiveArray
 
     @staticmethod
     def create() -> "ChannelArray":
         """Create a new, empty channel array."""
         return ChannelArray([], _PrimitiveArray())
 
@@ -39,18 +37,18 @@
         """
         Create a primitive array from an in-order iterable of registry keys.
         """
 
         result = ChannelArray.create()
 
         curr_fields: _Optional[_BitFields] = None
-        invalid_field_names: _Set[str] = set()
-        available_field_names: _Set[str] = set()
+        invalid_field_names: set[str] = set()
+        available_field_names: set[str] = set()
 
-        names: _Set[str] = set()
+        names: set[str] = set()
 
         for key in keys:
             # All keys must be registered names.
             name = self.channels.names.name(key)
             assert name is not None, f"Unknown name '{key}'!"
 
             # Ensure channels and fields don't appear twice.
```

### Comparing `runtimepy-3.9.0/runtimepy/channel/environment/base.py` & `runtimepy-4.0.0/runtimepy/channel/environment/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 """
 A module implementing a base channel environment.
 """
 
 # built-in
-from typing import Dict as _Dict
 from typing import Iterable as _Iterable
 from typing import Optional as _Optional
-from typing import Set as _Set
-from typing import Tuple as _Tuple
 from typing import Union as _Union
 from typing import cast as _cast
 
 # third-party
 from vcorelib.namespace import DEFAULT_DELIM, Namespace
 from vcorelib.namespace import NamespaceMixin as _NamespaceMixin
 
@@ -29,20 +26,20 @@
 from runtimepy.primitives.field.fields import BitFields as _BitFields
 from runtimepy.primitives.field.manager import (
     BitFieldsManager as _BitFieldsManager,
 )
 from runtimepy.registry.name import RegistryKey as _RegistryKey
 
 ChannelValue = _Union[bool, int, float, str]
-ValueMap = _Dict[_RegistryKey, ChannelValue]
+ValueMap = dict[_RegistryKey, ChannelValue]
 
-ChannelResult = _Tuple[_AnyChannel, _Optional[_RuntimeEnum]]
-BitfieldResult = _Tuple[_BitField, _Optional[_RuntimeEnum]]
-BoolChannelResult = _Tuple[_BoolChannel, _Optional[_RuntimeEnum]]
-IntChannelResult = _Tuple[_IntChannel, _Optional[_RuntimeEnum]]
+ChannelResult = tuple[_AnyChannel, _Optional[_RuntimeEnum]]
+BitfieldResult = tuple[_BitField, _Optional[_RuntimeEnum]]
+BoolChannelResult = tuple[_BoolChannel, _Optional[_RuntimeEnum]]
+IntChannelResult = tuple[_IntChannel, _Optional[_RuntimeEnum]]
 
 FieldOrChannel = _Union[_BitField, _AnyChannel]
 
 
 class BaseChannelEnvironment(_NamespaceMixin, FinalizeMixin):
     """A class integrating channel and enumeration registries."""
 
@@ -65,43 +62,49 @@
         if channels is None:
             channels = _ChannelRegistry()
         if enums is None:
             enums = _EnumRegistry()
 
         self.channels = channels
         self.enums = enums
-        self.fields = _BitFieldsManager(channels.names, enums, fields=fields)
+        self.fields = _BitFieldsManager(
+            channels.names, self.enums, fields=fields
+        )
 
         # Keep a mapping of each channel's name and integer identifier to the
         # underlying enumeration.
-        self.channel_enums: _Dict[_AnyChannel, _RuntimeEnum] = {
+        self.channel_enums: dict[_AnyChannel, _RuntimeEnum] = {
             chan: self.enums[chan.enum]
             for chan in self.channels.items.values()
             if chan.is_enum
         }
 
         # Organize channel by Python type.
-        self.bools: _Set[_BoolChannel] = {
+        self.bools: set[_BoolChannel] = {
             chan
             for chan in self.channels.items.values()
             if chan.type.is_boolean
         }
-        self.ints: _Set[_IntChannel] = {
+        self.ints: set[_IntChannel] = {
             chan
             for chan in self.channels.items.values()
             if chan.type.is_integer
         }
-        self.floats: _Set[_FloatChannel] = {
+        self.floats: set[_FloatChannel] = {
             chan for chan in self.channels.items.values() if chan.type.is_float
         }
 
         # Apply initial values if they were provided.
         if values is not None:
             self.apply(values)
 
+    def __setitem__(self, key: _RegistryKey, value: ChannelValue) -> None:
+        """Mapping-set interface."""
+        return self.set(key, value)
+
     def set(self, key: _RegistryKey, value: ChannelValue) -> None:
         """Attempt to set an arbitrary channel value."""
 
         # Set a field value if this key maps to a bit-field.
         if self.fields.has_field(key):
             assert not isinstance(value, float)
             self.fields.set(key, value)
```

### Comparing `runtimepy-3.9.0/runtimepy/channel/environment/command/__init__.py` & `runtimepy-4.0.0/runtimepy/channel/environment/command/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -231,15 +231,15 @@
 
         assert (
             name not in self or self[name] is env
         ), f"Can't register environment '{name}'!"
 
         if name not in self:
             self[name] = env
-            self.logger.info("Registered channel environment '%s'.", name)
+            self.logger.debug("Registered channel environment '%s'.", name)
 
 
 GLOBAL = GlobalEnvironment()
 ENVIRONMENTS = GLOBAL
 
 
 def clear_env() -> None:
```

### Comparing `runtimepy-3.9.0/runtimepy/channel/environment/command/parser.py` & `runtimepy-4.0.0/runtimepy/channel/environment/command/parser.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.9.0/runtimepy/channel/environment/command/processor.py` & `runtimepy-4.0.0/runtimepy/channel/environment/command/processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         """Initialize this instance."""
 
         super().__init__(env=env, **kwargs)
         self.logger = logger
         self.hooks: list[CommandHook] = []
 
         self.parser_data: dict[str, Any] = {}
-        self.parser = CommandParser()
+        self.parser = CommandParser(prog="")
         self.parser.data = self.parser_data
 
         self.parser.initialize()
 
     def get_suggestion(self, value: str) -> Optional[str]:
         """Get an input suggestion."""
```

### Comparing `runtimepy-3.9.0/runtimepy/channel/environment/command/result.py` & `runtimepy-4.0.0/runtimepy/channel/environment/command/result.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.9.0/runtimepy/channel/environment/create.py` & `runtimepy-4.0.0/runtimepy/channel/environment/create.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 )
 from runtimepy.channel.environment.base import (
     IntChannelResult as _IntChannelResult,
 )
 from runtimepy.channel.environment.base import ChannelResult as _ChannelResult
 from runtimepy.enum import RuntimeEnum as _RuntimeEnum
 from runtimepy.enum.registry import DEFAULT_ENUM_PRIMITIVE
-from runtimepy.enum.type import EnumTypelike as _EnumTypelike
+from runtimepy.enum.types import EnumTypelike as _EnumTypelike
 from runtimepy.mapping import EnumMappingData as _EnumMappingData
 from runtimepy.primitives import ChannelScaling, Primitive
 from runtimepy.primitives import Primitivelike as _Primitivelike
 from runtimepy.primitives.field import BitField
 from runtimepy.primitives.field.fields import BitFields
 from runtimepy.registry.name import RegistryKey as _RegistryKey
 
@@ -40,29 +40,35 @@
         self,
         name: str,
         kind: _Union[Primitive[_Any], _Primitivelike],
         commandable: bool = False,
         enum: _Union[_RegistryKey, _RuntimeEnum] = None,
         namespace: _Namespace = None,
         scaling: ChannelScaling = None,
+        **kwargs,
     ) -> _ChannelResult:
         """Create a new channel from the environment."""
 
         assert not self.finalized, "Environment already finalized!"
 
         # Apply the current (or provided) namespace.
         name = self.namespace(name=name, namespace=namespace)
 
         if enum is not None:
             if isinstance(enum, _RuntimeEnum):
                 enum = enum.id
 
         # Register the channel.
         result = self.channels.channel(
-            name, kind, commandable=commandable, enum=enum, scaling=scaling
+            name,
+            kind,
+            commandable=commandable,
+            enum=enum,
+            scaling=scaling,
+            **kwargs,
         )
         assert result is not None, f"Can't create channel '{name}'!"
 
         # Keep track of any new enum channels.
         if enum is not None:
             self.channel_enums[result] = self.enums[enum]
 
@@ -72,60 +78,70 @@
         self,
         name: str,
         kind: _Union[Primitive[_Any], _Primitivelike] = "uint32",
         commandable: bool = False,
         enum: _Union[_RegistryKey, _RuntimeEnum] = None,
         namespace: _Namespace = None,
         scaling: ChannelScaling = None,
+        **kwargs,
     ) -> _IntChannelResult:
         """Create an integer channel."""
 
         result = self.channel(
             name,
             kind,
             commandable=commandable,
             enum=enum,
             namespace=namespace,
             scaling=scaling,
+            **kwargs,
         )
         assert result[0].raw.kind.is_integer
         return _cast(_IntChannelResult, result)
 
     def bool_channel(
         self,
         name: str,
         kind: _Union[Primitive[_Any], _Primitivelike] = "bool",
         commandable: bool = False,
         enum: _Union[_RegistryKey, _RuntimeEnum] = None,
         namespace: _Namespace = None,
+        **kwargs,
     ) -> _BoolChannelResult:
         """Create a boolean channel."""
 
         result = self.channel(
-            name, kind, commandable=commandable, enum=enum, namespace=namespace
+            name,
+            kind,
+            commandable=commandable,
+            enum=enum,
+            namespace=namespace,
+            **kwargs,
         )
         assert result[0].raw.kind.is_boolean
         return _cast(_BoolChannelResult, result)
 
     def float_channel(
         self,
         name: str,
         kind: _Union[Primitive[_Any], _Primitivelike] = "float",
         commandable: bool = False,
         namespace: _Namespace = None,
         scaling: ChannelScaling = None,
+        **kwargs,
     ) -> _FloatChannel:
         """Create a floating-point channel."""
 
         result = self.channel(
             name,
             kind,
             commandable=commandable,
             namespace=namespace,
             scaling=scaling,
+            **kwargs,
         )[0]
         assert result.raw.kind.is_float
         return _cast(_FloatChannel, result)
 
     def enum(
         self,
         name: str,
@@ -148,8 +164,9 @@
     def add_field(self, field: BitField, namespace: _Namespace = None) -> str:
         """Add a bit field to the environment."""
 
         fields = BitFields.new()
         name = self.namespace(name=field.name, namespace=namespace)
         fields.fields[name] = field
         self.fields.add(fields)
+
         return name
```

### Comparing `runtimepy-3.9.0/runtimepy/channel/environment/file.py` & `runtimepy-4.0.0/runtimepy/channel/environment/file.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 """
 A channel-environment extension for loading and saving files.
 """
 
 # built-in
-from typing import Dict as _Dict
 from typing import Optional as _Optional
-from typing import Type as _Type
 from typing import TypeVar as _TypeVar
 from typing import cast as _cast
 
 # third-party
 from vcorelib.io import ARBITER as _ARBITER
 from vcorelib.io.types import JsonObject as _JsonObject
 from vcorelib.io.types import JsonValue as _JsonValue
@@ -45,17 +43,15 @@
 FIELDS_FILE = f"{FIELDS_KEY}.json"
 NAMES_FILE = f"{NAMES_KEY}.json"
 
 
 class FileChannelEnvironment(_BaseChannelEnvironment):
     """A class integrating file-system operations with channel environments."""
 
-    def export_json(
-        self, resolve_enum: bool = True
-    ) -> _Dict[str, _JsonObject]:
+    def export_json(self, resolve_enum: bool = True) -> dict[str, _JsonObject]:
         """Get this channel environment as a single dictionary."""
 
         # Only allow exporting finalized environments.
         self.finalize(strict=False)
 
         return {
             CHANNELS_KEY: self.channels.asdict(),
@@ -123,15 +119,15 @@
             names=path.joinpath(NAMES_FILE),
             resolve_enum=resolve_enum,
             **kwargs,
         )
 
     @classmethod
     def load_json(
-        cls: _Type[T], data: _Dict[str, _JsonObject], finalize: bool = True
+        cls: type[T], data: dict[str, _JsonObject], finalize: bool = True
     ) -> T:
         """Load a channel environment from JSON data."""
 
         chan_reg = _ChannelRegistry.create(data[CHANNELS_KEY])
         enum_reg = _EnumRegistry.create(data[ENUMS_KEY])
 
         # Handle name data.
@@ -154,15 +150,15 @@
         if finalize:
             result.finalize()
 
         return result
 
     @classmethod
     def load(
-        cls: _Type[T],
+        cls: type[T],
         channels: _Pathlike = CHANNELS_FILE,
         enums: _Pathlike = ENUMS_FILE,
         values: _Pathlike = VALUES_FILE,
         fields: _Pathlike = FIELDS_FILE,
         names: _Pathlike = NAMES_FILE,
         finalize: bool = True,
     ) -> T:
@@ -202,15 +198,15 @@
         if finalize:
             result.finalize()
 
         return result
 
     @classmethod
     def load_directory(
-        cls: _Type[T], path: _Pathlike, finalize: bool = True
+        cls: type[T], path: _Pathlike, finalize: bool = True
     ) -> T:
         """Load a channel environment from a directory."""
 
         path = _normalize(path, require=True)
         assert path.is_dir(), f"'{path}' is not a directory!"
         return cls.load(
             channels=path.joinpath(CHANNELS_FILE),
```

### Comparing `runtimepy-3.9.0/runtimepy/channel/event/__init__.py` & `runtimepy-4.0.0/runtimepy/channel/event/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.9.0/runtimepy/channel/event/header.py` & `runtimepy-4.0.0/runtimepy/channel/event/header.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.9.0/runtimepy/channel/registry.py` & `runtimepy-4.0.0/runtimepy/channel/registry.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 """
 
 # built-in
 from contextlib import ExitStack, contextmanager
 from typing import Any as _Any
 from typing import BinaryIO, Iterable, Iterator, NamedTuple
 from typing import Optional as _Optional
-from typing import Type as _Type
 from typing import Union, cast
 
 # third-party
 from vcorelib.io import ByteFifo
 from vcorelib.io.types import JsonObject as _JsonObject
 
 # internal
@@ -20,15 +19,15 @@
 from runtimepy.channel.event.header import PrimitiveEventHeader
 from runtimepy.codec.protocol import Protocol
 from runtimepy.mapping import DEFAULT_PATTERN
 from runtimepy.mixins.regex import CHANNEL_PATTERN as _CHANNEL_PATTERN
 from runtimepy.primitives import ChannelScaling, Primitive
 from runtimepy.primitives import Primitivelike as _Primitivelike
 from runtimepy.primitives import normalize
-from runtimepy.primitives.type.base import PythonPrimitive
+from runtimepy.primitives.types.base import PythonPrimitive
 from runtimepy.registry import Registry as _Registry
 from runtimepy.registry.name import NameRegistry as _NameRegistry
 from runtimepy.registry.name import RegistryKey as _RegistryKey
 
 
 class ChannelNameRegistry(_NameRegistry):
     """A name registry with a name-matching pattern for channel names."""
@@ -66,15 +65,15 @@
     name_registry = ChannelNameRegistry
 
     event_header: Protocol
     event_fifo: ByteFifo
     header_ready: bool
 
     @property
-    def kind(self) -> _Type[_Channel[_Any]]:
+    def kind(self) -> type[_Channel[_Any]]:
         """Determine what kind of registry this is."""
         return _Channel
 
     def init(self, data: _JsonObject) -> None:
         """Perform implementation-specific initialization."""
 
         super().init(data)
@@ -85,14 +84,15 @@
     def channel(
         self,
         name: str,
         kind: Union[Primitive[_Any], _Primitivelike],
         commandable: bool = False,
         enum: _RegistryKey = None,
         scaling: ChannelScaling = None,
+        description: str = None,
     ) -> _Optional[_AnyChannel]:
         """Create a new channel."""
 
         if isinstance(kind, str):
             kind = normalize(kind)
 
         if isinstance(kind, Primitive):
@@ -110,14 +110,17 @@
         data: _JsonObject = {
             "type": str(primitive.kind),
             "commandable": commandable,
         }
         if enum is not None:
             data["enum"] = enum
 
+        if description:
+            data["description"] = description
+
         result = self.register_dict(name, data)
 
         # Replace the underlying primitive, in case it was direclty passed in.
         if result is not None:
             result.raw = primitive
             result.event.primitive = primitive  # type: ignore
```

### Comparing `runtimepy-3.9.0/runtimepy/codec/protocol/__init__.py` & `runtimepy-4.0.0/runtimepy/codec/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.9.0/runtimepy/codec/protocol/base.py` & `runtimepy-4.0.0/runtimepy/codec/protocol/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 """
 A module implementing an interface to build communication protocols.
 """
 
 # built-in
 from contextlib import contextmanager
 from copy import copy as _copy
-from typing import Dict as _Dict
 from typing import Iterator as _Iterator
-from typing import List as _List
 from typing import NamedTuple
 from typing import Optional as _Optional
 from typing import TypeVar as _TypeVar
 from typing import Union as _Union
 
 # third-party
 from vcorelib.io.types import JsonObject as _JsonObject
@@ -65,15 +63,15 @@
     """A class for defining runtime communication protocols."""
 
     def __init__(
         self,
         enum_registry: _EnumRegistry,
         names: _NameRegistry = None,
         fields: BitFieldsManager = None,
-        build: _List[_Union[int, FieldSpec, str]] = None,
+        build: list[_Union[int, FieldSpec, str]] = None,
         identifier: int = 1,
         byte_order: _Union[_ByteOrder, _RegistryKey] = _DEFAULT_BYTE_ORDER,
         serializables: SerializableMap = None,
     ) -> None:
         """Initialize this protocol."""
 
         self.id = identifier
@@ -94,19 +92,19 @@
             names = _NameRegistry()
         self.names = names
 
         if fields is None:
             fields = BitFieldsManager(self.names, self._enum_registry)
         self._fields = fields
 
-        self._regular_fields: _Dict[str, _AnyPrimitive] = {}
-        self._enum_fields: _Dict[str, _RuntimeEnum] = {}
+        self._regular_fields: dict[str, _AnyPrimitive] = {}
+        self._enum_fields: dict[str, _RuntimeEnum] = {}
 
         # Keep track of the order that the protocol was created.
-        self._build: _List[_Union[int, FieldSpec, str]] = []
+        self._build: list[_Union[int, FieldSpec, str]] = []
 
         # Keep track of named serializables.
         self.serializables: SerializableMap = {}
 
         # Add fields if necessary.
         if build is None:
             build = []
```

### Comparing `runtimepy-3.9.0/runtimepy/codec/protocol/json.py` & `runtimepy-4.0.0/runtimepy/codec/protocol/json.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 """
 A protocol extension for importing and exporting JSON.
 """
 
 # built-in
 from json import dumps as _dumps
 from typing import BinaryIO as _BinaryIO
-from typing import Dict as _Dict
-from typing import List as _List
-from typing import Set as _Set
-from typing import Type as _Type
 from typing import TypeVar as _TypeVar
 from typing import Union as _Union
 from typing import cast as _cast
 
 # third-party
 from vcorelib.io.types import JsonObject as _JsonObject
 from vcorelib.io.types import JsonValue as _JsonValue
@@ -42,17 +38,15 @@
         """Get protocol metadata as a bytes object."""
         return self.meta_str(resolve_enum=resolve_enum).encode()
 
     def write_meta(self, stream: _BinaryIO, resolve_enum: bool = True) -> int:
         """Write protocol metadata to a stream."""
         return stream.write(self.meta_bytes(resolve_enum=resolve_enum))
 
-    def export_json(
-        self, resolve_enum: bool = True
-    ) -> _Dict[str, _JsonObject]:
+    def export_json(self, resolve_enum: bool = True) -> dict[str, _JsonObject]:
         """Export this protocol's data to JSON."""
 
         data = self._fields.export_json(resolve_enum=resolve_enum)
         data[META_KEY] = {
             "id": self.id,
             "byte_order": self.array.byte_order.name.lower(),
         }
@@ -63,26 +57,26 @@
             {
                 name: self.names.identifier(name)
                 for name in self._regular_fields
             }
         )
 
         # Export enums used by regular fields.
-        enum_ids: _Set[int] = {x.id for x in self._enum_fields.values()}
+        enum_ids: set[int] = {x.id for x in self._enum_fields.values()}
         json_obj = data[ENUMS_KEY]
         json_obj.update(
             {
                 name: _cast(_JsonValue, val.asdict())
                 for name, val in self._enum_registry.items.items()
                 if val.id in enum_ids and name not in json_obj
             }
         )
 
         # Export the build specification.
-        build: _List[_Union[int, _JsonObject, str]] = []
+        build: list[_Union[int, _JsonObject, str]] = []
         for item in self._build:
             if isinstance(item, (int, str)):
                 build.append(item)
             else:
                 build.append(item.asdict())
         data[BUILD_KEY] = _cast(_JsonObject, build)
 
@@ -92,26 +86,26 @@
             json_obj[name] = self.value(name)
         if json_obj:
             data[VALUES_KEY] = json_obj
 
         return data
 
     @classmethod
-    def import_json(cls: _Type[T], data: _Dict[str, _JsonObject]) -> T:
+    def import_json(cls: type[T], data: dict[str, _JsonObject]) -> T:
         """Create a bit-fields manager from JSON data."""
 
         # Only set values once (at the end).
         values = data.get(VALUES_KEY, {})
         if VALUES_KEY in data:
             del data[VALUES_KEY]
 
         fields = BitFieldsManager.import_json(data)
 
         # Create the build specification.
-        build: _List[_Union[int, FieldSpec, str]] = []
+        build: list[_Union[int, FieldSpec, str]] = []
         for item in data[BUILD_KEY]:
             if isinstance(item, int):
                 build.append(item)
             else:
                 build.append(
                     FieldSpec(
                         item["name"],  # type: ignore
```

### Comparing `runtimepy-3.9.0/runtimepy/codec/system/__init__.py` & `runtimepy-4.0.0/runtimepy/codec/system/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 A basic type-system implementation.
 """
 
 # built-in
-from typing import Dict, Iterable, Optional, Type
+from typing import Iterable, Optional
 
 # third-party
 from vcorelib.logging import LoggerMixin
 from vcorelib.namespace import CPP_DELIM, Namespace
 
 # internal
 from runtimepy import PKG_NAME
@@ -15,15 +15,15 @@
 from runtimepy.enum import RuntimeEnum
 from runtimepy.enum.registry import (
     DEFAULT_ENUM_PRIMITIVE,
     EnumRegistry,
     RuntimeIntEnum,
 )
 from runtimepy.primitives.byte_order import ByteOrder
-from runtimepy.primitives.type import AnyPrimitiveType, PrimitiveTypes
+from runtimepy.primitives.types import AnyPrimitiveType, PrimitiveTypes
 
 
 def resolve_name(matches: Iterable[str]) -> str:
     """Resolve a possible name conflict."""
 
     by_len: dict[int, list[str]] = {}
     shortest = -1
@@ -44,16 +44,16 @@
     """A class for managing a custom type system."""
 
     def __init__(self, *namespace: str) -> None:
         """Initialize this instance."""
 
         super().__init__()
 
-        self.primitives: Dict[str, AnyPrimitiveType] = {}
-        self.custom: Dict[str, Protocol] = {}
+        self.primitives: dict[str, AnyPrimitiveType] = {}
+        self.custom: dict[str, Protocol] = {}
         self._enums = EnumRegistry()
 
         global_namespace = Namespace(delim=CPP_DELIM)
 
         # Register global names.
         for name, kind in PrimitiveTypes.items():
             self.primitives[global_namespace.namespace(name)] = kind
@@ -72,25 +72,25 @@
     ) -> RuntimeEnum:
         """Lookup an enum type at runtime."""
 
         found = self._find_name(name, *namespace, strict=True, exact=exact)
         assert found is not None
         return self._enums[found]
 
-    def runtime_int_enum(self, enum: Type[RuntimeIntEnum]) -> None:
+    def runtime_int_enum(self, enum: type[RuntimeIntEnum]) -> None:
         """Register an enumeration class."""
 
         name = self._name(enum.enum_name(), check_available=True)
         runtime = enum.register_enum(self._enums, name=name)
         self._register_primitive(name, runtime.primitive)
 
     def enum(
         self,
         name: str,
-        items: Dict[str, int],
+        items: dict[str, int],
         *namespace: str,
         primitive: str = DEFAULT_ENUM_PRIMITIVE,
     ) -> None:
         """Register an enumeration."""
 
         name = self._name(name, *namespace, check_available=True)
```

### Comparing `runtimepy-3.9.0/runtimepy/commands/all.py` & `runtimepy-4.0.0/runtimepy/commands/all.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.9.0/runtimepy/commands/arbiter.py` & `runtimepy-4.0.0/runtimepy/commands/arbiter.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.9.0/runtimepy/commands/common.py` & `runtimepy-4.0.0/runtimepy/commands/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,26 +2,31 @@
 A module for package command-line argument interfaces.
 """
 
 # built-in
 from argparse import ArgumentParser as _ArgumentParser
 from argparse import Namespace as _Namespace
 from contextlib import contextmanager
-from typing import Any, Dict, Iterator
+from typing import Any, Iterator
 
 # third-party
 from vcorelib.args import CommandFunction as _CommandFunction
 from vcorelib.io import ARBITER
 from vcorelib.paths.context import tempfile
 
+# internal
+from runtimepy import DEFAULT_EXT, PKG_NAME
+
 try:
     import curses as _curses
 except ModuleNotFoundError:  # pragma: nocover
     _curses = {}  # type: ignore
 
+FACTORIES = f"package://{PKG_NAME}/factories.{DEFAULT_EXT}"
+
 
 def arbiter_flags(parser: _ArgumentParser) -> None:
     """Add arbiter command-line flag arguments."""
 
     parser.add_argument(
         "-i",
         "--init_only",
@@ -70,15 +75,15 @@
     yield
     parser.add_argument(
         "configs", nargs=nargs, help="the configuration to load"
     )
 
 
 def cmd_with_jit(
-    command: _CommandFunction, args: _Namespace, data: Dict[str, Any]
+    command: _CommandFunction, args: _Namespace, data: dict[str, Any]
 ) -> int:
     """Run an 'arbiter' command with custom data inserted."""
 
-    with tempfile(suffix=".yaml") as temp_config:
+    with tempfile(suffix=f".{DEFAULT_EXT}") as temp_config:
         ARBITER.encode(temp_config, data)
         args.configs.append(str(temp_config))
         return command(args)
```

### Comparing `runtimepy-3.9.0/runtimepy/commands/server.py` & `runtimepy-4.0.0/runtimepy/commands/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,51 +1,50 @@
 """
 An entry-point for the 'server' command.
 """
 
 # built-in
 from argparse import ArgumentParser as _ArgumentParser
 from argparse import Namespace as _Namespace
-from typing import Any, Dict, List
+from typing import Any
 
 # third-party
 from vcorelib.args import CommandFunction as _CommandFunction
 
 # internal
-from runtimepy import PKG_NAME
 from runtimepy.commands.arbiter import arbiter_cmd
-from runtimepy.commands.common import arbiter_args, cmd_with_jit
+from runtimepy.commands.common import FACTORIES, arbiter_args, cmd_with_jit
 
 
 def port_name(args: _Namespace, port: str = "port") -> str:
     """Get the name for a connection factory's port."""
     return f"{args.factory}_{'udp' if args.udp else 'tcp'}_{port}"
 
 
-def server_data(args: _Namespace) -> Dict[str, Any]:
+def server_data(args: _Namespace) -> dict[str, Any]:
     """Get server data based on command-line arguments."""
 
     return {
         "factory": args.factory,
         "kwargs": {"port": f"${port_name(args)}", "host": args.host},
     }
 
 
 def is_websocket(args: _Namespace) -> bool:
     """Determine if the specified factory uses WebSocket or not."""
     return "websocket" in args.factory.lower()
 
 
-def client_data(args: _Namespace) -> Dict[str, Any]:
+def client_data(args: _Namespace) -> dict[str, Any]:
     """Get client data based on command-line arguments."""
 
     port = f"${port_name(args)}"
 
-    arg_list: List[Any] = []
-    kwargs: Dict[str, Any] = {}
+    arg_list: list[Any] = []
+    kwargs: dict[str, Any] = {}
 
     if is_websocket(args):
         arg_list.append(f"ws://localhost:{port}")
     elif not args.udp:
         kwargs["host"] = "localhost"
         kwargs["port"] = port
     else:
@@ -60,15 +59,15 @@
         result["args"] = arg_list
     if kwargs:
         result["kwargs"] = kwargs
 
     return result
 
 
-def config_data(args: _Namespace) -> Dict[str, Any]:
+def config_data(args: _Namespace) -> dict[str, Any]:
     """Get configuration data for the 'server' command."""
 
     servers = []
     clients = []
 
     if not args.udp:
         servers.append(server_data(args))
@@ -82,15 +81,15 @@
         )
 
     # Add a loopback connection if specified.
     if args.loopback:
         clients.append(client_data(args))
 
     return {
-        "includes": [f"package://{PKG_NAME}/factories.yaml"],
+        "includes": [FACTORIES] + args.configs,
         "clients": clients,
         "servers": servers,
         "ports": [
             {
                 "name": port_name(args),
                 "port": args.port,
                 "type": "udp" if args.udp else "tcp",
```

### Comparing `runtimepy-3.9.0/runtimepy/commands/task.py` & `runtimepy-4.0.0/runtimepy/commands/task.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 """
 An entry-point for the 'task' command.
 """
 
 # built-in
 from argparse import ArgumentParser as _ArgumentParser
 from argparse import Namespace as _Namespace
-from typing import Any, Dict
+from typing import Any
 
 # third-party
 from vcorelib.args import CommandFunction as _CommandFunction
 
 # internal
-from runtimepy import PKG_NAME
 from runtimepy.commands.arbiter import arbiter_cmd
-from runtimepy.commands.common import arbiter_args, cmd_with_jit
+from runtimepy.commands.common import FACTORIES, arbiter_args, cmd_with_jit
 
 
-def config_data(args: _Namespace) -> Dict[str, Any]:
+def config_data(args: _Namespace) -> dict[str, Any]:
     """Get configuration data for the 'task' command."""
 
     return {
-        "includes": [f"package://{PKG_NAME}/factories.yaml"],
+        "includes": [FACTORIES],
         "tasks": [
             {
                 "name": args.factory,
                 "factory": args.factory,
                 "period_s": 1.0 / args.rate,
             }
         ],
```

### Comparing `runtimepy-3.9.0/runtimepy/commands/tui.py` & `runtimepy-4.0.0/runtimepy/commands/tui.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.9.0/runtimepy/data/factories.yaml` & `runtimepy-4.0.0/runtimepy/data/factories.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -15,16 +15,23 @@
   - {name: runtimepy.net.factories.UdpNull, namespaces: [udp, "null"]}
   - name: runtimepy.net.factories.WebsocketNull
     namespaces: [websocket, "null"]
 
   # Useful protocols.
   - {name: runtimepy.net.factories.Http}
   - {name: runtimepy.net.factories.RuntimepyHttp}
+  - {name: runtimepy.net.factories.RuntimepyWebsocketJson}
+  - {name: runtimepy.net.factories.RuntimepyWebsocketData}
 
   # Useful tasks.
   - {name: runtimepy.task.trig.Sinusoid}
+  - {name: runtimepy.task.sample.Sample}
+
+  # Useful structs.
+  - {name: runtimepy.net.arbiter.struct.SampleStruct}
+  - {name: runtimepy.net.server.struct.UiState}
 
 ports:
   # Reserve ports for JSON listeners.
   - {name: udp_json, type: udp}
   - {name: tcp_json, type: tcp}
   - {name: websocket_json, type: tcp}
```

### Comparing `runtimepy-3.9.0/runtimepy/data/favicon.ico` & `runtimepy-4.0.0/runtimepy/data/favicon.ico`

 * *Files identical despite different names*

### Comparing `runtimepy-3.9.0/runtimepy/data/schemas/BitFields.yaml` & `runtimepy-4.0.0/runtimepy/data/schemas/BitFields.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -23,14 +23,17 @@
       additionalProperties: false
 
       properties:
         name:
           type: string
           pattern: "^[a-z0-9-_.]+$"
 
+        description:
+          type: string
+
         index:
           type: integer
           minimum: 0
 
         width:
           type: integer
           minimum: 1
```

### Comparing `runtimepy-3.9.0/runtimepy/data/schemas/ConnectionArbiterConfig.yaml` & `runtimepy-4.0.0/runtimepy/data/schemas/ConnectionArbiterConfig.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -9,32 +9,40 @@
       $ref: package://runtimepy/schemas/ClientConnectionConfig.yaml
 
   servers:
     type: array
     items:
       $ref: package://runtimepy/schemas/ServerConnectionConfig.yaml
 
+  structs:
+    type: array
+    items:
+      $ref: package://runtimepy/schemas/StructConfig.yaml
+
   tasks:
     type: array
     items:
       $ref: package://runtimepy/schemas/TaskConfig.yaml
 
   # Runtime application or applications.
   # defaults to: "runtimepy.net.apps.init_only"
-  app:
+  app: &applike
     oneOf:
       - type: string
       - type: array
         items:
           oneOf:
             - type: string
             - type: array
               items:
                 type: string
 
+  # Initialization methods.
+  init: *applike
+
   # Application configuration data.
   config:
     type: object
 
   # A 'site' directory to add for discovering modules that may appear in other
   # parts of the configuration. If this isn't specified, the current directory
   # is used.
```

### Comparing `runtimepy-3.9.0/runtimepy/data/schemas/FindFile.yaml` & `runtimepy-4.0.0/runtimepy/data/schemas/FindFile.yaml`

 * *Files identical despite different names*

### Comparing `runtimepy-3.9.0/runtimepy/entry.py` & `runtimepy-4.0.0/runtimepy/entry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.9.0/runtimepy/enum/__init__.py` & `runtimepy-4.0.0/runtimepy/enum/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 """
 A module implementing a runtime enumeration interface.
 """
 
 # built-in
 from enum import IntEnum as _IntEnum
 from typing import Optional as _Optional
-from typing import Type as _Type
 from typing import Union as _Union
 from typing import cast as _cast
 
 # third-party
 from vcorelib.io.types import JsonObject as _JsonObject
 from vcorelib.io.types import JsonValue as _JsonValue
 
 # internal
-from runtimepy.enum.type import EnumType as _EnumType
+from runtimepy.enum.types import EnumType as _EnumType
 from runtimepy.mapping import BoolMappingData as _BoolMappingData
 from runtimepy.mapping import IntMappingData as _IntMappingData
 from runtimepy.registry.bool import BooleanRegistry as _BooleanRegistry
 from runtimepy.registry.item import RegistryItem as _RegistryItem
 from runtimepy.registry.name import NameRegistry as _NameRegistry
 from runtimepy.util import StrToBool
 
@@ -105,15 +104,25 @@
         result = self.as_str(value)
         if result is None:
             raise KeyError(f"No enum entry for '{value}'")
         return result
 
     def as_int(self, value: _Union[str, int]) -> _Optional[int]:
         """Attempt to get an enumeration integer."""
-        return self.ints.identifier(value)
+
+        result = self.ints.identifier(value)
+
+        # Try 'value' as a converted integer.
+        if result is None and isinstance(value, str):
+            try:
+                result = self.ints.identifier(int(value))
+            except ValueError:
+                pass
+
+        return result
 
     def get_int(self, value: _Union[str, int, bool]) -> int:
         """Get an enumeration integer."""
 
         result: _Union[int, bool, None] = None
         if self._ints is not None:
             result = self.as_int(value)
@@ -151,22 +160,22 @@
         return self.ints.register_name(name)
 
     def register_bool(self, name: str, value: bool) -> bool:
         """Register a boolean enumeration."""
         return self.bools.register(name, value)
 
     @staticmethod
-    def data_from_enum(enum: _Type[_IntEnum]) -> _JsonObject:
+    def data_from_enum(enum: type[_IntEnum]) -> _JsonObject:
         """Get JSON data from an enumeration class."""
 
         return {
             "type": "int",
             "items": {x.name.lower(): x.value for x in enum},
         }
 
     @staticmethod
-    def from_enum(enum: _Type[_IntEnum], identifier: int) -> "RuntimeEnum":
+    def from_enum(enum: type[_IntEnum], identifier: int) -> "RuntimeEnum":
         """Create a runtime enumeration from an enum class."""
 
         data = RuntimeEnum.data_from_enum(enum)
         data["id"] = identifier
         return RuntimeEnum.create(data)
```

### Comparing `runtimepy-3.9.0/runtimepy/enum/registry.py` & `runtimepy-4.0.0/runtimepy/enum/registry.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 """
 A module implementing and enumeration registry.
 """
 
 # built-in
 from enum import IntEnum as _IntEnum
 from typing import Optional as _Optional
-from typing import Type as _Type
+from typing import TypeVar
 from typing import cast as _cast
 
 # third-party
 from vcorelib.io.types import JsonObject as _JsonObject
 
 # internal
 from runtimepy.enum import RuntimeEnum as _RuntimeEnum
-from runtimepy.enum.type import EnumTypelike as _EnumTypelike
+from runtimepy.enum.types import EnumTypelike as _EnumTypelike
 from runtimepy.mapping import EnumMappingData as _EnumMappingData
 from runtimepy.registry import Registry as _Registry
 
 DEFAULT_ENUM_PRIMITIVE = "uint8"
 
 
 class EnumRegistry(_Registry[_RuntimeEnum]):
     """A runtime enumeration registry."""
 
     @property
-    def kind(self) -> _Type[_RuntimeEnum]:
+    def kind(self) -> type[_RuntimeEnum]:
         """Determine what kind of registry this is."""
         return _RuntimeEnum
 
     def enum(
         self,
         name: str,
         kind: _EnumTypelike,
@@ -39,18 +39,35 @@
 
         data: _JsonObject = {"type": _cast(str, kind), "primitive": primitive}
         if items is not None:
             data["items"] = items  # type: ignore
         return self.register_dict(name, data)
 
 
+T = TypeVar("T", bound="RuntimeIntEnum")
+
+
 class RuntimeIntEnum(_IntEnum):
     """An integer enumeration extension."""
 
     @classmethod
+    def normalize(cls: type[T], data: int | str | T) -> T:
+        """
+        Normalize a value at runtime that is either integer, string or an enum
+        instance.
+        """
+
+        if isinstance(data, int):
+            data = cls(data)
+        elif isinstance(data, str):
+            data = cls[data.upper()]
+
+        return data
+
+    @classmethod
     def primitive(cls) -> str:
         """The underlying primitive type for this runtime enumeration."""
         return DEFAULT_ENUM_PRIMITIVE
 
     @classmethod
     def enum_name(cls) -> str:
         """Get a name for this enumeration."""
```

### Comparing `runtimepy-3.9.0/runtimepy/enum/type.py` & `runtimepy-4.0.0/runtimepy/enum/types.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.9.0/runtimepy/mapping.py` & `runtimepy-4.0.0/runtimepy/mapping.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 """
 A module implementing a generic, two-way mapping interface.
 """
 
 # built-in
 import re
-from typing import Dict as _Dict
 from typing import Generic as _Generic
 from typing import Iterable, Iterator
-from typing import List as _List
 from typing import MutableMapping as _MutableMapping
 from typing import Optional as _Optional
-from typing import Type as _Type
 from typing import TypeVar as _TypeVar
 from typing import Union as _Union
 from typing import cast as _cast
 
 # third-party
 from vcorelib.logging import LoggerMixin
 
@@ -60,17 +57,17 @@
     def __init__(
         self,
         mapping: KeyToName[T] = None,
         reverse: NameToKey[T] = None,
     ) -> None:
         """Initialize this name registry."""
 
-        self._mapping: _Dict[T, str] = {}
-        self._reverse: _Dict[str, T] = {}
-        self.registered_order: _List[str] = []
+        self._mapping: dict[T, str] = {}
+        self._reverse: dict[str, T] = {}
+        self.registered_order: list[str] = []
         LoggerMixin.__init__(self)
 
         if mapping is not None:
             self.load_key_to_name(mapping)
         if reverse is not None:
             self.load_name_to_key(reverse)
 
@@ -126,21 +123,21 @@
         return self._mapping.get(_cast(T, key))
 
     @property
     def names(self) -> Iterator[str]:
         """Iterate over names."""
         yield from self._reverse
 
-    def asdict(self) -> _Dict[str, T]:
+    def asdict(self) -> dict[str, T]:
         """Provide a dictionary representation."""
         return self._reverse
 
     @classmethod
     def int_from_dict(
-        cls: _Type[IntMapping], data: IntMappingData
+        cls: type[IntMapping], data: IntMappingData
     ) -> IntMapping:
         """
         Create an integer-to-name mapping from a dictionary with arbitrary
         data.
         """
 
         mapping: KeyToName[int] = {}
@@ -157,15 +154,15 @@
 
     def search(self, pattern: str, exact: bool = False) -> Iterator[str]:
         """Get names in this mapping based on a pattern."""
         yield from name_search(self.names, pattern, exact=exact)
 
     @classmethod
     def bool_from_dict(
-        cls: _Type[BoolMapping], data: BoolMappingData
+        cls: type[BoolMapping], data: BoolMappingData
     ) -> BoolMapping:
         """
         Create a boolean-to-name mapping from a dictionary with arbitrary data.
         """
 
         mapping: KeyToName[bool] = {}
         reverse: NameToKey[bool] = {}
```

### Comparing `runtimepy-3.9.0/runtimepy/metrics/channel.py` & `runtimepy-4.0.0/runtimepy/metrics/channel.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,14 +23,22 @@
         self.message_rate = _Float()
         self._message_rate_tracker = _RateTracker(depth=METRICS_DEPTH)
 
         self.bytes = _Uint64()
         self.kbps = _Float()
         self._kbps_tracker = _RateTracker(depth=METRICS_DEPTH)
 
+    def update(self, other: "ChannelMetrics") -> None:
+        """Update values in this instance from values in another instance."""
+
+        self.messages.value = other.messages.value
+        self.message_rate.value = other.message_rate.value
+        self.bytes.value = other.bytes.value
+        self.kbps.value = other.kbps.value
+
     def __str__(self) -> str:
         """Get metrics as a string."""
 
         return "\t".join(
             [
                 f"messages={self.messages.value}",
                 f"message_rate={self.message_rate.value:.2f}",
```

### Comparing `runtimepy-3.9.0/runtimepy/metrics/connection.py` & `runtimepy-4.0.0/runtimepy/metrics/connection.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,14 +11,20 @@
 
     def __init__(self) -> None:
         """Initialize this instance."""
 
         self.tx = ChannelMetrics()
         self.rx = ChannelMetrics()
 
+    def update(self, other: "ConnectionMetrics") -> None:
+        """Update values in this instance from values in another instance."""
+
+        self.tx.update(other.tx)
+        self.rx.update(other.rx)
+
     def reset(self) -> None:
         """Reset metrics."""
         self.tx.reset()
         self.rx.reset()
 
     def poll(self, time_ns: int = None) -> None:
         """Poll channels."""
```

### Comparing `runtimepy-3.9.0/runtimepy/metrics/task.py` & `runtimepy-4.0.0/runtimepy/metrics/task.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.9.0/runtimepy/mixins/async_command.py` & `runtimepy-4.0.0/runtimepy/mixins/async_command.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.9.0/runtimepy/mixins/enum.py` & `runtimepy-4.0.0/runtimepy/mixins/enum.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.9.0/runtimepy/mixins/finalize.py` & `runtimepy-4.0.0/runtimepy/mixins/finalize.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.9.0/runtimepy/mixins/logging.py` & `runtimepy-4.0.0/runtimepy/mixins/logging.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,19 +32,23 @@
         self.logger.setLevel(new_value)
 
     def setup_level_channel(
         self,
         env: ChannelEnvironment,
         name: str = "log_level",
         initial: str = "info",
+        description: str = "Text-log level filter for this environment.",
     ) -> None:
         """Add a commandable log-level channel to the environment."""
 
         chan = env.int_channel(
-            name, enum=LogLevel.register_enum(env.enums), commandable=True
+            name,
+            enum=LogLevel.register_enum(env.enums),
+            commandable=True,
+            description=description,
         )
 
         # Set up change handler.
         chan[0].raw.register_callback(self._log_level_changed)
 
         # Set the initial log level.
         env.set(name, initial)
```

### Comparing `runtimepy-3.9.0/runtimepy/mixins/regex.py` & `runtimepy-4.0.0/runtimepy/mixins/regex.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.9.0/runtimepy/net/__init__.py` & `runtimepy-4.0.0/runtimepy/net/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.9.0/runtimepy/net/apps/__init__.py` & `runtimepy-4.0.0/runtimepy/net/apps/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.9.0/runtimepy/net/arbiter/__init__.py` & `runtimepy-4.0.0/runtimepy/net/arbiter/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 """
 A module implementing a connection arbiter interface.
 """
 
 # built-in
-from runtimepy.net.arbiter.base import NetworkApplication, init_only
+from runtimepy.net.arbiter.base import init_only
 from runtimepy.net.arbiter.config import (
     ConfigConnectionArbiter as _ConfigConnectionArbiter,
 )
-from runtimepy.net.arbiter.info import AppInfo, ConnectionMap
+from runtimepy.net.arbiter.info import (
+    AppInfo,
+    ConnectionMap,
+    NetworkApplication,
+)
 from runtimepy.net.arbiter.task import (
     ArbiterTask,
     ArbiterTaskManager,
     TaskFactory,
 )
 
 __all__ = [
```

### Comparing `runtimepy-3.9.0/runtimepy/net/arbiter/base.py` & `runtimepy-4.0.0/runtimepy/net/arbiter/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,63 +1,67 @@
 """
 A module implementing a base connection-arbiter interface.
 """
 
 # built-in
 import asyncio as _asyncio
 from contextlib import AsyncExitStack as _AsyncExitStack
+from contextlib import suppress as _suppress
 from inspect import isawaitable as _isawaitable
 from typing import Awaitable as _Awaitable
-from typing import Callable as _Callable
 from typing import Iterable as _Iterable
-from typing import List as _List
 from typing import MutableMapping as _MutableMapping
 from typing import Optional
 from typing import Union as _Union
 
 # third-party
-from vcorelib.asyncio import run_handle_stop as _run_handle_stop
+from vcorelib.asyncio import log_exceptions, run_handle_stop
 from vcorelib.io.types import JsonObject as _JsonObject
 from vcorelib.logging import LoggerMixin as _LoggerMixin
 from vcorelib.logging import LoggerType as _LoggerType
 from vcorelib.namespace import Namespace as _Namespace
 from vcorelib.namespace import NamespaceMixin as _NamespaceMixin
 
 # internal
 from runtimepy.channel.environment.command import (
     clear_env,
     env_json_data,
     register_env,
 )
 from runtimepy.net.arbiter.housekeeping import metrics_poller
-from runtimepy.net.arbiter.info import AppInfo, ConnectionMap
+from runtimepy.net.arbiter.info import (
+    AppInfo,
+    ArbiterApps,
+    ConnectionMap,
+    NetworkApplication,
+    NetworkApplicationlike,
+)
 from runtimepy.net.arbiter.result import AppResult, ResultState
+from runtimepy.net.arbiter.struct import RuntimeStruct
 from runtimepy.net.arbiter.task import (
     ArbiterTaskManager as _ArbiterTaskManager,
 )
 from runtimepy.net.connection import Connection as _Connection
 from runtimepy.net.manager import ConnectionManager as _ConnectionManager
 from runtimepy.net.server import RuntimepyServerConnection
 from runtimepy.tui.mixin import CursesWindow, TuiMixin
 
-NetworkApplication = _Callable[[AppInfo], _Awaitable[int]]
-NetworkApplicationlike = _Union[NetworkApplication, _List[NetworkApplication]]
 ServerTask = _Awaitable[None]
 
 
 async def init_only(app: AppInfo) -> int:
     """A network application that doesn't do anything."""
 
     await app.all_finalized()
     return 0
 
 
 def normalize_app(
     app: NetworkApplicationlike = None,
-) -> _List[_List[NetworkApplication]]:
+) -> ArbiterApps:
     """
     Normalize some application parameter into a list of network applications.
     """
 
     if app is None:
         app = [init_only]
 
@@ -100,28 +104,32 @@
             stop_sig = _asyncio.Event()
         self.stop_sig = stop_sig
 
         _NamespaceMixin.__init__(self, namespace=namespace)
 
         # A fallback application. Set a class attribute so this can be more
         # easily externally updated.
-        self._apps: _List[_List[NetworkApplication]] = normalize_app(app)
+        self._inits: ArbiterApps = []
+        self._apps: ArbiterApps = normalize_app(app)
 
         # Application configuration data.
         if config is None:
             config = {}
         self._config = config
 
         # Keep track of connection objects.
         self._connections: ConnectionMap = {}
         self._deferred_connections: _MutableMapping[
             str, _Awaitable[_Connection]
         ] = {}
 
-        self._servers: _List[_asyncio.Task[None]] = []
+        # Runtime structures.
+        self._structs: dict[str, RuntimeStruct] = {}
+
+        self._servers: list[_asyncio.Task[None]] = []
         self._servers_started = _asyncio.Semaphore(0)
 
         self._init()
 
     def _init(self) -> None:
         """Additional initialization tasks."""
 
@@ -166,14 +174,52 @@
 
         # Connect configuration data.
         cls.json_data["config"] = info.original_config()
 
         # Connect environment data.
         cls.json_data["environments"] = env_json_data()
 
+    def _register_envs(self) -> None:
+        """Register environments."""
+
+        clear_env()
+        for name, conn in self._connections.items():
+            register_env(name, conn.command)
+        for struct in self._structs.values():
+            register_env(struct.name, struct.command)
+
+    async def _init_connections(self) -> None:
+        """Initialize network connections."""
+
+        # Wait for servers to start.
+        for _ in range(len(self._servers)):
+            await self._servers_started.acquire()
+
+        # Start deferred connections.
+        for key, value in zip(
+            self._deferred_connections,
+            await _asyncio.gather(*self._deferred_connections.values()),
+        ):
+            self._register_connection(value, key)
+
+        # Ensure connections are all initialized.
+        await _asyncio.gather(
+            *(x.initialized.wait() for x in self._connections.values())
+        )
+
+    async def _build_structs(self, info: AppInfo) -> None:
+        """Build structs."""
+
+        with self.log_time("Building structs", reminder=True):
+            await _asyncio.gather(
+                *(x.build(info) for x in self._structs.values())
+            )
+            for struct in self._structs.values():
+                struct.env.finalize(strict=False)
+
     async def _entry(
         self,
         app: NetworkApplicationlike = None,
         check_connections: bool = True,
         config: _JsonObject = None,
     ) -> int:
         """
@@ -181,40 +227,22 @@
         application, clean up connections and return the application's result.
         """
 
         result = -1
         info: Optional[AppInfo] = None
 
         try:
-            # Wait for servers to start.
-            for _ in range(len(self._servers)):
-                await self._servers_started.acquire()
-
-            # Start deferred connections.
-            for key, value in zip(
-                self._deferred_connections,
-                await _asyncio.gather(*self._deferred_connections.values()),
-            ):
-                self._register_connection(value, key)
-
-            # Ensure connections are all initialized.
-            await _asyncio.gather(
-                *(x.initialized.wait() for x in self._connections.values())
-            )
-
-            self.logger.info("Connections initialized.")
-
-            tasks = {x.name: x for x in self.task_manager.tasks}
+            with self.log_time("Connection initialization", reminder=True):
+                await self._init_connections()
 
             # Register environments.
-            clear_env()
+            self._register_envs()
+            tasks = {x.name: x for x in self.task_manager.tasks}
             for task in tasks.values():
                 register_env(task.name, task.command)
-            for name, conn in self._connections.items():
-                register_env(name, conn.command)
 
             # Run application, but only if all the registered connections are
             # still alive after initialization.
             if not check_connections or not any(
                 x.disabled for x in self._connections.values()
             ):
                 async with _AsyncExitStack() as stack:
@@ -228,65 +256,81 @@
                         self._namespace,
                         self.stop_sig,
                         config if config is not None else self._config,
                         self,
                         tasks,  # type: ignore
                         self.task_manager,
                         [],
+                        self._structs,  # type: ignore
                     )
 
+                    # Build structs.
+                    await self._build_structs(info)
+
                     # Initialize tasks.
-                    self.logger.debug("Initializing periodic tasks...")
-                    await _asyncio.gather(
-                        *(x.init(info) for x in self.task_manager.tasks)
-                    )
-                    for task in self.task_manager.tasks:
-                        task.env.finalize(strict=False)
-                    self.logger.debug("Periodic tasks initialized.")
+                    with self.log_time(
+                        "Initializing periodic tasks", reminder=True
+                    ):
+                        await _asyncio.gather(
+                            *(x.init(info) for x in self.task_manager.tasks)
+                        )
+                        for task in self.task_manager.tasks:
+                            task.env.finalize(strict=False)
 
                     # Wire runtime data to server JSON.
                     self._setup_server_json(info)
 
                     # Start tasks.
-                    self.logger.debug("Starting periodic tasks...")
                     await stack.enter_async_context(
                         self.task_manager.running(stop_sig=self.stop_sig)
                     )
-                    self.logger.debug("Periodic tasks started.")
 
-                    # Get application methods.
-                    apps = self._apps
-                    if app is not None:
-                        apps = normalize_app(app)
-
-                    # Run applications in order.
-                    result = 0
-                    for curr_app in apps:
-                        if result == 0:
-                            result = await self._run_apps(curr_app, info)
-
-                        # Populate "not run" statuses.
-                        else:
-                            info.results.append(
-                                [AppResult(app.__name__) for app in curr_app]
-                            )
+                    # Run initialization methods.
+                    result = await self._run_apps_list(self._inits, info)
+                    if result == 0:
+                        # Get application methods.
+                        apps = self._apps
+                        if app is not None:
+                            apps = normalize_app(app)
 
+                        # Run applications in order.
+                        result = await self._run_apps_list(apps, info)
         finally:
             for conn in self._connections.values():
                 conn.disable(f"app exit {result}")
+
+            # Stop runtime entities.
             self.stop_sig.set()
+            await _asyncio.sleep(0)
 
             # Summarize results.
             if info is not None:
                 info.result(logger=self.logger)
 
         return result
 
+    async def _run_apps_list(self, apps: ArbiterApps, info: AppInfo) -> int:
+        """Run application methods."""
+
+        # Run applications in order.
+        result = 0
+        for curr_app in apps:
+            if result == 0:
+                result = await self._run_apps(curr_app, info)
+
+            # Populate "not run" statuses.
+            else:
+                info.results.append(
+                    [AppResult(app.__name__) for app in curr_app]
+                )
+
+        return result
+
     async def _run_apps(
-        self, apps: _List[NetworkApplication], info: AppInfo
+        self, apps: list[NetworkApplication], info: AppInfo
     ) -> int:
         """Run application methods in parallel."""
 
         pairs = [(app, info.with_new_logger(app.__name__)) for app in apps]
 
         # Pre-populate stage results with "not run" placeholders.
         stage_results = [AppResult(app.__name__) for app in apps]
@@ -325,37 +369,46 @@
         check_connections: bool = True,
         config: _JsonObject = None,
     ) -> int:
         """
         Run the application alongside the connection manager and server tasks.
         """
 
-        result = await _asyncio.gather(
-            self._entry(
-                app=app, check_connections=check_connections, config=config
-            ),
-            self.manager.manage(self.stop_sig),
-            *self._servers,
+        # Create task for connection manager.
+        conns = _asyncio.create_task(self.manager.manage(self.stop_sig))
+
+        # Run application.
+        result = await self._entry(
+            app=app, check_connections=check_connections, config=config
         )
-        assert result is not None
-        assert result[0] is not None
-        return int(result[0])
+
+        # Shutdown any pending tasks.
+        pending = log_exceptions(self._servers + [conns], logger=self.logger)
+        if pending:
+            for task in pending:
+                task.cancel()
+                with _suppress(KeyboardInterrupt, _asyncio.CancelledError):
+                    await task
+
+            assert not log_exceptions(pending, logger=self.logger)
+
+        return int(result)
 
     def run(
         self,
         app: NetworkApplicationlike = None,
         eloop: _asyncio.AbstractEventLoop = None,
         signals: _Iterable[int] = None,
         check_connections: bool = True,
         config: _JsonObject = None,
         enable_uvloop: bool = True,
     ) -> int:
         """Run the application until the stop signal is set."""
 
-        return _run_handle_stop(
+        return run_handle_stop(
             self.stop_sig,
             self.app(
                 app=app, check_connections=check_connections, config=config
             ),
             eloop=eloop,
             signals=signals,
             enable_uvloop=enable_uvloop,
```

### Comparing `runtimepy-3.9.0/runtimepy/net/arbiter/config.py` & `runtimepy-4.0.0/runtimepy/net/arbiter/config/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,146 +1,75 @@
 """
 A module implementing a configuration-file interface for registering client
 connections or servers.
 """
 
 # built-in
-from pathlib import Path as _Path
 from site import addsitedir as _addsitedir
-import socket as _socket
-import sys
-from typing import Any as _Any
-from typing import Dict as _Dict
 from typing import Iterable as _Iterable
-from typing import List as _List
-from typing import Optional as _Optional
-from typing import cast as _cast
 
 # third-party
 from vcorelib.dict import merge as _merge
 from vcorelib.dict.env import dict_resolve_env_vars, list_resolve_env_vars
 from vcorelib.io import ARBITER as _ARBITER
 from vcorelib.io.types import JsonObject as _JsonObject
 from vcorelib.paths import Pathlike as _Pathlike
 from vcorelib.paths import find_file
 from vcorelib.paths import normalize as _normalize
 
 # internal
-from runtimepy.net import get_free_socket_name, normalize_host
+from runtimepy import DEFAULT_EXT, PKG_NAME
+from runtimepy.net.arbiter.config.codec import ConnectionArbiterConfig
+from runtimepy.net.arbiter.config.util import fix_args, fix_kwargs, list_adder
 from runtimepy.net.arbiter.imports import (
     ImportConnectionArbiter as _ImportConnectionArbiter,
 )
-from runtimepy.schemas import RuntimepyDictCodec as _RuntimepyDictCodec
-
-
-class ConnectionArbiterConfig(_RuntimepyDictCodec):
-    """
-    A class for encoding and decoding connection-arbiter configuration data.
-    """
-
-    directory: _Path
-
-    def init(self, data: _JsonObject) -> None:
-        """Perform implementation-specific initialization."""
-
-        self.data = data
-
-        port_overrides: _Dict[str, int] = data.get(
-            "port_overrides",
-            {},  # type: ignore
-        )
-
-        # Process ports.
-        self.ports: _Dict[str, int] = {}
-        for item in _cast(_List[_Dict[str, _Any]], data.get("ports", [])):
-            port = get_free_socket_name(
-                local=normalize_host(
-                    item["host"],
-                    port_overrides.get(item["name"], item["port"]),
-                ),
-                kind=(
-                    _socket.SOCK_STREAM
-                    if item["type"] == "tcp"
-                    else _socket.SOCK_DGRAM
-                ),
-            ).port
-
-            # Update the original structure.
-            self.ports[item["name"]] = port
-            item["port"] = port
-
-        self.app: _Optional[str] = data.get("app")  # type: ignore
-        self.config: _Optional[_JsonObject] = _cast(
-            _JsonObject, data.get("config")
-        )
-
-        self.factories: _List[_Any] = data.get("factories", [])  # type: ignore
-        self.clients: _List[_Any] = data.get("clients", [])  # type: ignore
-        self.servers: _List[_Any] = data.get("servers", [])  # type: ignore
-        self.tasks: _List[_Any] = data.get("tasks", [])  # type: ignore
-
-        directory_str = str(data.get("directory", "."))
-        self.directory = _Path(directory_str)
-
-        # Add directory to Python path.
-        if directory_str not in sys.path:
-            sys.path.append(directory_str)
-
-    def asdict(self) -> _JsonObject:
-        """Obtain a dictionary representing this instance."""
-        return self.data
-
-
-def fix_kwargs(data: _Dict[str, _Any]) -> _Dict[str, _Any]:
-    """
-    Fix data depending on nuances of what some Python interfaces require.
-    """
-
-    # Convert some keys to tuples.
-    for key in ["local_addr", "remote_addr"]:
-        if key in data:
-            data[key] = tuple(data[key])
-
-    return data
-
-
-def fix_args(data: _List[_Any], ports: _Dict[str, int]) -> _List[_Any]:
-    """Fix positional arguments."""
-
-    for idx, item in enumerate(data):
-        # Allow port variables to be used in host strings.
-        if isinstance(item, str):
-            data[idx] = ":".join(
-                str(x)
-                for x in list_resolve_env_vars(
-                    item.split(":"),
-                    env=ports,  # type: ignore
-                )
-            )
-
-    return data
+from runtimepy.net.arbiter.imports.util import get_apps
 
 
 class ConfigConnectionArbiter(_ImportConnectionArbiter):
     """
     A class implementing a configuration loading interface for the connection
     arbiter.
     """
 
+    search_packages: list[str] = []
+
+    @classmethod
+    def add_search_package(cls, name: str, front: bool = True) -> None:
+        """Add a package to the search path."""
+
+        name = name.replace("-", "_")
+        if name not in cls.search_packages:
+            list_adder(cls.search_packages, name, front=front)
+
     async def load_configs(
         self, paths: _Iterable[_Pathlike], wait_for_stop: bool = False
     ) -> None:
         """Load a client and server configuration to the arbiter."""
 
         loaded = set()
 
         # Load and meld configuration data.
         config_data: _JsonObject = {}
         for path in paths:
+            # Try the path itself.
             found = find_file(path, logger=self.logger, include_cwd=True)
+
+            # Try package search path next.
+            if found is None:
+                for pkg in self.search_packages:
+                    found = find_file(
+                        f"{path}.{DEFAULT_EXT}",
+                        logger=self.logger,
+                        package=pkg,
+                    )
+                    if found is not None:
+                        break
+
             assert found is not None, f"Couldn't find '{path}'!"
 
             # Only load files once.
             absolute = found.resolve()
             if absolute not in loaded:
                 _merge(
                     config_data,
@@ -236,16 +165,32 @@
             assert self.factory_task(
                 factory,
                 name,
                 period_s=task["period_s"],
                 average_depth=task["average_depth"],
             ), f"Couldn't register task '{name}' ({factory})!"
 
+        # Register structs.
+        for struct in config.structs:
+            name = struct["name"]
+            factory = struct["factory"]
+            assert self.factory_struct(
+                struct["factory"], struct["name"], struct.get("config", {})
+            ), f"Couldn't register struct '{name}' ({factory})!"
+
+        # Load initialization methods.
+        self._inits = get_apps(config.inits)
+
         # Set the new application entry if it's set.
-        self.set_app(config.app, wait_for_stop=wait_for_stop)
+        apps = get_apps(config.app, wait_for_stop=wait_for_stop)
+        if apps:
+            self._apps = apps
 
         # Update application configuration data if necessary.
         if config.config is not None:
             root = self._config["root"]
             self._config = config.config
             assert "root" not in config.config, config.config
             config.config["root"] = root
+
+
+ConfigConnectionArbiter.add_search_package(PKG_NAME)
```

### Comparing `runtimepy-3.9.0/runtimepy/net/arbiter/factory/connection.py` & `runtimepy-4.0.0/runtimepy/net/arbiter/factory/connection.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 """
 A module implementing an interface extension to the base connection-arbiter so
 that methods that create connections can be registered by name.
 """
 
 # built-in
 import asyncio as _asyncio
-from typing import Dict as _Dict
-from typing import List as _List
 
 # third-party
 from vcorelib.names import obj_class_to_snake
 
 # internal
 from runtimepy.net.arbiter.base import (
     BaseConnectionArbiter as _BaseConnectionArbiter,
@@ -45,16 +43,16 @@
     used for creating new connections (that can then be registered).
     """
 
     def _init(self) -> None:
         """Additional initialization tasks."""
 
         super()._init()
-        self._conn_factories: _Dict[str, ConnectionFactory] = {}
-        self._conn_names: _Dict[ConnectionFactory, _List[str]] = {}
+        self._conn_factories: dict[str, ConnectionFactory] = {}
+        self._conn_names: dict[ConnectionFactory, list[str]] = {}
 
     def register_connection_factory(
         self, factory: ConnectionFactory, *namespaces: str
     ) -> bool:
         """Attempt to register a connection factory."""
 
         result = False
```

### Comparing `runtimepy-3.9.0/runtimepy/net/arbiter/factory/task.py` & `runtimepy-4.0.0/runtimepy/net/arbiter/factory/task.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 """
 A module implementing task-factory registration.
 """
 
-# built-in
-from typing import Dict as _Dict
-from typing import List as _List
-
 # third-party
 from vcorelib.names import obj_class_to_snake
 
 # internal
 from runtimepy.net.arbiter.base import (
     BaseConnectionArbiter as _BaseConnectionArbiter,
 )
@@ -22,16 +18,16 @@
 class TaskConnectionArbiter(_BaseConnectionArbiter):
     """A class for managing task factories."""
 
     def _init(self) -> None:
         """Additional initialization tasks."""
 
         super()._init()
-        self._task_factories: _Dict[str, Factory] = {}
-        self._task_names: _Dict[Factory, _List[str]] = {}
+        self._task_factories: dict[str, Factory] = {}
+        self._task_names: dict[Factory, list[str]] = {}
 
     def factory_task(
         self, factory: str, name: str, period_s: float = None, **kwargs
     ) -> bool:
         """
         Register a periodic task from one of the registered task factories.
         """
```

### Comparing `runtimepy-3.9.0/runtimepy/net/arbiter/housekeeping/__init__.py` & `runtimepy-4.0.0/runtimepy/net/arbiter/housekeeping/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.9.0/runtimepy/net/arbiter/info.py` & `runtimepy-4.0.0/runtimepy/net/arbiter/info.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,36 +4,40 @@
 
 # built-in
 import asyncio as _asyncio
 from contextlib import AsyncExitStack as _AsyncExitStack
 from dataclasses import dataclass
 from logging import getLogger as _getLogger
 from re import compile as _compile
-from typing import Any, Dict
+from typing import Any
+from typing import Awaitable as _Awaitable
+from typing import Callable as _Callable
 from typing import Iterator as _Iterator
 from typing import MutableMapping as _MutableMapping
-from typing import Type as _Type
 from typing import TypeVar as _TypeVar
+from typing import Union as _Union
 
 # third-party
 from vcorelib.io.types import JsonObject as _JsonObject
 from vcorelib.logging import LoggerType as _LoggerType
 from vcorelib.namespace import Namespace as _Namespace
 
 # internal
 from runtimepy.mapping import DEFAULT_PATTERN
 from runtimepy.net.arbiter.result import OverallResult, results
 from runtimepy.net.connection import Connection as _Connection
 from runtimepy.net.manager import ConnectionManager
+from runtimepy.struct import StructMap as _StructMap
 from runtimepy.task import PeriodicTask, PeriodicTaskManager
 from runtimepy.tui.mixin import TuiMixin
 
 ConnectionMap = _MutableMapping[str, _Connection]
 T = _TypeVar("T", bound=_Connection)
 V = _TypeVar("V", bound=PeriodicTask)
+Z = _TypeVar("Z")
 
 
 @dataclass
 class AppInfo:
     """References provided to network applications."""
 
     # A logger for applications to use.
@@ -55,20 +59,23 @@
     stop: _asyncio.Event
 
     # Configuration data that may be specified in a configuration file.
     config: _JsonObject
 
     tui: TuiMixin
 
-    tasks: Dict[str, PeriodicTask]
+    tasks: dict[str, PeriodicTask]
     task_manager: PeriodicTaskManager[Any]
 
     # Keep track of application state.
     results: OverallResult
 
+    # A name-to-struct mapping.
+    structs: _StructMap
+
     def with_new_logger(self, name: str) -> "AppInfo":
         """Get a copy of this AppInfo instance, but with a new logger."""
 
         return AppInfo(
             _getLogger(name),
             self.stack,
             self.connections,
@@ -76,21 +83,22 @@
             self.names,
             self.stop,
             self.config,
             self.tui,
             self.tasks,
             self.task_manager,
             self.results,
+            self.structs,
         )
 
     def search(
         self,
         *names: str,
         pattern: str = DEFAULT_PATTERN,
-        kind: _Type[T] = _Connection,  # type: ignore
+        kind: type[T] = _Connection,  # type: ignore
     ) -> _Iterator[T]:
         """
         Get all connections that are matching a naming convention or are
         specific kind (or both).
         """
 
         seen: set[T] = set()
@@ -105,30 +113,28 @@
         # default pattern is used.
         if pattern == DEFAULT_PATTERN:
             for conn in self.conn_manager.by_type(kind):
                 if conn not in seen:
                     yield conn
                     seen.add(conn)
 
-    def search_tasks(
-        self, kind: _Type[V], pattern: str = ".*"
-    ) -> _Iterator[V]:
+    def search_tasks(self, kind: type[V], pattern: str = ".*") -> _Iterator[V]:
         """Search for tasks by type or pattern."""
 
         compiled = _compile(pattern)
 
         for name, task in self.tasks.items():
             if compiled.search(name) is not None and isinstance(task, kind):
                 yield task
 
     def single(
         self,
         *names: str,
         pattern: str = ".*",
-        kind: _Type[T] = _Connection,  # type: ignore
+        kind: type[T] = _Connection,  # type: ignore
     ) -> T:
         """Search for a single node."""
 
         result = list(self.search(*names, pattern=pattern, kind=kind))
         assert len(result) == 1, result
         return result[0]
 
@@ -177,7 +183,25 @@
                 result["config"][key] = val
 
         for key, val in self.config.get("root", {}).items():  # type: ignore
             if key != "config":
                 result[key] = val
 
         return result
+
+    def config_param(self, key: str, default: Z, strict: bool = False) -> Z:
+        """Attempt to get a configuration parameter."""
+
+        config: dict[str, Z] = self.config["root"].setdefault(  # type: ignore
+            "config",
+            {},
+        )
+
+        if strict:
+            assert key in config, (key, config)
+
+        return config.get(key, default)
+
+
+NetworkApplication = _Callable[[AppInfo], _Awaitable[int]]
+NetworkApplicationlike = _Union[NetworkApplication, list[NetworkApplication]]
+ArbiterApps = list[list[NetworkApplication]]
```

### Comparing `runtimepy-3.9.0/runtimepy/net/arbiter/result.py` & `runtimepy-4.0.0/runtimepy/net/arbiter/result.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.9.0/runtimepy/net/arbiter/task.py` & `runtimepy-4.0.0/runtimepy/net/arbiter/task.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 A module implement a base class for arbiter periodic tasks.
 """
 
 # built-in
 from typing import Generic as _Generic
-from typing import Type as _Type
 from typing import TypeVar as _TypeVar
 
 # internal
 from runtimepy.net.arbiter.info import AppInfo
 from runtimepy.task import PeriodicTask, PeriodicTaskManager
 
 
@@ -30,8 +29,8 @@
 
 T = _TypeVar("T", bound=ArbiterTask)
 
 
 class TaskFactory(_Generic[T]):
     """A task-factory base class."""
 
-    kind: _Type[T]
+    kind: type[T]
```

### Comparing `runtimepy-3.9.0/runtimepy/net/arbiter/tcp/__init__.py` & `runtimepy-4.0.0/runtimepy/net/arbiter/tcp/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
 A module implementing a basic TCP connection factory that can be extended.
 """
 
 # built-in
 import asyncio as _asyncio
 from typing import Generic as _Generic
-from typing import Type as _Type
 from typing import TypeVar as _TypeVar
 
 # internal
 from runtimepy.net.arbiter.base import ServerTask as _ServerTask
 from runtimepy.net.arbiter.factory import (
     ConnectionFactory as _ConnectionFactory,
 )
@@ -19,15 +18,15 @@
 
 T = _TypeVar("T", bound=_TcpConnection)
 
 
 class TcpConnectionFactory(_ConnectionFactory, _Generic[T]):
     """A class implementing a basic TCP connection factory."""
 
-    kind: _Type[T]
+    kind: type[T]
 
     async def client(self, name: str, *args, **kwargs) -> _Connection:
         """Create a client connection."""
 
         del name
         assert not [*args], "Only keyword arguments are used!"
         return await self.kind.create_connection(**kwargs)
```

### Comparing `runtimepy-3.9.0/runtimepy/net/arbiter/tcp/json.py` & `runtimepy-4.0.0/runtimepy/net/arbiter/tcp/json.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.9.0/runtimepy/net/arbiter/udp.py` & `runtimepy-4.0.0/runtimepy/net/arbiter/udp.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 A module implementing a basic UDP connection factory that can be extended.
 """
 
 # built-in
 from typing import Generic as _Generic
-from typing import Type as _Type
 from typing import TypeVar as _TypeVar
 
 # internal
 from runtimepy.net.arbiter.factory import (
     ConnectionFactory as _ConnectionFactory,
 )
 from runtimepy.net.connection import Connection as _Connection
@@ -18,15 +17,15 @@
 
 
 class UdpConnectionFactory(
     _ConnectionFactory, _Generic[T]
 ):  # pylint: disable=abstract-method
     """A class implementing a basic UDP connection factory."""
 
-    kind: _Type[T]
+    kind: type[T]
 
     async def client(self, name: str, *args, **kwargs) -> _Connection:
         """Create a client connection."""
 
         del name
         assert not [*args], "Only keyword arguments are used!"
         return await self.kind.create_connection(**kwargs)
```

### Comparing `runtimepy-3.9.0/runtimepy/net/arbiter/websocket.py` & `runtimepy-4.0.0/runtimepy/net/arbiter/websocket.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 A module implementing a basic WebSocket connection factory that can be
 extended.
 """
 
 # built-in
 import asyncio as _asyncio
 from typing import Generic as _Generic
-from typing import Type as _Type
 from typing import TypeVar as _TypeVar
 
 # internal
 from runtimepy.net.arbiter.base import ServerTask as _ServerTask
 from runtimepy.net.arbiter.factory import (
     ConnectionFactory as _ConnectionFactory,
 )
@@ -22,15 +21,15 @@
 
 T = _TypeVar("T", bound=_WebsocketConnection)
 
 
 class WebsocketConnectionFactory(_ConnectionFactory, _Generic[T]):
     """A class implementing a basic WebSocket connection factory."""
 
-    kind: _Type[T]
+    kind: type[T]
 
     async def client(self, name: str, *args, **kwargs) -> _Connection:
         """Create a client connection."""
 
         del name
         return await self.kind.create_connection(*args, **kwargs)
```

### Comparing `runtimepy-3.9.0/runtimepy/net/backoff.py` & `runtimepy-4.0.0/runtimepy/net/backoff.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.9.0/runtimepy/net/connection.py` & `runtimepy-4.0.0/runtimepy/net/connection.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 A module implementing a network-connection interface.
 """
 
 # built-in
 from abc import ABC as _ABC
 import asyncio as _asyncio
 from contextlib import suppress as _suppress
-from typing import List as _List
 from typing import Optional as _Optional
 from typing import Union as _Union
 
 # third-party
 from vcorelib.asyncio import log_exceptions as _log_exceptions
 from vcorelib.logging import LoggerType as _LoggerType
 
@@ -58,40 +57,60 @@
 
         # A queue for out-going binary messages. Connections that don't use
         # this can set 'uses_binary_tx_queue' to False to avoid scheduling a
         # task for it.
         self._binary_messages: _asyncio.Queue[BinaryMessage] = _asyncio.Queue()
         self.tx_binary_hwm: int = 0
 
-        self._tasks: _List[_asyncio.Task[None]] = []
+        self._tasks: list[_asyncio.Task[None]] = []
         self.initialized = _asyncio.Event()
         self.exited = _asyncio.Event()
 
         self.metrics = ConnectionMetrics()
 
         ChannelEnvironmentMixin.__init__(self, env=env)
         self.setup_level_channel(self.env)
         self.command = ChannelCommandProcessor(self.env, self.logger)
         if add_metrics:
             self.register_connection_metrics(self.metrics)
 
         # State.
         self._enabled = Bool()
         self.disabled_event = _asyncio.Event()
-        self.env.channel("enabled", self._enabled)
+        self.env.channel(
+            "enabled",
+            self._enabled,
+            description="Whether or not this connection is enabled.",
+        )
         self._set_enabled(True)
 
         # Restart state and behavior.
         self._restarts = Uint8()
         self._restart_attempts = Uint8()
-        self.env.channel("restarts", self._restarts)
-        self.env.channel("restart_attempts", self._restarts)
+        self.env.channel(
+            "restarts",
+            self._restarts,
+            description="Number of successful connection restarts.",
+        )
+        self.env.channel(
+            "restart_attempts",
+            self._restarts,
+            description="Number of connection restart attempts.",
+        )
 
         self._auto_restart = Bool(self.default_auto_restart)
-        self.env.channel("auto_restart", self._auto_restart, commandable=True)
+        self.env.channel(
+            "auto_restart",
+            self._auto_restart,
+            commandable=True,
+            description=(
+                "Whether or not this connection will "
+                "automatically attempt re-connection."
+            ),
+        )
 
         self.init()
 
     @property
     def auto_restart(self) -> bool:
         """Determine if this connection should be automatically restarted."""
         return bool(self._auto_restart)
```

### Comparing `runtimepy-3.9.0/runtimepy/net/factories/__init__.py` & `runtimepy-4.0.0/runtimepy/net/factories/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,18 @@
     TcpJsonMessageConnection,
     UdpJsonMessageConnection,
     WebsocketJsonMessageConnection,
 )
 from runtimepy.net.arbiter.udp import UdpConnectionFactory
 from runtimepy.net.arbiter.websocket import WebsocketConnectionFactory
 from runtimepy.net.server import RuntimepyServerConnection
+from runtimepy.net.server.websocket import (
+    RuntimepyDataWebsocketConnection,
+    RuntimepyWebsocketConnection,
+)
 from runtimepy.net.stream import (
     EchoTcpMessageConnection,
     EchoUdpMessageConnection,
     TcpPrefixedMessageConnection,
     UdpPrefixedMessageConnection,
 )
 from runtimepy.net.tcp import (
@@ -50,14 +54,16 @@
     "UdpMessageEcho",
     "UdpNull",
     "WebsocketConnection",
     "WebsocketConnectionFactory",
     "WebsocketEcho",
     "WebsocketNull",
     "HttpConnection",
+    "RuntimepyWebsocketJson",
+    "RuntimepyWebsocketConnection",
 ]
 
 
 class UdpEcho(UdpConnectionFactory[EchoUdpConnection]):
     """UDP echo-connection factory."""
 
     kind = EchoUdpConnection
@@ -143,7 +149,23 @@
     kind = HttpConnection
 
 
 class RuntimepyHttp(TcpConnectionFactory[RuntimepyServerConnection]):
     """HTTP connection factory for this package."""
 
     kind = RuntimepyServerConnection
+
+
+class RuntimepyWebsocketJson(
+    WebsocketConnectionFactory[RuntimepyWebsocketConnection]
+):
+    """WebSocket JSON-connection factory."""
+
+    kind = RuntimepyWebsocketConnection
+
+
+class RuntimepyWebsocketData(
+    WebsocketConnectionFactory[RuntimepyDataWebsocketConnection]
+):
+    """WebSocket JSON-connection factory."""
+
+    kind = RuntimepyDataWebsocketConnection
```

### Comparing `runtimepy-3.9.0/runtimepy/net/http/__init__.py` & `runtimepy-4.0.0/runtimepy/net/http/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 A module implementing an HTTP-message processing interface.
 """
 
 # built-in
-from typing import Iterator, Optional, Tuple, Type, cast
+from typing import Iterator, Optional, cast
 
 # third-party
 from vcorelib.io import ByteFifo
 
 # internal
 from runtimepy.net.http.common import HeadersMixin
 from runtimepy.net.http.state import HeaderProcessingState, T
@@ -25,16 +25,16 @@
         # Header parsing.
         self.buffer = ByteFifo()
         self.header = HeaderProcessingState.create()
 
         self.current_header: Optional[HeadersMixin] = None
 
     def ingest(
-        self, data: bytes, kind: Type[T]
-    ) -> Iterator[Tuple[T, Optional[bytes]]]:
+        self, data: bytes, kind: type[T]
+    ) -> Iterator[tuple[T, Optional[bytes]]]:
         """Process a binary frame."""
 
         self.buffer.ingest(data)
 
         can_read_payload = True
         while self.buffer.size > 0 and can_read_payload:
             # Finish parsing header if necessary.
```

### Comparing `runtimepy-3.9.0/runtimepy/net/http/common.py` & `runtimepy-4.0.0/runtimepy/net/http/common.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.9.0/runtimepy/net/http/header.py` & `runtimepy-4.0.0/runtimepy/net/http/header.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 A module implementing interfaces for HTTP headers.
 """
 
 # built-in
 import http
 from io import StringIO
+import logging
 
 # third-party
 from vcorelib.logging import LoggerType
 
 # internal
 from runtimepy.net.http.common import (
     HEADER_LINESEP,
@@ -49,18 +50,21 @@
         method_raw, request_target_raw, version_raw = lines[0].split(" ")
 
         self.method = normalize_method(method_raw)
         self.target = RequestTarget(self.method, request_target_raw)
         self.version = HttpVersion(version_raw)
         HeadersMixin.__init__(self, lines[1:])
 
-    def log(self, logger: LoggerType, out: bool) -> None:
+    def log(
+        self, logger: LoggerType, out: bool, level: int = logging.DEBUG
+    ) -> None:
         """Log information about this request header."""
 
-        logger.info(
+        logger.log(
+            level,
             "(%s request) %s - %s",
             "outgoing" if out else "incoming",
             self.request_line,
             self.headers,
         )
 
     @property
```

### Comparing `runtimepy-3.9.0/runtimepy/net/http/request_target.py` & `runtimepy-4.0.0/runtimepy/net/http/request_target.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.9.0/runtimepy/net/http/response.py` & `runtimepy-4.0.0/runtimepy/net/http/response.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,14 +72,14 @@
 
             return stream.getvalue()
 
     def log(self, logger: LoggerType, out: bool) -> None:
         """Log information about this response header."""
 
         level = logging.INFO if (200 <= self.status <= 299) else logging.ERROR
-        logger.log(
+        logger.debug(
             level,
             "(%s response) %s - %s",
             "outgoing" if out else "incoming",
             self.status_line,
             self.headers,
         )
```

### Comparing `runtimepy-3.9.0/runtimepy/net/http/state.py` & `runtimepy-4.0.0/runtimepy/net/http/state.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 A module implementing an HTTP-header processing state interface.
 """
 
 # built-in
 from dataclasses import dataclass
-from typing import List, Optional, Type, TypeVar
+from typing import Optional, TypeVar
 
 # third-party
 from vcorelib import DEFAULT_ENCODING
 from vcorelib.io import ByteFifo
 
 # internal
 from runtimepy.net.http.common import HeadersMixin
@@ -16,23 +16,23 @@
 T = TypeVar("T", bound=HeadersMixin)
 
 
 @dataclass
 class HeaderProcessingState:
     """A container for header-related processing state."""
 
-    lines: List[str]
+    lines: list[str]
     line: str
 
     @staticmethod
     def create() -> "HeaderProcessingState":
         """Create a default instance."""
         return HeaderProcessingState([], "")
 
-    def service(self, buffer: ByteFifo, kind: Type[T]) -> Optional[T]:
+    def service(self, buffer: ByteFifo, kind: type[T]) -> Optional[T]:
         """
         Continue processing the input fifo as if it contains request-header
         data.
         """
 
         result = None
```

### Comparing `runtimepy-3.9.0/runtimepy/net/http/version.py` & `runtimepy-4.0.0/runtimepy/net/http/version.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.9.0/runtimepy/net/manager.py` & `runtimepy-4.0.0/runtimepy/net/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,15 @@
 
 from __future__ import annotations
 
 # built-in
 import asyncio as _asyncio
 from contextlib import suppress as _suppress
 from typing import Iterator as _Iterator
-from typing import List as _List
 from typing import Optional as _Optional
-from typing import Type as _Type
 from typing import TypeVar as _TypeVar
 
 # third-party
 from vcorelib.asyncio import log_exceptions as _log_exceptions
 from vcorelib.logging import LoggerMixin
 from vcorelib.math import default_time_ns as _default_time_ns
 
@@ -29,22 +27,22 @@
 
     def __init__(self) -> None:
         """Initialize this connection manager."""
 
         super().__init__()
         self.queue: _asyncio.Queue[_Connection] = _asyncio.Queue()
         self._running = False
-        self._conns: _List[_Connection] = []
+        self._conns: list[_Connection] = []
 
     @property
     def num_connections(self) -> int:
         """Return the number of managed connections."""
         return len(self._conns)
 
-    def by_type(self, kind: _Type[T]) -> _Iterator[T]:
+    def by_type(self, kind: type[T]) -> _Iterator[T]:
         """Iterate over connections of a specific type."""
         for conn in self._conns:
             if isinstance(conn, kind):
                 yield conn
 
     def reset_metrics(self) -> None:
         """Reset connection metrics."""
@@ -67,15 +65,15 @@
         if self._running:
             await stop_sig.wait()
             return
 
         self._running = True
 
         stop_sig_task = _asyncio.create_task(stop_sig.wait())
-        tasks: _List[_asyncio.Task[None]] = []
+        tasks: list[_asyncio.Task[None]] = []
         self._conns = []
         new_conn_task: _Optional[_asyncio.Task[_Connection]] = None
 
         while not stop_sig.is_set():
             # Create a new-connection handler.
             if new_conn_task is None:
                 # Wait for a connection to be established.
```

### Comparing `runtimepy-3.9.0/runtimepy/net/mixin.py` & `runtimepy-4.0.0/runtimepy/net/mixin.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.9.0/runtimepy/net/server/html.py` & `runtimepy-4.0.0/runtimepy/net/server/html.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,58 +2,42 @@
 A module implementing HTML interfaces for web applications.
 """
 
 # built-in
 from typing import Awaitable, Callable, Optional, TextIO
 
 # third-party
-from svgen.element import Element
 from svgen.element.html import Html
 from vcorelib import DEFAULT_ENCODING
 
 # internal
 from runtimepy.net.http.header import RequestHeader
 from runtimepy.net.http.response import ResponseHeader
 from runtimepy.net.tcp.http import HttpConnection
 
 HtmlApp = Callable[
-    [Html, RequestHeader, ResponseHeader, Optional[bytes]], Awaitable[None]
+    [Html, RequestHeader, ResponseHeader, Optional[bytes]], Awaitable[Html]
 ]
 HtmlApps = dict[str, HtmlApp]
 
 
-async def default_html_app(
-    document: Html,
-    request: RequestHeader,
-    response: ResponseHeader,
-    request_data: Optional[bytes],
-) -> None:
-    """A simple 'Hello, world!' application."""
-
-    del request
-    del response
-    del request_data
-
-    document.body.children.append(Element(tag="div", text="Hello, world!"))
-
-
 async def html_handler(
     apps: HtmlApps,
     stream: TextIO,
     request: RequestHeader,
     response: ResponseHeader,
     request_data: Optional[bytes],
-    default_app: HtmlApp = default_html_app,
+    default_app: HtmlApp = None,
 ) -> None:
     """Render an HTML document in response to an HTTP request."""
 
     # Set response headers.
     response["Content-Type"] = f"text/html; charset={DEFAULT_ENCODING}"
 
     # Create the application.
-    document = Html(HttpConnection.identity)
-    await apps.get(request.target.path, default_app)(
-        document, request, response, request_data
-    )
-
-    stream.write("<!DOCTYPE html>\n")
-    document.encode(stream)
+    app = apps.get(request.target.path, default_app)
+    if app is not None:
+        document = await app(
+            Html(HttpConnection.identity), request, response, request_data
+        )
+        stream.write("<!DOCTYPE html>\n")
+        document.encode(stream)
```

### Comparing `runtimepy-3.9.0/runtimepy/net/server/json.py` & `runtimepy-4.0.0/runtimepy/net/server/json.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.9.0/runtimepy/net/stream/__init__.py` & `runtimepy-4.0.0/runtimepy/net/stream/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.9.0/runtimepy/net/stream/base.py` & `runtimepy-4.0.0/runtimepy/net/stream/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
 A module implementing a base, stream-oriented connection interface.
 """
 
 # built-in
 from io import BytesIO as _BytesIO
 from typing import BinaryIO as _BinaryIO
-from typing import Tuple, Type
 
 # third-party
 from vcorelib.io import ByteFifo
 
 # internal
 from runtimepy.net.connection import BinaryMessage
 from runtimepy.net.connection import Connection as _Connection
@@ -18,66 +17,66 @@
 
 class PrefixedMessageConnection(_Connection):
     """
     A connection for handling inter-frame message size prefixes for some
     stream-oriented protocols.
     """
 
-    message_length_kind: Type[UnsignedInt] = Uint32
+    message_length_kind: type[UnsignedInt] = Uint32
     reading_header: bool
 
     def init(self) -> None:
         """Initialize this instance."""
 
         # Header parsing.
         self.buffer = ByteFifo()
         self.reading_header = True
         self.message_length_in = self.message_length_kind()
         self.prefix_size = self.message_length_in.size
 
         self.message_length_out = self.message_length_kind()
 
     def _send_message(
-        self, data: BinaryMessage, addr: Tuple[str, int] = None
+        self, data: BinaryMessage, addr: tuple[str, int] = None
     ) -> None:
         """Underlying data send."""
 
         del addr
         self.send_binary(data)
 
     def send_message(
-        self, data: BinaryMessage, addr: Tuple[str, int] = None
+        self, data: BinaryMessage, addr: tuple[str, int] = None
     ) -> None:
         """Handle inter-message prefixes for outgoing messages."""
 
         self.message_length_out.value = len(data)
 
         with _BytesIO() as stream:
             self.message_length_out.to_stream(
                 stream, byte_order=self.byte_order
             )
             stream.write(data)
             self._send_message(stream.getvalue(), addr=addr)
 
     def send_message_str(
-        self, data: str, addr: Tuple[str, int] = None
+        self, data: str, addr: tuple[str, int] = None
     ) -> None:
         """Convert a message to bytes before sending."""
         self.send_message(data.encode(), addr=addr)
 
     async def process_single(
-        self, stream: _BinaryIO, addr: Tuple[str, int] = None
+        self, stream: _BinaryIO, addr: tuple[str, int] = None
     ) -> bool:
         """Process a single message."""
         del stream
         del addr
         return True
 
     async def process_binary(
-        self, data: bytes, addr: Tuple[str, int] = None
+        self, data: bytes, addr: tuple[str, int] = None
     ) -> bool:
         """Process an incoming message."""
 
         result = True
 
         self.buffer.ingest(data)
```

### Comparing `runtimepy-3.9.0/runtimepy/net/stream/json/base.py` & `runtimepy-4.0.0/runtimepy/net/stream/json/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # built-in
 from argparse import Namespace
 import asyncio
 from copy import copy
 from json import JSONDecodeError, dumps, loads
 import logging
-from typing import Any, Dict, List, Optional, Tuple, Type, Union
+from typing import Any, Optional, Union
 
 # third-party
 from vcorelib.dict.codec import JsonCodec
 from vcorelib.target.resolver import TargetResolver
 
 # internal
 from runtimepy import PKG_NAME, VERSION
@@ -40,15 +40,15 @@
 
 
 class JsonMessageConnection(
     StringMessageConnection, AsyncCommandProcessingMixin
 ):
     """A connection interface for JSON messaging."""
 
-    _log_messages: List[Dict[str, Any]]
+    _log_messages: list[dict[str, Any]]
     remote_meta: Optional[JsonMessage]
 
     def _register_handlers(self) -> None:
         """Register connection-specific command handlers."""
 
         # Extra handlers.
         self.typed_handler("find_file", FindFile, find_file_request_handler)
@@ -70,18 +70,18 @@
             "package": PKG_NAME,
             "version": VERSION,
             "kind": type(self).__name__,
         }
 
         self.curr_id: int = 1
 
-        self.ids_waiting: Dict[int, asyncio.Event] = {}
-        self.id_responses: Dict[int, JsonMessage] = {}
+        self.ids_waiting: dict[int, asyncio.Event] = {}
+        self.id_responses: dict[int, JsonMessage] = {}
 
-        self._log_messages: List[Dict[str, Any]] = []
+        self._log_messages: list[dict[str, Any]] = []
         self.remote_meta = None
 
         # Standard handlers.
         self.basic_handler("loopback")
         self.basic_handler("meta", self._meta_handler)
 
         self._register_handlers()
@@ -102,22 +102,22 @@
         self, key: str, handler: MessageHandler = loopback_handler
     ) -> None:
         """Register a basic handler."""
 
         assert self.targets.register(key, (key, handler, None))
 
     def typed_handler(
-        self, key: str, kind: Type[T], handler: TypedHandler[T]
+        self, key: str, kind: type[T], handler: TypedHandler[T]
     ) -> None:
         """Register a typed handler."""
 
         assert self.targets.register(key, (key, handler, kind))
 
     def send_json(
-        self, data: Union[JsonMessage, JsonCodec], addr: Tuple[str, int] = None
+        self, data: Union[JsonMessage, JsonCodec], addr: tuple[str, int] = None
     ) -> None:
         """Send a JSON message."""
 
         if isinstance(data, JsonCodec):
             data = data.asdict()
 
         # Add any pending log messages to this message.
@@ -156,15 +156,15 @@
                 ),
             )
 
     async def channel_command(
         self,
         command: str,
         environment: str = "default",
-        addr: Tuple[str, int] = None,
+        addr: tuple[str, int] = None,
     ) -> CommandResult:
         """Send a channel command to an endpoint."""
 
         result = await self.wait_json(
             {
                 "channel_command": {
                     "environment": environment,
@@ -179,15 +179,15 @@
             result["channel_command"]["success"],
             result["channel_command"].get("reason"),
         )
 
     async def wait_json(
         self,
         data: Union[JsonMessage, JsonCodec],
-        addr: Tuple[str, int] = None,
+        addr: tuple[str, int] = None,
         timeout: float = DEFAULT_TIMEOUT,
     ) -> JsonMessage:
         """Send a JSON message and wait for a response."""
 
         if isinstance(data, JsonCodec):
             data = data.asdict()
 
@@ -215,15 +215,15 @@
         del self.id_responses[ident]
 
         return result
 
     async def loopback(
         self,
         data: JsonMessage = None,
-        addr: Tuple[str, int] = None,
+        addr: tuple[str, int] = None,
         timeout: float = DEFAULT_TIMEOUT,
     ) -> bool:
         """Perform a simple loopback test on this connection."""
 
         if data is None:
             data = DEFAULT_LOOPBACK
 
@@ -306,15 +306,15 @@
                         "remote: " + message["msg"],
                         *message.get("args", []),
                     )
 
         return should_respond
 
     async def process_json(
-        self, data: JsonMessage, addr: Tuple[str, int] = None
+        self, data: JsonMessage, addr: tuple[str, int] = None
     ) -> bool:
         """Process a JSON message."""
 
         response: JsonMessage = {}
 
         keys_ignored = []
 
@@ -359,22 +359,25 @@
         for key, sub_response in sub_responses.items():
             if sub_response:
                 response[key] = sub_response
         del sub_responses
 
         if keys_ignored:
             response["keys_ignored"] = sorted(keys_ignored)
+            self.logger.warning(
+                "Ignored incoming message keys: %s.", ", ".join(keys_ignored)
+            )
 
         if self._handle_reserved(data, response) and response:
             self.send_json(response, addr=addr)
 
         return True
 
     async def process_message(
-        self, data: str, addr: Tuple[str, int] = None
+        self, data: str, addr: tuple[str, int] = None
     ) -> bool:
         """Process a string message."""
 
         result = True
 
         try:
             decoded = loads(data)
```

### Comparing `runtimepy-3.9.0/runtimepy/net/stream/json/handlers.py` & `runtimepy-4.0.0/runtimepy/net/stream/json/handlers.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.9.0/runtimepy/net/stream/json/types.py` & `runtimepy-4.0.0/runtimepy/net/stream/json/types.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """
 A module containing useful type definitions for JSON messaging.
 """
 
 # built-in
-from typing import Any, Awaitable, Callable, Dict, TypeVar
+from typing import Any, Awaitable, Callable, TypeVar
 
 # third-party
 from vcorelib.dict.codec import JsonCodec
 
-JsonMessage = Dict[str, Any]
+JsonMessage = dict[str, Any]
 
 #
 # async def message_handler(response: JsonMessage, data: JsonMessage) -> None:
 #     """A sample message handler."""
 #
 MessageHandler = Callable[[JsonMessage, JsonMessage], Awaitable[None]]
-MessageHandlers = Dict[str, MessageHandler]
+MessageHandlers = dict[str, MessageHandler]
 RESERVED_KEYS = {"keys_ignored", "__id__", "__log_messages__"}
 
 #
 # async def message_handler(response: JsonMessage, data: JsonCodec) -> None:
 #     """A sample message handler."""
 #
 T = TypeVar("T", bound=JsonCodec)
```

### Comparing `runtimepy-3.9.0/runtimepy/net/stream/string.py` & `runtimepy-4.0.0/runtimepy/net/stream/string.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.9.0/runtimepy/net/tcp/connection.py` & `runtimepy-4.0.0/runtimepy/net/tcp/connection.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,21 +10,20 @@
 from contextlib import asynccontextmanager as _asynccontextmanager
 from logging import getLogger as _getLogger
 import socket as _socket
 from typing import Any as _Any
 from typing import AsyncIterator as _AsyncIterator
 from typing import Callable as _Callable
 from typing import Optional as _Optional
-from typing import Tuple as _Tuple
-from typing import Type as _Type
 from typing import TypeVar as _TypeVar
 from typing import Union as _Union
 
 # internal
 from runtimepy.net import sockname as _sockname
+from runtimepy.net.backoff import ExponentialBackoff
 from runtimepy.net.connection import BinaryMessage as _BinaryMessage
 from runtimepy.net.connection import Connection as _Connection
 from runtimepy.net.connection import EchoConnection as _EchoConnection
 from runtimepy.net.connection import NullConnection as _NullConnection
 from runtimepy.net.manager import ConnectionManager as _ConnectionManager
 from runtimepy.net.mixin import TransportMixin as _TransportMixin
 from runtimepy.net.tcp.create import (
@@ -42,24 +41,27 @@
 class TcpConnection(_Connection, _TransportMixin):
     """A TCP connection interface."""
 
     # TCP connections send data directly without going through queues.
     uses_text_tx_queue = False
     uses_binary_tx_queue = False
 
+    log_alias = "TCP"
+    log_prefix = ""
+
     def __init__(self, transport: _Transport, protocol: QueueProtocol) -> None:
         """Initialize this TCP connection."""
 
         _TransportMixin.__init__(self, transport)
 
         # Re-assign with updated type information.
         self._transport: _Transport = transport
         self._set_protocol(protocol)
 
-        super().__init__(_getLogger(self.logger_name("TCP ")))
+        super().__init__(_getLogger(self.logger_name(f"{self.log_alias} ")))
 
         # Store connection-instantiation arguments.
         self._conn_kwargs: dict[str, _Any] = {}
 
     def _set_protocol(self, protocol: QueueProtocol) -> None:
         """Set a new protocol for this instance."""
 
@@ -97,30 +99,34 @@
 
         result = await try_tcp_transport_protocol(
             callback=callback, **self._conn_kwargs
         )
         return result is not None
 
     @classmethod
-    async def create_connection(cls: _Type[T], **kwargs) -> T:
+    async def create_connection(
+        cls: type[T], backoff: ExponentialBackoff = None, **kwargs
+    ) -> T:
         """Create a TCP connection."""
 
-        transport, protocol = await tcp_transport_protocol_backoff(**kwargs)
+        transport, protocol = await tcp_transport_protocol_backoff(
+            backoff=backoff, **kwargs
+        )
         inst = cls(transport, protocol)
 
         # Is there a better way to do this? We can't restart a server's side
         # of a connection (seems okay).
         inst._conn_kwargs = {**kwargs}
 
         return inst
 
     @classmethod
     @_asynccontextmanager
     async def serve(
-        cls: _Type[T],
+        cls: type[T],
         callback: ConnectionCallback[T] = None,
         **kwargs,
     ) -> _AsyncIterator[_Any]:
         """Serve incoming connections."""
 
         class CallbackProtocol(QueueProtocol):
             """Protocol that calls the provided callback."""
@@ -135,22 +141,29 @@
 
         eloop = _get_event_loop()
         server = await eloop.create_server(
             CallbackProtocol, family=_socket.AF_INET, **kwargs
         )
         async with server:
             for socket in server.sockets:
+                sockname = socket.getsockname()
                 LOG.info(
-                    "Started TCP server listening on '%s'.", _sockname(socket)
+                    "Started %s server listening on '%s%s' (%s%s:%d).",
+                    cls.log_alias,
+                    cls.log_prefix,
+                    _sockname(socket),
+                    cls.log_prefix,
+                    sockname[0] if sockname[0] != "0.0.0.0" else "localhost",
+                    sockname[1],
                 )
             yield server
 
     @classmethod
     async def app(
-        cls: _Type[T],
+        cls: type[T],
         stop_sig: _asyncio.Event,
         callback: ConnectionCallback[T] = None,
         serving_callback: _Callable[[_Any], None] = None,
         manager: _ConnectionManager = None,
         **kwargs,
     ) -> None:
         """Run an application that serves new connections."""
@@ -165,23 +178,23 @@
             assert manager is not None
             manager.queue.put_nowait(conn)
 
         async with cls.serve(app_cb, **kwargs) as server:
             if serving_callback is not None:
                 serving_callback(server)
 
-            LOG.info("TCP Application starting.")
+            LOG.info("%s Application starting.", cls.log_alias)
             await manager.manage(stop_sig)
-            LOG.info("TCP Application stopped.")
+            LOG.info("%s Application stopped.", cls.log_alias)
 
-        LOG.info("TCP Server closed.")
+        LOG.info("%s Server closed.", cls.log_alias)
 
     @classmethod
     @_asynccontextmanager
-    async def create_pair(cls: _Type[T]) -> _AsyncIterator[_Tuple[T, T]]:
+    async def create_pair(cls: type[T]) -> _AsyncIterator[tuple[T, T]]:
         """Create a connection pair."""
 
         cond = _Semaphore(0)
         conn1: _Optional[T] = None
 
         def callback(conn: T) -> None:
             """Signal the semaphore."""
```

### Comparing `runtimepy-3.9.0/runtimepy/net/tcp/create.py` & `runtimepy-4.0.0/runtimepy/net/tcp/create.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.9.0/runtimepy/net/tcp/http/__init__.py` & `runtimepy-4.0.0/runtimepy/net/tcp/http/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,14 +53,17 @@
 class HttpConnection(_TcpConnection):
     """A class implementing a basic HTTP interface."""
 
     identity = f"{PKG_NAME}/{VERSION}"
 
     expecting_response: bool
 
+    log_alias = "HTTP"
+    log_prefix = "http://"
+
     # Handlers registered at the class level so that instances created at
     # runtime don't need additional initialization.
     handlers: HttpRequestHandlers = {}
 
     def init(self) -> None:
         """Initialize this instance."""
```

### Comparing `runtimepy-3.9.0/runtimepy/net/tcp/protocol.py` & `runtimepy-4.0.0/runtimepy/net/tcp/protocol.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.9.0/runtimepy/net/tcp/telnet/__init__.py` & `runtimepy-4.0.0/runtimepy/net/tcp/telnet/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,16 @@
     "CARRIAGE_RETURN",
 ]
 
 
 class Telnet(_TcpConnection):
     """A class implementing a basic telnet interface."""
 
+    log_alias = "TELNET"
+
     async def process_telnet_message(self, data: bytes) -> bool:
         """By default, treat all incoming data bytes as text."""
         return await self.process_text(data.decode(encoding=DEFAULT_ENCODING))
 
     @_abstractmethod
     async def process_command(self, code: TelnetCode) -> None:
         """Process a telnet command."""
```

### Comparing `runtimepy-3.9.0/runtimepy/net/tcp/telnet/codes.py` & `runtimepy-4.0.0/runtimepy/net/tcp/telnet/codes.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.9.0/runtimepy/net/udp/connection.py` & `runtimepy-4.0.0/runtimepy/net/udp/connection.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 # built-in
 from abc import abstractmethod as _abstractmethod
 from asyncio import DatagramTransport as _DatagramTransport
 from contextlib import suppress as _suppress
 from logging import getLogger as _getLogger
 import socket as _socket
 from typing import Any as _Any
-from typing import Tuple as _Tuple
-from typing import Type as _Type
 from typing import TypeVar as _TypeVar
 from typing import Union as _Union
 
 # internal
 from runtimepy.net import IpHost, get_free_socket, normalize_host
 from runtimepy.net.connection import BinaryMessage as _BinaryMessage
 from runtimepy.net.connection import Connection as _Connection
@@ -72,20 +70,20 @@
         """
         self.remote_address = addr
         self.logger = _getLogger(self.logger_name("UDP "))
         self._protocol.logger = self.logger
 
     @_abstractmethod
     async def process_datagram(
-        self, data: bytes, addr: _Tuple[str, int]
+        self, data: bytes, addr: tuple[str, int]
     ) -> bool:
         """Process a datagram."""
 
     def sendto(
-        self, data: bytes, addr: _Union[IpHost, _Tuple[str, int]] = None
+        self, data: bytes, addr: _Union[IpHost, tuple[str, int]] = None
     ) -> None:
         """Send to a specific address."""
 
         try:
             self._transport.sendto(data, addr=addr)
             self.metrics.tx.increment(len(data))
 
@@ -119,15 +117,15 @@
         result = await try_udp_transport_protocol(
             callback=callback, **self._conn_kwargs
         )
         return result is not None
 
     @classmethod
     async def create_connection(
-        cls: _Type[T], connect: bool = True, **kwargs
+        cls: type[T], connect: bool = True, **kwargs
     ) -> T:
         """Create a UDP connection."""
 
         LOG.debug("kwargs: %s", kwargs)
 
         # If the caller specifies a remote address but doesn't want a connected
         # socket, handle this after initial creation.
@@ -151,15 +149,15 @@
         # Set the remote address manually if necessary.
         if not connect and remote_addr is not None:
             conn.set_remote_address(normalize_host(*remote_addr))
 
         return conn
 
     @classmethod
-    async def create_pair(cls: _Type[T]) -> _Tuple[T, T]:
+    async def create_pair(cls: type[T]) -> tuple[T, T]:
         """Create a connection pair."""
 
         # On Windows, local UDP sockets can't even be connected until the
         # receiving port is bound.
         sock1 = get_free_socket(kind=_socket.SOCK_DGRAM)
         sock2 = get_free_socket(kind=_socket.SOCK_DGRAM)
 
@@ -198,23 +196,23 @@
                     self.disable("read processing error")
 
 
 class EchoUdpConnection(UdpConnection, _EchoConnection):
     """An echo connection for UDP."""
 
     async def process_datagram(
-        self, data: bytes, addr: _Tuple[str, int]
+        self, data: bytes, addr: tuple[str, int]
     ) -> bool:
         """Process a datagram."""
 
         self.sendto(data, addr=addr)
         return True
 
 
 class NullUdpConnection(UdpConnection, _NullConnection):
     """A null UDP connection."""
 
     async def process_datagram(
-        self, data: bytes, addr: _Tuple[str, int]
+        self, data: bytes, addr: tuple[str, int]
     ) -> bool:
         """Process a datagram."""
         return True
```

### Comparing `runtimepy-3.9.0/runtimepy/net/udp/create.py` & `runtimepy-4.0.0/runtimepy/net/udp/create.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.9.0/runtimepy/net/udp/protocol.py` & `runtimepy-4.0.0/runtimepy/net/udp/protocol.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.9.0/runtimepy/net/util.py` & `runtimepy-4.0.0/runtimepy/net/util.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.9.0/runtimepy/net/websocket/connection.py` & `runtimepy-4.0.0/runtimepy/net/websocket/connection.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,16 +9,14 @@
 from contextlib import asynccontextmanager as _asynccontextmanager
 from contextlib import suppress as _suppress
 from logging import getLogger as _getLogger
 from typing import AsyncIterator as _AsyncIterator
 from typing import Awaitable as _Awaitable
 from typing import Callable as _Callable
 from typing import Optional as _Optional
-from typing import Tuple as _Tuple
-from typing import Type as _Type
 from typing import TypeVar as _TypeVar
 from typing import Union as _Union
 
 # third-party
 from vcorelib.asyncio import log_exceptions as _log_exceptions
 import websockets
 from websockets.client import (
@@ -87,31 +85,31 @@
         self.metrics.tx.increment(len(data))
 
     async def close(self) -> None:
         """Close this connection."""
         await self.protocol.close()
 
     @classmethod
-    async def create_connection(cls: _Type[T], uri: str, **kwargs) -> T:
+    async def create_connection(cls: type[T], uri: str, **kwargs) -> T:
         """Connect a client to an endpoint."""
 
         protocol = await getattr(websockets, "connect")(uri, **kwargs)
         return cls(protocol)
 
     @classmethod
     @_asynccontextmanager
-    async def client(cls: _Type[T], uri: str, **kwargs) -> _AsyncIterator[T]:
+    async def client(cls: type[T], uri: str, **kwargs) -> _AsyncIterator[T]:
         """A wrapper for connecting a client."""
 
         async with getattr(websockets, "connect")(uri, **kwargs) as protocol:
             yield cls(protocol)
 
     @classmethod
     def server_handler(
-        cls: _Type[T],
+        cls: type[T],
         init: ConnectionInit[T] = None,
         stop_sig: _asyncio.Event = None,
         manager: _ConnectionManager = None,
     ) -> _Callable[[_WebSocketServerProtocol], _Awaitable[None]]:
         """
         A wrapper for passing in a websocket handler and initializing a
         connection.
@@ -151,15 +149,15 @@
                 else:
                     await conn.process(stop_sig=stop_sig)
 
         return _handler
 
     @classmethod
     @_asynccontextmanager
-    async def create_pair(cls: _Type[T]) -> _AsyncIterator[_Tuple[T, T]]:
+    async def create_pair(cls: type[T]) -> _AsyncIterator[tuple[T, T]]:
         """Obtain a connected pair of WebsocketConnection objects."""
 
         server_conn: _Optional[T] = None
 
         async def server_init(protocol: _WebSocketServerProtocol) -> bool:
             """Create one side of the connection and update the reference."""
             nonlocal server_conn
@@ -175,15 +173,15 @@
             async with cls.client(f"ws://localhost:{host[1]}") as client_conn:
                 assert server_conn is not None
                 yield server_conn, client_conn
 
     @classmethod
     @_asynccontextmanager
     async def serve(
-        cls: _Type[T],
+        cls: type[T],
         init: ConnectionInit[T] = None,
         stop_sig: _asyncio.Event = None,
         manager: _ConnectionManager = None,
         **kwargs,
     ) -> _AsyncIterator[_WebSocketServer]:
         """Serve a WebSocket server."""
 
@@ -196,15 +194,15 @@
                     "Started WebSocket server listening on '%s'.",
                     _sockname(socket),
                 )
             yield server
 
     @classmethod
     async def app(
-        cls: _Type[T],
+        cls: type[T],
         stop_sig: _asyncio.Event,
         init: ConnectionInit[T] = None,
         manager: _ConnectionManager = None,
         serving_callback: _Callable[[_WebSocketServer], None] = None,
         **kwargs,
     ) -> None:
         """Run a WebSocket-server application."""
```

### Comparing `runtimepy-3.9.0/runtimepy/primitives/__init__.py` & `runtimepy-4.0.0/runtimepy/primitives/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 """
 A module implementing a primitive-type storage entity.
 """
 
 # built-in
-from typing import Dict as _Dict
-from typing import Type as _Type
 from typing import TypeVar as _TypeVar
 from typing import Union as _Union
 
 # internal
 from runtimepy.primitives.base import Primitive
 from runtimepy.primitives.bool import Bool
 from runtimepy.primitives.float import Double, Float, Half
@@ -81,33 +79,33 @@
     Uint64,
     Half,
     Float,
     Double,
     Bool,
 )
 
-Primitives: _Dict[str, _Type[AnyPrimitive]] = {
+Primitives: dict[str, type[AnyPrimitive]] = {
     Int8().kind.name: Int8,
     Int16().kind.name: Int16,
     Int32().kind.name: Int32,
     Int64().kind.name: Int64,
     Uint8().kind.name: Uint8,
     Uint16().kind.name: Uint16,
     Uint32().kind.name: Uint32,
     Uint64().kind.name: Uint64,
     Half().kind.name: Half,
     Float().kind.name: Float,
     Double().kind.name: Double,
     Bool().kind.name: Bool,
 }
 
-Primitivelike = _Union[_Type[AnyPrimitive], str]
+Primitivelike = _Union[type[AnyPrimitive], str]
 
 
-def normalize(value: Primitivelike) -> _Type[AnyPrimitive]:
+def normalize(value: Primitivelike) -> type[AnyPrimitive]:
     """Normalize a type of primitive or a string into a type of primitive."""
 
     if isinstance(value, str):
         value = value.lower()
         assert value in Primitives, f"No primitive '{value}'!"
         value = Primitives[value]
     return value
```

### Comparing `runtimepy-3.9.0/runtimepy/primitives/array/__init__.py` & `runtimepy-4.0.0/runtimepy/primitives/array/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 A module for implementing arrays of arbitrary primitives.
 """
 
 # built-in
 from copy import copy as _copy
 from struct import pack as _pack
 from struct import unpack as _unpack
-from typing import Dict as _Dict
-from typing import List as _List
 from typing import NamedTuple
 from typing import cast as _cast
 
 # internal
 from runtimepy.primitives import AnyPrimitive as _AnyPrimitive
 from runtimepy.primitives import Primitivelike as _Primitivelike
 from runtimepy.primitives import create as _create
@@ -34,39 +32,39 @@
 class PrimitiveArray(Serializable):
     """A class for managing primitives as arrays."""
 
     def __init__(
         self,
         *primitives: _AnyPrimitive,
         byte_order: _ByteOrder = _DEFAULT_BYTE_ORDER,
-        fragments: _List[ArrayFragmentSpec] = None,
+        fragments: list[ArrayFragmentSpec] = None,
         chain: Serializable = None,
     ) -> None:
         """Initialize this primitive array."""
 
-        self._primitives: _List[_AnyPrimitive] = []
+        self._primitives: list[_AnyPrimitive] = []
         self.byte_order = byte_order
         self._format: str = self.byte_order.fmt
 
         # Keep track of a quick lookup for converting between element indices
         # and byte indices.
-        self._bytes_to_index: _Dict[int, int] = {0: 0}
-        self._index_to_bytes: _Dict[int, int] = {0: 0}
+        self._bytes_to_index: dict[int, int] = {0: 0}
+        self._index_to_bytes: dict[int, int] = {0: 0}
 
         self.size = 0
         self.chain = None
 
         # Add initial items.
         for item in primitives:
             self.add(item)
 
         super().__init__(byte_order=self.byte_order, chain=chain)
 
-        self._fragments: _List["PrimitiveArray"] = []
-        self._fragment_specs: _List[ArrayFragmentSpec] = []
+        self._fragments: list["PrimitiveArray"] = []
+        self._fragment_specs: list[ArrayFragmentSpec] = []
 
         # Create array fragments from the specifications.
         if fragments is None:
             fragments = []
         for spec in fragments:
             self._add_fragment(spec)
```

### Comparing `runtimepy-3.9.0/runtimepy/primitives/base.py` & `runtimepy-4.0.0/runtimepy/primitives/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,29 +3,27 @@
 """
 
 # built-in
 from copy import copy as _copy
 from math import isclose as _isclose
 from typing import BinaryIO as _BinaryIO
 from typing import Callable as _Callable
-from typing import Dict as _Dict
 from typing import Generic as _Generic
-from typing import Tuple as _Tuple
 from typing import TypeVar as _TypeVar
 
 # third-party
 from vcorelib.math.time import default_time_ns, nano_str
 
 # internal
 from runtimepy.primitives.byte_order import (
     DEFAULT_BYTE_ORDER as _DEFAULT_BYTE_ORDER,
 )
 from runtimepy.primitives.byte_order import ByteOrder as _ByteOrder
 from runtimepy.primitives.scaling import ChannelScaling, Numeric, apply, invert
-from runtimepy.primitives.type import AnyPrimitiveType as _AnyPrimitiveType
+from runtimepy.primitives.types import AnyPrimitiveType as _AnyPrimitiveType
 
 T = _TypeVar("T", bool, int, float)
 
 # Current value first, new value next.
 PrimitiveChangeCallaback = _Callable[[T, T], None]
 
 
@@ -41,17 +39,17 @@
     def __init__(
         self, value: T = None, scaling: ChannelScaling = None
     ) -> None:
         """Initialize this primitive."""
 
         self.raw = self.kind.instance()
         self.curr_callback: int = 0
-        self.callbacks: _Dict[
-            int, _Tuple[PrimitiveChangeCallaback[T], bool]
-        ] = {}
+        self.callbacks: dict[int, tuple[PrimitiveChangeCallaback[T], bool]] = (
+            {}
+        )
         self(value=value)
         self.last_updated_ns: int = default_time_ns()
         self.scaling = scaling
 
     def age_ns(self, now: int = None) -> int:
         """Get the age of this primitive's value in nanoseconds."""
```

### Comparing `runtimepy-3.9.0/runtimepy/primitives/bool.py` & `runtimepy-4.0.0/runtimepy/primitives/bool.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 """
 A module implementing a boolean-primitive interface.
 """
 
 # internal
 from runtimepy.primitives.base import Primitive as _Primitive
-from runtimepy.primitives.type.bool import Bool as _Bool
+from runtimepy.primitives.types.bool import Bool as _Bool
 
 
 class BooleanPrimitive(_Primitive[bool]):
     """A simple primitive class for booleans."""
 
     kind = _Bool
+    value: bool
 
     def __init__(self, value: bool = False) -> None:
         """Initialize this boolean primitive."""
         super().__init__(value=value)
 
     def toggle(self) -> None:
         """Toggle the underlying value."""
-        self.raw.value = not self.raw.value
+        self.value = not self.raw.value
 
     def set(self) -> None:
         """Coerce the underlying value to true."""
-        self.raw.value = True
+        self.value = True
 
     def clear(self) -> None:
         """Coerce the underlying value to false."""
-        self.raw.value = False
+        self.value = False
 
 
 Bool = BooleanPrimitive
```

### Comparing `runtimepy-3.9.0/runtimepy/primitives/byte_order.py` & `runtimepy-4.0.0/runtimepy/primitives/byte_order.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.9.0/runtimepy/primitives/field/__init__.py` & `runtimepy-4.0.0/runtimepy/primitives/field/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,20 +21,22 @@
 
     def __init__(
         self,
         raw: _UnsignedInt,
         index: int,
         width: int,
         commandable: bool = False,
+        description: str = None,
     ) -> None:
         """Initialize this bit-field."""
 
         self.raw = raw
         self.index = index
         self.commandable = commandable
+        self.description = description
 
         # Compute a bit-mask for this field.
         self.width = width
         self.mask = (2**self.width) - 1
         self.shifted_mask = self.mask << self.index
 
     def where_str(self) -> str:
@@ -89,18 +91,21 @@
         self,
         name: str,
         raw: _UnsignedInt,
         index: int,
         width: int,
         enum: _RegistryKey = None,
         commandable: bool = False,
+        description: str = None,
     ) -> None:
         """Initialize this bit-field."""
 
-        super().__init__(raw, index, width, commandable=commandable)
+        super().__init__(
+            raw, index, width, commandable=commandable, description=description
+        )
 
         # Verify bit-field parameters.
         assert (
             raw.kind.is_integer
         ), f"Can't create a bit field with {raw.kind}!"
         assert (
             index < raw.kind.bits
@@ -133,19 +138,26 @@
     def __init__(
         self,
         name: str,
         raw: _UnsignedInt,
         index: int,
         enum: _RegistryKey = None,
         commandable: bool = False,
+        description: str = None,
     ) -> None:
         """Initialize this bit flag."""
 
         super().__init__(
-            name, raw, index, 1, enum=enum, commandable=commandable
+            name,
+            raw,
+            index,
+            1,
+            enum=enum,
+            commandable=commandable,
+            description=description,
         )
 
     def clear(self) -> None:
         """Clear this field."""
         self(val=0)
 
     def set(self, val: bool = True) -> None:
```

### Comparing `runtimepy-3.9.0/runtimepy/primitives/field/fields.py` & `runtimepy-4.0.0/runtimepy/primitives/field/fields.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 """
 A module implementing a data structure for managing multiple bit fields.
 """
 
 # built-in
-from typing import Dict as _Dict
 from typing import Iterator as _Iterator
-from typing import List as _List
 from typing import Optional as _Optional
-from typing import Tuple as _Tuple
-from typing import Type as _Type
 from typing import TypeVar as _TypeVar
 from typing import Union as _Union
 from typing import cast as _cast
 
 # third-party
 from vcorelib.io.types import JsonObject as _JsonObject
 from vcorelib.io.types import JsonValue as _JsonValue
@@ -42,41 +38,46 @@
         # Create the underlying storage element.
         self.raw: _UnsignedInt = _cast(
             _UnsignedInt, _normalize(_cast(str, data["type"]))()
         )
 
         self.curr_index = 0
         self.bits_available = set(range(self.raw.kind.bits))
-        self.fields: _Dict[str, _BitField] = {}
-        self.by_index: _Dict[int, _Union[_BitField, _Tuple[int, int]]] = {}
+        self.fields: dict[str, _BitField] = {}
+        self.by_index: dict[int, _Union[_BitField, tuple[int, int]]] = {}
 
         # Set this initially false while we're initializing.
         self._finalized: bool = False
 
         # Load initial fields and flags.
-        for item in _cast(_List[_Dict[str, int]], data["fields"]):
+        for item in _cast(list[dict[str, int]], data["fields"]):
             name: str = _cast(str, item.get("name", ""))
             index: _Optional[int] = item.get("index")
             width: int = item["width"]
             value: int = int(item["value"])
             enum = item.get("enum")
+            desc: _Optional[str] = _cast(str, item.get("description"))
 
             # Fields without names are considered padding.
             if not name:
                 assert value == 0, "Can't set padding to non-zero value!"
                 assert enum is None, f"Enum '{enum}' specified for padding!"
                 item["index"] = self.pad(width=width, index=index)
                 continue
 
             if width == 1:
-                flag = self.flag(name, index=index, enum=enum)
+                flag = self.flag(
+                    name, index=index, enum=enum, description=desc
+                )
                 flag(value)
                 item["index"] = flag.index
             else:
-                field = self.field(name, width, index=index, enum=enum)
+                field = self.field(
+                    name, width, index=index, enum=enum, description=desc
+                )
                 field(value)
                 item["index"] = field.index
 
         self._finalized: bool = _cast(bool, data["finalized"])
 
     @property
     def names(self) -> _Iterator[str]:
@@ -86,15 +87,15 @@
     def finalize(self) -> None:
         """Finalize the fields so that new fields can't be added."""
         self._finalized = True
 
     def asdict(self) -> _JsonObject:
         """Get these bit fields as a dictionary."""
 
-        fields: _List[_Dict[str, _Union[str, int]]] = []
+        fields: list[dict[str, _Union[str, int]]] = []
 
         # Ensure both real fields and padding are encoded.
         for index, item in self.by_index.items():
             if isinstance(item, tuple):
                 fields.append(
                     {"index": index, "width": item[0], "value": item[1]}
                 )
@@ -122,21 +123,27 @@
 
         result = self.get_field(key)
         if result is None:
             raise KeyError(f"No field '{key}'!")
         return result
 
     def flag(
-        self, name: str, index: int = None, enum: _RegistryKey = None
+        self,
+        name: str,
+        index: int = None,
+        enum: _RegistryKey = None,
+        description: str = None,
     ) -> _BitFlag:
         """Create a new bit flag."""
 
         index = self._claim_bits(1, index=index)
 
-        result = _BitFlag(name, self.raw, index, enum=enum)
+        result = _BitFlag(
+            name, self.raw, index, enum=enum, description=description
+        )
 
         self.fields[name] = result
         self.by_index[index] = result
         return result
 
     def _claim_bits(self, width: int, index: int = None) -> int:
         """Allocate bits within this primitive."""
@@ -175,27 +182,30 @@
 
     def field(
         self,
         name: str,
         width: int,
         index: int = None,
         enum: _RegistryKey = None,
+        description: str = None,
     ) -> _BitField:
         """Create a new bit field."""
 
         assert width != 1, "Use bit-flags for single-width fields!"
 
         index = self._claim_bits(width, index=index)
 
-        result = _BitField(name, self.raw, index, width, enum=enum)
+        result = _BitField(
+            name, self.raw, index, width, enum=enum, description=description
+        )
 
         self.fields[name] = result
         self.by_index[index] = result
         return result
 
     @classmethod
-    def new(cls: _Type[T], value: _Primitivelike = "uint8") -> T:
+    def new(cls: type[T], value: _Primitivelike = "uint8") -> T:
         """Create a new bit-field storage entity."""
 
         return cls.create(
             {"type": _cast(str, value), "fields": [], "finalized": False}
         )
```

### Comparing `runtimepy-3.9.0/runtimepy/primitives/field/manager/__init__.py` & `runtimepy-4.0.0/runtimepy/primitives/field/manager/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 """
 A management entity for bit-fields.
 """
 
 # built-in
-from typing import Dict as _Dict
 from typing import Iterable as _Iterable
-from typing import Set as _Set
 from typing import cast as _cast
 
 # third-party
 from vcorelib.io import ARBITER as _ARBITER
 from vcorelib.io.types import JsonObject as _JsonObject
 from vcorelib.io.types import JsonValue as _JsonValue
 from vcorelib.paths import Pathlike as _Pathlike
@@ -40,26 +38,24 @@
 
     return fields_from_dict(_ARBITER.decode(path, require_success=True).data)
 
 
 class BitFieldsManager(BitFieldsManagerBase):
     """A class for managing multiple bit-fields objects."""
 
-    def export_json(
-        self, resolve_enum: bool = True
-    ) -> _Dict[str, _JsonObject]:
+    def export_json(self, resolve_enum: bool = True) -> dict[str, _JsonObject]:
         """Export this manager's data to JSON."""
 
         # Only export names that we're using.
         names: _JsonObject = {
             name: self.registry.identifier(name) for name in self.lookup
         }
 
         # Only export enums that we're using.
-        enum_ids: _Set[int] = {x.id for x in self.enums.items.values()}
+        enum_ids: set[int] = {x.id for x in self.enums.items.values()}
         enums: _JsonObject = {
             name: _cast(_JsonValue, val.asdict())
             for name, val in self.enums.items.items()
             if val.id in enum_ids
         }
 
         return {
@@ -68,19 +64,19 @@
             FIELDS_KEY: self.asdict(),
             VALUES_KEY: _cast(
                 _JsonObject, self.values(resolve_enum=resolve_enum)
             ),
         }
 
     @classmethod
-    def import_json(cls, data: _Dict[str, _JsonObject]) -> "BitFieldsManager":
+    def import_json(cls, data: dict[str, _JsonObject]) -> "BitFieldsManager":
         """Create a bit-fields manager from JSON data."""
 
         result = cls(
-            _NameRegistry(reverse=_cast(_Dict[str, int], data[NAMES_KEY])),
+            _NameRegistry(reverse=_cast(dict[str, int], data[NAMES_KEY])),
             _EnumRegistry.create(data[ENUMS_KEY]),
             fields=fields_from_dict(data[FIELDS_KEY]),
         )
 
         # Set values.
         for name, value in data.get(VALUES_KEY, {}).items():
             result.set(name, _cast(int, value))
```

### Comparing `runtimepy-3.9.0/runtimepy/primitives/field/manager/base.py` & `runtimepy-4.0.0/runtimepy/primitives/field/manager/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 """
 A base management entity for bit-fields.
 """
 
 # built-in
 from copy import copy as _copy
-from typing import Dict as _Dict
 from typing import Iterable as _Iterable
-from typing import List as _List
 from typing import Optional as _Optional
 from typing import TypeVar as _TypeVar
 from typing import Union as _Union
 from typing import cast as _cast
 
 # third-party
 from vcorelib.io import ARBITER as _ARBITER
@@ -58,17 +56,17 @@
         # Use a channel registry to register field names to.
         self.registry = registry
         self.enums = enums
 
         if fields is None:
             fields = []
 
-        self.fields: _List[_BitFields] = []
-        self.lookup: _Dict[str, int] = {}
-        self.enum_lookup: _Dict[str, _RuntimeEnum] = {}
+        self.fields: list[_BitFields] = []
+        self.lookup: dict[str, int] = {}
+        self.enum_lookup: dict[str, _RuntimeEnum] = {}
 
         # Add initial fields.
         for field in fields:
             self.add(field)
 
     def __copy__(self: T) -> T:
         """
@@ -130,23 +128,24 @@
     ) -> _Union[int, bool, str]:
         """Get the value of a field."""
 
         field = self[key]
         value: _Union[int, str] = field()
 
         if field.is_enum and resolve_enum:
-            value = self.enum_lookup[field.name].get_str(value)
+            name = self.registry.name(key)
+            assert name is not None, key
+            value = self.enum_lookup[name].get_str(value)
+
         elif field.width == 1:
             value = bool(value)
 
         return value
 
-    def values(
-        self, resolve_enum: bool = True
-    ) -> _Dict[str, _Union[str, int]]:
+    def values(self, resolve_enum: bool = True) -> dict[str, _Union[str, int]]:
         """Get a new dictionary of current field values."""
 
         return {
             name: self.get(name, resolve_enum=resolve_enum)
             for name in self.lookup
         }
```

### Comparing `runtimepy-3.9.0/runtimepy/primitives/float.py` & `runtimepy-4.0.0/runtimepy/primitives/float.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 A module implementing a floating-point primitive interface.
 """
 
 # internal
 from runtimepy.primitives.base import Primitive as _Primitive
 from runtimepy.primitives.scaling import ChannelScaling
-from runtimepy.primitives.type.float import Double as _Double
-from runtimepy.primitives.type.float import Float as _Float
-from runtimepy.primitives.type.float import Half as _Half
+from runtimepy.primitives.types.float import Double as _Double
+from runtimepy.primitives.types.float import Float as _Float
+from runtimepy.primitives.types.float import Half as _Half
 
 
 class HalfPrimitive(_Primitive[float]):
     """A simple primitive class for single-precision floating-point."""
 
     kind = _Half
```

### Comparing `runtimepy-3.9.0/runtimepy/primitives/int.py` & `runtimepy-4.0.0/runtimepy/primitives/int.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 
 # built-in
 from typing import Union as _Union
 
 # internal
 from runtimepy.primitives.base import Primitive as _Primitive
 from runtimepy.primitives.scaling import ChannelScaling
-from runtimepy.primitives.type.int import Int8 as _Int8
-from runtimepy.primitives.type.int import Int16 as _Int16
-from runtimepy.primitives.type.int import Int32 as _Int32
-from runtimepy.primitives.type.int import Int64 as _Int64
-from runtimepy.primitives.type.int import Uint8 as _Uint8
-from runtimepy.primitives.type.int import Uint16 as _Uint16
-from runtimepy.primitives.type.int import Uint32 as _Uint32
-from runtimepy.primitives.type.int import Uint64 as _Uint64
+from runtimepy.primitives.types.int import Int8 as _Int8
+from runtimepy.primitives.types.int import Int16 as _Int16
+from runtimepy.primitives.types.int import Int32 as _Int32
+from runtimepy.primitives.types.int import Int64 as _Int64
+from runtimepy.primitives.types.int import Uint8 as _Uint8
+from runtimepy.primitives.types.int import Uint16 as _Uint16
+from runtimepy.primitives.types.int import Uint32 as _Uint32
+from runtimepy.primitives.types.int import Uint64 as _Uint64
 
 
 class Int8Primitive(_Primitive[int]):
     """A simple primitive class for integer primitives."""
 
     kind = _Int8
```

### Comparing `runtimepy-3.9.0/runtimepy/primitives/scaling.py` & `runtimepy-4.0.0/runtimepy/primitives/scaling.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 A module implementing interfaces for working with channel scaling polynomials.
 """
 
 # built-in
-from typing import List, Union
+from typing import Union
 
 Numeric = Union[float, int]
-ChannelScaling = List[Numeric]
+ChannelScaling = list[Numeric]
 
 
 def invert(
     value: Numeric, scaling: ChannelScaling = None, should_round: bool = False
 ) -> Numeric:
     """Apply a scaling polynomial to a value."""
```

### Comparing `runtimepy-3.9.0/runtimepy/primitives/serializable/base.py` & `runtimepy-4.0.0/runtimepy/primitives/serializable/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.9.0/runtimepy/primitives/serializable/fixed.py` & `runtimepy-4.0.0/runtimepy/primitives/serializable/fixed.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.9.0/runtimepy/primitives/serializable/prefixed.py` & `runtimepy-4.0.0/runtimepy/primitives/serializable/prefixed.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 A module implementing a variable-size bytes serializable, using an integer
 primitive prefix to determine the size of the chunk portion.
 """
 
 # built-in
 from typing import BinaryIO as _BinaryIO
-from typing import Type, TypeVar
+from typing import TypeVar
 
 # internal
 from runtimepy.primitives import Primitivelike, UnsignedInt, create
 from runtimepy.primitives.byte_order import (
     DEFAULT_BYTE_ORDER as _DEFAULT_BYTE_ORDER,
 )
 from runtimepy.primitives.byte_order import ByteOrder as _ByteOrder
@@ -81,14 +81,14 @@
                 self.prefix.from_stream(stream, byte_order=self.byte_order)
             )
         )
         return self._update_size()
 
     @classmethod
     def create(
-        cls: Type[T],
+        cls: type[T],
         prefix: Primitivelike = "uint16",
         chain: Serializable = None,
     ) -> T:
         """Create a prefixed chunk."""
 
         return cls(create(prefix), chain=chain)  # type: ignore
```

### Comparing `runtimepy-3.9.0/runtimepy/primitives/string.py` & `runtimepy-4.0.0/runtimepy/primitives/string.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 A module implementing integer-prefixed string reading and writing.
 """
 
 # built-in
 from typing import BinaryIO as _BinaryIO
-from typing import Type as _Type
 
 # internal
 from runtimepy.primitives.base import Primitive as _Primitive
 from runtimepy.primitives.byte_order import (
     DEFAULT_BYTE_ORDER as _DEFAULT_BYTE_ORDER,
 )
 from runtimepy.primitives.byte_order import ByteOrder as _ByteOrder
@@ -17,15 +16,15 @@
 
 class StringPrimitive:
     """A class implementing a string-primitive interface."""
 
     def __init__(
         self,
         value: str = "",
-        kind: _Type[_Primitive[int]] = _Uint16,
+        kind: type[_Primitive[int]] = _Uint16,
         byte_order: _ByteOrder = _DEFAULT_BYTE_ORDER,
     ) -> None:
         """Initialize this string primitive."""
 
         assert kind.kind.is_integer
         self._value = value
         self._size = kind(value=len(self._value))
@@ -42,15 +41,15 @@
     def __eq__(self, other) -> bool:
         """Determine if this instance is equivalent to another."""
         return self._value == str(other)
 
     @staticmethod
     def from_stream(
         stream: _BinaryIO,
-        kind: _Type[_Primitive[int]] = _Uint16,
+        kind: type[_Primitive[int]] = _Uint16,
         byte_order: _ByteOrder = _DEFAULT_BYTE_ORDER,
     ) -> "StringPrimitive":
         """Create a new string primitive from a stream."""
 
         result = StringPrimitive(kind=kind, byte_order=byte_order)
         result.read(stream)
         return result
```

### Comparing `runtimepy-3.9.0/runtimepy/primitives/type/__init__.py` & `runtimepy-4.0.0/runtimepy/primitives/types/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 """
 A module exposing primitive types.
 """
 
 # built-in
-from typing import Dict as _Dict
 from typing import Union as _Union
 
 # internal
-from runtimepy.primitives.type.bool import Bool, BooleanType
-from runtimepy.primitives.type.float import (
+from runtimepy.primitives.types.bool import Bool, BooleanType
+from runtimepy.primitives.types.float import (
     Double,
     DoubleType,
     Float,
     FloatType,
     Half,
     HalfType,
 )
-from runtimepy.primitives.type.int import (
+from runtimepy.primitives.types.int import (
     Int8,
     Int8Type,
     Int16,
     Int16Type,
     Int32,
     Int32Type,
     Int64,
@@ -40,15 +39,15 @@
 
 AnyIntegerType = _Union[SignedIntegerType, UnsignedIntegerType]
 
 AnyPrimitiveType = _Union[
     AnyIntegerType, HalfType, FloatType, DoubleType, BooleanType
 ]
 
-PrimitiveTypes: _Dict[str, AnyPrimitiveType] = {
+PrimitiveTypes: dict[str, AnyPrimitiveType] = {
     # Integer types.
     Int8.name: Int8,
     Int16.name: Int16,
     Int32.name: Int32,
     Int64.name: Int64,
     Uint8.name: Uint8,
     Uint16.name: Uint16,
```

### Comparing `runtimepy-3.9.0/runtimepy/primitives/type/base.py` & `runtimepy-4.0.0/runtimepy/primitives/types/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,25 +6,24 @@
 import ctypes as _ctypes
 from struct import calcsize as _calcsize
 from struct import pack as _pack
 from struct import unpack as _unpack
 from typing import BinaryIO as _BinaryIO
 from typing import Generic as _Generic
 from typing import Optional as _Optional
-from typing import Type as _Type
 from typing import TypeVar as _TypeVar
 from typing import Union as _Union
 from typing import cast as _cast
 
 # internal
 from runtimepy.primitives.byte_order import (
     DEFAULT_BYTE_ORDER as _DEFAULT_BYTE_ORDER,
 )
 from runtimepy.primitives.byte_order import ByteOrder as _ByteOrder
-from runtimepy.primitives.type.bounds import IntegerBounds
+from runtimepy.primitives.types.bounds import IntegerBounds
 
 # Integer type aliases.
 Int8Ctype = _ctypes.c_byte
 Int16Ctype = _ctypes.c_short
 Int32Ctype = _ctypes.c_int
 Int64Ctype = _ctypes.c_longlong
 Uint8Ctype = _ctypes.c_ubyte
@@ -64,15 +63,15 @@
 
 
 class PrimitiveType(_Generic[T]):
     """A simple wrapper around ctype primitives."""
 
     # Sub-classes must set these class attributes.
     name: str
-    c_type: _Type[T]
+    c_type: type[T]
 
     def __init__(self, struct_format: str, signed: bool = True) -> None:
         """Initialize this primitive type."""
 
         self.format = struct_format
         self.signed = signed
         self.int_bounds: _Optional[IntegerBounds] = None
```

### Comparing `runtimepy-3.9.0/runtimepy/primitives/type/bool.py` & `runtimepy-4.0.0/runtimepy/primitives/types/bool.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 A module implementing a type interface for booleans.
 """
 
 # internal
-from runtimepy.primitives.type.base import BoolCtype as _BoolCtype
-from runtimepy.primitives.type.base import PrimitiveType as _PrimitiveType
+from runtimepy.primitives.types.base import BoolCtype as _BoolCtype
+from runtimepy.primitives.types.base import PrimitiveType as _PrimitiveType
 
 
 class BooleanType(_PrimitiveType[_BoolCtype]):
     """A simple type interface for booleans."""
 
     name = "bool"
     c_type = _BoolCtype
```

### Comparing `runtimepy-3.9.0/runtimepy/primitives/type/bounds.py` & `runtimepy-4.0.0/runtimepy/primitives/types/bounds.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.9.0/runtimepy/primitives/type/float.py` & `runtimepy-4.0.0/runtimepy/primitives/types/float.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 A module implementing a type interface for floating-point numbers.
 """
 
 # internal
-from runtimepy.primitives.type.base import DoubleCtype as _DoubleCtype
-from runtimepy.primitives.type.base import FloatCtype as _FloatCtype
-from runtimepy.primitives.type.base import PrimitiveType as _PrimitiveType
+from runtimepy.primitives.types.base import DoubleCtype as _DoubleCtype
+from runtimepy.primitives.types.base import FloatCtype as _FloatCtype
+from runtimepy.primitives.types.base import PrimitiveType as _PrimitiveType
 
 
 class HalfType(_PrimitiveType[_FloatCtype]):
     """A simple type interface for single-precision floating-point."""
 
     name = "half"
```

### Comparing `runtimepy-3.9.0/runtimepy/primitives/type/int.py` & `runtimepy-4.0.0/runtimepy/primitives/types/int.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """
 A module implementing a type interface for integers.
 """
 
 # internal
-from runtimepy.primitives.type.base import Int8Ctype as _Int8Ctype
-from runtimepy.primitives.type.base import Int16Ctype as _Int16Ctype
-from runtimepy.primitives.type.base import Int32Ctype as _Int32Ctype
-from runtimepy.primitives.type.base import Int64Ctype as _Int64Ctype
-from runtimepy.primitives.type.base import PrimitiveType as _PrimitiveType
-from runtimepy.primitives.type.base import Uint8Ctype as _Uint8Ctype
-from runtimepy.primitives.type.base import Uint16Ctype as _Uint16Ctype
-from runtimepy.primitives.type.base import Uint32Ctype as _Uint32Ctype
-from runtimepy.primitives.type.base import Uint64Ctype as _Uint64Ctype
-from runtimepy.primitives.type.bounds import IntegerBounds
+from runtimepy.primitives.types.base import Int8Ctype as _Int8Ctype
+from runtimepy.primitives.types.base import Int16Ctype as _Int16Ctype
+from runtimepy.primitives.types.base import Int32Ctype as _Int32Ctype
+from runtimepy.primitives.types.base import Int64Ctype as _Int64Ctype
+from runtimepy.primitives.types.base import PrimitiveType as _PrimitiveType
+from runtimepy.primitives.types.base import Uint8Ctype as _Uint8Ctype
+from runtimepy.primitives.types.base import Uint16Ctype as _Uint16Ctype
+from runtimepy.primitives.types.base import Uint32Ctype as _Uint32Ctype
+from runtimepy.primitives.types.base import Uint64Ctype as _Uint64Ctype
+from runtimepy.primitives.types.bounds import IntegerBounds
 
 
 class Int8Type(_PrimitiveType[_Int8Ctype]):
     """A simple type interface for int8's."""
 
     name = "int8"
     c_type = _Int8Ctype
```

### Comparing `runtimepy-3.9.0/runtimepy/registry/__init__.py` & `runtimepy-4.0.0/runtimepy/registry/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 """
 A generic registry interface for keeping track of objects by either string or
 integer identifier.
 """
 
 # built-in
 from abc import abstractmethod as _abstractmethod
-from typing import Dict as _Dict
 from typing import Generic as _Generic
 from typing import Iterator
 from typing import Optional as _Optional
-from typing import Tuple
-from typing import Type as _Type
 from typing import TypeVar as _TypeVar
 from typing import cast as _cast
 
 # third-party
 from vcorelib.io.types import JsonObject as _JsonObject
 from vcorelib.io.types import JsonValue as _JsonValue
 
@@ -26,38 +23,38 @@
 
 T = _TypeVar("T", bound=_RegistryItem)
 
 
 class Registry(_RuntimepyDictCodec, _Generic[T]):
     """A base class for a generic registry."""
 
-    name_registry: _Type[_NameRegistry] = _NameRegistry
+    name_registry: type[_NameRegistry] = _NameRegistry
 
     @property
     @_abstractmethod
-    def kind(self) -> _Type[T]:
+    def kind(self) -> type[T]:
         """Determine what kind of registry this is."""
 
     def init(self, data: _JsonObject) -> None:
         """Perform implementation-specific initialization."""
 
         # Create the registry items and name mapping.
-        self.items: _Dict[str, T] = {
+        self.items: dict[str, T] = {
             name: self.kind.create(_cast(_JsonObject, data))
             for name, data in data.items()
         }
 
         # Create the name registry.
         self.names = self.name_registry(
             reverse={name: item.id for name, item in self.items.items()}
         )
 
     def search(
         self, pattern: str, exact: bool = False
-    ) -> Iterator[Tuple[str, T]]:
+    ) -> Iterator[tuple[str, T]]:
         """Search for items in the registry by name."""
 
         for name in self.names.search(pattern, exact=exact):
             yield name, self.items[name]
 
     def asdict(self) -> _JsonObject:
         """Get this registry as a dictionary."""
```

### Comparing `runtimepy-3.9.0/runtimepy/registry/bool.py` & `runtimepy-4.0.0/runtimepy/registry/bool.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.9.0/runtimepy/registry/item.py` & `runtimepy-4.0.0/runtimepy/registry/item.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.9.0/runtimepy/registry/name.py` & `runtimepy-4.0.0/runtimepy/registry/name.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.9.0/runtimepy/schemas.py` & `runtimepy-4.0.0/runtimepy/schemas.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.9.0/runtimepy/task/asynchronous.py` & `runtimepy-4.0.0/runtimepy/task/asynchronous.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.9.0/runtimepy/task/basic/manager.py` & `runtimepy-4.0.0/runtimepy/task/basic/manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 A module implementing a periodic-task manager.
 """
 
 # built-in
 import asyncio as _asyncio
 from contextlib import asynccontextmanager as _asynccontextmanager
 from typing import AsyncIterator as _AsyncIterator
-from typing import Dict as _Dict
 from typing import Generic as _Generic
 from typing import Iterator as _Iterator
 from typing import TypeVar as _TypeVar
 
 # internal
 from runtimepy.task.basic.periodic import PeriodicTask as _PeriodicTask
 
@@ -18,15 +17,15 @@
 
 
 class PeriodicTaskManager(_Generic[T]):
     """A class for managing periodic tasks as a single group."""
 
     def __init__(self) -> None:
         """Initialize this instance."""
-        self._tasks: _Dict[str, T] = {}
+        self._tasks: dict[str, T] = {}
 
     def register(self, task: T, period_s: float = None) -> bool:
         """Register a periodic task."""
 
         result = task.name not in self._tasks
         if result:
             self._tasks[task.name] = task
```

### Comparing `runtimepy-3.9.0/runtimepy/task/basic/periodic.py` & `runtimepy-4.0.0/runtimepy/task/basic/periodic.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,16 +63,26 @@
 
         ChannelEnvironmentMixin.__init__(self, env=env)
         self.setup_level_channel(self.env)
         self.command = ChannelCommandProcessor(self.env, self.logger)
         self.register_task_metrics(self.metrics)
 
         # State.
-        self.env.channel("paused", self._paused, commandable=True)
-        self.env.channel("period_s", self.period_s, commandable=True)
+        self.env.channel(
+            "paused",
+            self._paused,
+            commandable=True,
+            description="Whether or not this task is paused.",
+        )
+        self.env.channel(
+            "period_s",
+            self.period_s,
+            commandable=True,
+            description="Iteration period for this task.",
+        )
         self._init_state()
         if self.auto_finalize:
             self.env.finalize()
 
         self._dispatch_rate = _RateTracker(depth=average_depth)
         self._dispatch_time = _MovingAverage(depth=average_depth)
```

### Comparing `runtimepy-3.9.0/runtimepy/task/trig/__init__.py` & `runtimepy-4.0.0/runtimepy/task/trig/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.9.0/runtimepy/tui/channels/__init__.py` & `runtimepy-4.0.0/runtimepy/tui/channels/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 A module implementing a channel-environment user interface.
 """
 
 # built-in
-from typing import List as _List
 from typing import Optional as _Optional
 
 try:
     import curses as _curses
 except ModuleNotFoundError:  # pragma: nocover
     _curses = {}  # type: ignore
 
@@ -32,15 +31,15 @@
 
         super().__init__()
 
         self._header: _Optional[CursesWindow] = None
         self._body: _Optional[CursesWindow] = None
 
         self.env = env
-        self.channel_names: _List[str] = []
+        self.channel_names: list[str] = []
         self.value_col: int = 0
 
     @property
     def header(self) -> CursesWindow:
         """Get this interface's header window."""
         assert self._header is not None
         return self._header
```

### Comparing `runtimepy-3.9.0/runtimepy/tui/cursor.py` & `runtimepy-4.0.0/runtimepy/tui/cursor.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.9.0/runtimepy/tui/mixin.py` & `runtimepy-4.0.0/runtimepy/tui/mixin.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.9.0/runtimepy/tui/mock.py` & `runtimepy-4.0.0/runtimepy/tui/mock.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.9.0/runtimepy/tui/task.py` & `runtimepy-4.0.0/runtimepy/tui/task.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.9.0/runtimepy.egg-info/PKG-INFO` & `runtimepy-4.0.0/runtimepy.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runtimepy
-Version: 3.9.0
+Version: 4.0.0
 Summary: A framework for implementing Python services.
 Home-page: https://github.com/vkottler/runtimepy
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -13,43 +13,44 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: svgen>=0.5.0
-Requires-Dist: vcorelib>=3.2.0
 Requires-Dist: websockets
+Requires-Dist: vcorelib>=3.2.2
+Requires-Dist: svgen>=0.6.5
 Provides-Extra: test
 Requires-Dist: pylint; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: black; extra == "test"
 Requires-Dist: ruff; extra == "test"
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: isort; extra == "test"
 Requires-Dist: yamllint; extra == "test"
 Requires-Dist: yambs; extra == "test"
 Requires-Dist: vmklib; extra == "test"
 Requires-Dist: sphinx; extra == "test"
 Requires-Dist: sphinx-book-theme; extra == "test"
 Requires-Dist: pytest-asyncio; extra == "test"
+Requires-Dist: pytest-timeout; extra == "test"
 Requires-Dist: setuptools-wrapper; extra == "test"
 Requires-Dist: types-setuptools; extra == "test"
 Requires-Dist: uvloop; (sys_platform != "win32" and sys_platform != "cygwin") and extra == "test"
 
 <!--
     =====================================
     generator=datazen
     version=3.1.4
-    hash=c7bfaabcb235afbdae1921e1defa2f1a
+    hash=66a0cf61a6081296df95d09b170cf551
     =====================================
 -->
 
-# runtimepy ([3.9.0](https://pypi.org/project/runtimepy/))
+# runtimepy ([4.0.0](https://pypi.org/project/runtimepy/))
 
 [![python](https://img.shields.io/pypi/pyversions/runtimepy.svg)](https://pypi.org/project/runtimepy/)
 ![Build Status](https://github.com/vkottler/runtimepy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/runtimepy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/runtimepy)
 ![PyPI - Status](https://img.shields.io/pypi/status/runtimepy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/runtimepy)
 
@@ -80,15 +81,15 @@
 * `windows-latest`
 
 # Introduction
 
 # Command-line Options
 
 ```
-$ ./venv3.11/bin/runtimepy -h
+$ ./venv3.12/bin/runtimepy -h
 
 usage: runtimepy [-h] [--version] [-v] [-q] [--curses] [--no-uvloop] [-C DIR]
                  {arbiter,server,task,tui,noop} ...
 
 A framework for implementing Python services.
 
 options:
@@ -112,15 +113,15 @@
 ```
 
 ## Sub-command Options
 
 ### `arbiter`
 
 ```
-$ ./venv3.11/bin/runtimepy arbiter -h
+$ ./venv3.12/bin/runtimepy arbiter -h
 
 usage: runtimepy arbiter [-h] [-i] [-w] configs [configs ...]
 
 positional arguments:
   configs               the configuration to load
 
 options:
@@ -132,15 +133,15 @@
                         run last
 
 ```
 
 ### `server`
 
 ```
-$ ./venv3.11/bin/runtimepy server -h
+$ ./venv3.12/bin/runtimepy server -h
 
 usage: runtimepy server [-h] [-i] [-w] [--host HOST] [-p PORT] [-u] [-l]
                         factory [configs ...]
 
 positional arguments:
   factory               name of connection factory to create server for
   configs               the configuration to load
@@ -159,15 +160,15 @@
   -l, --loopback        if true a client of the same connection type is added
 
 ```
 
 ### `task`
 
 ```
-$ ./venv3.11/bin/runtimepy task -h
+$ ./venv3.12/bin/runtimepy task -h
 
 usage: runtimepy task [-h] [-i] [-w] [-r RATE] factory [configs ...]
 
 positional arguments:
   factory               name of task factory to create task with
   configs               the configuration to load
 
@@ -181,15 +182,15 @@
   -r RATE, --rate RATE  rate (in Hz) that the task should run (default: 10)
 
 ```
 
 ### `tui`
 
 ```
-$ ./venv3.11/bin/runtimepy tui -h
+$ ./venv3.12/bin/runtimepy tui -h
 
 usage: runtimepy tui [-h] [-i ITERATIONS] [-r RATE]
 
 options:
   -h, --help            show this help message and exit
   -i ITERATIONS, --iterations ITERATIONS
                         maximum number of program iterations (if greater than
```

### Comparing `runtimepy-3.9.0/runtimepy.egg-info/SOURCES.txt` & `runtimepy-4.0.0/runtimepy.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 runtimepy/channel/__init__.py
 runtimepy/channel/registry.py
 runtimepy/channel/environment/__init__.py
 runtimepy/channel/environment/array.py
 runtimepy/channel/environment/base.py
 runtimepy/channel/environment/create.py
 runtimepy/channel/environment/file.py
+runtimepy/channel/environment/sample.py
 runtimepy/channel/environment/command/__init__.py
 runtimepy/channel/environment/command/parser.py
 runtimepy/channel/environment/command/processor.py
 runtimepy/channel/environment/command/result.py
 runtimepy/channel/event/__init__.py
 runtimepy/channel/event/header.py
 runtimepy/codec/__init__.py
@@ -39,33 +40,60 @@
 runtimepy/commands/__init__.py
 runtimepy/commands/all.py
 runtimepy/commands/arbiter.py
 runtimepy/commands/common.py
 runtimepy/commands/server.py
 runtimepy/commands/task.py
 runtimepy/commands/tui.py
+runtimepy/data/dummy_load.yaml
 runtimepy/data/factories.yaml
 runtimepy/data/favicon.ico
+runtimepy/data/server.yaml
+runtimepy/data/server_base.yaml
+runtimepy/data/server_dev.yaml
+runtimepy/data/css/bootstrap_extra.css
+runtimepy/data/css/main.css
+runtimepy/data/js/DataConnection.js
+runtimepy/data/js/JsonConnection.js
+runtimepy/data/js/audio.js
+runtimepy/data/js/init.js
+runtimepy/data/js/main.js
+runtimepy/data/js/util.js
+runtimepy/data/js/worker.js
+runtimepy/data/js/classes/App.js
+runtimepy/data/js/classes/ChannelTable.js
+runtimepy/data/js/classes/DataConnection.js
+runtimepy/data/js/classes/JsonConnection.js
+runtimepy/data/js/classes/Plot.js
+runtimepy/data/js/classes/PlotManager.js
+runtimepy/data/js/classes/TabFilter.js
+runtimepy/data/js/classes/TabInterface.js
+runtimepy/data/js/classes/WindowHashManager.js
+runtimepy/data/js/classes/WorkerInterface.js
+runtimepy/data/js/tab/env.js
+runtimepy/data/js/tab/sound.js
+runtimepy/data/js/unused/pyodide.js
 runtimepy/data/schemas/BitFields.yaml
 runtimepy/data/schemas/Channel.yaml
 runtimepy/data/schemas/ChannelCommand.yaml
 runtimepy/data/schemas/ChannelRegistry.yaml
 runtimepy/data/schemas/ClientConnectionConfig.yaml
 runtimepy/data/schemas/ConnectionArbiterConfig.yaml
 runtimepy/data/schemas/EnumRegistry.yaml
 runtimepy/data/schemas/FindFile.yaml
 runtimepy/data/schemas/RuntimeEnum.yaml
 runtimepy/data/schemas/ServerConnectionConfig.yaml
+runtimepy/data/schemas/StructConfig.yaml
 runtimepy/data/schemas/TaskConfig.yaml
 runtimepy/data/schemas/has_factory.yaml
 runtimepy/data/schemas/has_name.yaml
 runtimepy/data/schemas/has_request_flag.yaml
 runtimepy/enum/__init__.py
 runtimepy/enum/registry.py
-runtimepy/enum/type.py
+runtimepy/enum/types.py
 runtimepy/metrics/__init__.py
 runtimepy/metrics/channel.py
 runtimepy/metrics/connection.py
 runtimepy/metrics/task.py
 runtimepy/mixins/__init__.py
 runtimepy/mixins/async_command.py
 runtimepy/mixins/enum.py
@@ -78,38 +106,64 @@
 runtimepy/net/connection.py
 runtimepy/net/manager.py
 runtimepy/net/mixin.py
 runtimepy/net/util.py
 runtimepy/net/apps/__init__.py
 runtimepy/net/arbiter/__init__.py
 runtimepy/net/arbiter/base.py
-runtimepy/net/arbiter/config.py
-runtimepy/net/arbiter/imports.py
 runtimepy/net/arbiter/info.py
 runtimepy/net/arbiter/result.py
 runtimepy/net/arbiter/task.py
 runtimepy/net/arbiter/udp.py
 runtimepy/net/arbiter/websocket.py
+runtimepy/net/arbiter/config/__init__.py
+runtimepy/net/arbiter/config/codec.py
+runtimepy/net/arbiter/config/util.py
 runtimepy/net/arbiter/factory/__init__.py
 runtimepy/net/arbiter/factory/connection.py
 runtimepy/net/arbiter/factory/task.py
 runtimepy/net/arbiter/housekeeping/__init__.py
+runtimepy/net/arbiter/imports/__init__.py
+runtimepy/net/arbiter/imports/util.py
+runtimepy/net/arbiter/struct/__init__.py
 runtimepy/net/arbiter/tcp/__init__.py
 runtimepy/net/arbiter/tcp/json.py
 runtimepy/net/factories/__init__.py
 runtimepy/net/http/__init__.py
 runtimepy/net/http/common.py
 runtimepy/net/http/header.py
 runtimepy/net/http/request_target.py
 runtimepy/net/http/response.py
 runtimepy/net/http/state.py
 runtimepy/net/http/version.py
 runtimepy/net/server/__init__.py
 runtimepy/net/server/html.py
 runtimepy/net/server/json.py
+runtimepy/net/server/app/__init__.py
+runtimepy/net/server/app/base.py
+runtimepy/net/server/app/create.py
+runtimepy/net/server/app/elements.py
+runtimepy/net/server/app/files.py
+runtimepy/net/server/app/placeholder.py
+runtimepy/net/server/app/pyodide.py
+runtimepy/net/server/app/sound.py
+runtimepy/net/server/app/tab.py
+runtimepy/net/server/app/bootstrap/__init__.py
+runtimepy/net/server/app/bootstrap/elements.py
+runtimepy/net/server/app/bootstrap/tabs.py
+runtimepy/net/server/app/env/__init__.py
+runtimepy/net/server/app/env/modal.py
+runtimepy/net/server/app/env/widgets.py
+runtimepy/net/server/app/env/tab/__init__.py
+runtimepy/net/server/app/env/tab/base.py
+runtimepy/net/server/app/env/tab/html.py
+runtimepy/net/server/app/env/tab/logger.py
+runtimepy/net/server/app/env/tab/message.py
+runtimepy/net/server/struct/__init__.py
+runtimepy/net/server/websocket/__init__.py
 runtimepy/net/stream/__init__.py
 runtimepy/net/stream/base.py
 runtimepy/net/stream/string.py
 runtimepy/net/stream/json/__init__.py
 runtimepy/net/stream/json/base.py
 runtimepy/net/stream/json/handlers.py
 runtimepy/net/stream/json/types.py
@@ -139,26 +193,28 @@
 runtimepy/primitives/field/fields.py
 runtimepy/primitives/field/manager/__init__.py
 runtimepy/primitives/field/manager/base.py
 runtimepy/primitives/serializable/__init__.py
 runtimepy/primitives/serializable/base.py
 runtimepy/primitives/serializable/fixed.py
 runtimepy/primitives/serializable/prefixed.py
-runtimepy/primitives/type/__init__.py
-runtimepy/primitives/type/base.py
-runtimepy/primitives/type/bool.py
-runtimepy/primitives/type/bounds.py
-runtimepy/primitives/type/float.py
-runtimepy/primitives/type/int.py
+runtimepy/primitives/types/__init__.py
+runtimepy/primitives/types/base.py
+runtimepy/primitives/types/bool.py
+runtimepy/primitives/types/bounds.py
+runtimepy/primitives/types/float.py
+runtimepy/primitives/types/int.py
 runtimepy/registry/__init__.py
 runtimepy/registry/bool.py
 runtimepy/registry/item.py
 runtimepy/registry/name.py
+runtimepy/struct/__init__.py
 runtimepy/task/__init__.py
 runtimepy/task/asynchronous.py
+runtimepy/task/sample.py
 runtimepy/task/basic/__init__.py
 runtimepy/task/basic/manager.py
 runtimepy/task/basic/periodic.py
 runtimepy/task/trig/__init__.py
 runtimepy/telemetry/__init__.py
 runtimepy/tui/__init__.py
 runtimepy/tui/cursor.py
```

### Comparing `runtimepy-3.9.0/setup.py` & `runtimepy-4.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.9.0/tests/test_entry.py` & `runtimepy-4.0.0/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.9.0/tests/test_mapping.py` & `runtimepy-4.0.0/tests/test_mapping.py`

 * *Files identical despite different names*

