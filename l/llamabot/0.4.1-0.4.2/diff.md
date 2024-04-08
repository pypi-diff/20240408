# Comparing `tmp/llamabot-0.4.1.tar.gz` & `tmp/llamabot-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llamabot-0.4.1.tar", last modified: Sun Mar 31 15:56:28 2024, max compression
+gzip compressed data, was "llamabot-0.4.2.tar", last modified: Mon Apr  8 05:53:21 2024, max compression
```

## Comparing `llamabot-0.4.1.tar` & `llamabot-0.4.2.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 15:56:28.916450 llamabot-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-31 15:52:35.000000 llamabot-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    13519 2024-03-31 15:56:28.916450 llamabot-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12212 2024-03-31 15:52:35.000000 llamabot-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 15:56:28.908450 llamabot-0.4.1/llamabot/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-03-31 15:52:35.000000 llamabot-0.4.1/llamabot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 15:56:28.908450 llamabot-0.4.1/llamabot/bot/
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-03-31 15:52:35.000000 llamabot-0.4.1/llamabot/bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-03-31 15:52:35.000000 llamabot-0.4.1/llamabot/bot/chatbot.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-03-31 15:52:35.000000 llamabot-0.4.1/llamabot/bot/imagebot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-03-31 15:52:35.000000 llamabot-0.4.1/llamabot/bot/kgbot.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-03-31 15:52:35.000000 llamabot-0.4.1/llamabot/bot/model_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-03-31 15:56:22.000000 llamabot-0.4.1/llamabot/bot/ollama_model_names.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-03-31 15:52:35.000000 llamabot-0.4.1/llamabot/bot/qabot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-03-31 15:52:35.000000 llamabot-0.4.1/llamabot/bot/querybot.py
--rw-r--r--   0 runner    (1001) docker     (127)     8176 2024-03-31 15:52:35.000000 llamabot-0.4.1/llamabot/bot/simplebot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 15:56:28.912450 llamabot-0.4.1/llamabot/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-03-31 15:52:35.000000 llamabot-0.4.1/llamabot/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-03-31 15:52:35.000000 llamabot-0.4.1/llamabot/cli/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-03-31 15:52:35.000000 llamabot-0.4.1/llamabot/cli/blog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-03-31 15:52:35.000000 llamabot-0.4.1/llamabot/cli/configure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-03-31 15:52:35.000000 llamabot-0.4.1/llamabot/cli/doc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-03-31 15:52:35.000000 llamabot-0.4.1/llamabot/cli/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-03-31 15:52:35.000000 llamabot-0.4.1/llamabot/cli/python.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-03-31 15:52:35.000000 llamabot-0.4.1/llamabot/cli/repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-03-31 15:52:35.000000 llamabot-0.4.1/llamabot/cli/serve.py
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-03-31 15:52:35.000000 llamabot-0.4.1/llamabot/cli/tutorial.py
--rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-03-31 15:52:35.000000 llamabot-0.4.1/llamabot/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-03-31 15:52:35.000000 llamabot-0.4.1/llamabot/cli/zotero.py
--rw-r--r--   0 runner    (1001) docker     (127)    14939 2024-03-31 15:52:35.000000 llamabot-0.4.1/llamabot/code_manipulation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 15:56:28.912450 llamabot-0.4.1/llamabot/components/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-31 15:52:35.000000 llamabot-0.4.1/llamabot/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-03-31 15:52:35.000000 llamabot-0.4.1/llamabot/components/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-03-31 15:52:35.000000 llamabot-0.4.1/llamabot/components/chatui.py
--rw-r--r--   0 runner    (1001) docker     (127)     9433 2024-03-31 15:52:35.000000 llamabot-0.4.1/llamabot/components/docstore.py
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-03-31 15:52:35.000000 llamabot-0.4.1/llamabot/components/history.py
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-03-31 15:52:35.000000 llamabot-0.4.1/llamabot/components/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-03-31 15:52:35.000000 llamabot-0.4.1/llamabot/components/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-03-31 15:52:35.000000 llamabot-0.4.1/llamabot/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-03-31 15:52:35.000000 llamabot-0.4.1/llamabot/doc_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-03-31 15:52:35.000000 llamabot-0.4.1/llamabot/dummy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-03-31 15:52:35.000000 llamabot-0.4.1/llamabot/file_finder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 15:56:28.916450 llamabot-0.4.1/llamabot/prompt_library/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-31 15:52:35.000000 llamabot-0.4.1/llamabot/prompt_library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-03-31 15:52:35.000000 llamabot-0.4.1/llamabot/prompt_library/blog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-03-31 15:52:35.000000 llamabot-0.4.1/llamabot/prompt_library/diffbot.py
--rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-03-31 15:52:35.000000 llamabot-0.4.1/llamabot/prompt_library/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-03-31 15:52:35.000000 llamabot-0.4.1/llamabot/prompt_library/output_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-03-31 15:52:35.000000 llamabot-0.4.1/llamabot/prompt_library/python.py
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-03-31 15:52:35.000000 llamabot-0.4.1/llamabot/prompt_library/sembr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-03-31 15:52:35.000000 llamabot-0.4.1/llamabot/prompt_library/tutorial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-03-31 15:52:35.000000 llamabot-0.4.1/llamabot/prompt_library/zotero.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-03-31 15:52:35.000000 llamabot-0.4.1/llamabot/prompt_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-03-31 15:52:35.000000 llamabot-0.4.1/llamabot/recorder.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-31 15:52:35.000000 llamabot-0.4.1/llamabot/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-31 15:52:38.000000 llamabot-0.4.1/llamabot/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 15:56:28.916450 llamabot-0.4.1/llamabot/zotero/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-31 15:52:35.000000 llamabot-0.4.1/llamabot/zotero/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-03-31 15:52:35.000000 llamabot-0.4.1/llamabot/zotero/completer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6042 2024-03-31 15:52:35.000000 llamabot-0.4.1/llamabot/zotero/library.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-03-31 15:52:35.000000 llamabot-0.4.1/llamabot/zotero/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 15:56:28.916450 llamabot-0.4.1/llamabot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13519 2024-03-31 15:56:28.000000 llamabot-0.4.1/llamabot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-03-31 15:56:28.000000 llamabot-0.4.1/llamabot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 15:56:28.000000 llamabot-0.4.1/llamabot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-31 15:56:28.000000 llamabot-0.4.1/llamabot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-03-31 15:56:28.000000 llamabot-0.4.1/llamabot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-31 15:56:28.000000 llamabot-0.4.1/llamabot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-03-31 15:52:38.000000 llamabot-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 15:56:28.916450 llamabot-0.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 15:56:28.916450 llamabot-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-31 15:52:35.000000 llamabot-0.4.1/tests/test_bot.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-03-31 15:52:35.000000 llamabot-0.4.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     8181 2024-03-31 15:52:35.000000 llamabot-0.4.1/tests/test_code_manipulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-03-31 15:52:35.000000 llamabot-0.4.1/tests/test_doc_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-03-31 15:52:35.000000 llamabot-0.4.1/tests/test_file_finder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-03-31 15:52:35.000000 llamabot-0.4.1/tests/test_prompt_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-03-31 15:52:35.000000 llamabot-0.4.1/tests/test_recorder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:53:21.345262 llamabot-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-08 05:49:56.000000 llamabot-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    13519 2024-04-08 05:53:21.345262 llamabot-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12212 2024-04-08 05:49:56.000000 llamabot-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:53:21.333262 llamabot-0.4.2/llamabot/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-08 05:49:56.000000 llamabot-0.4.2/llamabot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:53:21.337262 llamabot-0.4.2/llamabot/bot/
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-08 05:49:56.000000 llamabot-0.4.2/llamabot/bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-04-08 05:49:56.000000 llamabot-0.4.2/llamabot/bot/chatbot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-08 05:49:56.000000 llamabot-0.4.2/llamabot/bot/imagebot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-08 05:49:56.000000 llamabot-0.4.2/llamabot/bot/kgbot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-08 05:49:56.000000 llamabot-0.4.2/llamabot/bot/model_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-08 05:53:14.000000 llamabot-0.4.2/llamabot/bot/ollama_model_names.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-04-08 05:49:56.000000 llamabot-0.4.2/llamabot/bot/qabot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-08 05:49:56.000000 llamabot-0.4.2/llamabot/bot/querybot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8176 2024-04-08 05:49:56.000000 llamabot-0.4.2/llamabot/bot/simplebot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:53:21.337262 llamabot-0.4.2/llamabot/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-08 05:49:56.000000 llamabot-0.4.2/llamabot/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-08 05:49:56.000000 llamabot-0.4.2/llamabot/cli/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-04-08 05:49:56.000000 llamabot-0.4.2/llamabot/cli/blog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-08 05:49:56.000000 llamabot-0.4.2/llamabot/cli/configure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-08 05:49:56.000000 llamabot-0.4.2/llamabot/cli/doc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-04-08 05:49:56.000000 llamabot-0.4.2/llamabot/cli/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-04-08 05:49:56.000000 llamabot-0.4.2/llamabot/cli/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-08 05:49:56.000000 llamabot-0.4.2/llamabot/cli/repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-08 05:49:56.000000 llamabot-0.4.2/llamabot/cli/serve.py
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-08 05:49:56.000000 llamabot-0.4.2/llamabot/cli/tutorial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-04-08 05:49:56.000000 llamabot-0.4.2/llamabot/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-04-08 05:49:56.000000 llamabot-0.4.2/llamabot/cli/zotero.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14939 2024-04-08 05:49:56.000000 llamabot-0.4.2/llamabot/code_manipulation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:53:21.341262 llamabot-0.4.2/llamabot/components/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-08 05:49:56.000000 llamabot-0.4.2/llamabot/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-08 05:49:56.000000 llamabot-0.4.2/llamabot/components/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-08 05:49:56.000000 llamabot-0.4.2/llamabot/components/chatui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9433 2024-04-08 05:49:56.000000 llamabot-0.4.2/llamabot/components/docstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-04-08 05:49:56.000000 llamabot-0.4.2/llamabot/components/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-08 05:49:56.000000 llamabot-0.4.2/llamabot/components/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-04-08 05:49:56.000000 llamabot-0.4.2/llamabot/components/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-08 05:49:56.000000 llamabot-0.4.2/llamabot/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-04-08 05:49:56.000000 llamabot-0.4.2/llamabot/doc_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-08 05:49:56.000000 llamabot-0.4.2/llamabot/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-08 05:49:56.000000 llamabot-0.4.2/llamabot/file_finder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:53:21.341262 llamabot-0.4.2/llamabot/prompt_library/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-08 05:49:56.000000 llamabot-0.4.2/llamabot/prompt_library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-04-08 05:49:56.000000 llamabot-0.4.2/llamabot/prompt_library/blog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-08 05:49:56.000000 llamabot-0.4.2/llamabot/prompt_library/diffbot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-04-08 05:49:56.000000 llamabot-0.4.2/llamabot/prompt_library/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-08 05:49:56.000000 llamabot-0.4.2/llamabot/prompt_library/output_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-04-08 05:49:56.000000 llamabot-0.4.2/llamabot/prompt_library/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-04-08 05:49:56.000000 llamabot-0.4.2/llamabot/prompt_library/sembr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-08 05:49:56.000000 llamabot-0.4.2/llamabot/prompt_library/tutorial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-08 05:49:56.000000 llamabot-0.4.2/llamabot/prompt_library/zotero.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-08 05:49:56.000000 llamabot-0.4.2/llamabot/prompt_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-08 05:49:56.000000 llamabot-0.4.2/llamabot/recorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-08 05:49:56.000000 llamabot-0.4.2/llamabot/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-08 05:49:58.000000 llamabot-0.4.2/llamabot/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:53:21.341262 llamabot-0.4.2/llamabot/zotero/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-08 05:49:56.000000 llamabot-0.4.2/llamabot/zotero/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-08 05:49:56.000000 llamabot-0.4.2/llamabot/zotero/completer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6042 2024-04-08 05:49:56.000000 llamabot-0.4.2/llamabot/zotero/library.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-08 05:49:56.000000 llamabot-0.4.2/llamabot/zotero/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:53:21.341262 llamabot-0.4.2/llamabot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13519 2024-04-08 05:53:21.000000 llamabot-0.4.2/llamabot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-08 05:53:21.000000 llamabot-0.4.2/llamabot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 05:53:21.000000 llamabot-0.4.2/llamabot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-08 05:53:21.000000 llamabot-0.4.2/llamabot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-08 05:53:21.000000 llamabot-0.4.2/llamabot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-08 05:53:21.000000 llamabot-0.4.2/llamabot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-04-08 05:49:58.000000 llamabot-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 05:53:21.345262 llamabot-0.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 05:53:21.341262 llamabot-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-08 05:49:56.000000 llamabot-0.4.2/tests/test_bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-08 05:49:56.000000 llamabot-0.4.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8181 2024-04-08 05:49:56.000000 llamabot-0.4.2/tests/test_code_manipulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-04-08 05:49:56.000000 llamabot-0.4.2/tests/test_doc_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-04-08 05:49:56.000000 llamabot-0.4.2/tests/test_file_finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-08 05:49:56.000000 llamabot-0.4.2/tests/test_prompt_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-08 05:49:56.000000 llamabot-0.4.2/tests/test_recorder.py
```

### Comparing `llamabot-0.4.1/PKG-INFO` & `llamabot-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: llamabot
-Version: 0.4.1
+Version: 0.4.2
 Summary: A Pythonic interface to LLMs.
 Requires-Python: >3.10
 Description-Content-Type: text/markdown
 Requires-Dist: openai
 Requires-Dist: panel>=1.1.0
 Requires-Dist: jupyter_bokeh
 Requires-Dist: bokeh>=3.1.0
 Requires-Dist: loguru
 Requires-Dist: pyperclip
 Requires-Dist: astor>=0.8.1
 Requires-Dist: python-dotenv
