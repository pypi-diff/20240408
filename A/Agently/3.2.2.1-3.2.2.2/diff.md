# Comparing `tmp/Agently-3.2.2.1.tar.gz` & `tmp/Agently-3.2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Agently-3.2.2.1.tar", last modified: Sun Apr  7 01:34:49 2024, max compression
+gzip compressed data, was "Agently-3.2.2.2.tar", last modified: Sun Apr  7 14:01:41 2024, max compression
```

## Comparing `Agently-3.2.2.1.tar` & `Agently-3.2.2.2.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-07 01:34:49.625518 Agently-3.2.2.1/
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-07 01:34:49.602983 Agently-3.2.2.1/Agently/
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-07 01:34:49.604312 Agently-3.2.2.1/Agently/Agent/
--rw-r--r--   0 moxin      (501) staff       (20)    14078 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/Agent/Agent.py
--rw-r--r--   0 moxin      (501) staff       (20)     2259 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/Agent/AgentFactory.py
--rw-r--r--   0 moxin      (501) staff       (20)       38 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/Agent/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-07 01:34:49.605373 Agently-3.2.2.1/Agently/Facility/
--rw-r--r--   0 moxin      (501) staff       (20)     1819 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/Facility/FacilityManager.py
--rw-r--r--   0 moxin      (501) staff       (20)       44 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/Facility/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-07 01:34:49.605823 Agently-3.2.2.1/Agently/Request/
--rw-r--r--   0 moxin      (501) staff       (20)     9783 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/Request/Request.py
--rw-r--r--   0 moxin      (501) staff       (20)       28 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/Request/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-07 01:34:49.606319 Agently-3.2.2.1/Agently/WebSocket/
--rw-r--r--   0 moxin      (501) staff       (20)     9550 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/WebSocket/WebSocket.py
--rw-r--r--   0 moxin      (501) staff       (20)       55 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/WebSocket/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-07 01:34:49.608870 Agently-3.2.2.1/Agently/Workflow/
--rw-r--r--   0 moxin      (501) staff       (20)     7650 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/Workflow/Chunk.py
--rw-r--r--   0 moxin      (501) staff       (20)    16640 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/Workflow/MainExecutor.py
--rw-r--r--   0 moxin      (501) staff       (20)     6775 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/Workflow/Schema.py
--rw-r--r--   0 moxin      (501) staff       (20)     3165 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/Workflow/Workflow.py
--rw-r--r--   0 moxin      (501) staff       (20)       57 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/Workflow/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-07 01:34:49.609407 Agently-3.2.2.1/Agently/Workflow/executors/
--rw-r--r--   0 moxin      (501) staff       (20)       67 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/Workflow/executors/StartExecutor.py
--rw-r--r--   0 moxin      (501) staff       (20)        0 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/Workflow/executors/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)      245 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/Workflow/executors/install.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-07 01:34:49.610400 Agently-3.2.2.1/Agently/Workflow/lib/
--rw-r--r--   0 moxin      (501) staff       (20)     1470 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/Workflow/lib/BreakingHub.py
--rw-r--r--   0 moxin      (501) staff       (20)      656 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/Workflow/lib/ChunkExecutorABC.py
--rw-r--r--   0 moxin      (501) staff       (20)      426 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/Workflow/lib/ChunkExecutorManager.py
--rw-r--r--   0 moxin      (501) staff       (20)      483 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/Workflow/lib/Store.py
--rw-r--r--   0 moxin      (501) staff       (20)        0 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/Workflow/lib/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)      515 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/Workflow/lib/constants.py
--rw-r--r--   0 moxin      (501) staff       (20)     2058 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/Workflow/lib/painter.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-07 01:34:49.611386 Agently-3.2.2.1/Agently/Workflow/utils/
--rw-r--r--   0 moxin      (501) staff       (20)        0 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/Workflow/utils/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)     4599 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/Workflow/utils/exec_tree.py
--rw-r--r--   0 moxin      (501) staff       (20)     1411 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/Workflow/utils/find.py
--rw-r--r--   0 moxin      (501) staff       (20)      613 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/Workflow/utils/logger.py
--rw-r--r--   0 moxin      (501) staff       (20)      892 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/Workflow/utils/runtime_supports.py
--rw-r--r--   0 moxin      (501) staff       (20)      242 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/Workflow/utils/verify.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-07 01:34:49.611636 Agently-3.2.2.1/Agently/Workflow/yamlflow/
--rw-r--r--   0 moxin      (501) staff       (20)       63 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/Workflow/yamlflow/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-07 01:34:49.612327 Agently-3.2.2.1/Agently/Workflow/yamlflow/preset_chunks/
--rw-r--r--   0 moxin      (501) staff       (20)      500 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/Workflow/yamlflow/preset_chunks/Print.py
--rw-r--r--   0 moxin      (501) staff       (20)      108 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/Workflow/yamlflow/preset_chunks/Start.py
--rw-r--r--   0 moxin      (501) staff       (20)      289 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/Workflow/yamlflow/preset_chunks/UserInput.py
--rw-r--r--   0 moxin      (501) staff       (20)      767 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/Workflow/yamlflow/preset_chunks/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)     5710 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/Workflow/yamlflow/yamlflow.py
--rw-r--r--   0 moxin      (501) staff       (20)      527 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)      515 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/_global.py
--rw-r--r--   0 moxin      (501) staff       (20)      149 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/global_plugin_manager.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-07 01:34:49.612453 Agently-3.2.2.1/Agently/plugins/
--rw-r--r--   0 moxin      (501) staff       (20)     4920 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/plugins/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-07 01:34:49.615603 Agently-3.2.2.1/Agently/plugins/agent_component/
--rw-r--r--   0 moxin      (501) staff       (20)     2870 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/plugins/agent_component/Decorator.py
--rw-r--r--   0 moxin      (501) staff       (20)     1384 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/plugins/agent_component/EventListener.py
--rw-r--r--   0 moxin      (501) staff       (20)     5290 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/plugins/agent_component/OpenAIAssistant.py
--rw-r--r--   0 moxin      (501) staff       (20)      785 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/plugins/agent_component/ReplyReformer.py
--rw-r--r--   0 moxin      (501) staff       (20)     3050 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/plugins/agent_component/Role.py
--rw-r--r--   0 moxin      (501) staff       (20)     4075 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/plugins/agent_component/Search.py
--rw-r--r--   0 moxin      (501) staff       (20)     9781 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/plugins/agent_component/Segment.py
--rw-r--r--   0 moxin      (501) staff       (20)     8287 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/plugins/agent_component/Session.py
--rw-r--r--   0 moxin      (501) staff       (20)     3508 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/plugins/agent_component/Status.py
--rw-r--r--   0 moxin      (501) staff       (20)     8861 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/plugins/agent_component/Tool.py
--rw-r--r--   0 moxin      (501) staff       (20)     2977 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/plugins/agent_component/UserInfo.py
--rw-r--r--   0 moxin      (501) staff       (20)     3062 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/plugins/agent_component/YAMLLoader.py
--rw-r--r--   0 moxin      (501) staff       (20)     2220 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/plugins/agent_component/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)      505 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/plugins/agent_component/config.ini
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-07 01:34:49.615862 Agently-3.2.2.1/Agently/plugins/agent_component/utils/
--rw-r--r--   0 moxin      (501) staff       (20)      588 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/plugins/agent_component/utils/ComponentABC.py
--rw-r--r--   0 moxin      (501) staff       (20)       38 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/plugins/agent_component/utils/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-07 01:34:49.616751 Agently-3.2.2.1/Agently/plugins/facility/
--rw-r--r--   0 moxin      (501) staff       (20)     4633 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/plugins/facility/Embedding.py
--rw-r--r--   0 moxin      (501) staff       (20)     1874 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/plugins/facility/RoleManager.py
--rw-r--r--   0 moxin      (501) staff       (20)     1216 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/plugins/facility/StatusManager.py
--rw-r--r--   0 moxin      (501) staff       (20)     2120 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/plugins/facility/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)       85 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/plugins/facility/config.ini
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-07 01:34:49.617085 Agently-3.2.2.1/Agently/plugins/facility/utils/
--rw-r--r--   0 moxin      (501) staff       (20)      266 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/plugins/facility/utils/FacilityABC.py
--rw-r--r--   0 moxin      (501) staff       (20)       36 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/plugins/facility/utils/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-07 01:34:49.619378 Agently-3.2.2.1/Agently/plugins/request/
--rw-r--r--   0 moxin      (501) staff       (20)     7323 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/plugins/request/Claude.py
--rw-r--r--   0 moxin      (501) staff       (20)    10303 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/plugins/request/ERNIE.py
--rw-r--r--   0 moxin      (501) staff       (20)     7372 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/plugins/request/Google.py
--rw-r--r--   0 moxin      (501) staff       (20)     7769 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/plugins/request/Kimi.py
--rw-r--r--   0 moxin      (501) staff       (20)    12270 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/plugins/request/MiniMax.py
--rw-r--r--   0 moxin      (501) staff       (20)    15598 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/plugins/request/OAIClient.py
--rw-r--r--   0 moxin      (501) staff       (20)    11525 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/plugins/request/OpenAI.py
--rw-r--r--   0 moxin      (501) staff       (20)    12624 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/plugins/request/ZhipuAI.py
--rw-r--r--   0 moxin      (501) staff       (20)     2120 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/plugins/request/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)      139 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/plugins/request/config.ini
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-07 01:34:49.620068 Agently-3.2.2.1/Agently/plugins/request/utils/
--rw-r--r--   0 moxin      (501) staff       (20)     5307 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/plugins/request/utils/RequestABC.py
--rw-r--r--   0 moxin      (501) staff       (20)      118 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/plugins/request/utils/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)     4330 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/plugins/request/utils/transform.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-07 01:34:49.620521 Agently-3.2.2.1/Agently/plugins/storage/
--rw-r--r--   0 moxin      (501) staff       (20)     3160 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/plugins/storage/FileStorage.py
--rw-r--r--   0 moxin      (501) staff       (20)     2120 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/plugins/storage/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)      131 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/plugins/storage/config.ini
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-07 01:34:49.620764 Agently-3.2.2.1/Agently/plugins/storage/utils/
--rw-r--r--   0 moxin      (501) staff       (20)      745 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/plugins/storage/utils/StorageABC.py
--rw-r--r--   0 moxin      (501) staff       (20)       34 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/plugins/storage/utils/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-07 01:34:49.621535 Agently-3.2.2.1/Agently/plugins/tool/
--rw-r--r--   0 moxin      (501) staff       (20)     1828 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/plugins/tool/Code.py
--rw-r--r--   0 moxin      (501) staff       (20)     6912 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/plugins/tool/Web.py
--rw-r--r--   0 moxin      (501) staff       (20)     2120 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/plugins/tool/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)      104 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/plugins/tool/config.ini
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-07 01:34:49.621946 Agently-3.2.2.1/Agently/plugins/tool/utils/
--rw-r--r--   0 moxin      (501) staff       (20)      443 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/plugins/tool/utils/ToolABC.py
--rw-r--r--   0 moxin      (501) staff       (20)       28 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/plugins/tool/utils/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)      168 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/requirements.txt
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-07 01:34:49.624919 Agently-3.2.2.1/Agently/utils/
--rw-r--r--   0 moxin      (501) staff       (20)     2896 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/utils/AliasManager.py
--rw-r--r--   0 moxin      (501) staff       (20)     6706 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/utils/DataOps.py
--rw-r--r--   0 moxin      (501) staff       (20)      323 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/utils/IdGenerator.py
--rw-r--r--   0 moxin      (501) staff       (20)     2282 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/utils/PluginManager.py
--rw-r--r--   0 moxin      (501) staff       (20)     2418 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/utils/RuntimeCtx.py
--rw-r--r--   0 moxin      (501) staff       (20)     1934 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/utils/StorageDelegate.py
--rw-r--r--   0 moxin      (501) staff       (20)     4758 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/utils/ToolManager.py
--rw-r--r--   0 moxin      (501) staff       (20)      491 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/utils/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)     1928 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/utils/check_version.py
--rw-r--r--   0 moxin      (501) staff       (20)     2773 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/utils/load_json.py
--rw-r--r--   0 moxin      (501) staff       (20)     4328 2024-04-07 01:29:15.000000 Agently-3.2.2.1/Agently/utils/transform.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-07 01:34:49.625122 Agently-3.2.2.1/Agently.egg-info/
--rw-r--r--   0 moxin      (501) staff       (20)      819 2024-04-07 01:34:49.000000 Agently-3.2.2.1/Agently.egg-info/PKG-INFO
--rw-r--r--   0 moxin      (501) staff       (20)     3745 2024-04-07 01:34:49.000000 Agently-3.2.2.1/Agently.egg-info/SOURCES.txt
--rw-r--r--   0 moxin      (501) staff       (20)        1 2024-04-07 01:34:49.000000 Agently-3.2.2.1/Agently.egg-info/dependency_links.txt
--rw-r--r--   0 moxin      (501) staff       (20)      118 2024-04-07 01:34:49.000000 Agently-3.2.2.1/Agently.egg-info/requires.txt
--rw-r--r--   0 moxin      (501) staff       (20)        8 2024-04-07 01:34:49.000000 Agently-3.2.2.1/Agently.egg-info/top_level.txt
--rw-r--r--   0 moxin      (501) staff       (20)      819 2024-04-07 01:34:49.625335 Agently-3.2.2.1/PKG-INFO
--rw-r--r--   0 moxin      (501) staff       (20)       38 2024-04-07 01:34:49.625552 Agently-3.2.2.1/setup.cfg
--rw-------   0 moxin      (501) staff       (20)      974 2024-04-07 00:47:49.000000 Agently-3.2.2.1/setup.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-07 14:01:41.930056 Agently-3.2.2.2/
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-07 14:01:41.904799 Agently-3.2.2.2/Agently/
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-07 14:01:41.906916 Agently-3.2.2.2/Agently/Agent/
+-rw-r--r--   0 moxin      (501) staff       (20)    14078 2024-04-07 13:56:24.000000 Agently-3.2.2.2/Agently/Agent/Agent.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2259 2024-04-07 13:56:24.000000 Agently-3.2.2.2/Agently/Agent/AgentFactory.py
+-rw-r--r--   0 moxin      (501) staff       (20)       38 2024-04-07 13:56:24.000000 Agently-3.2.2.2/Agently/Agent/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-07 14:01:41.907351 Agently-3.2.2.2/Agently/Facility/
+-rw-r--r--   0 moxin      (501) staff       (20)     1819 2024-04-07 13:56:24.000000 Agently-3.2.2.2/Agently/Facility/FacilityManager.py
+-rw-r--r--   0 moxin      (501) staff       (20)       44 2024-04-07 13:56:24.000000 Agently-3.2.2.2/Agently/Facility/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-07 14:01:41.908546 Agently-3.2.2.2/Agently/Request/
+-rw-r--r--   0 moxin      (501) staff       (20)     9783 2024-04-07 13:56:24.000000 Agently-3.2.2.2/Agently/Request/Request.py
+-rw-r--r--   0 moxin      (501) staff       (20)       28 2024-04-07 13:56:24.000000 Agently-3.2.2.2/Agently/Request/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-07 14:01:41.910687 Agently-3.2.2.2/Agently/WebSocket/
+-rw-r--r--   0 moxin      (501) staff       (20)     9550 2024-04-07 13:56:24.000000 Agently-3.2.2.2/Agently/WebSocket/WebSocket.py
+-rw-r--r--   0 moxin      (501) staff       (20)       55 2024-04-07 13:56:24.000000 Agently-3.2.2.2/Agently/WebSocket/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-07 14:01:41.912564 Agently-3.2.2.2/Agently/Workflow/
+-rw-r--r--   0 moxin      (501) staff       (20)     7650 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/Workflow/Chunk.py
+-rw-r--r--   0 moxin      (501) staff       (20)    16640 2024-04-07 13:56:24.000000 Agently-3.2.2.2/Agently/Workflow/MainExecutor.py
+-rw-r--r--   0 moxin      (501) staff       (20)     6775 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/Workflow/Schema.py
+-rw-r--r--   0 moxin      (501) staff       (20)     3165 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/Workflow/Workflow.py
+-rw-r--r--   0 moxin      (501) staff       (20)       57 2024-04-07 13:56:24.000000 Agently-3.2.2.2/Agently/Workflow/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-07 14:01:41.913179 Agently-3.2.2.2/Agently/Workflow/executors/
+-rw-r--r--   0 moxin      (501) staff       (20)       67 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/Workflow/executors/StartExecutor.py
+-rw-r--r--   0 moxin      (501) staff       (20)        0 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/Workflow/executors/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      245 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/Workflow/executors/install.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-07 14:01:41.914911 Agently-3.2.2.2/Agently/Workflow/lib/
+-rw-r--r--   0 moxin      (501) staff       (20)     1470 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/Workflow/lib/BreakingHub.py
+-rw-r--r--   0 moxin      (501) staff       (20)      656 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/Workflow/lib/ChunkExecutorABC.py
+-rw-r--r--   0 moxin      (501) staff       (20)      426 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/Workflow/lib/ChunkExecutorManager.py
+-rw-r--r--   0 moxin      (501) staff       (20)      483 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/Workflow/lib/Store.py
+-rw-r--r--   0 moxin      (501) staff       (20)        0 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/Workflow/lib/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      515 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/Workflow/lib/constants.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2058 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/Workflow/lib/painter.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-07 14:01:41.915908 Agently-3.2.2.2/Agently/Workflow/utils/
+-rw-r--r--   0 moxin      (501) staff       (20)        0 2024-04-07 13:56:24.000000 Agently-3.2.2.2/Agently/Workflow/utils/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)     4599 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/Workflow/utils/exec_tree.py
+-rw-r--r--   0 moxin      (501) staff       (20)     1411 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/Workflow/utils/find.py
+-rw-r--r--   0 moxin      (501) staff       (20)      613 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/Workflow/utils/logger.py
+-rw-r--r--   0 moxin      (501) staff       (20)      892 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/Workflow/utils/runtime_supports.py
+-rw-r--r--   0 moxin      (501) staff       (20)      242 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/Workflow/utils/verify.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-07 14:01:41.916244 Agently-3.2.2.2/Agently/Workflow/yamlflow/
+-rw-r--r--   0 moxin      (501) staff       (20)       63 2024-04-07 13:56:24.000000 Agently-3.2.2.2/Agently/Workflow/yamlflow/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-07 14:01:41.917428 Agently-3.2.2.2/Agently/Workflow/yamlflow/preset_chunks/
+-rw-r--r--   0 moxin      (501) staff       (20)      500 2024-04-07 13:56:24.000000 Agently-3.2.2.2/Agently/Workflow/yamlflow/preset_chunks/Print.py
+-rw-r--r--   0 moxin      (501) staff       (20)      108 2024-04-07 13:56:24.000000 Agently-3.2.2.2/Agently/Workflow/yamlflow/preset_chunks/Start.py
+-rw-r--r--   0 moxin      (501) staff       (20)      289 2024-04-07 13:56:24.000000 Agently-3.2.2.2/Agently/Workflow/yamlflow/preset_chunks/UserInput.py
+-rw-r--r--   0 moxin      (501) staff       (20)      767 2024-04-07 13:56:24.000000 Agently-3.2.2.2/Agently/Workflow/yamlflow/preset_chunks/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)     5710 2024-04-07 13:56:24.000000 Agently-3.2.2.2/Agently/Workflow/yamlflow/yamlflow.py
+-rw-r--r--   0 moxin      (501) staff       (20)      527 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      515 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/_global.py
+-rw-r--r--   0 moxin      (501) staff       (20)      149 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/global_plugin_manager.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-07 14:01:41.917672 Agently-3.2.2.2/Agently/plugins/
+-rw-r--r--   0 moxin      (501) staff       (20)     4920 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/plugins/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-07 14:01:41.920939 Agently-3.2.2.2/Agently/plugins/agent_component/
+-rw-r--r--   0 moxin      (501) staff       (20)     2870 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/plugins/agent_component/Decorator.py
+-rw-r--r--   0 moxin      (501) staff       (20)     1384 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/plugins/agent_component/EventListener.py
+-rw-r--r--   0 moxin      (501) staff       (20)     5290 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/plugins/agent_component/OpenAIAssistant.py
+-rw-r--r--   0 moxin      (501) staff       (20)      785 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/plugins/agent_component/ReplyReformer.py
+-rw-r--r--   0 moxin      (501) staff       (20)     3050 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/plugins/agent_component/Role.py
+-rw-r--r--   0 moxin      (501) staff       (20)     4075 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/plugins/agent_component/Search.py
+-rw-r--r--   0 moxin      (501) staff       (20)     9781 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/plugins/agent_component/Segment.py
+-rw-r--r--   0 moxin      (501) staff       (20)     8287 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/plugins/agent_component/Session.py
+-rw-r--r--   0 moxin      (501) staff       (20)     3508 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/plugins/agent_component/Status.py
+-rw-r--r--   0 moxin      (501) staff       (20)     8861 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/plugins/agent_component/Tool.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2977 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/plugins/agent_component/UserInfo.py
+-rw-r--r--   0 moxin      (501) staff       (20)     3062 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/plugins/agent_component/YAMLLoader.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2220 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/plugins/agent_component/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      505 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/plugins/agent_component/config.ini
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-07 14:01:41.921205 Agently-3.2.2.2/Agently/plugins/agent_component/utils/
+-rw-r--r--   0 moxin      (501) staff       (20)      588 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/plugins/agent_component/utils/ComponentABC.py
+-rw-r--r--   0 moxin      (501) staff       (20)       38 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/plugins/agent_component/utils/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-07 14:01:41.922076 Agently-3.2.2.2/Agently/plugins/facility/
+-rw-r--r--   0 moxin      (501) staff       (20)     4633 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/plugins/facility/Embedding.py
+-rw-r--r--   0 moxin      (501) staff       (20)     1874 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/plugins/facility/RoleManager.py
+-rw-r--r--   0 moxin      (501) staff       (20)     1216 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/plugins/facility/StatusManager.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2120 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/plugins/facility/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)       85 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/plugins/facility/config.ini
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-07 14:01:41.922468 Agently-3.2.2.2/Agently/plugins/facility/utils/
+-rw-r--r--   0 moxin      (501) staff       (20)      266 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/plugins/facility/utils/FacilityABC.py
+-rw-r--r--   0 moxin      (501) staff       (20)       36 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/plugins/facility/utils/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-07 14:01:41.924839 Agently-3.2.2.2/Agently/plugins/request/
+-rw-r--r--   0 moxin      (501) staff       (20)     7323 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/plugins/request/Claude.py
+-rw-r--r--   0 moxin      (501) staff       (20)    10303 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/plugins/request/ERNIE.py
+-rw-r--r--   0 moxin      (501) staff       (20)     7372 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/plugins/request/Google.py
+-rw-r--r--   0 moxin      (501) staff       (20)     7769 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/plugins/request/Kimi.py
+-rw-r--r--   0 moxin      (501) staff       (20)    12270 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/plugins/request/MiniMax.py
+-rw-r--r--   0 moxin      (501) staff       (20)    15605 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/plugins/request/OAIClient.py
+-rw-r--r--   0 moxin      (501) staff       (20)    11446 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/plugins/request/OpenAI.py
+-rw-r--r--   0 moxin      (501) staff       (20)    12624 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/plugins/request/ZhipuAI.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2120 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/plugins/request/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      139 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/plugins/request/config.ini
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-07 14:01:41.925396 Agently-3.2.2.2/Agently/plugins/request/utils/
+-rw-r--r--   0 moxin      (501) staff       (20)     5307 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/plugins/request/utils/RequestABC.py
+-rw-r--r--   0 moxin      (501) staff       (20)      118 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/plugins/request/utils/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)     4330 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/plugins/request/utils/transform.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-07 14:01:41.925905 Agently-3.2.2.2/Agently/plugins/storage/
+-rw-r--r--   0 moxin      (501) staff       (20)     3160 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/plugins/storage/FileStorage.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2120 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/plugins/storage/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      131 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/plugins/storage/config.ini
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-07 14:01:41.926188 Agently-3.2.2.2/Agently/plugins/storage/utils/
+-rw-r--r--   0 moxin      (501) staff       (20)      745 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/plugins/storage/utils/StorageABC.py
+-rw-r--r--   0 moxin      (501) staff       (20)       34 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/plugins/storage/utils/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-07 14:01:41.926871 Agently-3.2.2.2/Agently/plugins/tool/
+-rw-r--r--   0 moxin      (501) staff       (20)     1828 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/plugins/tool/Code.py
+-rw-r--r--   0 moxin      (501) staff       (20)     6912 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/plugins/tool/Web.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2120 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/plugins/tool/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      104 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/plugins/tool/config.ini
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-07 14:01:41.927279 Agently-3.2.2.2/Agently/plugins/tool/utils/
+-rw-r--r--   0 moxin      (501) staff       (20)      443 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/plugins/tool/utils/ToolABC.py
+-rw-r--r--   0 moxin      (501) staff       (20)       28 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/plugins/tool/utils/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      168 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/requirements.txt
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-07 14:01:41.929394 Agently-3.2.2.2/Agently/utils/
+-rw-r--r--   0 moxin      (501) staff       (20)     2896 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/utils/AliasManager.py
+-rw-r--r--   0 moxin      (501) staff       (20)     6706 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/utils/DataOps.py
+-rw-r--r--   0 moxin      (501) staff       (20)      323 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/utils/IdGenerator.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2282 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/utils/PluginManager.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2418 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/utils/RuntimeCtx.py
+-rw-r--r--   0 moxin      (501) staff       (20)     1934 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/utils/StorageDelegate.py
+-rw-r--r--   0 moxin      (501) staff       (20)     4758 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/utils/ToolManager.py
+-rw-r--r--   0 moxin      (501) staff       (20)      491 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/utils/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)     1928 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/utils/check_version.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2773 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/utils/load_json.py
+-rw-r--r--   0 moxin      (501) staff       (20)     4328 2024-04-07 13:56:25.000000 Agently-3.2.2.2/Agently/utils/transform.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-07 14:01:41.929637 Agently-3.2.2.2/Agently.egg-info/
+-rw-r--r--   0 moxin      (501) staff       (20)      819 2024-04-07 14:01:41.000000 Agently-3.2.2.2/Agently.egg-info/PKG-INFO
+-rw-r--r--   0 moxin      (501) staff       (20)     3745 2024-04-07 14:01:41.000000 Agently-3.2.2.2/Agently.egg-info/SOURCES.txt
+-rw-r--r--   0 moxin      (501) staff       (20)        1 2024-04-07 14:01:41.000000 Agently-3.2.2.2/Agently.egg-info/dependency_links.txt
+-rw-r--r--   0 moxin      (501) staff       (20)      118 2024-04-07 14:01:41.000000 Agently-3.2.2.2/Agently.egg-info/requires.txt
+-rw-r--r--   0 moxin      (501) staff       (20)        8 2024-04-07 14:01:41.000000 Agently-3.2.2.2/Agently.egg-info/top_level.txt
+-rw-r--r--   0 moxin      (501) staff       (20)      819 2024-04-07 14:01:41.929861 Agently-3.2.2.2/PKG-INFO
+-rw-r--r--   0 moxin      (501) staff       (20)       38 2024-04-07 14:01:41.930094 Agently-3.2.2.2/setup.cfg
+-rw-------   0 moxin      (501) staff       (20)      974 2024-04-07 14:01:37.000000 Agently-3.2.2.2/setup.py
```

### Comparing `Agently-3.2.2.1/Agently/Agent/Agent.py` & `Agently-3.2.2.2/Agently/Agent/Agent.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/Agent/AgentFactory.py` & `Agently-3.2.2.2/Agently/Agent/AgentFactory.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/Facility/FacilityManager.py` & `Agently-3.2.2.2/Agently/Facility/FacilityManager.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/Request/Request.py` & `Agently-3.2.2.2/Agently/Request/Request.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/WebSocket/WebSocket.py` & `Agently-3.2.2.2/Agently/WebSocket/WebSocket.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/Workflow/Chunk.py` & `Agently-3.2.2.2/Agently/Workflow/Chunk.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/Workflow/MainExecutor.py` & `Agently-3.2.2.2/Agently/Workflow/MainExecutor.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/Workflow/Schema.py` & `Agently-3.2.2.2/Agently/Workflow/Schema.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/Workflow/Workflow.py` & `Agently-3.2.2.2/Agently/Workflow/Workflow.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/Workflow/lib/BreakingHub.py` & `Agently-3.2.2.2/Agently/Workflow/lib/BreakingHub.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/Workflow/lib/ChunkExecutorABC.py` & `Agently-3.2.2.2/Agently/Workflow/lib/ChunkExecutorABC.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/Workflow/lib/constants.py` & `Agently-3.2.2.2/Agently/Workflow/lib/constants.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/Workflow/lib/painter.py` & `Agently-3.2.2.2/Agently/Workflow/lib/painter.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/Workflow/utils/exec_tree.py` & `Agently-3.2.2.2/Agently/Workflow/utils/exec_tree.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/Workflow/utils/find.py` & `Agently-3.2.2.2/Agently/Workflow/utils/find.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/Workflow/utils/logger.py` & `Agently-3.2.2.2/Agently/Workflow/utils/logger.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/Workflow/utils/runtime_supports.py` & `Agently-3.2.2.2/Agently/Workflow/utils/runtime_supports.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/Workflow/yamlflow/preset_chunks/__init__.py` & `Agently-3.2.2.2/Agently/Workflow/yamlflow/preset_chunks/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/Workflow/yamlflow/yamlflow.py` & `Agently-3.2.2.2/Agently/Workflow/yamlflow/yamlflow.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/__init__.py` & `Agently-3.2.2.2/Agently/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/_global.py` & `Agently-3.2.2.2/Agently/_global.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/plugins/__init__.py` & `Agently-3.2.2.2/Agently/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/plugins/agent_component/Decorator.py` & `Agently-3.2.2.2/Agently/plugins/agent_component/Decorator.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/plugins/agent_component/EventListener.py` & `Agently-3.2.2.2/Agently/plugins/agent_component/EventListener.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/plugins/agent_component/OpenAIAssistant.py` & `Agently-3.2.2.2/Agently/plugins/agent_component/OpenAIAssistant.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/plugins/agent_component/ReplyReformer.py` & `Agently-3.2.2.2/Agently/plugins/agent_component/ReplyReformer.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/plugins/agent_component/Role.py` & `Agently-3.2.2.2/Agently/plugins/agent_component/Role.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/plugins/agent_component/Search.py` & `Agently-3.2.2.2/Agently/plugins/agent_component/Search.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/plugins/agent_component/Segment.py` & `Agently-3.2.2.2/Agently/plugins/agent_component/Segment.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/plugins/agent_component/Session.py` & `Agently-3.2.2.2/Agently/plugins/agent_component/Session.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/plugins/agent_component/Status.py` & `Agently-3.2.2.2/Agently/plugins/agent_component/Status.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/plugins/agent_component/Tool.py` & `Agently-3.2.2.2/Agently/plugins/agent_component/Tool.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/plugins/agent_component/UserInfo.py` & `Agently-3.2.2.2/Agently/plugins/agent_component/UserInfo.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/plugins/agent_component/YAMLLoader.py` & `Agently-3.2.2.2/Agently/plugins/agent_component/YAMLLoader.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/plugins/agent_component/__init__.py` & `Agently-3.2.2.2/Agently/plugins/agent_component/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/plugins/agent_component/utils/ComponentABC.py` & `Agently-3.2.2.2/Agently/plugins/agent_component/utils/ComponentABC.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/plugins/facility/Embedding.py` & `Agently-3.2.2.2/Agently/plugins/facility/Embedding.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/plugins/facility/RoleManager.py` & `Agently-3.2.2.2/Agently/plugins/facility/RoleManager.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/plugins/facility/StatusManager.py` & `Agently-3.2.2.2/Agently/plugins/facility/StatusManager.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/plugins/facility/__init__.py` & `Agently-3.2.2.2/Agently/plugins/facility/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/plugins/request/Claude.py` & `Agently-3.2.2.2/Agently/plugins/request/Claude.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/plugins/request/ERNIE.py` & `Agently-3.2.2.2/Agently/plugins/request/ERNIE.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/plugins/request/Google.py` & `Agently-3.2.2.2/Agently/plugins/request/Google.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/plugins/request/Kimi.py` & `Agently-3.2.2.2/Agently/plugins/request/Kimi.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/plugins/request/MiniMax.py` & `Agently-3.2.2.2/Agently/plugins/request/MiniMax.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/plugins/request/OAIClient.py` & `Agently-3.2.2.2/Agently/plugins/request/OAIClient.py`

 * *Files 0% similar despite different names*

```diff
@@ -231,17 +231,17 @@
 
     async def request_model(self, request_data: dict):
         # create client
         client_params = {}
         base_url = self.model_settings.get_trace_back("url")
         if base_url:
             client_params.update({ "base_url": base_url })
