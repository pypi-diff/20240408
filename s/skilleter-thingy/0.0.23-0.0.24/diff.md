# Comparing `tmp/skilleter_thingy-0.0.23.tar.gz` & `tmp/skilleter_thingy-0.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skilleter_thingy-0.0.23.tar", last modified: Wed Mar 27 12:13:27 2024, max compression
+gzip compressed data, was "skilleter_thingy-0.0.24.tar", last modified: Mon Apr  8 08:46:04 2024, max compression
```

## Comparing `skilleter_thingy-0.0.23.tar` & `skilleter_thingy-0.0.24.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxrwxr-x   0 jms       (1000) jms       (1000)        0 2024-03-27 12:13:27.926976 skilleter_thingy-0.0.23/
--rw-rw-r--   0 jms       (1000) jms       (1000)    32422 2024-03-27 11:04:20.000000 skilleter_thingy-0.0.23/LICENSE
--rw-r--r--   0 jms       (1000) jms       (1000)     5231 2024-03-27 12:13:27.926976 skilleter_thingy-0.0.23/PKG-INFO
--rw-rw-r--   0 jms       (1000) jms       (1000)     4510 2024-03-27 12:12:35.000000 skilleter_thingy-0.0.23/README.md
--rw-rw-r--   0 jms       (1000) jms       (1000)     2868 2024-03-27 12:12:44.000000 skilleter_thingy-0.0.23/pyproject.toml
--rw-rw-r--   0 jms       (1000) jms       (1000)       38 2024-03-27 12:13:27.926976 skilleter_thingy-0.0.23/setup.cfg
-drwxrwxr-x   0 jms       (1000) jms       (1000)        0 2024-03-27 12:13:27.922977 skilleter_thingy-0.0.23/skilleter_thingy/
--rw-rw-r--   0 jms       (1000) jms       (1000)        0 2024-03-01 11:14:28.000000 skilleter_thingy-0.0.23/skilleter_thingy/__init__.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     3842 2024-03-01 11:14:28.000000 skilleter_thingy-0.0.23/skilleter_thingy/addpath.py
--rw-rw-r--   0 jms       (1000) jms       (1000)    18614 2024-03-01 11:14:28.000000 skilleter_thingy-0.0.23/skilleter_thingy/aws.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     7832 2024-03-01 11:14:28.000000 skilleter_thingy-0.0.23/skilleter_thingy/borger.py
--rw-rw-r--   0 jms       (1000) jms       (1000)     7031 2024-03-27 11:09:57.000000 skilleter_thingy-0.0.23/skilleter_thingy/colour.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     1786 2024-03-27 11:09:57.000000 skilleter_thingy-0.0.23/skilleter_thingy/console_colours.py
--rw-rw-r--   0 jms       (1000) jms       (1000)     8539 2024-03-01 11:14:28.000000 skilleter_thingy-0.0.23/skilleter_thingy/dc_curses.py
--rw-rw-r--   0 jms       (1000) jms       (1000)     6170 2024-03-01 11:14:28.000000 skilleter_thingy-0.0.23/skilleter_thingy/dc_defaults.py
--rw-rw-r--   0 jms       (1000) jms       (1000)     1783 2024-03-01 11:14:28.000000 skilleter_thingy-0.0.23/skilleter_thingy/dc_util.py
--rw-rw-r--   0 jms       (1000) jms       (1000)    12268 2024-03-01 11:14:28.000000 skilleter_thingy-0.0.23/skilleter_thingy/dircolors.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     2072 2024-03-01 11:14:28.000000 skilleter_thingy-0.0.23/skilleter_thingy/diskspacecheck.py
--rw-rw-r--   0 jms       (1000) jms       (1000)     2453 2024-03-01 11:14:28.000000 skilleter_thingy-0.0.23/skilleter_thingy/docker.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     3359 2024-03-01 11:14:28.000000 skilleter_thingy-0.0.23/skilleter_thingy/docker_purge.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)    19373 2024-03-01 11:14:28.000000 skilleter_thingy-0.0.23/skilleter_thingy/ffind.py
--rw-rw-r--   0 jms       (1000) jms       (1000)     4261 2024-03-01 11:14:28.000000 skilleter_thingy-0.0.23/skilleter_thingy/files.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     2493 2024-03-01 11:14:28.000000 skilleter_thingy-0.0.23/skilleter_thingy/ggit.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     5876 2024-03-01 11:14:28.000000 skilleter_thingy-0.0.23/skilleter_thingy/ggrep.py
--rw-rw-r--   0 jms       (1000) jms       (1000)    37887 2024-03-27 11:09:57.000000 skilleter_thingy-0.0.23/skilleter_thingy/git.py
--rw-rw-r--   0 jms       (1000) jms       (1000)    35764 2024-03-27 11:09:57.000000 skilleter_thingy-0.0.23/skilleter_thingy/git2.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     5812 2024-03-27 11:09:57.000000 skilleter_thingy-0.0.23/skilleter_thingy/git_br.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     4981 2024-03-27 11:09:57.000000 skilleter_thingy-0.0.23/skilleter_thingy/git_ca.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)    10214 2024-03-27 11:09:57.000000 skilleter_thingy-0.0.23/skilleter_thingy/git_cleanup.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     8225 2024-03-01 11:14:28.000000 skilleter_thingy-0.0.23/skilleter_thingy/git_co.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     1892 2024-03-01 11:14:28.000000 skilleter_thingy-0.0.23/skilleter_thingy/git_common.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     4630 2024-03-01 11:14:28.000000 skilleter_thingy-0.0.23/skilleter_thingy/git_hold.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     3100 2024-03-01 11:14:28.000000 skilleter_thingy-0.0.23/skilleter_thingy/git_mr.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     2696 2024-03-01 11:14:28.000000 skilleter_thingy-0.0.23/skilleter_thingy/git_parent.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)    51276 2024-03-01 11:14:28.000000 skilleter_thingy-0.0.23/skilleter_thingy/git_review.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)    13985 2024-03-27 11:09:57.000000 skilleter_thingy-0.0.23/skilleter_thingy/git_update.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     3143 2024-03-27 11:09:57.000000 skilleter_thingy-0.0.23/skilleter_thingy/git_wt.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)    11279 2024-03-01 11:14:28.000000 skilleter_thingy-0.0.23/skilleter_thingy/gitcmp_helper.py
--rw-rw-r--   0 jms       (1000) jms       (1000)     6062 2024-03-27 11:09:57.000000 skilleter_thingy-0.0.23/skilleter_thingy/gitlab.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     8925 2024-03-01 11:14:28.000000 skilleter_thingy-0.0.23/skilleter_thingy/gitprompt.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     5964 2024-03-01 11:14:28.000000 skilleter_thingy-0.0.23/skilleter_thingy/gl.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)    22040 2024-03-01 11:14:28.000000 skilleter_thingy-0.0.23/skilleter_thingy/gphotosync.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     4316 2024-03-01 11:14:28.000000 skilleter_thingy-0.0.23/skilleter_thingy/linecount.py
--rw-rw-r--   0 jms       (1000) jms       (1000)     3107 2024-03-27 11:09:57.000000 skilleter_thingy-0.0.23/skilleter_thingy/logger.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     4470 2024-03-01 11:14:28.000000 skilleter_thingy-0.0.23/skilleter_thingy/moviemover.py
--rw-rw-r--   0 jms       (1000) jms       (1000)     4737 2024-03-27 11:09:57.000000 skilleter_thingy-0.0.23/skilleter_thingy/path.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     3178 2024-03-01 11:14:28.000000 skilleter_thingy-0.0.23/skilleter_thingy/photodupe.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     7823 2024-03-01 11:14:28.000000 skilleter_thingy-0.0.23/skilleter_thingy/phototidier.py
--rw-rw-r--   0 jms       (1000) jms       (1000)     2529 2024-03-01 11:14:28.000000 skilleter_thingy-0.0.23/skilleter_thingy/popup.py
--rw-rw-r--   0 jms       (1000) jms       (1000)     3565 2024-03-27 11:09:57.000000 skilleter_thingy-0.0.23/skilleter_thingy/process.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     4395 2024-03-01 11:14:28.000000 skilleter_thingy-0.0.23/skilleter_thingy/py_audit.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     9465 2024-03-20 15:29:15.000000 skilleter_thingy-0.0.23/skilleter_thingy/readable.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     4620 2024-03-01 11:14:28.000000 skilleter_thingy-0.0.23/skilleter_thingy/remdir.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)    17117 2024-03-01 11:14:28.000000 skilleter_thingy-0.0.23/skilleter_thingy/rmdupe.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     2639 2024-03-01 11:14:28.000000 skilleter_thingy-0.0.23/skilleter_thingy/rpylint.py
--rw-rw-r--   0 jms       (1000) jms       (1000)    12619 2024-03-01 11:14:28.000000 skilleter_thingy-0.0.23/skilleter_thingy/run.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)    13849 2024-03-01 11:14:28.000000 skilleter_thingy-0.0.23/skilleter_thingy/s3_sync.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     3266 2024-03-01 11:14:28.000000 skilleter_thingy-0.0.23/skilleter_thingy/splitpics.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     2539 2024-03-01 11:14:28.000000 skilleter_thingy-0.0.23/skilleter_thingy/strreplace.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)    11347 2024-03-27 10:30:15.000000 skilleter_thingy-0.0.23/skilleter_thingy/sysmon.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)    33712 2024-03-01 11:14:28.000000 skilleter_thingy-0.0.23/skilleter_thingy/tfm.py
--rw-rw-r--   0 jms       (1000) jms       (1000)    19829 2024-03-06 10:03:10.000000 skilleter_thingy-0.0.23/skilleter_thingy/tfm_pane.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     2993 2024-03-01 11:14:28.000000 skilleter_thingy-0.0.23/skilleter_thingy/tfparse.py
--rw-rw-r--   0 jms       (1000) jms       (1000)     5402 2024-03-18 14:00:25.000000 skilleter_thingy-0.0.23/skilleter_thingy/tidy.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     2397 2024-03-01 11:14:28.000000 skilleter_thingy-0.0.23/skilleter_thingy/trimpath.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     3128 2024-03-01 11:14:28.000000 skilleter_thingy-0.0.23/skilleter_thingy/window_rename.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     4590 2024-03-27 11:09:57.000000 skilleter_thingy-0.0.23/skilleter_thingy/xchmod.py
--rwxrwxr-x   0 jms       (1000) jms       (1000)     2868 2024-03-01 11:14:28.000000 skilleter_thingy-0.0.23/skilleter_thingy/yamlcheck.py
-drwxrwxr-x   0 jms       (1000) jms       (1000)        0 2024-03-27 12:13:27.926976 skilleter_thingy-0.0.23/skilleter_thingy.egg-info/
--rw-r--r--   0 jms       (1000) jms       (1000)     5231 2024-03-27 12:13:27.000000 skilleter_thingy-0.0.23/skilleter_thingy.egg-info/PKG-INFO
--rw-rw-r--   0 jms       (1000) jms       (1000)     2012 2024-03-27 12:13:27.000000 skilleter_thingy-0.0.23/skilleter_thingy.egg-info/SOURCES.txt
--rw-rw-r--   0 jms       (1000) jms       (1000)        1 2024-03-27 12:13:27.000000 skilleter_thingy-0.0.23/skilleter_thingy.egg-info/dependency_links.txt
--rw-rw-r--   0 jms       (1000) jms       (1000)     1971 2024-03-27 12:13:27.000000 skilleter_thingy-0.0.23/skilleter_thingy.egg-info/entry_points.txt
--rw-rw-r--   0 jms       (1000) jms       (1000)       76 2024-03-27 12:13:27.000000 skilleter_thingy-0.0.23/skilleter_thingy.egg-info/requires.txt
--rw-rw-r--   0 jms       (1000) jms       (1000)       17 2024-03-27 12:13:27.000000 skilleter_thingy-0.0.23/skilleter_thingy.egg-info/top_level.txt
+drwxrwxr-x   0 jms       (1000) jms       (1000)        0 2024-04-08 08:46:04.591760 skilleter_thingy-0.0.24/
+-rw-rw-r--   0 jms       (1000) jms       (1000)    32422 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/LICENSE
+-rw-r--r--   0 jms       (1000) jms       (1000)     5231 2024-04-08 08:46:04.587760 skilleter_thingy-0.0.24/PKG-INFO
+-rw-rw-r--   0 jms       (1000) jms       (1000)     4510 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/README.md
+-rw-rw-r--   0 jms       (1000) jms       (1000)     2868 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/pyproject.toml
+-rw-rw-r--   0 jms       (1000) jms       (1000)       38 2024-04-08 08:46:04.591760 skilleter_thingy-0.0.24/setup.cfg
+drwxrwxr-x   0 jms       (1000) jms       (1000)        0 2024-04-08 08:46:04.587760 skilleter_thingy-0.0.24/skilleter_thingy/
+-rw-rw-r--   0 jms       (1000) jms       (1000)        0 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/__init__.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     3842 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/addpath.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)    18614 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/aws.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     7832 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/borger.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)     7031 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/colour.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     1786 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/console_colours.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)     8539 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/dc_curses.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)     6170 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/dc_defaults.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)     1783 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/dc_util.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)    12268 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/dircolors.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     2072 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/diskspacecheck.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)     2453 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/docker.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     3359 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/docker_purge.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)    19373 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/ffind.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)     4261 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/files.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     2493 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/ggit.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     5876 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/ggrep.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)    37887 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/git.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)    35764 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/git2.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     5812 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/git_br.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     4981 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/git_ca.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)    10214 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/git_cleanup.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     8225 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/git_co.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     1892 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/git_common.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     4630 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/git_hold.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     3100 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/git_mr.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     2696 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/git_parent.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)    51276 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/git_review.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)    13985 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/git_update.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     3143 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/git_wt.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)    11279 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/gitcmp_helper.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)     6062 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/gitlab.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     8925 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/gitprompt.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     5964 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/gl.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)    22040 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/gphotosync.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     4316 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/linecount.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)     3107 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/logger.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     4470 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/moviemover.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)     4737 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/path.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     3178 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/photodupe.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     7823 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/phototidier.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)     2529 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/popup.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)     3565 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/process.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     4395 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/py_audit.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     9465 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/readable.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     4620 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/remdir.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)    17117 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/rmdupe.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     2639 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/rpylint.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)    12619 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/run.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)    13849 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/s3_sync.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     3266 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/splitpics.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     2539 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/strreplace.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)    11348 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/sysmon.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)    33712 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/tfm.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)    19829 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/tfm_pane.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     2993 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/tfparse.py
+-rw-rw-r--   0 jms       (1000) jms       (1000)     5402 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/tidy.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     2397 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/trimpath.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     3128 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/window_rename.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     4590 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/xchmod.py
+-rwxrwxr-x   0 jms       (1000) jms       (1000)     2868 2024-04-08 08:31:14.000000 skilleter_thingy-0.0.24/skilleter_thingy/yamlcheck.py
+drwxrwxr-x   0 jms       (1000) jms       (1000)        0 2024-04-08 08:46:04.587760 skilleter_thingy-0.0.24/skilleter_thingy.egg-info/
+-rw-r--r--   0 jms       (1000) jms       (1000)     5231 2024-04-08 08:46:04.000000 skilleter_thingy-0.0.24/skilleter_thingy.egg-info/PKG-INFO
+-rw-rw-r--   0 jms       (1000) jms       (1000)     2012 2024-04-08 08:46:04.000000 skilleter_thingy-0.0.24/skilleter_thingy.egg-info/SOURCES.txt
+-rw-rw-r--   0 jms       (1000) jms       (1000)        1 2024-04-08 08:46:04.000000 skilleter_thingy-0.0.24/skilleter_thingy.egg-info/dependency_links.txt
+-rw-rw-r--   0 jms       (1000) jms       (1000)     1971 2024-04-08 08:46:04.000000 skilleter_thingy-0.0.24/skilleter_thingy.egg-info/entry_points.txt
+-rw-rw-r--   0 jms       (1000) jms       (1000)       76 2024-04-08 08:46:04.000000 skilleter_thingy-0.0.24/skilleter_thingy.egg-info/requires.txt
+-rw-rw-r--   0 jms       (1000) jms       (1000)       17 2024-04-08 08:46:04.000000 skilleter_thingy-0.0.24/skilleter_thingy.egg-info/top_level.txt
```

### Comparing `skilleter_thingy-0.0.23/LICENSE` & `skilleter_thingy-0.0.24/LICENSE`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/PKG-INFO` & `skilleter_thingy-0.0.24/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skilleter_thingy
-Version: 0.0.23
+Version: 0.0.24
 Summary: A collection of useful utilities, mainly aimed at making Git more friendly
 Author-email: John Skilleter <john@skilleter.org.uk>
 Project-URL: Home, https://skilleter.org.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `skilleter_thingy-0.0.23/README.md` & `skilleter_thingy-0.0.24/README.md`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/pyproject.toml` & `skilleter_thingy-0.0.24/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "skilleter_thingy"
 
 # Version must be incremented to install updated Thingy
 
-version = "0.0.23"
+version = "0.0.24"
 
 authors = [
     {name="John Skilleter", email="john@skilleter.org.uk"},
 ]
 
 description = "A collection of useful utilities, mainly aimed at making Git more friendly"
```

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy/addpath.py` & `skilleter_thingy-0.0.24/skilleter_thingy/addpath.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy/aws.py` & `skilleter_thingy-0.0.24/skilleter_thingy/aws.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy/borger.py` & `skilleter_thingy-0.0.24/skilleter_thingy/borger.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy/colour.py` & `skilleter_thingy-0.0.24/skilleter_thingy/colour.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy/console_colours.py` & `skilleter_thingy-0.0.24/skilleter_thingy/console_colours.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy/dc_curses.py` & `skilleter_thingy-0.0.24/skilleter_thingy/dc_curses.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy/dc_defaults.py` & `skilleter_thingy-0.0.24/skilleter_thingy/dc_defaults.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy/dc_util.py` & `skilleter_thingy-0.0.24/skilleter_thingy/dc_util.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy/dircolors.py` & `skilleter_thingy-0.0.24/skilleter_thingy/dircolors.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy/diskspacecheck.py` & `skilleter_thingy-0.0.24/skilleter_thingy/diskspacecheck.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy/docker.py` & `skilleter_thingy-0.0.24/skilleter_thingy/docker.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy/docker_purge.py` & `skilleter_thingy-0.0.24/skilleter_thingy/docker_purge.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy/ffind.py` & `skilleter_thingy-0.0.24/skilleter_thingy/ffind.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy/files.py` & `skilleter_thingy-0.0.24/skilleter_thingy/files.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy/ggit.py` & `skilleter_thingy-0.0.24/skilleter_thingy/ggit.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy/ggrep.py` & `skilleter_thingy-0.0.24/skilleter_thingy/ggrep.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy/git.py` & `skilleter_thingy-0.0.24/skilleter_thingy/git.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy/git2.py` & `skilleter_thingy-0.0.24/skilleter_thingy/git2.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy/git_br.py` & `skilleter_thingy-0.0.24/skilleter_thingy/git_br.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy/git_ca.py` & `skilleter_thingy-0.0.24/skilleter_thingy/git_ca.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy/git_cleanup.py` & `skilleter_thingy-0.0.24/skilleter_thingy/git_cleanup.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy/git_co.py` & `skilleter_thingy-0.0.24/skilleter_thingy/git_co.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy/git_common.py` & `skilleter_thingy-0.0.24/skilleter_thingy/git_common.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy/git_hold.py` & `skilleter_thingy-0.0.24/skilleter_thingy/git_hold.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy/git_mr.py` & `skilleter_thingy-0.0.24/skilleter_thingy/git_mr.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy/git_parent.py` & `skilleter_thingy-0.0.24/skilleter_thingy/git_parent.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy/git_review.py` & `skilleter_thingy-0.0.24/skilleter_thingy/git_review.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy/git_update.py` & `skilleter_thingy-0.0.24/skilleter_thingy/git_update.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy/git_wt.py` & `skilleter_thingy-0.0.24/skilleter_thingy/git_wt.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy/gitcmp_helper.py` & `skilleter_thingy-0.0.24/skilleter_thingy/gitcmp_helper.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy/gitlab.py` & `skilleter_thingy-0.0.24/skilleter_thingy/gitlab.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy/gitprompt.py` & `skilleter_thingy-0.0.24/skilleter_thingy/gitprompt.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy/gl.py` & `skilleter_thingy-0.0.24/skilleter_thingy/gl.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy/gphotosync.py` & `skilleter_thingy-0.0.24/skilleter_thingy/gphotosync.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy/linecount.py` & `skilleter_thingy-0.0.24/skilleter_thingy/linecount.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy/logger.py` & `skilleter_thingy-0.0.24/skilleter_thingy/logger.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy/moviemover.py` & `skilleter_thingy-0.0.24/skilleter_thingy/moviemover.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy/path.py` & `skilleter_thingy-0.0.24/skilleter_thingy/path.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy/photodupe.py` & `skilleter_thingy-0.0.24/skilleter_thingy/photodupe.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy/phototidier.py` & `skilleter_thingy-0.0.24/skilleter_thingy/phototidier.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy/popup.py` & `skilleter_thingy-0.0.24/skilleter_thingy/popup.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy/process.py` & `skilleter_thingy-0.0.24/skilleter_thingy/process.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy/py_audit.py` & `skilleter_thingy-0.0.24/skilleter_thingy/py_audit.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy/readable.py` & `skilleter_thingy-0.0.24/skilleter_thingy/readable.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy/remdir.py` & `skilleter_thingy-0.0.24/skilleter_thingy/remdir.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy/rmdupe.py` & `skilleter_thingy-0.0.24/skilleter_thingy/rmdupe.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy/rpylint.py` & `skilleter_thingy-0.0.24/skilleter_thingy/rpylint.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy/run.py` & `skilleter_thingy-0.0.24/skilleter_thingy/run.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy/s3_sync.py` & `skilleter_thingy-0.0.24/skilleter_thingy/s3_sync.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy/splitpics.py` & `skilleter_thingy-0.0.24/skilleter_thingy/splitpics.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy/strreplace.py` & `skilleter_thingy-0.0.24/skilleter_thingy/strreplace.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy/sysmon.py` & `skilleter_thingy-0.0.24/skilleter_thingy/sysmon.py`

 * *Files 0% similar despite different names*

```diff
@@ -213,15 +213,15 @@
             scr.addstr(y+yo+1, x+xo+10, f'{n:<2}')
             scr.addstr(y+yo+1, x+xo+14, f'{cpu:5.1f}%')
             scr.addstr(y+yo+1, x+xo+23, f'{freq[n].current:8.2f}')
 
         yo += 1
 
         if yo > h-2:
