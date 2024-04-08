# Comparing `tmp/drops-1.1.4.tar.gz` & `tmp/drops-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drops-1.1.4.tar", last modified: Fri Mar 29 13:37:22 2024, max compression
+gzip compressed data, was "drops-1.1.5.tar", last modified: Mon Apr  8 08:51:19 2024, max compression
```

## Comparing `drops-1.1.4.tar` & `drops-1.1.5.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:37:22.030311 drops-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-29 13:37:17.000000 drops-1.1.4/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (127)       26 2024-03-29 13:37:17.000000 drops-1.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    52264 2024-03-29 13:37:22.030311 drops-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11022 2024-03-29 13:37:17.000000 drops-1.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-03-29 13:37:17.000000 drops-1.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 13:37:22.030311 drops-1.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:37:22.018311 drops-1.1.4/src/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:37:17.000000 drops-1.1.4/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:37:22.022311 drops-1.1.4/src/drops/
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-03-29 13:37:17.000000 drops-1.1.4/src/drops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:37:22.022311 drops-1.1.4/src/drops/console/
--rwxr-xr-x   0 runner    (1001) docker     (127)      737 2024-03-29 13:37:17.000000 drops-1.1.4/src/drops/console/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2165 2024-03-29 13:37:17.000000 drops-1.1.4/src/drops/console/main.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3299 2024-03-29 13:37:17.000000 drops-1.1.4/src/drops/console/main_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:37:22.026311 drops-1.1.4/src/drops/console/pkg/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3249 2024-03-29 13:37:17.000000 drops-1.1.4/src/drops/console/pkg/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17680 2024-03-29 13:37:17.000000 drops-1.1.4/src/drops/console/pkg/biz.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17692 2024-03-29 13:37:17.000000 drops-1.1.4/src/drops/console/pkg/cmd.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11553 2024-03-29 13:37:17.000000 drops-1.1.4/src/drops/console/pkg/config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4186 2024-03-29 13:37:17.000000 drops-1.1.4/src/drops/console/pkg/er.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1158 2024-03-29 13:37:17.000000 drops-1.1.4/src/drops/console/pkg/globa.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2616 2024-03-29 13:37:17.000000 drops-1.1.4/src/drops/console/pkg/helper.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      979 2024-03-29 13:37:17.000000 drops-1.1.4/src/drops/console/pkg/log.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4227 2024-03-29 13:37:17.000000 drops-1.1.4/src/drops/console/pkg/system.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       22 2024-03-29 13:37:17.000000 drops-1.1.4/src/drops/console/pkg/version.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      402 2024-03-29 13:37:17.000000 drops-1.1.4/src/drops/console/test.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7436 2024-03-29 13:37:17.000000 drops-1.1.4/src/drops/console/test_biz.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      978 2024-03-29 13:37:17.000000 drops-1.1.4/src/drops/console/test_cmd.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2145 2024-03-29 13:37:17.000000 drops-1.1.4/src/drops/console/test_config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2286 2024-03-29 13:37:17.000000 drops-1.1.4/src/drops/console/test_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:37:22.026311 drops-1.1.4/src/drops/docker_ops/
--rwxr-xr-x   0 runner    (1001) docker     (127)       26 2024-03-29 13:37:17.000000 drops-1.1.4/src/drops/docker_ops/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (127)     4230 2024-03-29 13:37:17.000000 drops-1.1.4/src/drops/docker_ops/docker-compose.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:37:22.026311 drops-1.1.4/src/drops/docker_ops/release/
--rwxr-xr-x   0 runner    (1001) docker     (127)      374 2024-03-29 13:37:17.000000 drops-1.1.4/src/drops/docker_ops/release/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:37:22.026311 drops-1.1.4/src/drops/docker_ops/release/web/
--rwxr-xr-x   0 runner    (1001) docker     (127)       72 2024-03-29 13:37:17.000000 drops-1.1.4/src/drops/docker_ops/release/web/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:37:22.026311 drops-1.1.4/src/drops/docker_ops/secret/
--rwxr-xr-x   0 runner    (1001) docker     (127)      159 2024-03-29 13:37:17.000000 drops-1.1.4/src/drops/docker_ops/secret/README.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:37:22.026311 drops-1.1.4/src/drops/docker_ops/secret/ssh/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:37:17.000000 drops-1.1.4/src/drops/docker_ops/secret/ssh/known_hosts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:37:22.026311 drops-1.1.4/src/drops/docker_ops/servers/
--rwxr-xr-x   0 runner    (1001) docker     (127)      205 2024-03-29 13:37:17.000000 drops-1.1.4/src/drops/docker_ops/servers/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:37:22.026311 drops-1.1.4/src/drops/docker_ops/servers/acme.sh/
--rwxr-xr-x   0 runner    (1001) docker     (127)      488 2024-03-29 13:37:17.000000 drops-1.1.4/src/drops/docker_ops/servers/acme.sh/redeploy-ssl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:37:22.026311 drops-1.1.4/src/drops/docker_ops/servers/drops/
--rwxr-xr-x   0 runner    (1001) docker     (127)      262 2024-03-29 13:37:17.000000 drops-1.1.4/src/drops/docker_ops/servers/drops/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:37:22.026311 drops-1.1.4/src/drops/docker_ops/servers/drops/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:37:17.000000 drops-1.1.4/src/drops/docker_ops/servers/drops/bin/.keep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:37:22.018311 drops-1.1.4/src/drops/docker_ops/servers/drops/cron/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:37:22.026311 drops-1.1.4/src/drops/docker_ops/servers/drops/cron/daily/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:37:17.000000 drops-1.1.4/src/drops/docker_ops/servers/drops/cron/daily/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:37:22.026311 drops-1.1.4/src/drops/docker_ops/servers/drops/cron/hourly/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:37:17.000000 drops-1.1.4/src/drops/docker_ops/servers/drops/cron/hourly/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:37:22.026311 drops-1.1.4/src/drops/docker_ops/servers/drops/cron/monthly/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:37:17.000000 drops-1.1.4/src/drops/docker_ops/servers/drops/cron/monthly/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:37:22.026311 drops-1.1.4/src/drops/docker_ops/servers/drops/cron/weekly/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:37:17.000000 drops-1.1.4/src/drops/docker_ops/servers/drops/cron/weekly/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:37:22.026311 drops-1.1.4/src/drops/docker_ops/servers/drops/cron_example/
--rwxr-xr-x   0 runner    (1001) docker     (127)      265 2024-03-29 13:37:17.000000 drops-1.1.4/src/drops/docker_ops/servers/drops/cron_example/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      751 2024-03-29 13:37:17.000000 drops-1.1.4/src/drops/docker_ops/servers/drops/cron_example/backup.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      190 2024-03-29 13:37:17.000000 drops-1.1.4/src/drops/docker_ops/servers/drops/cron_example/backupdb.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      491 2024-03-29 13:37:17.000000 drops-1.1.4/src/drops/docker_ops/servers/drops/cron_example/drops-backup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:37:22.026311 drops-1.1.4/src/drops/docker_ops/servers/drops/drops/
--rwxr-xr-x   0 runner    (1001) docker     (127)      139 2024-03-29 13:37:17.000000 drops-1.1.4/src/drops/docker_ops/servers/drops/drops/README.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:37:22.026311 drops-1.1.4/src/drops/docker_ops/servers/nginx/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:37:22.026311 drops-1.1.4/src/drops/docker_ops/servers/nginx/auth_basic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 13:37:17.000000 drops-1.1.4/src/drops/docker_ops/servers/nginx/auth_basic/metrics.pwd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:37:22.026311 drops-1.1.4/src/drops/docker_ops/servers/nginx/conf.d/
--rwxr-xr-x   0 runner    (1001) docker     (127)      347 2024-03-29 13:37:17.000000 drops-1.1.4/src/drops/docker_ops/servers/nginx/conf.d/drops.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:37:22.026311 drops-1.1.4/src/drops/docker_ops/servers/nginx/lib/
--rwxr-xr-x   0 runner    (1001) docker     (127)      228 2024-03-29 13:37:17.000000 drops-1.1.4/src/drops/docker_ops/servers/nginx/lib/gzip.conf
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-03-29 13:37:17.000000 drops-1.1.4/src/drops/docker_ops/servers/nginx/lib/metrics.conf
--rwxr-xr-x   0 runner    (1001) docker     (127)      557 2024-03-29 13:37:17.000000 drops-1.1.4/src/drops/docker_ops/servers/nginx/lib/referer.conf
--rwxr-xr-x   0 runner    (1001) docker     (127)      428 2024-03-29 13:37:17.000000 drops-1.1.4/src/drops/docker_ops/servers/nginx/lib/ssl.conf
--rwxr-xr-x   0 runner    (1001) docker     (127)      302 2024-03-29 13:37:17.000000 drops-1.1.4/src/drops/docker_ops/servers/nginx/lib/tohttps.conf
--rwxr-xr-x   0 runner    (1001) docker     (127)      892 2024-03-29 13:37:17.000000 drops-1.1.4/src/drops/docker_ops/servers/nginx/nginx.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:37:22.018311 drops-1.1.4/src/drops/docker_ops/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:37:22.030311 drops-1.1.4/src/drops/docker_ops/src/server/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:37:22.018311 drops-1.1.4/src/drops/docker_ops/src/server/cmd/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:37:22.030311 drops-1.1.4/src/drops/docker_ops/src/server/cmd/drops/
--rwxr-xr-x   0 runner    (1001) docker     (127)       49 2024-03-29 13:37:17.000000 drops-1.1.4/src/drops/docker_ops/src/server/cmd/drops/main.go
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:37:22.030311 drops-1.1.4/src/drops/docker_ops/src/server/cmd/te/
--rwxr-xr-x   0 runner    (1001) docker     (127)       46 2024-03-29 13:37:17.000000 drops-1.1.4/src/drops/docker_ops/src/server/cmd/te/main.go
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:37:22.030311 drops-1.1.4/src/drops/docker_ops/src/server/drops/
--rwxr-xr-x   0 runner    (1001) docker     (127)      861 2024-03-29 13:37:17.000000 drops-1.1.4/src/drops/docker_ops/src/server/drops/build.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       23 2024-03-29 13:37:17.000000 drops-1.1.4/src/drops/docker_ops/src/server/go.mod
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:37:22.030311 drops-1.1.4/src/drops/docker_ops/src/web/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:37:22.030311 drops-1.1.4/src/drops/docker_ops/src/web/drops/
--rwxr-xr-x   0 runner    (1001) docker     (127)      921 2024-03-29 13:37:17.000000 drops-1.1.4/src/drops/docker_ops/src/web/drops/build.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)       72 2024-03-29 13:37:17.000000 drops-1.1.4/src/drops/docker_ops/src/web/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:37:22.030311 drops-1.1.4/src/drops/docker_ops/var/
--rwxr-xr-x   0 runner    (1001) docker     (127)      156 2024-03-29 13:37:17.000000 drops-1.1.4/src/drops/docker_ops/var/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:37:22.018311 drops-1.1.4/src/drops/docker_ops/var/log/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:37:22.030311 drops-1.1.4/src/drops/docker_ops/var/log/nginx/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:37:17.000000 drops-1.1.4/src/drops/docker_ops/var/log/nginx/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:37:22.030311 drops-1.1.4/src/drops/docker_ops/volumes/
--rwxr-xr-x   0 runner    (1001) docker     (127)      465 2024-03-29 13:37:17.000000 drops-1.1.4/src/drops/docker_ops/volumes/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)       82 2024-03-29 13:37:17.000000 drops-1.1.4/src/drops/drops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:37:22.030311 drops-1.1.4/src/drops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    52264 2024-03-29 13:37:22.000000 drops-1.1.4/src/drops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-03-29 13:37:22.000000 drops-1.1.4/src/drops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 13:37:22.000000 drops-1.1.4/src/drops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-29 13:37:22.000000 drops-1.1.4/src/drops.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-29 13:37:22.000000 drops-1.1.4/src/drops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-29 13:37:22.000000 drops-1.1.4/src/drops.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:51:19.549757 drops-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-08 08:51:15.000000 drops-1.1.5/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (127)       26 2024-04-08 08:51:15.000000 drops-1.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    52577 2024-04-08 08:51:19.549757 drops-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11335 2024-04-08 08:51:15.000000 drops-1.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-08 08:51:15.000000 drops-1.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 08:51:19.549757 drops-1.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:51:19.541757 drops-1.1.5/src/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:51:15.000000 drops-1.1.5/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:51:19.541757 drops-1.1.5/src/drops/
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-08 08:51:15.000000 drops-1.1.5/src/drops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:51:19.541757 drops-1.1.5/src/drops/console/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      737 2024-04-08 08:51:15.000000 drops-1.1.5/src/drops/console/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1975 2024-04-08 08:51:15.000000 drops-1.1.5/src/drops/console/main.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3299 2024-04-08 08:51:15.000000 drops-1.1.5/src/drops/console/main_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:51:19.545757 drops-1.1.5/src/drops/console/pkg/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3249 2024-04-08 08:51:15.000000 drops-1.1.5/src/drops/console/pkg/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18707 2024-04-08 08:51:15.000000 drops-1.1.5/src/drops/console/pkg/biz.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19816 2024-04-08 08:51:15.000000 drops-1.1.5/src/drops/console/pkg/cmd.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11977 2024-04-08 08:51:15.000000 drops-1.1.5/src/drops/console/pkg/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4186 2024-04-08 08:51:15.000000 drops-1.1.5/src/drops/console/pkg/er.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1158 2024-04-08 08:51:15.000000 drops-1.1.5/src/drops/console/pkg/globa.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2616 2024-04-08 08:51:15.000000 drops-1.1.5/src/drops/console/pkg/helper.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      979 2024-04-08 08:51:15.000000 drops-1.1.5/src/drops/console/pkg/log.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4227 2024-04-08 08:51:15.000000 drops-1.1.5/src/drops/console/pkg/system.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       22 2024-04-08 08:51:15.000000 drops-1.1.5/src/drops/console/pkg/version.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      402 2024-04-08 08:51:15.000000 drops-1.1.5/src/drops/console/test.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7436 2024-04-08 08:51:15.000000 drops-1.1.5/src/drops/console/test_biz.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      978 2024-04-08 08:51:15.000000 drops-1.1.5/src/drops/console/test_cmd.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2145 2024-04-08 08:51:15.000000 drops-1.1.5/src/drops/console/test_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2286 2024-04-08 08:51:15.000000 drops-1.1.5/src/drops/console/test_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:51:19.545757 drops-1.1.5/src/drops/docker_ops/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       26 2024-04-08 08:51:15.000000 drops-1.1.5/src/drops/docker_ops/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4230 2024-04-08 08:51:15.000000 drops-1.1.5/src/drops/docker_ops/docker-compose.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:51:19.545757 drops-1.1.5/src/drops/docker_ops/release/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      374 2024-04-08 08:51:15.000000 drops-1.1.5/src/drops/docker_ops/release/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:51:19.545757 drops-1.1.5/src/drops/docker_ops/release/web/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       72 2024-04-08 08:51:15.000000 drops-1.1.5/src/drops/docker_ops/release/web/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:51:19.545757 drops-1.1.5/src/drops/docker_ops/secret/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      159 2024-04-08 08:51:15.000000 drops-1.1.5/src/drops/docker_ops/secret/README.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:51:19.545757 drops-1.1.5/src/drops/docker_ops/secret/ssh/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:51:15.000000 drops-1.1.5/src/drops/docker_ops/secret/ssh/known_hosts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:51:19.545757 drops-1.1.5/src/drops/docker_ops/servers/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      205 2024-04-08 08:51:15.000000 drops-1.1.5/src/drops/docker_ops/servers/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:51:19.545757 drops-1.1.5/src/drops/docker_ops/servers/acme.sh/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      488 2024-04-08 08:51:15.000000 drops-1.1.5/src/drops/docker_ops/servers/acme.sh/redeploy-ssl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:51:19.545757 drops-1.1.5/src/drops/docker_ops/servers/drops/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      262 2024-04-08 08:51:15.000000 drops-1.1.5/src/drops/docker_ops/servers/drops/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:51:19.545757 drops-1.1.5/src/drops/docker_ops/servers/drops/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:51:15.000000 drops-1.1.5/src/drops/docker_ops/servers/drops/bin/.keep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:51:19.537757 drops-1.1.5/src/drops/docker_ops/servers/drops/cron/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:51:19.545757 drops-1.1.5/src/drops/docker_ops/servers/drops/cron/daily/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:51:15.000000 drops-1.1.5/src/drops/docker_ops/servers/drops/cron/daily/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:51:19.545757 drops-1.1.5/src/drops/docker_ops/servers/drops/cron/hourly/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:51:15.000000 drops-1.1.5/src/drops/docker_ops/servers/drops/cron/hourly/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:51:19.545757 drops-1.1.5/src/drops/docker_ops/servers/drops/cron/monthly/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:51:15.000000 drops-1.1.5/src/drops/docker_ops/servers/drops/cron/monthly/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:51:19.545757 drops-1.1.5/src/drops/docker_ops/servers/drops/cron/weekly/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:51:15.000000 drops-1.1.5/src/drops/docker_ops/servers/drops/cron/weekly/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:51:19.545757 drops-1.1.5/src/drops/docker_ops/servers/drops/cron_example/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      265 2024-04-08 08:51:15.000000 drops-1.1.5/src/drops/docker_ops/servers/drops/cron_example/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      751 2024-04-08 08:51:15.000000 drops-1.1.5/src/drops/docker_ops/servers/drops/cron_example/backup.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      190 2024-04-08 08:51:15.000000 drops-1.1.5/src/drops/docker_ops/servers/drops/cron_example/backupdb.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      491 2024-04-08 08:51:15.000000 drops-1.1.5/src/drops/docker_ops/servers/drops/cron_example/drops-backup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:51:19.545757 drops-1.1.5/src/drops/docker_ops/servers/drops/drops/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      139 2024-04-08 08:51:15.000000 drops-1.1.5/src/drops/docker_ops/servers/drops/drops/README.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:51:19.545757 drops-1.1.5/src/drops/docker_ops/servers/nginx/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:51:19.545757 drops-1.1.5/src/drops/docker_ops/servers/nginx/auth_basic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 08:51:15.000000 drops-1.1.5/src/drops/docker_ops/servers/nginx/auth_basic/metrics.pwd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:51:19.549757 drops-1.1.5/src/drops/docker_ops/servers/nginx/conf.d/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      347 2024-04-08 08:51:15.000000 drops-1.1.5/src/drops/docker_ops/servers/nginx/conf.d/drops.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:51:19.549757 drops-1.1.5/src/drops/docker_ops/servers/nginx/lib/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      228 2024-04-08 08:51:15.000000 drops-1.1.5/src/drops/docker_ops/servers/nginx/lib/gzip.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-08 08:51:15.000000 drops-1.1.5/src/drops/docker_ops/servers/nginx/lib/metrics.conf
+-rwxr-xr-x   0 runner    (1001) docker     (127)      557 2024-04-08 08:51:15.000000 drops-1.1.5/src/drops/docker_ops/servers/nginx/lib/referer.conf
+-rwxr-xr-x   0 runner    (1001) docker     (127)      428 2024-04-08 08:51:15.000000 drops-1.1.5/src/drops/docker_ops/servers/nginx/lib/ssl.conf
+-rwxr-xr-x   0 runner    (1001) docker     (127)      302 2024-04-08 08:51:15.000000 drops-1.1.5/src/drops/docker_ops/servers/nginx/lib/tohttps.conf
+-rwxr-xr-x   0 runner    (1001) docker     (127)      892 2024-04-08 08:51:15.000000 drops-1.1.5/src/drops/docker_ops/servers/nginx/nginx.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:51:19.537757 drops-1.1.5/src/drops/docker_ops/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:51:19.549757 drops-1.1.5/src/drops/docker_ops/src/server/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:51:19.537757 drops-1.1.5/src/drops/docker_ops/src/server/cmd/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:51:19.549757 drops-1.1.5/src/drops/docker_ops/src/server/cmd/drops/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       49 2024-04-08 08:51:15.000000 drops-1.1.5/src/drops/docker_ops/src/server/cmd/drops/main.go
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:51:19.549757 drops-1.1.5/src/drops/docker_ops/src/server/cmd/te/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       46 2024-04-08 08:51:15.000000 drops-1.1.5/src/drops/docker_ops/src/server/cmd/te/main.go
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:51:19.549757 drops-1.1.5/src/drops/docker_ops/src/server/drops/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      861 2024-04-08 08:51:15.000000 drops-1.1.5/src/drops/docker_ops/src/server/drops/build.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       23 2024-04-08 08:51:15.000000 drops-1.1.5/src/drops/docker_ops/src/server/go.mod
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:51:19.549757 drops-1.1.5/src/drops/docker_ops/src/web/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:51:19.549757 drops-1.1.5/src/drops/docker_ops/src/web/drops/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      921 2024-04-08 08:51:15.000000 drops-1.1.5/src/drops/docker_ops/src/web/drops/build.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       72 2024-04-08 08:51:15.000000 drops-1.1.5/src/drops/docker_ops/src/web/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:51:19.549757 drops-1.1.5/src/drops/docker_ops/var/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      156 2024-04-08 08:51:15.000000 drops-1.1.5/src/drops/docker_ops/var/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:51:19.537757 drops-1.1.5/src/drops/docker_ops/var/log/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:51:19.549757 drops-1.1.5/src/drops/docker_ops/var/log/nginx/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:51:15.000000 drops-1.1.5/src/drops/docker_ops/var/log/nginx/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:51:19.549757 drops-1.1.5/src/drops/docker_ops/volumes/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      465 2024-04-08 08:51:15.000000 drops-1.1.5/src/drops/docker_ops/volumes/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)       82 2024-04-08 08:51:15.000000 drops-1.1.5/src/drops/drops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 08:51:19.549757 drops-1.1.5/src/drops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    52577 2024-04-08 08:51:19.000000 drops-1.1.5/src/drops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-04-08 08:51:19.000000 drops-1.1.5/src/drops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 08:51:19.000000 drops-1.1.5/src/drops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-08 08:51:19.000000 drops-1.1.5/src/drops.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-08 08:51:19.000000 drops-1.1.5/src/drops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-08 08:51:19.000000 drops-1.1.5/src/drops.egg-info/top_level.txt
```

### Comparing `drops-1.1.4/LICENSE` & `drops-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `drops-1.1.4/PKG-INFO` & `drops-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drops
-Version: 1.1.4
+Version: 1.1.5
 Summary: drops 是基于 ssh 和 docker-compose 的运维模板，附带的 drops 命令可以方便的管理项目，部署服务。
 Author-email: szerr <i@szerr.org>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -869,14 +869,26 @@
 
 `servers/nginx/lib` 中有几个可复用的配置
 
 `servers/nginx/nginx.conf` 可以选择开启的配置
 
 `servers/crond/periodic_example/drops-backup.py` 是一个异地备份脚本。
 
+## 测试与打包
+
+首先安装打包需要的依赖
+
+```sh
+pip install build
+```
+
+进入 script 目录，`build.sh` 生成包，`install.sh` 会先调用 `build.sh` ，并安装包到本地。
+
+执行 `release.py <版本号>`  更改版本信息，并用 `gh` 创建发布，联合 `workflows` 实现发包。
+
 ## 致谢
 
 感谢 [JetBrains](https://jb.gg/OpenSourceSupport) 提供的 IDE
 
 ## 如何贡献
 
 非常欢迎你的加入！[提一个 Issue](https://github.com/szerr/drops/issues/new) 或者提交一个 Pull Request。
```