-        proxy = self.model_settings.get_trace_back("proxy")
+        proxy = self.request.settings.get_trace_back("proxy")
         if proxy:
-            client_params.update({ "http_client": httpx.Client( proxies = proxy ) })
+            client_params.update({ "http_client": httpx.AsyncClient( proxies = proxy ) })
         api_key = self.model_settings.get_trace_back("auth.api_key")
         if api_key:
             client_params.update({ "api_key": api_key })
         else:
             client_params.update({ "api_key": "None" })
         client = OpenAIClient(**client_params)
         # request
```

### Comparing `Agently-3.2.2.1/Agently/plugins/request/OpenAI.py` & `Agently-3.2.2.2/Agently/plugins/request/OpenAI.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     def _create_client(self):
         client_params = {}
         base_url = self.model_settings.get_trace_back("url")
         if base_url:
             client_params.update({ "base_url": base_url })
         proxy = self.request.settings.get_trace_back("proxy")
         if proxy:
-            client_params.update({ "http_client": httpx.Client( proxies = proxy ) })
+            client_params.update({ "http_client": httpx.AsyncClient( proxies = proxy ) })
         api_key = self.model_settings.get_trace_back("auth.api_key")
         if api_key:
             client_params.update({ "api_key": api_key })
         else:
             raise Exception("[Request] OpenAI require api_key. use .set_auth({ 'api_key': '<Your-API-Key>' }) to set it.")
         client = OpenAIClient(**client_params)
         return client