-Requires-Dist: typer>=0.4.1
+Requires-Dist: typer>=0.4.2
 Requires-Dist: gitpython
 Requires-Dist: pyprojroot
 Requires-Dist: frozenlist
 Requires-Dist: beautifulsoup4
 Requires-Dist: rich
 Requires-Dist: pyzotero
 Requires-Dist: case-converter
```

### Comparing `llamabot-0.4.1/README.md` & `llamabot-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.1/llamabot/bot/chatbot.py` & `llamabot-0.4.2/llamabot/bot/chatbot.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.1/llamabot/bot/imagebot.py` & `llamabot-0.4.2/llamabot/bot/imagebot.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.1/llamabot/bot/kgbot.py` & `llamabot-0.4.2/llamabot/bot/kgbot.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.1/llamabot/bot/model_tokens.py` & `llamabot-0.4.2/llamabot/bot/model_tokens.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.1/llamabot/bot/ollama_model_names.txt` & `llamabot-0.4.2/llamabot/bot/ollama_model_names.txt`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.1/llamabot/bot/qabot.py` & `llamabot-0.4.2/llamabot/bot/qabot.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.1/llamabot/bot/querybot.py` & `llamabot-0.4.2/llamabot/bot/querybot.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.1/llamabot/bot/simplebot.py` & `llamabot-0.4.2/llamabot/bot/simplebot.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.1/llamabot/cli/__init__.py` & `llamabot-0.4.2/llamabot/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.1/llamabot/cli/apps.py` & `llamabot-0.4.2/llamabot/cli/apps.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.1/llamabot/cli/blog.py` & `llamabot-0.4.2/llamabot/cli/blog.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.1/llamabot/cli/configure.py` & `llamabot-0.4.2/llamabot/cli/configure.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.1/llamabot/cli/doc.py` & `llamabot-0.4.2/llamabot/cli/doc.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.1/llamabot/cli/git.py` & `llamabot-0.4.2/llamabot/cli/git.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,11 +140,13 @@
         api_key=os.environ["MISTRAL_API_KEY"],
         stream_target="stdout",
     )
     notes = bot(compose_release_notes(log_info))
 
     # Create release_notes_dir if it doesn't exist:
     release_notes_dir.mkdir(parents=True, exist_ok=True)
+    # Ensure only one newline at the end of the file
+    trimmed_notes = notes.content.rstrip() + "\n"
 
-    # Write release notes to the file:
+    # Write release notes to the file
     with open(release_notes_dir / f"{tag2.name}.md", "w+") as f:
-        f.write(notes.content)
+        f.write(trimmed_notes)
```