### Comparing `drops-1.1.4/README.md` & `drops-1.1.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -177,14 +177,26 @@
 
 `servers/nginx/lib` 中有几个可复用的配置
 
 `servers/nginx/nginx.conf` 可以选择开启的配置
 
 `servers/crond/periodic_example/drops-backup.py` 是一个异地备份脚本。
 
+## 测试与打包
+
+首先安装打包需要的依赖
+
+```sh
+pip install build
+```
+
+进入 script 目录，`build.sh` 生成包，`install.sh` 会先调用 `build.sh` ，并安装包到本地。
+
+执行 `release.py <版本号>`  更改版本信息，并用 `gh` 创建发布，联合 `workflows` 实现发包。
+
 ## 致谢
 
 感谢 [JetBrains](https://jb.gg/OpenSourceSupport) 提供的 IDE
 
 ## 如何贡献
 
 非常欢迎你的加入！[提一个 Issue](https://github.com/szerr/drops/issues/new) 或者提交一个 Pull Request。
```

### Comparing `drops-1.1.4/pyproject.toml` & `drops-1.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "drops"
-version = "1.1.4"
+version = "1.1.5"
 authors = [
   { name="szerr", email="i@szerr.org" },
 ]
 description = "drops 是基于 ssh 和 docker-compose 的运维模板，附带的 drops 命令可以方便的管理项目，部署服务。"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
```

### Comparing `drops-1.1.4/src/drops/__init__.py` & `drops-1.1.5/src/drops/__init__.py`

 * *Files identical despite different names*

### Comparing `drops-1.1.4/src/drops/console/__init__.py` & `drops-1.1.5/src/drops/console/__init__.py`

 * *Files identical despite different names*

### Comparing `drops-1.1.4/src/drops/console/main.py` & `drops-1.1.5/src/drops/console/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -38,21 +38,16 @@
         from .pkg import version
         print(version.__version__)
         return 0
     pkg.globa.args = args
     # 调用相关命令，没有命令时打印 help
     if 'func' in args:
         if not args.debug:
-            try:
-                status = args.func(args)
-                return status
-            except Exception as e:
-                pkg.globa.thread_exit = True
-                print('Fatal:', type(e).__name__, ':', e)
-                return 126
+            status = args.func(args)
+            return status
         else:
             pkg.biz.log.set_level(pkg.biz.log.DEBUG)
             return args.func(args)
     else:
         parser.print_help()
     return 0
```

### Comparing `drops-1.1.4/src/drops/console/main_test.py` & `drops-1.1.5/src/drops/console/main_test.py`

 * *Files identical despite different names*

### Comparing `drops-1.1.4/src/drops/console/pkg/__init__.py` & `drops-1.1.5/src/drops/console/pkg/__init__.py`

 * *Files identical despite different names*

### Comparing `drops-1.1.4/src/drops/console/pkg/biz.py` & `drops-1.1.5/src/drops/console/pkg/biz.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import os
 import sys
 import threading
 import time
 import shutil
 import watchdog.events
 import watchdog.observers
-from fnmatch import fnmatch
+import fnmatch 
 
 import drops
 
 from . import er, log
 from . import system
 from . import config
 from . import globa
@@ -57,14 +57,46 @@
         env = config.gen_env_by_args(name, globa.args)
         config.Conf().init_template(name).set_env(
             env).save(globa.args.config)
     else:
         config.Conf().init_template(name).save(globa.args.config)
     return 0
 
+def git(project_name, gbin):
+    subprojects = config.get_conf().get_subprojects()
+    if project_name:
+        filtered = fnmatch.filter([i['name'] for i in subprojects], project_name)
+        subprojects = [i for i in subprojects if i['name'] in filtered]
+    if not subprojects:
+        log.error("匹配到 subprojects 为空，无事可做")
+        return -1
+
+    work_path = os.getcwd()
+    src_dir_name = 'src'
+    if not os.path.isdir(src_dir_name):
+        os.mkdir(src_dir_name)
+    os.chdir(src_dir_name)
+    src_path = os.getcwd()
+
+    if gbin == "clone":
+        get_bin = "git clone "
+        for s in subprojects:
+            run_bin = get_bin + s['url'] + ' ' + s['name']
+            print(os.getcwd() + " > " + run_bin)
+            system.system(run_bin)
+    elif gbin == "pull":
+        run_bin = "git pull "
+        for s in subprojects:
+            os.chdir(s['name'])
+            print(os.getcwd() + " > " + run_bin)
+            system.system(run_bin)
+        os.chdir(src_path)
+    os.chdir(work_path)
+    return 0
+
 
 def rsync2remotely(env, src, target, exclude=[]):
     # rsync 本地同步到远程路径
     exclude = ' --exclude '.join(['', './.gitignore',
                                  './.git', './'+globa.args.config, './src', './secret'] + exclude)
     if env.identity_file:
         b = 'rsync -avzP --del -e "ssh -p {port} -i {key_path}" {exclude} {src} {username}@{host}:{target}'
```

### Comparing `drops-1.1.4/src/drops/console/pkg/cmd.py` & `drops-1.1.5/src/drops/console/pkg/cmd.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import os
 import time
 
 from . import config
 from . import biz
 from . import er
 from . import globa
-
+from . import log
 
 def add_new_cmd(s):
     p = s.add_parser(
         'new', help='Create a drops project.')
     p.add_argument("project_path",  type=str,
                    help="项目路径，使用最后一个文件夹作为项目名。")
     p.set_defaults(func=new_cmd)
@@ -59,14 +59,75 @@
     p.add_argument("project_name", help="项目名。")
 
 
 def init_cmd(p):
     return biz.init_project(p.project_name, '.')
 
 
+def add_git_cmd(s):
+    p = s.add_parser(
+        'git', help='在 src 目录下对配置中 subprojects 进行 git 操作')
+    p.set_defaults(func=git_cmd)
+    p.add_argument("bin", help="clone, pull")
+    p.add_argument("project_name", help="项目名，支持通配符", nargs="?")
+
+
+def git_cmd(p):
+    subprojects = config.get_conf().get_subprojects()
+    config.get_conf().save()
+    if not subprojects:
+        print("subprojects 为空，无事可做。请执行 drops subproject add <项目名> <url> 添加项目")
+        return
+    return biz.git(p.project_name, p.bin)
+
+def add_subproject_cmd(s):
+    p = s.add_parser(
+        'subproject', help='管理 subproject')
+    p.set_defaults(func=subproject_cmd)
+    p.add_argument("bin", help="ls, add, remove, set")
+    p.add_argument("url", help="远程地址", default="", nargs="?")
+    p.add_argument("name", help="项目名", default="", nargs="?")
+
+
+def subproject_cmd(p):
+    conf = config.get_conf()
+    subprojects = conf.get_subprojects()
+    if not p.url and p.bin != "ls":
+        log.error("url 不能为空")
+        return -1
+    if not p.name:
+        p.name = os.path.splitext(os.path.basename(p.url))[0]
+    if p.bin == "add":
+        if p.name in [i["name"] for i in subprojects]:
+            log.error(p.name, "已存在")
+            return 1
+        subprojects.append({"name": p.name, "url": p.url})
+        conf.set_subprojects(subprojects)
+        conf.save()
+    elif p.bin == "set":
+        for s in subprojects:
+            if s['name'] == p.name:
+                s['url'] = p.url
+        conf.set_subprojects(subprojects)
+        conf.save()
+    elif p.bin == "remove":
+        if p.name in [i["name"] for i in subprojects]:
+            subprojects = [i for i in subprojects if i["name"] != p.name]
+            conf.set_subprojects(subprojects)
+            conf.save()
+        else:
+            log.error(p.name, "不存在")
+    elif p.bin == "ls":
+        for i in subprojects:
+            print(i["name"] + '\t' + i["url"])
+    else:
+        log.error("不支持的命令：", p.bin)
+        return 1
+    return 0
+
 def add_backup_cmd(s):
     p = s.add_parser(
         'backup', help='基于 rsync 的增量备份。')
     p.set_defaults(func=backup_cmd)
     p.add_argument('obj', type=str, default='volumes', choices=[
         'docker',  'release', 'servers', 'var', 'volumes', 'ops', 'all'], nargs='?',
         help='''备份项目。docker: docker-compose，ops 是除 var 和 volumes 的所有。默认 volumes''')
```

### Comparing `drops-1.1.4/src/drops/console/pkg/config.py` & `drops-1.1.5/src/drops/console/pkg/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,14 +181,16 @@
             c = yaml.load(fd.read(), Loader=yaml.Loader)
         if 'project' not in c:
             raise er.ConfigurationFileMissObj('project')
         if 'name' not in c['project']:
             raise er.ConfigurationFileMissObj('project.name')
         if 'env' not in c:
             c['env'] = {}
+        if 'subprojects' not in c:
+            c['subprojects'] = []
         self._data = c
         return self
 
     # 方便获取配置对象
     def __getattr__(self, name):
         # 自动获取参数和配置文件内容
         print(self._data['env'])
@@ -227,14 +229,20 @@
                 'deploy_path': '/srv/drops/example',
             }
         },
             'project': {
                 'name': name,
                 'default_env': 'local',
         },
