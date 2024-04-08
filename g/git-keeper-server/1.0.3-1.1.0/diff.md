# Comparing `tmp/git-keeper-server-1.0.3.tar.gz` & `tmp/git-keeper-server-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git-keeper-server-1.0.3.tar", last modified: Fri Mar 10 19:54:31 2023, max compression
+gzip compressed data, was "git-keeper-server-1.1.0.tar", last modified: Mon Apr  8 14:14:59 2024, max compression
```

## Comparing `git-keeper-server-1.0.3.tar` & `git-keeper-server-1.1.0.tar`

### file list

```diff
@@ -1,71 +1,73 @@
-drwxr-xr-x   0 nws       (1000) nws       (1000)        0 2023-03-10 19:54:31.905143 git-keeper-server-1.0.3/
--rw-r--r--   0 nws       (1000) nws       (1000)    32386 2021-09-08 21:14:19.000000 git-keeper-server-1.0.3/LICENSE
--rw-r--r--   0 nws       (1000) nws       (1000)     1151 2023-03-10 19:54:31.905143 git-keeper-server-1.0.3/PKG-INFO
--rw-r--r--   0 nws       (1000) nws       (1000)      314 2021-09-08 21:14:19.000000 git-keeper-server-1.0.3/README.md
-drwxr-xr-x   0 nws       (1000) nws       (1000)        0 2023-03-10 19:54:31.901810 git-keeper-server-1.0.3/git_keeper_server.egg-info/
--rw-r--r--   0 nws       (1000) nws       (1000)     1151 2023-03-10 19:54:31.000000 git-keeper-server-1.0.3/git_keeper_server.egg-info/PKG-INFO
--rw-r--r--   0 nws       (1000) nws       (1000)     2230 2023-03-10 19:54:31.000000 git-keeper-server-1.0.3/git_keeper_server.egg-info/SOURCES.txt
--rw-r--r--   0 nws       (1000) nws       (1000)        1 2023-03-10 19:54:31.000000 git-keeper-server-1.0.3/git_keeper_server.egg-info/dependency_links.txt
--rw-r--r--   0 nws       (1000) nws       (1000)       51 2023-03-10 19:54:31.000000 git-keeper-server-1.0.3/git_keeper_server.egg-info/entry_points.txt
--rw-r--r--   0 nws       (1000) nws       (1000)       23 2023-03-10 19:54:31.000000 git-keeper-server-1.0.3/git_keeper_server.egg-info/requires.txt
--rw-r--r--   0 nws       (1000) nws       (1000)       12 2023-03-10 19:54:31.000000 git-keeper-server-1.0.3/git_keeper_server.egg-info/top_level.txt
-drwxr-xr-x   0 nws       (1000) nws       (1000)        0 2023-03-10 19:54:31.905143 git-keeper-server-1.0.3/gkeepserver/
--rw-r--r--   0 nws       (1000) nws       (1000)        0 2021-09-08 21:14:19.000000 git-keeper-server-1.0.3/gkeepserver/__init__.py
--rw-r--r--   0 nws       (1000) nws       (1000)    18805 2022-08-03 14:49:00.000000 git-keeper-server-1.0.3/gkeepserver/assignments.py
--rw-r--r--   0 nws       (1000) nws       (1000)     2503 2022-07-02 19:27:08.000000 git-keeper-server-1.0.3/gkeepserver/check_config.py
--rw-r--r--   0 nws       (1000) nws       (1000)     7379 2022-08-26 02:25:47.000000 git-keeper-server-1.0.3/gkeepserver/check_system.py
-drwxr-xr-x   0 nws       (1000) nws       (1000)        0 2023-03-10 19:54:31.905143 git-keeper-server-1.0.3/gkeepserver/data/
--rw-r--r--   0 nws       (1000) nws       (1000)      161 2021-09-08 21:14:19.000000 git-keeper-server-1.0.3/gkeepserver/data/Dockerfile
--rwxr-xr-x   0 nws       (1000) nws       (1000)      448 2021-09-08 21:14:19.000000 git-keeper-server-1.0.3/gkeepserver/data/add_ssh_id
--rwxr-xr-x   0 nws       (1000) nws       (1000)      471 2021-09-08 21:14:19.000000 git-keeper-server-1.0.3/gkeepserver/data/exec
--rw-r--r--   0 nws       (1000) nws       (1000)      152 2021-09-08 21:14:19.000000 git-keeper-server-1.0.3/gkeepserver/data/exit
--rw-r--r--   0 nws       (1000) nws       (1000)       60 2021-09-08 21:14:19.000000 git-keeper-server-1.0.3/gkeepserver/data/go
--rwxr-xr-x   0 nws       (1000) nws       (1000)     1734 2021-09-08 21:14:19.000000 git-keeper-server-1.0.3/gkeepserver/data/post-receive
--rw-r--r--   0 nws       (1000) nws       (1000)     1349 2021-09-08 21:14:19.000000 git-keeper-server-1.0.3/gkeepserver/data/pre-receive
--rw-r--r--   0 nws       (1000) nws       (1000)      237 2021-09-08 21:14:19.000000 git-keeper-server-1.0.3/gkeepserver/data/run_action.sh
--rw-r--r--   0 nws       (1000) nws       (1000)    43738 2022-08-05 19:50:53.000000 git-keeper-server-1.0.3/gkeepserver/database.py
--rw-r--r--   0 nws       (1000) nws       (1000)     1483 2022-07-26 15:48:17.000000 git-keeper-server-1.0.3/gkeepserver/directory_locks.py
--rw-r--r--   0 nws       (1000) nws       (1000)     5340 2023-03-10 19:43:19.000000 git-keeper-server-1.0.3/gkeepserver/email_sender_thread.py
--rw-r--r--   0 nws       (1000) nws       (1000)     3999 2021-09-08 21:14:19.000000 git-keeper-server-1.0.3/gkeepserver/event_handler.py
--rw-r--r--   0 nws       (1000) nws       (1000)     5541 2022-07-02 19:27:08.000000 git-keeper-server-1.0.3/gkeepserver/event_handler_assigner.py
--rw-r--r--   0 nws       (1000) nws       (1000)     3521 2022-07-02 19:27:08.000000 git-keeper-server-1.0.3/gkeepserver/event_handler_thread.py
-drwxr-xr-x   0 nws       (1000) nws       (1000)        0 2023-03-10 19:54:31.905143 git-keeper-server-1.0.3/gkeepserver/event_handlers/
--rw-r--r--   0 nws       (1000) nws       (1000)      683 2021-09-08 21:14:19.000000 git-keeper-server-1.0.3/gkeepserver/event_handlers/__init__.py
--rw-r--r--   0 nws       (1000) nws       (1000)     3326 2021-09-08 21:14:19.000000 git-keeper-server-1.0.3/gkeepserver/event_handlers/admin_demote_handler.py
--rw-r--r--   0 nws       (1000) nws       (1000)     3108 2021-09-08 21:14:19.000000 git-keeper-server-1.0.3/gkeepserver/event_handlers/admin_promote_handler.py
--rw-r--r--   0 nws       (1000) nws       (1000)     2757 2022-08-03 14:49:00.000000 git-keeper-server-1.0.3/gkeepserver/event_handlers/check_handler.py
--rw-r--r--   0 nws       (1000) nws       (1000)     3374 2021-09-08 21:14:19.000000 git-keeper-server-1.0.3/gkeepserver/event_handlers/class_add_handler.py
--rw-r--r--   0 nws       (1000) nws       (1000)     3706 2021-09-08 21:14:19.000000 git-keeper-server-1.0.3/gkeepserver/event_handlers/class_status_handler.py
--rwxr-xr-x   0 nws       (1000) nws       (1000)     5351 2021-09-08 21:14:19.000000 git-keeper-server-1.0.3/gkeepserver/event_handlers/delete_handler.py
--rwxr-xr-x   0 nws       (1000) nws       (1000)     5721 2021-09-08 21:14:19.000000 git-keeper-server-1.0.3/gkeepserver/event_handlers/disable_handler.py
--rwxr-xr-x   0 nws       (1000) nws       (1000)     4335 2022-07-22 23:35:44.000000 git-keeper-server-1.0.3/gkeepserver/event_handlers/faculty_add_handler.py
--rw-r--r--   0 nws       (1000) nws       (1000)     2760 2022-08-03 14:49:00.000000 git-keeper-server-1.0.3/gkeepserver/event_handlers/handler_registry.py
--rw-r--r--   0 nws       (1000) nws       (1000)     3529 2021-09-08 21:14:19.000000 git-keeper-server-1.0.3/gkeepserver/event_handlers/passwd_handler.py
--rwxr-xr-x   0 nws       (1000) nws       (1000)     7677 2022-06-03 20:00:23.000000 git-keeper-server-1.0.3/gkeepserver/event_handlers/publish_handler.py
--rwxr-xr-x   0 nws       (1000) nws       (1000)    10666 2022-08-05 19:50:53.000000 git-keeper-server-1.0.3/gkeepserver/event_handlers/students_add_handler.py
--rw-r--r--   0 nws       (1000) nws       (1000)     4338 2021-09-08 21:14:19.000000 git-keeper-server-1.0.3/gkeepserver/event_handlers/students_modify_handler.py
--rw-r--r--   0 nws       (1000) nws       (1000)     5251 2021-09-08 21:14:19.000000 git-keeper-server-1.0.3/gkeepserver/event_handlers/students_remove_handler.py
--rw-r--r--   0 nws       (1000) nws       (1000)     5272 2022-08-05 19:50:53.000000 git-keeper-server-1.0.3/gkeepserver/event_handlers/submission_handler.py
--rwxr-xr-x   0 nws       (1000) nws       (1000)     7143 2022-06-03 20:00:23.000000 git-keeper-server-1.0.3/gkeepserver/event_handlers/trigger_handler.py
--rw-r--r--   0 nws       (1000) nws       (1000)     8194 2022-08-03 14:49:00.000000 git-keeper-server-1.0.3/gkeepserver/event_handlers/update_handler.py
--rw-r--r--   0 nws       (1000) nws       (1000)     9331 2022-08-03 14:49:00.000000 git-keeper-server-1.0.3/gkeepserver/event_handlers/upload_handler.py
--rw-r--r--   0 nws       (1000) nws       (1000)     2422 2021-09-08 21:14:19.000000 git-keeper-server-1.0.3/gkeepserver/faculty.py
--rw-r--r--   0 nws       (1000) nws       (1000)     1594 2021-09-08 21:14:19.000000 git-keeper-server-1.0.3/gkeepserver/file_writing.py
--rw-r--r--   0 nws       (1000) nws       (1000)     1442 2021-09-08 21:14:19.000000 git-keeper-server-1.0.3/gkeepserver/generate_password.py
--rw-r--r--   0 nws       (1000) nws       (1000)     7279 2022-08-03 14:49:00.000000 git-keeper-server-1.0.3/gkeepserver/gkeepd.py
--rw-r--r--   0 nws       (1000) nws       (1000)     6690 2021-09-08 21:14:19.000000 git-keeper-server-1.0.3/gkeepserver/gkeepd_logger.py
--rw-r--r--   0 nws       (1000) nws       (1000)     1492 2021-09-08 21:14:19.000000 git-keeper-server-1.0.3/gkeepserver/handler_utils.py
--rw-r--r--   0 nws       (1000) nws       (1000)    18866 2022-07-26 15:48:17.000000 git-keeper-server-1.0.3/gkeepserver/info_update_thread.py
--rw-r--r--   0 nws       (1000) nws       (1000)     2074 2021-09-08 21:14:19.000000 git-keeper-server-1.0.3/gkeepserver/initialize_log.py
--rw-r--r--   0 nws       (1000) nws       (1000)     1818 2021-09-08 21:14:19.000000 git-keeper-server-1.0.3/gkeepserver/local_log_file_reader.py
--rw-r--r--   0 nws       (1000) nws       (1000)     9740 2022-07-02 19:27:08.000000 git-keeper-server-1.0.3/gkeepserver/log_polling.py
--rw-r--r--   0 nws       (1000) nws       (1000)      911 2021-09-08 21:14:19.000000 git-keeper-server-1.0.3/gkeepserver/new_submission_queue.py
--rw-r--r--   0 nws       (1000) nws       (1000)     2426 2022-06-03 20:00:23.000000 git-keeper-server-1.0.3/gkeepserver/reports.py
--rw-r--r--   0 nws       (1000) nws       (1000)    14811 2022-08-26 02:25:47.000000 git-keeper-server-1.0.3/gkeepserver/server_configuration.py
--rw-r--r--   0 nws       (1000) nws       (1000)     7927 2022-09-12 21:27:09.000000 git-keeper-server-1.0.3/gkeepserver/server_email.py
--rw-r--r--   0 nws       (1000) nws       (1000)    17343 2022-10-21 20:05:12.000000 git-keeper-server-1.0.3/gkeepserver/submission.py
--rw-r--r--   0 nws       (1000) nws       (1000)     2517 2022-07-26 15:48:17.000000 git-keeper-server-1.0.3/gkeepserver/submission_test_thread.py
--rw-r--r--   0 nws       (1000) nws       (1000)    14301 2022-08-05 19:50:53.000000 git-keeper-server-1.0.3/gkeepserver/user_setup.py
--rw-r--r--   0 nws       (1000) nws       (1000)      216 2023-03-10 19:43:19.000000 git-keeper-server-1.0.3/gkeepserver/version.py
--rw-r--r--   0 nws       (1000) nws       (1000)       63 2023-03-10 19:54:31.905143 git-keeper-server-1.0.3/setup.cfg
--rw-r--r--   0 nws       (1000) nws       (1000)     1362 2021-09-08 21:14:19.000000 git-keeper-server-1.0.3/setup.py
+drwxr-xr-x   0 sommerm1   (503) staff       (20)        0 2024-04-08 14:14:59.658466 git-keeper-server-1.1.0/
+-rw-r--r--   0 sommerm1   (503) staff       (20)    32386 2020-09-08 19:32:38.000000 git-keeper-server-1.1.0/LICENSE
+-rw-r--r--   0 sommerm1   (503) staff       (20)     1204 2024-04-08 14:14:59.658254 git-keeper-server-1.1.0/PKG-INFO
+-rw-r--r--   0 sommerm1   (503) staff       (20)      314 2020-09-08 19:32:38.000000 git-keeper-server-1.1.0/README.md
+drwxr-xr-x   0 sommerm1   (503) staff       (20)        0 2024-04-08 14:14:59.657581 git-keeper-server-1.1.0/git_keeper_server.egg-info/
+-rw-r--r--   0 sommerm1   (503) staff       (20)     1204 2024-04-08 14:14:59.000000 git-keeper-server-1.1.0/git_keeper_server.egg-info/PKG-INFO
+-rw-r--r--   0 sommerm1   (503) staff       (20)     2303 2024-04-08 14:14:59.000000 git-keeper-server-1.1.0/git_keeper_server.egg-info/SOURCES.txt
+-rw-r--r--   0 sommerm1   (503) staff       (20)        1 2024-04-08 14:14:59.000000 git-keeper-server-1.1.0/git_keeper_server.egg-info/dependency_links.txt
+-rw-r--r--   0 sommerm1   (503) staff       (20)       51 2024-04-08 14:14:59.000000 git-keeper-server-1.1.0/git_keeper_server.egg-info/entry_points.txt
+-rw-r--r--   0 sommerm1   (503) staff       (20)       23 2024-04-08 14:14:59.000000 git-keeper-server-1.1.0/git_keeper_server.egg-info/requires.txt
+-rw-r--r--   0 sommerm1   (503) staff       (20)       12 2024-04-08 14:14:59.000000 git-keeper-server-1.1.0/git_keeper_server.egg-info/top_level.txt
+drwxr-xr-x   0 sommerm1   (503) staff       (20)        0 2024-04-08 14:14:59.629341 git-keeper-server-1.1.0/gkeepserver/
+-rw-r--r--   0 sommerm1   (503) staff       (20)        0 2019-03-18 18:24:29.000000 git-keeper-server-1.1.0/gkeepserver/__init__.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)    18821 2024-04-08 14:05:07.000000 git-keeper-server-1.1.0/gkeepserver/assignments.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)     2503 2023-12-22 15:51:42.000000 git-keeper-server-1.1.0/gkeepserver/check_config.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)     7379 2023-12-22 15:51:42.000000 git-keeper-server-1.1.0/gkeepserver/check_system.py
+drwxr-xr-x   0 sommerm1   (503) staff       (20)        0 2024-04-08 14:14:59.637872 git-keeper-server-1.1.0/gkeepserver/data/
+-rw-r--r--   0 sommerm1   (503) staff       (20)      161 2020-09-08 19:31:48.000000 git-keeper-server-1.1.0/gkeepserver/data/Dockerfile
+-rwxr-xr-x   0 sommerm1   (503) staff       (20)      448 2023-12-22 15:51:42.000000 git-keeper-server-1.1.0/gkeepserver/data/add_ssh_id
+-rwxr-xr-x   0 sommerm1   (503) staff       (20)      471 2023-12-22 15:51:42.000000 git-keeper-server-1.1.0/gkeepserver/data/exec
+-rw-r--r--   0 sommerm1   (503) staff       (20)      152 2023-12-22 15:51:42.000000 git-keeper-server-1.1.0/gkeepserver/data/exit
+-rw-r--r--   0 sommerm1   (503) staff       (20)       60 2020-09-08 19:31:48.000000 git-keeper-server-1.1.0/gkeepserver/data/go
+-rwxr-xr-x   0 sommerm1   (503) staff       (20)     1734 2020-09-08 19:32:38.000000 git-keeper-server-1.1.0/gkeepserver/data/post-receive
+-rw-r--r--   0 sommerm1   (503) staff       (20)     1349 2023-12-22 15:51:42.000000 git-keeper-server-1.1.0/gkeepserver/data/pre-receive
+-rw-r--r--   0 sommerm1   (503) staff       (20)      237 2020-09-08 19:31:52.000000 git-keeper-server-1.1.0/gkeepserver/data/run_action.sh
+-rw-r--r--   0 sommerm1   (503) staff       (20)      803 2019-12-12 08:23:51.000000 git-keeper-server-1.1.0/gkeepserver/data/schema.sql
+-rw-r--r--   0 sommerm1   (503) staff       (20)    43738 2023-12-22 15:51:42.000000 git-keeper-server-1.1.0/gkeepserver/database.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)     1483 2023-12-22 15:51:42.000000 git-keeper-server-1.1.0/gkeepserver/directory_locks.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)     5340 2024-04-08 14:05:07.000000 git-keeper-server-1.1.0/gkeepserver/email_sender_thread.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)     3999 2020-09-08 19:31:52.000000 git-keeper-server-1.1.0/gkeepserver/event_handler.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)     5541 2023-12-22 15:51:42.000000 git-keeper-server-1.1.0/gkeepserver/event_handler_assigner.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)     3521 2023-12-22 15:51:42.000000 git-keeper-server-1.1.0/gkeepserver/event_handler_thread.py
+drwxr-xr-x   0 sommerm1   (503) staff       (20)        0 2024-04-08 14:14:59.656596 git-keeper-server-1.1.0/gkeepserver/event_handlers/
+-rw-r--r--   0 sommerm1   (503) staff       (20)      683 2020-09-08 19:31:52.000000 git-keeper-server-1.1.0/gkeepserver/event_handlers/__init__.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)     3326 2023-12-22 15:51:42.000000 git-keeper-server-1.1.0/gkeepserver/event_handlers/admin_demote_handler.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)     3108 2023-12-22 15:51:42.000000 git-keeper-server-1.1.0/gkeepserver/event_handlers/admin_promote_handler.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)     2757 2023-12-22 15:51:42.000000 git-keeper-server-1.1.0/gkeepserver/event_handlers/check_handler.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)     3374 2023-12-22 15:51:42.000000 git-keeper-server-1.1.0/gkeepserver/event_handlers/class_add_handler.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)     3706 2023-12-22 15:51:42.000000 git-keeper-server-1.1.0/gkeepserver/event_handlers/class_status_handler.py
+-rwxr-xr-x   0 sommerm1   (503) staff       (20)     5351 2023-12-22 15:51:42.000000 git-keeper-server-1.1.0/gkeepserver/event_handlers/delete_handler.py
+-rwxr-xr-x   0 sommerm1   (503) staff       (20)     5721 2023-12-22 15:51:42.000000 git-keeper-server-1.1.0/gkeepserver/event_handlers/disable_handler.py
+-rwxr-xr-x   0 sommerm1   (503) staff       (20)     4335 2023-12-22 15:51:42.000000 git-keeper-server-1.1.0/gkeepserver/event_handlers/faculty_add_handler.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)     2760 2024-03-06 17:27:10.000000 git-keeper-server-1.1.0/gkeepserver/event_handlers/handler_registry.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)     3529 2023-12-22 15:51:42.000000 git-keeper-server-1.1.0/gkeepserver/event_handlers/passwd_handler.py
+-rwxr-xr-x   0 sommerm1   (503) staff       (20)     7678 2024-04-08 14:05:07.000000 git-keeper-server-1.1.0/gkeepserver/event_handlers/publish_handler.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)     6263 2024-03-06 20:32:08.000000 git-keeper-server-1.1.0/gkeepserver/event_handlers/resend_handler.py
+-rwxr-xr-x   0 sommerm1   (503) staff       (20)    10666 2023-12-22 15:51:42.000000 git-keeper-server-1.1.0/gkeepserver/event_handlers/students_add_handler.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)     4338 2023-12-22 15:51:42.000000 git-keeper-server-1.1.0/gkeepserver/event_handlers/students_modify_handler.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)     5251 2023-12-22 15:51:42.000000 git-keeper-server-1.1.0/gkeepserver/event_handlers/students_remove_handler.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)     5272 2023-12-22 15:51:42.000000 git-keeper-server-1.1.0/gkeepserver/event_handlers/submission_handler.py
+-rwxr-xr-x   0 sommerm1   (503) staff       (20)     7143 2023-12-22 15:51:42.000000 git-keeper-server-1.1.0/gkeepserver/event_handlers/trigger_handler.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)     8194 2023-12-22 15:51:42.000000 git-keeper-server-1.1.0/gkeepserver/event_handlers/update_handler.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)     9331 2023-12-22 15:51:42.000000 git-keeper-server-1.1.0/gkeepserver/event_handlers/upload_handler.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)     2422 2023-12-22 15:51:42.000000 git-keeper-server-1.1.0/gkeepserver/faculty.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)     1594 2022-07-29 05:21:36.000000 git-keeper-server-1.1.0/gkeepserver/file_writing.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)     1442 2020-09-08 19:31:37.000000 git-keeper-server-1.1.0/gkeepserver/generate_password.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)     7279 2023-12-22 15:51:42.000000 git-keeper-server-1.1.0/gkeepserver/gkeepd.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)     6690 2023-12-22 15:51:42.000000 git-keeper-server-1.1.0/gkeepserver/gkeepd_logger.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)     1492 2023-12-22 15:51:42.000000 git-keeper-server-1.1.0/gkeepserver/handler_utils.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)    18866 2023-12-22 15:51:42.000000 git-keeper-server-1.1.0/gkeepserver/info_update_thread.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)     2074 2022-07-29 05:21:36.000000 git-keeper-server-1.1.0/gkeepserver/initialize_log.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)     1818 2020-09-08 19:31:45.000000 git-keeper-server-1.1.0/gkeepserver/local_log_file_reader.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)     9740 2023-12-22 15:51:42.000000 git-keeper-server-1.1.0/gkeepserver/log_polling.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)      911 2020-09-08 19:31:38.000000 git-keeper-server-1.1.0/gkeepserver/new_submission_queue.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)     2426 2023-12-22 15:51:42.000000 git-keeper-server-1.1.0/gkeepserver/reports.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)    15116 2024-04-08 14:05:07.000000 git-keeper-server-1.1.0/gkeepserver/server_configuration.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)     7927 2023-12-22 15:51:42.000000 git-keeper-server-1.1.0/gkeepserver/server_email.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)    16953 2024-04-08 14:05:07.000000 git-keeper-server-1.1.0/gkeepserver/submission.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)     2517 2023-12-22 15:51:42.000000 git-keeper-server-1.1.0/gkeepserver/submission_test_thread.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)    14301 2023-12-22 15:51:42.000000 git-keeper-server-1.1.0/gkeepserver/user_setup.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)      216 2024-04-08 14:05:07.000000 git-keeper-server-1.1.0/gkeepserver/version.py
+-rw-r--r--   0 sommerm1   (503) staff       (20)       63 2024-04-08 14:14:59.659079 git-keeper-server-1.1.0/setup.cfg
+-rw-r--r--   0 sommerm1   (503) staff       (20)     1362 2023-12-22 15:51:42.000000 git-keeper-server-1.1.0/setup.py
```

### Comparing `git-keeper-server-1.0.3/LICENSE` & `git-keeper-server-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `git-keeper-server-1.0.3/PKG-INFO` & `git-keeper-server-1.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-keeper-server
-Version: 1.0.3
+Version: 1.1.0
 Summary: A git-based system for distributing and collecting programming assignments with automatic feedback.
 Home-page: https://github.com/git-keeper/git-keeper
 Author: Nathan Sommer and Ben Coleman
 Author-email: git-keeper@googlegroups.com
 License: GPL 3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
@@ -14,14 +14,16 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Natural Language :: English
 Classifier: Topic :: Education :: Testing
 Classifier: Topic :: Education
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: git-keeper-core
+Requires-Dist: peewee
 
 # git-keeper-server
 
 This package provides the server application for git-keeper, a git-based system
 for distributing, testing, and collecting programming assignments.
 
 For more detailed documentation, see our GitHub repository:
```