### Comparing `llamabot-0.4.1/llamabot/cli/python.py` & `llamabot-0.4.2/llamabot/cli/python.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.1/llamabot/cli/repo.py` & `llamabot-0.4.2/llamabot/cli/repo.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.1/llamabot/cli/serve.py` & `llamabot-0.4.2/llamabot/cli/serve.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.1/llamabot/cli/tutorial.py` & `llamabot-0.4.2/llamabot/cli/tutorial.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.1/llamabot/cli/utils.py` & `llamabot-0.4.2/llamabot/cli/utils.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.1/llamabot/cli/zotero.py` & `llamabot-0.4.2/llamabot/cli/zotero.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.1/llamabot/code_manipulation.py` & `llamabot-0.4.2/llamabot/code_manipulation.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.1/llamabot/components/api.py` & `llamabot-0.4.2/llamabot/components/api.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.1/llamabot/components/chatui.py` & `llamabot-0.4.2/llamabot/components/chatui.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.1/llamabot/components/docstore.py` & `llamabot-0.4.2/llamabot/components/docstore.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.1/llamabot/components/history.py` & `llamabot-0.4.2/llamabot/components/history.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.1/llamabot/components/messages.py` & `llamabot-0.4.2/llamabot/components/messages.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.1/llamabot/components/tools.py` & `llamabot-0.4.2/llamabot/components/tools.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.1/llamabot/doc_processor.py` & `llamabot-0.4.2/llamabot/doc_processor.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.1/llamabot/dummy.py` & `llamabot-0.4.2/llamabot/dummy.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.1/llamabot/file_finder.py` & `llamabot-0.4.2/llamabot/file_finder.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.1/llamabot/prompt_library/blog.py` & `llamabot-0.4.2/llamabot/prompt_library/blog.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.1/llamabot/prompt_library/diffbot.py` & `llamabot-0.4.2/llamabot/prompt_library/diffbot.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.1/llamabot/prompt_library/git.py` & `llamabot-0.4.2/llamabot/prompt_library/git.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.1/llamabot/prompt_library/output_formatter.py` & `llamabot-0.4.2/llamabot/prompt_library/output_formatter.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.1/llamabot/prompt_library/python.py` & `llamabot-0.4.2/llamabot/prompt_library/python.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.1/llamabot/prompt_library/sembr.py` & `llamabot-0.4.2/llamabot/prompt_library/sembr.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.1/llamabot/prompt_library/tutorial.py` & `llamabot-0.4.2/llamabot/prompt_library/tutorial.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.1/llamabot/prompt_library/zotero.py` & `llamabot-0.4.2/llamabot/prompt_library/zotero.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.1/llamabot/prompt_manager.py` & `llamabot-0.4.2/llamabot/prompt_manager.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.1/llamabot/recorder.py` & `llamabot-0.4.2/llamabot/recorder.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.1/llamabot/zotero/completer.py` & `llamabot-0.4.2/llamabot/zotero/completer.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.1/llamabot/zotero/library.py` & `llamabot-0.4.2/llamabot/zotero/library.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.1/llamabot.egg-info/PKG-INFO` & `llamabot-0.4.2/llamabot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: llamabot
-Version: 0.4.1
+Version: 0.4.2
 Summary: A Pythonic interface to LLMs.
 Requires-Python: >3.10
 Description-Content-Type: text/markdown
 Requires-Dist: openai
 Requires-Dist: panel>=1.1.0
 Requires-Dist: jupyter_bokeh
 Requires-Dist: bokeh>=3.1.0
 Requires-Dist: loguru
 Requires-Dist: pyperclip
 Requires-Dist: astor>=0.8.1
 Requires-Dist: python-dotenv