@@ -108,24 +108,24 @@
             assistant_id = self.model_settings.get_trace_back("assistant_id")
             if not assistant_id:
                 raise Exception("[Request] OpenAI require 'assistant_id' when 'use_assistant' is True. Use agent.OpenAIAssistant.update() to create an assistant if you don't have one.")
             else:
                 self.assistant_id = assistant_id
             options = self.model_settings.get_trace_back("options", {})
             if "model" not in options:
-                options.update({ "model": "gpt-3.5-turbo-1106" })
+                options.update({ "model": "gpt-3.5-turbo" })
             return {
                 "stream": True,
                 "messages": self.construct_request_messages(),
                 "options": options,
             }
         elif self.request_type == "chat":
             options = self.model_settings.get_trace_back("options", {})
             if "model" not in options:
-                options.update({ "model": "gpt-3.5-turbo-1106" })
+                options.update({ "model": "gpt-3.5-turbo" })
             return {
                 "stream": True,
                 "messages": self.construct_request_messages(),
                 **options
             }
         elif self.request_type == "vision":
             options = self.model_settings.get_trace_back("options", {})
@@ -177,15 +177,15 @@
             thread_id = thread.id,
         )
         # finally we get it...
         return message.content[0].text.value
 
     async def request_gpt(self, request_data: dict):
         client = self._create_client()