### Comparing `git-keeper-server-1.0.3/git_keeper_server.egg-info/PKG-INFO` & `git-keeper-server-1.1.0/git_keeper_server.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-keeper-server
-Version: 1.0.3
+Version: 1.1.0
 Summary: A git-based system for distributing and collecting programming assignments with automatic feedback.
 Home-page: https://github.com/git-keeper/git-keeper
 Author: Nathan Sommer and Ben Coleman
 Author-email: git-keeper@googlegroups.com
 License: GPL 3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
@@ -14,14 +14,16 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Natural Language :: English
 Classifier: Topic :: Education :: Testing
 Classifier: Topic :: Education
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: git-keeper-core
+Requires-Dist: peewee
 
 # git-keeper-server
 
 This package provides the server application for git-keeper, a git-based system
 for distributing, testing, and collecting programming assignments.
 
 For more detailed documentation, see our GitHub repository:
```

### Comparing `git-keeper-server-1.0.3/git_keeper_server.egg-info/SOURCES.txt` & `git-keeper-server-1.1.0/git_keeper_server.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -40,26 +40,28 @@
 gkeepserver/data/add_ssh_id
 gkeepserver/data/exec
 gkeepserver/data/exit
 gkeepserver/data/go
 gkeepserver/data/post-receive
 gkeepserver/data/pre-receive
 gkeepserver/data/run_action.sh