-            xo += w/3
+            xo += w//3
             yo = 0
 
     x += w//2
 
     if first:
         scr.addstr(y+1, x, 'Context switches:')
         scr.addstr(y+2, x, 'Interrupts:')
```

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy/tfm.py` & `skilleter_thingy-0.0.24/skilleter_thingy/tfm.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy/tfm_pane.py` & `skilleter_thingy-0.0.24/skilleter_thingy/tfm_pane.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy/tfparse.py` & `skilleter_thingy-0.0.24/skilleter_thingy/tfparse.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy/tidy.py` & `skilleter_thingy-0.0.24/skilleter_thingy/tidy.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy/trimpath.py` & `skilleter_thingy-0.0.24/skilleter_thingy/trimpath.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy/window_rename.py` & `skilleter_thingy-0.0.24/skilleter_thingy/window_rename.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy/xchmod.py` & `skilleter_thingy-0.0.24/skilleter_thingy/xchmod.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy/yamlcheck.py` & `skilleter_thingy-0.0.24/skilleter_thingy/yamlcheck.py`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy.egg-info/PKG-INFO` & `skilleter_thingy-0.0.24/skilleter_thingy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skilleter_thingy
-Version: 0.0.23
+Version: 0.0.24
 Summary: A collection of useful utilities, mainly aimed at making Git more friendly
 Author-email: John Skilleter <john@skilleter.org.uk>
 Project-URL: Home, https://skilleter.org.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy.egg-info/SOURCES.txt` & `skilleter_thingy-0.0.24/skilleter_thingy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `skilleter_thingy-0.0.23/skilleter_thingy.egg-info/entry_points.txt` & `skilleter_thingy-0.0.24/skilleter_thingy.egg-info/entry_points.txt`

 * *Files identical despite different names*