-        if self.request.request_runtime_ctx.get("response:type") == "JSON" and request_data["model"] in ("gpt-3.5-turbo-1106", "gpt-4-1106-preview"):
+        if self.request.request_runtime_ctx.get("response:type") == "JSON":
             request_data.update({ "response_format": { "type": "json_object" } })
         stream = await client.chat.completions.create(
             **request_data
         )
         return stream
 
     async def request_vision(self, request_data: dict):
```

### Comparing `Agently-3.2.2.1/Agently/plugins/request/ZhipuAI.py` & `Agently-3.2.2.2/Agently/plugins/request/ZhipuAI.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/plugins/request/__init__.py` & `Agently-3.2.2.2/Agently/plugins/request/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/plugins/request/utils/RequestABC.py` & `Agently-3.2.2.2/Agently/plugins/request/utils/RequestABC.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/plugins/request/utils/transform.py` & `Agently-3.2.2.2/Agently/plugins/request/utils/transform.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/plugins/storage/FileStorage.py` & `Agently-3.2.2.2/Agently/plugins/storage/FileStorage.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/plugins/storage/__init__.py` & `Agently-3.2.2.2/Agently/plugins/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/plugins/storage/utils/StorageABC.py` & `Agently-3.2.2.2/Agently/plugins/storage/utils/StorageABC.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/plugins/tool/Code.py` & `Agently-3.2.2.2/Agently/plugins/tool/Code.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/plugins/tool/Web.py` & `Agently-3.2.2.2/Agently/plugins/tool/Web.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/plugins/tool/__init__.py` & `Agently-3.2.2.2/Agently/plugins/tool/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/utils/AliasManager.py` & `Agently-3.2.2.2/Agently/utils/AliasManager.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/utils/DataOps.py` & `Agently-3.2.2.2/Agently/utils/DataOps.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/utils/PluginManager.py` & `Agently-3.2.2.2/Agently/utils/PluginManager.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/utils/RuntimeCtx.py` & `Agently-3.2.2.2/Agently/utils/RuntimeCtx.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/utils/StorageDelegate.py` & `Agently-3.2.2.2/Agently/utils/StorageDelegate.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/utils/ToolManager.py` & `Agently-3.2.2.2/Agently/utils/ToolManager.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/utils/check_version.py` & `Agently-3.2.2.2/Agently/utils/check_version.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/utils/load_json.py` & `Agently-3.2.2.2/Agently/utils/load_json.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently/utils/transform.py` & `Agently-3.2.2.2/Agently/utils/transform.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/Agently.egg-info/PKG-INFO` & `Agently-3.2.2.2/Agently.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Agently
-Version: 3.2.2.1
+Version: 3.2.2.2
 Summary: Agently, a framework to build applications based on language model powered intelligent agents.
 Home-page: https://github.com/Maplemx/Agently
 Author: Maplemx
 Author-email: maplemx@gmail.com
 License: Apache License, Version 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Agently-3.2.2.1/Agently.egg-info/SOURCES.txt` & `Agently-3.2.2.2/Agently.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.1/PKG-INFO` & `Agently-3.2.2.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Agently
-Version: 3.2.2.1
+Version: 3.2.2.2
 Summary: Agently, a framework to build applications based on language model powered intelligent agents.
 Home-page: https://github.com/Maplemx/Agently
 Author: Maplemx
 Author-email: maplemx@gmail.com
 License: Apache License, Version 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Agently-3.2.2.1/setup.py` & `Agently-3.2.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 requirements = []
 for requirement in origin_requirements:
     if not requirement.startswith("#"):
         requirements.append(requirement)
 
 setuptools.setup(
     name = "Agently",
-    version = "3.2.2.1",
+    version = "3.2.2.2",
     author = "Maplemx",
     author_email = "maplemx@gmail.com",
     description = "Agently, a framework to build applications based on language model powered intelligent agents.",
     long_description = "https://github.com/Maplemx/Agently",
     url = "https://github.com/Maplemx/Agently",
     license='Apache License, Version 2.0',
     packages = setuptools.find_packages(),
```