+gkeepserver/data/schema.sql
 gkeepserver/event_handlers/__init__.py
 gkeepserver/event_handlers/admin_demote_handler.py
 gkeepserver/event_handlers/admin_promote_handler.py
 gkeepserver/event_handlers/check_handler.py
 gkeepserver/event_handlers/class_add_handler.py
 gkeepserver/event_handlers/class_status_handler.py
 gkeepserver/event_handlers/delete_handler.py
 gkeepserver/event_handlers/disable_handler.py
 gkeepserver/event_handlers/faculty_add_handler.py
 gkeepserver/event_handlers/handler_registry.py
 gkeepserver/event_handlers/passwd_handler.py
 gkeepserver/event_handlers/publish_handler.py
+gkeepserver/event_handlers/resend_handler.py
 gkeepserver/event_handlers/students_add_handler.py
 gkeepserver/event_handlers/students_modify_handler.py
 gkeepserver/event_handlers/students_remove_handler.py
 gkeepserver/event_handlers/submission_handler.py
 gkeepserver/event_handlers/trigger_handler.py
 gkeepserver/event_handlers/update_handler.py
 gkeepserver/event_handlers/upload_handler.py
```

### Comparing `git-keeper-server-1.0.3/gkeepserver/assignments.py` & `git-keeper-server-1.1.0/gkeepserver/assignments.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 
 import os
 from tempfile import TemporaryDirectory
 
 from gkeepcore.action_scripts import get_action_script_and_interpreter
 from gkeepcore.assignment_config import AssignmentConfig