-Requires-Dist: typer>=0.4.1
+Requires-Dist: typer>=0.4.2
 Requires-Dist: gitpython
 Requires-Dist: pyprojroot
 Requires-Dist: frozenlist
 Requires-Dist: beautifulsoup4
 Requires-Dist: rich
 Requires-Dist: pyzotero
 Requires-Dist: case-converter
```

### Comparing `llamabot-0.4.1/llamabot.egg-info/SOURCES.txt` & `llamabot-0.4.2/llamabot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.1/pyproject.toml` & `llamabot-0.4.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -58,25 +58,25 @@
 
 [tool.setuptools.packages.find]
 where = ["."]
 namespaces = false
 
 [project]
 name = "llamabot"
-version = "0.4.1"
+version = "0.4.2"
 dependencies = [
     "openai",
     "panel>=1.1.0",
     "jupyter_bokeh",
     "bokeh>=3.1.0",
     "loguru",
     "pyperclip",
     "astor>=0.8.1",
     "python-dotenv",
-    "typer>=0.4.1",
+    "typer>=0.4.2",
     "gitpython",
     "pyprojroot",
     "frozenlist",
     "beautifulsoup4",
     "rich",
     "pyzotero",
     "case-converter",
```

### Comparing `llamabot-0.4.1/tests/test_code_manipulation.py` & `llamabot-0.4.2/tests/test_code_manipulation.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.1/tests/test_doc_processor.py` & `llamabot-0.4.2/tests/test_doc_processor.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.1/tests/test_file_finder.py` & `llamabot-0.4.2/tests/test_file_finder.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.1/tests/test_prompt_manager.py` & `llamabot-0.4.2/tests/test_prompt_manager.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.4.1/tests/test_recorder.py` & `llamabot-0.4.2/tests/test_recorder.py`

 * *Files identical despite different names*