+            'subprojects': [
+                {
+                    'name': 'clone_to_name',
+                    'url': 'git@github.com:szerr/drops.git'
+                }
+            ],
         }
         return self
 
     def set_env(self, env: Environment):
         if env.name:
             self._data['env'][env.name] = env.to_conf()
             return self
@@ -309,14 +317,20 @@
 
     def get_default_env(self) -> Environment:
         default_env = self._data.get('project', {}).get('default_env', None)
         if default_env:
             return self.get_env(default_env)
         raise er.NoDefaultEnvironmentIsSet
 
+    def get_subprojects(self):
+        return self._data['subprojects']
+    
+    def set_subprojects(self, subprojects):
+        self._data['subprojects'] = subprojects
+
 
 _CONF_OBJ = None
 
 
 def get_conf():
     global _CONF_OBJ
     if not _CONF_OBJ:
```

### Comparing `drops-1.1.4/src/drops/console/pkg/er.py` & `drops-1.1.5/src/drops/console/pkg/er.py`

 * *Files identical despite different names*

### Comparing `drops-1.1.4/src/drops/console/pkg/globa.py` & `drops-1.1.5/src/drops/console/pkg/globa.py`

 * *Files identical despite different names*

### Comparing `drops-1.1.4/src/drops/console/pkg/helper.py` & `drops-1.1.5/src/drops/console/pkg/helper.py`

 * *Files identical despite different names*

### Comparing `drops-1.1.4/src/drops/console/pkg/log.py` & `drops-1.1.5/src/drops/console/pkg/log.py`

 * *Files identical despite different names*

### Comparing `drops-1.1.4/src/drops/console/pkg/system.py` & `drops-1.1.5/src/drops/console/pkg/system.py`

 * *Files identical despite different names*

### Comparing `drops-1.1.4/src/drops/console/test_biz.py` & `drops-1.1.5/src/drops/console/test_biz.py`

 * *Files identical despite different names*

### Comparing `drops-1.1.4/src/drops/console/test_cmd.py` & `drops-1.1.5/src/drops/console/test_cmd.py`

 * *Files identical despite different names*

### Comparing `drops-1.1.4/src/drops/console/test_config.py` & `drops-1.1.5/src/drops/console/test_config.py`

 * *Files identical despite different names*

### Comparing `drops-1.1.4/src/drops/console/test_lib.py` & `drops-1.1.5/src/drops/console/test_lib.py`

 * *Files identical despite different names*

### Comparing `drops-1.1.4/src/drops/docker_ops/docker-compose.yaml` & `drops-1.1.5/src/drops/docker_ops/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `drops-1.1.4/src/drops/docker_ops/servers/drops/cron_example/backup.sh` & `drops-1.1.5/src/drops/docker_ops/servers/drops/cron_example/backup.sh`

 * *Files identical despite different names*