+from gkeepcore.git_clone_url import git_clone_url
 from gkeepcore.student import Student
 from pkg_resources import resource_exists, resource_string, ResolutionError, \
     ExtractionError
 
 from gkeepcore.git_commands import git_init_bare, git_init, git_add_all, \
     git_commit, git_push, git_config
 from gkeepcore.gkeep_exception import GkeepException
@@ -436,17 +437,16 @@
     assignment_config = assignment_dir.get_config()
 
     email_subject = (assignment_config.announcement_subject
                      .format(class_name=assignment_dir.class_name,
                              assignment_name=assignment_dir.assignment_name))
 
     # build the clone URL for the assignment
-    clone_url = '{0}@{1}:{2}'.format(student.username,
-                                     config.hostname,
-                                     assignment_repo_path)
+    clone_url = git_clone_url(student.username, config.hostname,
+                              config.ssh_port, assignment_repo_path)
 
     # read email.txt to get the customizable part of the email body
     try:
         with open(assignment_dir.email_path) as f:
             email_body = f.read()
     except OSError as e:
         error = 'error reading {0}: {1}'.format(assignment_dir.email_path,
```

### Comparing `git-keeper-server-1.0.3/gkeepserver/check_config.py` & `git-keeper-server-1.1.0/gkeepserver/check_config.py`

 * *Files identical despite different names*

### Comparing `git-keeper-server-1.0.3/gkeepserver/check_system.py` & `git-keeper-server-1.1.0/gkeepserver/check_system.py`

 * *Files identical despite different names*

### Comparing `git-keeper-server-1.0.3/gkeepserver/data/post-receive` & `git-keeper-server-1.1.0/gkeepserver/data/post-receive`

 * *Files identical despite different names*

### Comparing `git-keeper-server-1.0.3/gkeepserver/data/pre-receive` & `git-keeper-server-1.1.0/gkeepserver/data/pre-receive`

 * *Files identical despite different names*

### Comparing `git-keeper-server-1.0.3/gkeepserver/database.py` & `git-keeper-server-1.1.0/gkeepserver/database.py`

 * *Files identical despite different names*

### Comparing `git-keeper-server-1.0.3/gkeepserver/directory_locks.py` & `git-keeper-server-1.1.0/gkeepserver/directory_locks.py`

 * *Files identical despite different names*

### Comparing `git-keeper-server-1.0.3/gkeepserver/email_sender_thread.py` & `git-keeper-server-1.1.0/gkeepserver/email_sender_thread.py`

 * *Files identical despite different names*

### Comparing `git-keeper-server-1.0.3/gkeepserver/event_handler.py` & `git-keeper-server-1.1.0/gkeepserver/event_handler.py`

 * *Files identical despite different names*

### Comparing `git-keeper-server-1.0.3/gkeepserver/event_handler_assigner.py` & `git-keeper-server-1.1.0/gkeepserver/event_handler_assigner.py`

 * *Files identical despite different names*

### Comparing `git-keeper-server-1.0.3/gkeepserver/event_handler_thread.py` & `git-keeper-server-1.1.0/gkeepserver/event_handler_thread.py`

 * *Files identical despite different names*

### Comparing `git-keeper-server-1.0.3/gkeepserver/event_handlers/__init__.py` & `git-keeper-server-1.1.0/gkeepserver/event_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `git-keeper-server-1.0.3/gkeepserver/event_handlers/admin_demote_handler.py` & `git-keeper-server-1.1.0/gkeepserver/event_handlers/admin_demote_handler.py`

 * *Files identical despite different names*

### Comparing `git-keeper-server-1.0.3/gkeepserver/event_handlers/admin_promote_handler.py` & `git-keeper-server-1.1.0/gkeepserver/event_handlers/admin_promote_handler.py`

 * *Files identical despite different names*

### Comparing `git-keeper-server-1.0.3/gkeepserver/event_handlers/check_handler.py` & `git-keeper-server-1.1.0/gkeepserver/event_handlers/check_handler.py`

 * *Files identical despite different names*

### Comparing `git-keeper-server-1.0.3/gkeepserver/event_handlers/class_add_handler.py` & `git-keeper-server-1.1.0/gkeepserver/event_handlers/class_add_handler.py`

 * *Files identical despite different names*

### Comparing `git-keeper-server-1.0.3/gkeepserver/event_handlers/class_status_handler.py` & `git-keeper-server-1.1.0/gkeepserver/event_handlers/class_status_handler.py`

 * *Files identical despite different names*

### Comparing `git-keeper-server-1.0.3/gkeepserver/event_handlers/delete_handler.py` & `git-keeper-server-1.1.0/gkeepserver/event_handlers/delete_handler.py`

 * *Files identical despite different names*

### Comparing `git-keeper-server-1.0.3/gkeepserver/event_handlers/disable_handler.py` & `git-keeper-server-1.1.0/gkeepserver/event_handlers/disable_handler.py`

 * *Files identical despite different names*

### Comparing `git-keeper-server-1.0.3/gkeepserver/event_handlers/faculty_add_handler.py` & `git-keeper-server-1.1.0/gkeepserver/event_handlers/faculty_add_handler.py`

 * *Files identical despite different names*

### Comparing `git-keeper-server-1.0.3/gkeepserver/event_handlers/handler_registry.py` & `git-keeper-server-1.1.0/gkeepserver/event_handlers/handler_registry.py`

 * *Files identical despite different names*

### Comparing `git-keeper-server-1.0.3/gkeepserver/event_handlers/passwd_handler.py` & `git-keeper-server-1.1.0/gkeepserver/event_handlers/passwd_handler.py`

 * *Files identical despite different names*

### Comparing `git-keeper-server-1.0.3/gkeepserver/event_handlers/publish_handler.py` & `git-keeper-server-1.1.0/gkeepserver/event_handlers/publish_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,15 +101,15 @@
             for student in students:
                 student_report_path = \
                     os.path.join(temp_dir_path,
                                  student.get_last_first_username())
                 mkdir(student_report_path)
 
                 student_placeholder_path = os.path.join(student_report_path,
-                                                        '.placeholder')
+                                                        'no_submission')
                 touch(student_placeholder_path)
 
             git_add_all(temp_dir_path)
             git_commit(temp_dir_path, 'Initial commit')
 
     def _setup_students_assignment_repos(self,
                                          assignment_dir: AssignmentDirectory):
```

### Comparing `git-keeper-server-1.0.3/gkeepserver/event_handlers/students_add_handler.py` & `git-keeper-server-1.1.0/gkeepserver/event_handlers/students_add_handler.py`

 * *Files identical despite different names*

### Comparing `git-keeper-server-1.0.3/gkeepserver/event_handlers/students_modify_handler.py` & `git-keeper-server-1.1.0/gkeepserver/event_handlers/students_modify_handler.py`

 * *Files identical despite different names*

### Comparing `git-keeper-server-1.0.3/gkeepserver/event_handlers/students_remove_handler.py` & `git-keeper-server-1.1.0/gkeepserver/event_handlers/students_remove_handler.py`

 * *Files identical despite different names*

### Comparing `git-keeper-server-1.0.3/gkeepserver/event_handlers/submission_handler.py` & `git-keeper-server-1.1.0/gkeepserver/event_handlers/submission_handler.py`

 * *Files identical despite different names*

### Comparing `git-keeper-server-1.0.3/gkeepserver/event_handlers/trigger_handler.py` & `git-keeper-server-1.1.0/gkeepserver/event_handlers/trigger_handler.py`

 * *Files identical despite different names*

### Comparing `git-keeper-server-1.0.3/gkeepserver/event_handlers/update_handler.py` & `git-keeper-server-1.1.0/gkeepserver/event_handlers/update_handler.py`

 * *Files identical despite different names*

### Comparing `git-keeper-server-1.0.3/gkeepserver/event_handlers/upload_handler.py` & `git-keeper-server-1.1.0/gkeepserver/event_handlers/upload_handler.py`

 * *Files identical despite different names*

### Comparing `git-keeper-server-1.0.3/gkeepserver/faculty.py` & `git-keeper-server-1.1.0/gkeepserver/faculty.py`

 * *Files identical despite different names*

### Comparing `git-keeper-server-1.0.3/gkeepserver/file_writing.py` & `git-keeper-server-1.1.0/gkeepserver/file_writing.py`

 * *Files identical despite different names*

### Comparing `git-keeper-server-1.0.3/gkeepserver/generate_password.py` & `git-keeper-server-1.1.0/gkeepserver/generate_password.py`

 * *Files identical despite different names*

### Comparing `git-keeper-server-1.0.3/gkeepserver/gkeepd.py` & `git-keeper-server-1.1.0/gkeepserver/gkeepd.py`

 * *Files identical despite different names*

### Comparing `git-keeper-server-1.0.3/gkeepserver/gkeepd_logger.py` & `git-keeper-server-1.1.0/gkeepserver/gkeepd_logger.py`

 * *Files identical despite different names*

### Comparing `git-keeper-server-1.0.3/gkeepserver/handler_utils.py` & `git-keeper-server-1.1.0/gkeepserver/handler_utils.py`

 * *Files identical despite different names*

### Comparing `git-keeper-server-1.0.3/gkeepserver/info_update_thread.py` & `git-keeper-server-1.1.0/gkeepserver/info_update_thread.py`

 * *Files identical despite different names*

### Comparing `git-keeper-server-1.0.3/gkeepserver/initialize_log.py` & `git-keeper-server-1.1.0/gkeepserver/initialize_log.py`

 * *Files identical despite different names*

### Comparing `git-keeper-server-1.0.3/gkeepserver/local_log_file_reader.py` & `git-keeper-server-1.1.0/gkeepserver/local_log_file_reader.py`

 * *Files identical despite different names*

### Comparing `git-keeper-server-1.0.3/gkeepserver/log_polling.py` & `git-keeper-server-1.1.0/gkeepserver/log_polling.py`

 * *Files identical despite different names*

### Comparing `git-keeper-server-1.0.3/gkeepserver/new_submission_queue.py` & `git-keeper-server-1.1.0/gkeepserver/new_submission_queue.py`

 * *Files identical despite different names*

### Comparing `git-keeper-server-1.0.3/gkeepserver/reports.py` & `git-keeper-server-1.1.0/gkeepserver/reports.py`

 * *Files identical despite different names*

### Comparing `git-keeper-server-1.0.3/gkeepserver/server_configuration.py` & `git-keeper-server-1.1.0/gkeepserver/server_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,14 +211,17 @@
         # users and groups
         self.keeper_user = 'keeper'
         self.keeper_group = 'keeper'
         self.tester_user = 'tester'
         self.faculty_group = 'faculty'
         self.student_group = 'student'
 