### Comparing `drops-1.1.4/src/drops/docker_ops/servers/nginx/lib/metrics.conf` & `drops-1.1.5/src/drops/docker_ops/servers/nginx/lib/metrics.conf`

 * *Files identical despite different names*

### Comparing `drops-1.1.4/src/drops/docker_ops/servers/nginx/lib/referer.conf` & `drops-1.1.5/src/drops/docker_ops/servers/nginx/lib/referer.conf`

 * *Files identical despite different names*

### Comparing `drops-1.1.4/src/drops/docker_ops/servers/nginx/nginx.conf` & `drops-1.1.5/src/drops/docker_ops/servers/nginx/nginx.conf`

 * *Files identical despite different names*

### Comparing `drops-1.1.4/src/drops/docker_ops/src/server/drops/build.py` & `drops-1.1.5/src/drops/docker_ops/src/server/drops/build.py`

 * *Files identical despite different names*

### Comparing `drops-1.1.4/src/drops/docker_ops/src/web/drops/build.sh` & `drops-1.1.5/src/drops/docker_ops/src/web/drops/build.sh`

 * *Files identical despite different names*

### Comparing `drops-1.1.4/src/drops.egg-info/PKG-INFO` & `drops-1.1.5/src/drops.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drops
-Version: 1.1.4
+Version: 1.1.5
 Summary: drops 是基于 ssh 和 docker-compose 的运维模板，附带的 drops 命令可以方便的管理项目，部署服务。
 Author-email: szerr <i@szerr.org>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -869,14 +869,26 @@
 
 `servers/nginx/lib` 中有几个可复用的配置
 
 `servers/nginx/nginx.conf` 可以选择开启的配置
 
 `servers/crond/periodic_example/drops-backup.py` 是一个异地备份脚本。
 
+## 测试与打包
+
+首先安装打包需要的依赖
+
+```sh
+pip install build
+```
+
+进入 script 目录，`build.sh` 生成包，`install.sh` 会先调用 `build.sh` ，并安装包到本地。
+
+执行 `release.py <版本号>`  更改版本信息，并用 `gh` 创建发布，联合 `workflows` 实现发包。
+
 ## 致谢
 
 感谢 [JetBrains](https://jb.gg/OpenSourceSupport) 提供的 IDE
 
 ## 如何贡献
 
 非常欢迎你的加入！[提一个 Issue](https://github.com/szerr/drops/issues/new) 或者提交一个 Pull Request。
```

### Comparing `drops-1.1.4/src/drops.egg-info/SOURCES.txt` & `drops-1.1.5/src/drops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