+        # server
+        self.ssh_port = 22
+
         # email
         self.use_tls = True
         self.email_username = None
         self.email_password = None
         self.email_interval = 2
         self.use_html = True
 
@@ -311,14 +314,20 @@
         self._ensure_section_is_present('server')
 
         try:
             self.hostname = self._parser.get('server', 'hostname')
         except configparser.NoOptionError as e:
             raise ServerConfigurationError(e.message)
 
+        if self._parser.has_option('server', 'ssh_port'):
+            try:
+                self.ssh_port = int(self._parser.get('email', 'ssh_port'))
+            except ValueError:
+                raise ServerConfigurationError('ssh_port must be an integer')
+
     def _set_admin_options(self):
         # set admin-related attributes
 
         self._ensure_section_is_present('admin')
 
         required_options = [
             'admin_email',
```

### Comparing `git-keeper-server-1.0.3/gkeepserver/server_email.py` & `git-keeper-server-1.1.0/gkeepserver/server_email.py`

 * *Files identical despite different names*

### Comparing `git-keeper-server-1.0.3/gkeepserver/submission.py` & `git-keeper-server-1.1.0/gkeepserver/submission.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 on the submission.
 """
 
 import os
 from time import strftime, time
 from tempfile import TemporaryDirectory, mkdtemp
 
+from gkeepcore.temp_paths import TempPaths
 from gkeepserver.directory_locks import directory_locks
 from gkeepcore.action_scripts import get_action_script_and_interpreter
 from gkeepcore.gkeep_exception import GkeepException
 from gkeepcore.student import Student
 from gkeepserver.assignments import AssignmentDirectory
 from gkeepserver.database import db
 from gkeepserver.gkeepd_logger import gkeepd_logger as logger
@@ -39,34 +40,14 @@
 from gkeepserver.info_update_thread import info_updater
 from gkeepserver.reports import reports_clone
 from gkeepserver.server_configuration import config
 from gkeepserver.server_email import Email
 from gkeepcore.path_utils import user_home_dir
 
 
-class TempPaths:
-    """
-    Represents the various paths in a temporary testing directory.
-
-    Attributes:
-
-    temp_path - path to the temporary directory storing all items
-    submission_path - path to the clone of the student's submission
-    run_action_sh_path - path to run_action.sh that will be called ot initiate
-                         tests
-    assignment_cfg_path - path to assignment.cfg, which may or may not exist
-    """
-
-    def __init__(self, temp_path, assignment_name):
-        self.temp_path = temp_path
-        self.submission_path = os.path.join(temp_path, assignment_name)
-        self.run_action_sh_path = os.path.join(temp_path, 'run_action.sh')
-        self.assignment_cfg_path = os.path.join(temp_path, 'assignment.cfg')
-
-
 class Submission:
     """
     Stores student submission information and allows test running.
     """
 
     def __init__(self, student: Student, student_repo_path, commit_hash,
                  assignment_dir: AssignmentDirectory, faculty_username,
@@ -223,14 +204,20 @@
                 report_file_path = os.path.join(student_report_dir_path,
                                                 report_filename)
                 counter += 1
 
             with open(report_file_path, 'w') as f:
                 f.write(body)
 
+            for placeholder_filename in ('.placeholder', 'no_submission'):
+                placeholder_path = os.path.join(student_report_dir_path,
+                                                placeholder_filename)
+                if os.path.isfile(placeholder_path):
+                    os.remove(placeholder_path)
+
             reports_commit_message = ('Submission report for {}'
                                       .format(last_first_username))
 
             git_add_all(temp_reports_repo_path)
             git_commit(temp_reports_repo_path, reports_commit_message)
 
     def _email_results(self, body, assignment_cfg: AssignmentConfig):
```

### Comparing `git-keeper-server-1.0.3/gkeepserver/submission_test_thread.py` & `git-keeper-server-1.1.0/gkeepserver/submission_test_thread.py`

 * *Files identical despite different names*

### Comparing `git-keeper-server-1.0.3/gkeepserver/user_setup.py` & `git-keeper-server-1.1.0/gkeepserver/user_setup.py`

 * *Files identical despite different names*

### Comparing `git-keeper-server-1.0.3/setup.py` & `git-keeper-server-1.1.0/setup.py`

 * *Files identical despite different names*

