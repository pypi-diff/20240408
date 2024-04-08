# Comparing `tmp/pycityagent-1.0.0.tar.gz` & `tmp/pycityagent-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycityagent-1.0.0.tar", last modified: Wed Feb 28 14:20:42 2024, max compression
+gzip compressed data, was "pycityagent-1.1.0.tar", last modified: Mon Apr  8 09:08:15 2024, max compression
```

## Comparing `pycityagent-1.0.0.tar` & `pycityagent-1.1.0.tar`

### file list

```diff
@@ -1,66 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 14:20:42.509921 pycityagent-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-02-28 14:20:33.000000 pycityagent-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-02-28 14:20:42.509921 pycityagent-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4310 2024-02-28 14:20:33.000000 pycityagent-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 14:20:42.501921 pycityagent-1.0.0/pycityagent/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-28 14:20:33.000000 pycityagent-1.0.0/pycityagent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 14:20:42.505921 pycityagent-1.0.0/pycityagent/ac/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-02-28 14:20:33.000000 pycityagent-1.0.0/pycityagent/ac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-02-28 14:20:33.000000 pycityagent-1.0.0/pycityagent/ac/ac.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-02-28 14:20:33.000000 pycityagent-1.0.0/pycityagent/ac/action.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-02-28 14:20:33.000000 pycityagent-1.0.0/pycityagent/ac/controled.py
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-02-28 14:20:33.000000 pycityagent-1.0.0/pycityagent/ac/converse.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-02-28 14:20:33.000000 pycityagent-1.0.0/pycityagent/ac/idle.py
--rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-02-28 14:20:33.000000 pycityagent-1.0.0/pycityagent/ac/shop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-02-28 14:20:33.000000 pycityagent-1.0.0/pycityagent/ac/trip.py
--rw-r--r--   0 runner    (1001) docker     (127)     9637 2024-02-28 14:20:33.000000 pycityagent-1.0.0/pycityagent/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 14:20:42.505921 pycityagent-1.0.0/pycityagent/brain/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-02-28 14:20:33.000000 pycityagent-1.0.0/pycityagent/brain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-02-28 14:20:33.000000 pycityagent-1.0.0/pycityagent/brain/brain.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-02-28 14:20:33.000000 pycityagent-1.0.0/pycityagent/brain/brainfc.py
--rw-r--r--   0 runner    (1001) docker     (127)    19125 2024-02-28 14:20:33.000000 pycityagent-1.0.0/pycityagent/brain/memory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 14:20:42.505921 pycityagent-1.0.0/pycityagent/brain/persistence/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 14:20:33.000000 pycityagent-1.0.0/pycityagent/brain/persistence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-28 14:20:33.000000 pycityagent-1.0.0/pycityagent/brain/persistence/social.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-02-28 14:20:33.000000 pycityagent-1.0.0/pycityagent/brain/persistence/spatial.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 14:20:42.505921 pycityagent-1.0.0/pycityagent/brain/reason/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 14:20:33.000000 pycityagent-1.0.0/pycityagent/brain/reason/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-02-28 14:20:33.000000 pycityagent-1.0.0/pycityagent/brain/reason/shop.py
--rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-02-28 14:20:33.000000 pycityagent-1.0.0/pycityagent/brain/reason/social.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-02-28 14:20:33.000000 pycityagent-1.0.0/pycityagent/brain/reason/trip.py
--rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-02-28 14:20:33.000000 pycityagent-1.0.0/pycityagent/brain/reason/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 14:20:42.505921 pycityagent-1.0.0/pycityagent/brain/retrive/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 14:20:33.000000 pycityagent-1.0.0/pycityagent/brain/retrive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-02-28 14:20:33.000000 pycityagent-1.0.0/pycityagent/brain/retrive/social.py
--rw-r--r--   0 runner    (1001) docker     (127)    18492 2024-02-28 14:20:33.000000 pycityagent-1.0.0/pycityagent/brain/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    13715 2024-02-28 14:20:33.000000 pycityagent-1.0.0/pycityagent/brain/sence.py
--rw-r--r--   0 runner    (1001) docker     (127)    29081 2024-02-28 14:20:33.000000 pycityagent-1.0.0/pycityagent/brain/static.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 14:20:42.505921 pycityagent-1.0.0/pycityagent/cc/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-02-28 14:20:33.000000 pycityagent-1.0.0/pycityagent/cc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-02-28 14:20:33.000000 pycityagent-1.0.0/pycityagent/cc/cc.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-28 14:20:33.000000 pycityagent-1.0.0/pycityagent/cc/conve.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-02-28 14:20:33.000000 pycityagent-1.0.0/pycityagent/cc/idle.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-02-28 14:20:33.000000 pycityagent-1.0.0/pycityagent/cc/shop.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-02-28 14:20:33.000000 pycityagent-1.0.0/pycityagent/cc/trip.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-02-28 14:20:33.000000 pycityagent-1.0.0/pycityagent/cc/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 14:20:42.505921 pycityagent-1.0.0/pycityagent/hubconnector/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-28 14:20:33.000000 pycityagent-1.0.0/pycityagent/hubconnector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-02-28 14:20:33.000000 pycityagent-1.0.0/pycityagent/hubconnector/hubconnector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 14:20:42.509921 pycityagent-1.0.0/pycityagent/image/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-28 14:20:33.000000 pycityagent-1.0.0/pycityagent/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5225 2024-02-28 14:20:33.000000 pycityagent-1.0.0/pycityagent/image/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-02-28 14:20:33.000000 pycityagent-1.0.0/pycityagent/simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 14:20:42.509921 pycityagent-1.0.0/pycityagent/st/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-02-28 14:20:33.000000 pycityagent-1.0.0/pycityagent/st/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3743 2024-02-28 14:20:33.000000 pycityagent-1.0.0/pycityagent/st/st.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 14:20:42.509921 pycityagent-1.0.0/pycityagent/urbanllm/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-28 14:20:33.000000 pycityagent-1.0.0/pycityagent/urbanllm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4341 2024-02-28 14:20:33.000000 pycityagent-1.0.0/pycityagent/urbanllm/urbanllm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 14:20:42.509921 pycityagent-1.0.0/pycityagent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-02-28 14:20:42.000000 pycityagent-1.0.0/pycityagent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-02-28 14:20:42.000000 pycityagent-1.0.0/pycityagent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 14:20:42.000000 pycityagent-1.0.0/pycityagent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-02-28 14:20:42.000000 pycityagent-1.0.0/pycityagent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-28 14:20:42.000000 pycityagent-1.0.0/pycityagent.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-02-28 14:20:33.000000 pycityagent-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-28 14:20:42.509921 pycityagent-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:08:15.525119 pycityagent-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-08 09:08:11.000000 pycityagent-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7448 2024-04-08 09:08:15.525119 pycityagent-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-04-08 09:08:11.000000 pycityagent-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:08:15.517119 pycityagent-1.1.0/pycityagent/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:08:15.517119 pycityagent-1.1.0/pycityagent/ac/
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/ac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/ac/ac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/ac/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/ac/action_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:08:15.521119 pycityagent-1.1.0/pycityagent/ac/citizen_actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/ac/citizen_actions/controled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/ac/citizen_actions/converse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/ac/citizen_actions/idle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/ac/citizen_actions/shop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/ac/citizen_actions/trip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/ac/controled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/ac/converse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/ac/hub_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/ac/idle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/ac/shop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/ac/sim_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/ac/trip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8165 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/agent_citizen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/agent_func.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:08:15.521119 pycityagent-1.1.0/pycityagent/brain/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/brain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/brain/brain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/brain/brainfc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21934 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/brain/memory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:08:15.521119 pycityagent-1.1.0/pycityagent/brain/persistence/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/brain/persistence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/brain/persistence/social.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/brain/persistence/spatial.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:08:15.521119 pycityagent-1.1.0/pycityagent/brain/reason/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/brain/reason/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/brain/reason/shop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/brain/reason/social.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/brain/reason/trip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/brain/reason/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:08:15.521119 pycityagent-1.1.0/pycityagent/brain/retrive/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/brain/retrive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/brain/retrive/social.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18492 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/brain/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27610 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/brain/sence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29081 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/brain/static.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:08:15.525119 pycityagent-1.1.0/pycityagent/cc/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/cc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/cc/cc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/cc/conve.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/cc/idle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/cc/shop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/cc/trip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/cc/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:08:15.525119 pycityagent-1.1.0/pycityagent/hubconnector/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/hubconnector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/hubconnector/hubconnector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:08:15.525119 pycityagent-1.1.0/pycityagent/image/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/image/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5200 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:08:15.525119 pycityagent-1.1.0/pycityagent/st/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/st/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/st/st.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:08:15.525119 pycityagent-1.1.0/pycityagent/urbanllm/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/urbanllm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4341 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pycityagent/urbanllm/urbanllm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:08:15.525119 pycityagent-1.1.0/pycityagent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7448 2024-04-08 09:08:15.000000 pycityagent-1.1.0/pycityagent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-08 09:08:15.000000 pycityagent-1.1.0/pycityagent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 09:08:15.000000 pycityagent-1.1.0/pycityagent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-08 09:08:15.000000 pycityagent-1.1.0/pycityagent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-08 09:08:15.000000 pycityagent-1.1.0/pycityagent.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-08 09:08:11.000000 pycityagent-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 09:08:15.525119 pycityagent-1.1.0/setup.cfg
```

### Comparing `pycityagent-1.0.0/LICENSE` & `pycityagent-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pycityagent-1.0.0/PKG-INFO` & `pycityagent-1.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycityagent
-Version: 1.0.0
+Version: 1.1.0
 Summary: LLM-based城市模拟器agent构建库
 Author-email: Yuwei Yan <pinkgranite86@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 FIBLAB
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -35,15 +35,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: dashscope>=1.14.0
 Requires-Dist: geojson>=3.1.0
 Requires-Dist: numpy>=1.26.3
 Requires-Dist: openai>=1.8.0
 Requires-Dist: Pillow>=10.2.0
-Requires-Dist: pycitysim>=1.8.0
+Requires-Dist: pycitysim>=1.12.2
 Requires-Dist: citystreetview>=1.1.0
 Requires-Dist: PyYAML>=6.0.1
 Requires-Dist: Requests>=2.31.0
 Requires-Dist: transitions>=0.9.0
 
 # Pycityagent
 
@@ -88,53 +88,80 @@
 
 citysim_request:
   simulator: 
     server: https://api-opencity-2x.fiblab.net:58081
   map_request:
     mongo_coll: map_beijing_extend_20240205
     cache_dir: ./cache
+  route_request: 
+    server: http://api-opencity-2x.fiblab.net:58082
   streetview_request:
     engine: baidumap / googlemap
-    mapAK: your baidumap AK (if baidumap)
-    proxy: your googlemap proxy (if googlemap, optional)
+    mapAK: baidumap api-key (if you use baidumap engine)
+    proxy: googlemap proxy (if you use googlemap engine)
 
 apphub_request:
   hub_url: https://api-opencity-2x.fiblab.net:58080
   app_id: your APP ID
   app_secret: your APP Secret
   profile_image: the profile image of your agent
 ```
 - Forget about **citysim_request**, let's focus on the other two.
 
 #### LLM_REQUEST
-- As you can tell, the whole CityAgent is based on the LLM, by now, there are three different parts of config items: **text_request**, **img_understand_request** and **img_generate_request**
+- As you can see, the whole CityAgent is based on the LLM, by now, there are three different parts of config items: **text_request**, **img_understand_request** and **img_generate_request**
 - By now, we support [**qwen**](https://tongyi.aliyun.com/) and [**openai**](https://openai.com/)
     - `Notice: Our environments are basically conducted with qwen. If you prefer to use openai, then you may encounter hardships. AND fell free to issue us.`
 - Get your **api_key** and chooce your **model**s
 
-### CITYSIM_REQUEST
-- There are no need to change the 'simulator' and 'map_request' config
-- 'streetview_request': this is the config used for streetview
-  - By now, we support 'baidumap' and 'googlemap'
-  - If you use 'baidumap', then you need to apply for a mapAK
-  - If you use 'googlemap', then you can config your own proxy by 'proxy' attribute
+#### CITYSIM_REQUEST
+- Most of the configuration options in this part are determined, such as **simulator.server**, **map_request.mongo_coll**, **route_request.server**
+- **map_request.cache_dir**: used for storing map data your machine, you can justify the target dir as you wish (**create the dir first**)
+- **streetview_request**: used for obtaining streetview images, by now, we support baidumap engine and googlemap engine
+  - if you choose baidumap engine, you need to get a baidumap api-key
+    ``` yaml
+    streetview_request:
+      engine: baidumap
+      mapAK: xxxx
+    ```
+  - if you choose googlemap engine, you need to provide your proxy address, for example:
+    ``` yaml
+    streetview_request:
+      engine: googlemap
+      proxy: 
+        http: http://xxxx
+        https: https://xxxx
+    ```
 
 #### APPHUB_REQUEST
-- This is basically used to connect with the backend.
+- Used for creating the connection between backend server and client.
 - Put your **app_id** and **app_secret** here.
+  - Create your account and apply in [Opencity website](https://opencity.fiblab.net/)
 
 ### Installation
-- Install from **pip** easily.
-```shell
-pip install pycityagent
-```
+#### PyPI Installation
+  - Install from **pip** easily.
+  ```shell
+  pip install pycityagent
+  ```
+
+#### Install from source code
+- Clone this repo
+- Install required packages
+  ``` shell
+  pip install -r requirements.txt
+  ```
+- Install **libGL.so.1**, if you ara using Linux with a suitable package manager: (apt for instance)
+  ``` shell
+  apt-get install libgl1
+  ```
 
 ### CODE and RUN
 - Check the **example** folder and copy files from it (`Remember replace the config file`)
-- Look at the Demo:
+- Look at the Demo: (A citizen Agent demo)
 ```python
 import yaml
 from pycityagent.simulator import Simulator
 from pycityagent.urbanllm import LLMConfig, UrbanLLM
 import asyncio
 import time
 
@@ -143,25 +170,26 @@
     with open('config_template.yaml', 'r') as file:
         config = yaml.safe_load(file)
     
     # get the simulator object
     smi = Simulator(config['citysim_request'])
     
     # get the person by person_id, return agent
-    agent = await smi.GetAgent("name_of_agent", 8)
+    agent = await smi.GetCitizenAgent("name_of_agent", 8)
 
     # Help you build unique agent by scratch/profile
     agent.Image.load_scratch('scratch_template.json')
 
     # Load Memory and assist the agent to understand "Opencity"
     agent.Brain.Memory.Spatial.MemoryLoad('spatial_knowledge_template.json')
     agent.Brain.Memory.Social.MemoryLoad('social_background_template.json')
 
     # Connect to apphub so you can interact with your agent in front end
     agent.ConnectToHub(config['apphub_request'])
+    agent.Bind()
 
     # Creat the soul (a LLM processor actually)
     llmConfig = LLMConfig(config['llm_request'])
     soul = UrbanLLM(llmConfig)
 
     # Add the soul to your agent
     agent.add_soul(soul)
```

### Comparing `pycityagent-1.0.0/README.md` & `pycityagent-1.1.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -41,53 +41,80 @@
 
 citysim_request:
   simulator: 
     server: https://api-opencity-2x.fiblab.net:58081
   map_request:
     mongo_coll: map_beijing_extend_20240205
     cache_dir: ./cache
+  route_request: 
+    server: http://api-opencity-2x.fiblab.net:58082
   streetview_request:
     engine: baidumap / googlemap
-    mapAK: your baidumap AK (if baidumap)
-    proxy: your googlemap proxy (if googlemap, optional)
+    mapAK: baidumap api-key (if you use baidumap engine)
+    proxy: googlemap proxy (if you use googlemap engine)
 
 apphub_request:
   hub_url: https://api-opencity-2x.fiblab.net:58080
   app_id: your APP ID
   app_secret: your APP Secret
   profile_image: the profile image of your agent
 ```
 - Forget about **citysim_request**, let's focus on the other two.
 
 #### LLM_REQUEST
-- As you can tell, the whole CityAgent is based on the LLM, by now, there are three different parts of config items: **text_request**, **img_understand_request** and **img_generate_request**
+- As you can see, the whole CityAgent is based on the LLM, by now, there are three different parts of config items: **text_request**, **img_understand_request** and **img_generate_request**
 - By now, we support [**qwen**](https://tongyi.aliyun.com/) and [**openai**](https://openai.com/)
     - `Notice: Our environments are basically conducted with qwen. If you prefer to use openai, then you may encounter hardships. AND fell free to issue us.`
 - Get your **api_key** and chooce your **model**s
 
-### CITYSIM_REQUEST
-- There are no need to change the 'simulator' and 'map_request' config
-- 'streetview_request': this is the config used for streetview
-  - By now, we support 'baidumap' and 'googlemap'
-  - If you use 'baidumap', then you need to apply for a mapAK
-  - If you use 'googlemap', then you can config your own proxy by 'proxy' attribute
+#### CITYSIM_REQUEST
+- Most of the configuration options in this part are determined, such as **simulator.server**, **map_request.mongo_coll**, **route_request.server**
+- **map_request.cache_dir**: used for storing map data your machine, you can justify the target dir as you wish (**create the dir first**)
+- **streetview_request**: used for obtaining streetview images, by now, we support baidumap engine and googlemap engine
+  - if you choose baidumap engine, you need to get a baidumap api-key
+    ``` yaml
+    streetview_request:
+      engine: baidumap
+      mapAK: xxxx
+    ```
+  - if you choose googlemap engine, you need to provide your proxy address, for example:
+    ``` yaml
+    streetview_request:
+      engine: googlemap
+      proxy: 
+        http: http://xxxx
+        https: https://xxxx
+    ```
 
 #### APPHUB_REQUEST
-- This is basically used to connect with the backend.
+- Used for creating the connection between backend server and client.
 - Put your **app_id** and **app_secret** here.
+  - Create your account and apply in [Opencity website](https://opencity.fiblab.net/)
 
 ### Installation
-- Install from **pip** easily.
-```shell
-pip install pycityagent
-```
+#### PyPI Installation
+  - Install from **pip** easily.
+  ```shell
+  pip install pycityagent
+  ```
+
+#### Install from source code
+- Clone this repo
+- Install required packages
+  ``` shell
+  pip install -r requirements.txt
+  ```
+- Install **libGL.so.1**, if you ara using Linux with a suitable package manager: (apt for instance)
+  ``` shell
+  apt-get install libgl1
+  ```
 
 ### CODE and RUN
 - Check the **example** folder and copy files from it (`Remember replace the config file`)
-- Look at the Demo:
+- Look at the Demo: (A citizen Agent demo)
 ```python
 import yaml
 from pycityagent.simulator import Simulator
 from pycityagent.urbanllm import LLMConfig, UrbanLLM
 import asyncio
 import time
 
@@ -96,25 +123,26 @@
     with open('config_template.yaml', 'r') as file:
         config = yaml.safe_load(file)
     
     # get the simulator object
     smi = Simulator(config['citysim_request'])
     
     # get the person by person_id, return agent
-    agent = await smi.GetAgent("name_of_agent", 8)
+    agent = await smi.GetCitizenAgent("name_of_agent", 8)
 
     # Help you build unique agent by scratch/profile
     agent.Image.load_scratch('scratch_template.json')
 
     # Load Memory and assist the agent to understand "Opencity"
     agent.Brain.Memory.Spatial.MemoryLoad('spatial_knowledge_template.json')
     agent.Brain.Memory.Social.MemoryLoad('social_background_template.json')
 
     # Connect to apphub so you can interact with your agent in front end
     agent.ConnectToHub(config['apphub_request'])
+    agent.Bind()
 
     # Creat the soul (a LLM processor actually)
     llmConfig = LLMConfig(config['llm_request'])
     soul = UrbanLLM(llmConfig)
 
     # Add the soul to your agent
     agent.add_soul(soul)
```

### Comparing `pycityagent-1.0.0/pycityagent/ac/controled.py` & `pycityagent-1.1.0/pycityagent/ac/controled.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.0.0/pycityagent/ac/converse.py` & `pycityagent-1.1.0/pycityagent/ac/converse.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.0.0/pycityagent/ac/shop.py` & `pycityagent-1.1.0/pycityagent/ac/shop.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.0.0/pycityagent/ac/trip.py` & `pycityagent-1.1.0/pycityagent/ac/trip.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.0.0/pycityagent/agent.py` & `pycityagent-1.1.0/pycityagent/agent.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,43 @@
 from abc import ABC, abstractmethod
-from typing import Optional, Union
+from typing import Optional, Union, Callable
 import PIL.Image as Image
 from PIL.Image import Image
 import asyncio
 import time
 from pycitysim.sim import CityClient
 
 from pycityagent.urbanllm import UrbanLLM
 from .urbanllm import UrbanLLM
 from .brain.brain import Brain
 from .hubconnector.hubconnector import HubConnector
-from .image.image import AgentImage
-from .ac.ac import ActionController
-from .cc.cc import CommondController
-from .st.st import StateTransformer
+from .ac import ActionController
+from .cc import CommandController
+from .st import StateTransformer
 
+class AgentType:
+    """
+    Agent类型
+
+    - Citizen = 1, 指城市居民类型agent——行动受城市规则限制
+    - Func = 2, 功能型agent——行动规则宽松——本质上模拟器无法感知到Func类型的agent
+    """
+    Citizen = 1
+    Func = 2
 
 class Template:
     """
     The basic template of Agent
     """
-    def __init__(self, name, server, soul:UrbanLLM=None, simulator=None, id:int=None) -> None:
-        self.agent_name = name
+    def __init__(self, name, server, type:AgentType, soul:UrbanLLM=None, simulator=None) -> None:
+        self._name = name
         self._client = CityClient(server)
+        self._type = type
         self._soul = soul
         self._simulator = simulator
-        self._id = id
 
     def add_soul(self, llm_engine:UrbanLLM):
         """
         为Agent添加soul(UrbanLLM)
         Add soul for Agent
 
         Args:
@@ -55,77 +63,54 @@
     """
     Agent
     """
     def __init__(
             self, 
             name:str, 
             server:str, 
+            type:AgentType,
             soul:UrbanLLM=None, 
-            simulator=None, 
-            id:int=None, 
-            base=None,
-            motion=None,
-            scratch_file:str=None,
-            selfie:bool = False,
-            connect_to_hub:bool=False,
-            hub_url:str=None,
-            app_id:int=None,
-            app_secret:str=None,
-            profile_img:str=None
+            simulator=None
         ) -> None:
-        super().__init__(name, server, soul, simulator, id)
-        self.base = base
-        """
-        Agent/Person的基本属性, Agent指被代理的Person, Person指模拟器中的背景人
-        The base attributes of Agent/Person. Agent is the Person being represented. Persons are background persons in simulator
-        - https://cityproto.sim.fiblab.net/#city.agent.v2.Agent
-        """
-        self.motion = motion
-        """
-        Agent/Person的运动信息
-        The motion information of Agent/Person
-        - https://cityproto.sim.fiblab.net/#city.agent.v2.AgentMotion
-        """
-        if connect_to_hub:
-            self._hub_connector = HubConnector(
-                hub_url=hub_url,
-                app_id=app_id,
-                app_secret=app_secret,
-                agent=self,
-                profile_img=profile_img
-            )
-        else:
-            self._hub_connector = None
-        self._image = AgentImage(self, scratch_file, selfie)
+        super().__init__(name, server, type, soul, simulator)
+
+        self._hub_connector = None
         """
-        Agent画像
-        The Agent's Image
+        HubConnector: 用于和AppHub对接——可以通过Agent.connectToHub进行绑定
+        HubConnector: the connection between agent and AppHub, you can use 'Agent.connectToHub' to create the connection
         """
+
         self._brain = Brain(self)
         """
         Agent的大脑
         The Agent's Brain
         """
-        self._ac = ActionController(self)
-        """
-        Agent的行为控制器
-        The Agent's ActionController
-        """
-        self._cc = CommondController(self)
+
+        self._cc = CommandController(self)
         """
         Agent的命令控制器
         The Agent's CommondController
         """
+
         self._st = StateTransformer()
         """
         与Agent关联的状态转移器
         The related StateTransformer
         """
-        # * 默认trip构建
-        self.Scheduler.schedule_init()
+
+        self._ac = ActionController(self)
+        """
+        Agent的行为控制器
+        The Agent's ActionController
+        """
+
+        self._step_with_action = True
+        """
+        Step函数是否包含action执行 —— 当有自定义action需求(特指包含没有指定source的Action)时可置该选项为False并通过自定义方法执行action操作
+        """
     
     def ConnectToHub(self, config:dict):
         """
         与AppHub构建连接
         Connect to AppHub
 
         Args:
@@ -137,14 +122,39 @@
         self._hub_connector = HubConnector(
             hub_url=config['hub_url'],
             app_id=config['app_id'],
             app_secret=config['app_secret'],
             agent=self,
             profile_img=profile_img
         )
+
+    def set_streetview_config(self, config:dict):
+        """
+        街景感知配置
+        - engine: baidumap / googlemap
+        - mapAK: your baidumap AK (if baidumap)
+        - proxy: your googlemap proxy (if googlemap, optional)
+        """
+        if 'engine' in config:
+            if config['engine'] == 'baidumap':
+                self.Brain.Sence._engine = config['engine']
+                if 'mapAK' in config:
+                    self.Brain.Sence._baiduAK = config['mapAK']
+                else:
+                    print("ERROR: Please Provide a baidumap AK")
+            elif config['engine'] == 'googlemap':
+                self.Brain.Sence._engine = config['engine']
+                if 'proxy' in config:
+                    self.Brain.Sence._googleProxy = config['proxy']
+                else:
+                    print("ERROR: Please provide a googlemap proxy")
+            else:
+                print("ERROR: Wrong engine, only baidumap / googlemap are available")
+        else:
+            print("ERROR: Please provide a streetview engine, baidumap / googlemap")
     
     def enable_streetview(self):
         """
         开启街景相关功能
         Enable Streetview function
         """
         self._brain.Sence.enable_streeview = True
@@ -166,59 +176,44 @@
     def disable_user_interaction(self):
         """
         关闭用户交互功能
         Disable User Interaction function
         """
         self._brain.Memory.Working.enable_user_interaction = False
 
-    def enable_economy_behavior(self):
-        """
-        开启经济模拟相关功能(例如购物)
-        Enable Economy function. Shopping for instance.
-        """
-        self.Brain.Memory.Working.enable_economy = True
-
-    def disable_economy_behavior(self):
-        """
-        关闭经济模拟相关功能
-        Disable Economy function
-        """
-        self.Brain.Memory.Working.enable_economy = False
-
-    def enable_social_behavior(self):
-        """
-        开启社交相关功能
-        Enable Social function
-        """
-        self.Brain.Memory.Working.enable_social = True
-
-    def diable_social_behavior(self):
+    def set_step_with_action(self, flag:bool = None):
         """
-        关闭社交相关功能
-        Disable Social function
+        默认情况置反step_with_action属性: 即True->False, False->True
+        否则根据传入的flag进行设置
         """
-        self.Brain.Memory.Working.enable_social = False
+        if flag != None:
+            self._step_with_action = flag
+        else:
+            self._step_with_action = not self._step_with_action
+        
 
-    async def Pause(self):
-        """
-        暂停Agent行为使Agent进入'pause'状态
-        Pause the Agent, making the agent 'pause'
+    def sence_config(self, sence_content:Optional[list]=None, sence_radius:int=None):
+        '''
+        感知配置
 
-        """
-        req = {'person_id': self.base['id'], 'schedules': []}
-        await self._client.person_service.SetSchedule(req)
-        self.Scheduler.unset_schedule()
-        self._st.trigger('pause')
-
-    async def Active(self):
-        """
-        恢复Agent行为
-        Recover from 'pause'
-        """
-        self._st.pause_back()
+        Args:
+        - config: 配置选项——包含需要感知的数据类型
+            - time: 时间
+            - poi: 感兴趣地点
+            - position: 可达地点
+            - lane: 周围道路
+            - person: 周围活动person
+            - streetview: 街景
+            - user_message: 用户交互信息
+            - agent_message: 智能体交互信息
+        '''
+        if sence_content != None:
+            self._brain._sence.set_sence(sence_content)
+        if sence_radius != None:
+            self._brain._sence.set_sence_radius(sence_radius)
 
     async def Run(self, round:int=1, interval:int=1, log:bool=True):
         """
         Agent执行入口
         The Agent Run entrance
 
         Args:
@@ -234,57 +229,16 @@
             await self.Step(log)
 
     async def Step(self, log:bool):
         """
         单步Agent执行流
         Single step entrance
         (Not recommended, use Run() method)
-
-        Args:
-        - log (bool): 是否输出log信息. Whether console log message
         """
-        if self.state != 'paused':
-            # * 1. 模拟器时间更新
-            await self._simulator.GetTime()
-            # * 2. 拉取Agent最新状态
-            resp = await self._client.person_service.GetPerson({'person_id':self._id})
-            self.base = resp['base']
-            self.motion = resp['motion']
-            # * 3. Brain工作流
-            await self._brain.Run()
-            # * 4. Commond Controller工作流
-            commond = await self._cc.Run()
-            # * 5. State Transformer工作流
-            self._st.trigger(commond)
-            # * 6. Action Controller工作流
-            await self._ac.Run()
-        if log:
-            print(f"---------------------- SIM TIME: {self._simulator.time} ----------------------")
-            self.show_yourself()
-    
-    def show_yourself(self):
-        """
-        Log信息输出
-        Pring log message
-        """
-        print(f"【State Message】: {self.state}")
-        motion_message = ''''''
-        motion_message += f'''行为状态: {self.motion['status']}, '''
-        if 'lane_position' in self.motion['position'].keys():
-            motion_message += f'''位置信息: lane-{self.motion['position']['lane_position']['lane_id']}'''
-        else:
-            motion_message += f'''位置信息: aoi-{self.motion['position']['aoi_position']['aoi_id']}'''
-        motion_message += f'''-[x: {self.motion['position']['xy_position']['x']}, y: {self.motion['position']['xy_position']['y']}]'''
-        print(f'【Simulator Motion Message】: \n{motion_message}')
-        print(self.Scheduler)
-    
-    @property
-    def Image(self):
-        """The Agent's Image"""
-        return self._image
+        pass
     
     @property
     def Soul(self):
         """The Agent's Soul(UrbanLLM)"""
         return self._soul
     
     @property
@@ -292,27 +246,27 @@
         """The Agent's Brain"""
         return self._brain
     
     @property
     def ActionController(self):
         """The Agents's ActionController"""
         return self._ac
-
-    @property
-    def Scheduler(self):
-        """The Agent's Scheduler"""
-        return self._brain.Memory.Working.scheduler
     
     @property
     def state(self):
         """The state of the Agent"""
-        return self._st.state
+        return self._st.machine.state
     
     @property
     def StateTransformer(self):
         """The StateTransformer of the Agent"""
         return self._st
 
     @property
     def Hub(self):
         """The connected AppHub"""
-        return self._hub_connector
+        return self._hub_connector
+    
+    @property
+    def CommandController(self):
+        """The command controller"""
+        return self._cc
```

### Comparing `pycityagent-1.0.0/pycityagent/brain/brain.py` & `pycityagent-1.1.0/pycityagent/brain/brain.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.0.0/pycityagent/brain/memory.py` & `pycityagent-1.1.0/pycityagent/brain/memory.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,71 +29,129 @@
 
     LongTermMemory (LTM): 长时记忆的存储
     Working Memory (WM): 当前工作记忆的存储
     """
     LTM = 1
     WM = 2
 
+class Memory(BrainFunction):
+    """
+    记忆模板类
+    The template class of Memory: defined as a BrainFunction
+    """
+    def __init__(self, agent, type:MemoryType) -> None:
+        super().__init__(agent)
+        self.type = type
+    
+    def Forward(self, x):
+        """
+        数据工作流
+        The data workflow
+        """
+
+    def MemorySave(self):
+        """
+        记忆存储
+        Save Memory
+        """
+
+    def MemoryLoad(self, x):
+        """
+        记忆恢复
+        Load Memory
+        """
+
+class WMemory(Memory):
+    def __init__(self, agent) -> None:
+        super().__init__(agent, MemoryType.WM)
+
+class LTMemory(Memory):
+    def __init__(self, agent) -> None:
+        super().__init__(agent, MemoryType.LTM)
+
 class MemoryRetrive:
     """
     用于从LTM中获取对应信息
     LTM retrive: get information from LTM
 
     Args:
     - source (str): the name of source LTM
     - out (str): the output name of retrived information
     - user_func (function): the defined function used for retriving
+    - des (str): description of this Retrive module
     """
-    def __init__(self, source:str, out:str, user_func) -> None:
+    def __init__(self, source:str, out:str, user_func, des:str="None") -> None:
         self.source = source
         self.out = out
         self.user_func = user_func
+        self.des = des
+
+    def __str__(self) -> str:
+        return self.des
 
 class MemoryReason:
     """
     基于WM的记忆推理与生成, 可以添加MemoryRetrive模块以获取关联信息
     Memory Reason: reason new information from WK, your can add a list of MemoryRetrive to get related information
 
     Args:
     - out (str): the output name of memory reason
     - user_func (function): the defined function used for reasoning
+    - des (str): description of this Reason module
     - retrivees (Optional[list[MemoryRetrive]]): a list of MemoryRetrive block that help to get related information from LTM
     """
-    def __init__(self, out:str, user_func, retrives:Optional[list[MemoryRetrive]]=None) -> None:
+    def __init__(self, out:str, user_func, des:str, retrives:Optional[list[MemoryRetrive]]=None) -> None:
         self.out = out
         self.user_func = user_func
         self.retrives = retrives
+        self.des = des
+
+    def __str__(self) -> str:
+        return self.des
 
 class MemoryPersistence:
     """
     记忆持久化: 将WM中的内容存储到LTM中
     Memory Persistence: store memory from WM to LTM
 
     Args:
     - target (str): the name of target LTM
     - user_func (function): the defined function used for persistence
+    - des (str): description of the Persistence module
     """
-    def __init__(self, target: str, user_func) -> None:
+    def __init__(self, target: str, user_func, des:str) -> None:
         self.target = target  # 指代的是目标记忆体
         self.user_func = user_func  # 用户注入的可执行函数
+        self.des = des
+
+    def __str__(self) -> str:
+        return self.des
 
 class MemoryController:
     """
     记忆管理器
     Memory Controller
     """
-    def __init__(self, agent, memory_config:dict=None) -> None:
+    def __init__(self, agent) -> None:
         self._agent = agent
         self._soul = agent._soul
-        if memory_config != None:
-            pass
-        else:
-            self._wm = WorkingMemory(agent)
-            self._spatial = SpatialMemory(agent)
-            self._social = SocialMemory(agent)
+        self._wm = WorkingMemory(agent)
+        self._spatial = SpatialMemory(agent)
+        self._social = SocialMemory(agent)
+
+    def add_LTM(self, name:str, ltm: LTMemory):
+        """
+        添加LTM
+        Add a LTM
+
+        Args:
+        - name (str): the attribute name, you can use the LTM by '.name'
+        - ltm (LTMemory)
+        """
+        setattr(self, name, ltm)
 
     async def Forward(self):
         """
         记忆模块主工作流
         Main working flow of Memory
         """
         await self._wm.senceReceive(self._agent.Brain.Sence.sence_buffer)
@@ -136,114 +194,57 @@
     def Soul(self):
         return self._soul
     
     @property 
     def Hub(self):
         return self._agent._hub
 
-class Memory(BrainFunction):
-    """
-    记忆模板类
-    The template class of Memory: defined as a BrainFunction
-    """
-    def __init__(self, agent, type:MemoryType) -> None:
-        super().__init__(agent)
-        self.type = type
-    
-    def Forward(self, x):
-        """
-        数据工作流
-        The data workflow
-        """
-
-    def MemorySave(self):
-        """
-        记忆存储
-        Save Memory
-        """
-
-    def MemoryLoad(self, x):
-        """
-        记忆恢复
-        Load Memory
-        """
-
-class WorkingMemory(Memory):
+class WorkingMemory(WMemory):
     """
     当前工作记忆
     Working Memory
     """
     def __init__(self, agent) -> None:
-        super().__init__(agent, MemoryType.WM)
+        super().__init__(agent)
         self.sence = None
         """
         用于存储感知内容
         Store the sence content
         """
+
         self.scheduler = Scheduler(agent)
         """
         关联的规划器
         The related Scheduler
         """
-        self.Reason = {}
-        """
-        用于存储Reason结果的buffer: key值为MemoryReason.out
-        """
-
-        # * agent social
-        self.agent_converse_buffer = defaultdict(lambda: BASE_CONVERSE_DIALOG+[
-            {'role': 'system', 'content': f'''[角色基本信息]: {self._agent.Image.get_profile()}'''}, 
-            {'role': 'system', 'content': f'''[角色的空间知识]: {self._agent.Brain.Memory.Spatial.to_dialog_str()}'''},
-            {'role': 'system', 'content': f'''[角色的社交关系]: {self._agent.Brain.Memory.Social.to_dialog_str()}'''}
-        ])
-        """
-        存储当前仍未结束的对话内容
-        Store the content of working conversation
-        """
 
-        self.hello_dialog = [
-            {'role': 'system', 'content': '你将基于用户提供的基本信息以及周围人物信息, 预测用户当前对哪个人最感兴趣, 是否会和该人物进行对话, 以及进行对话的理由'},
-            {'role': 'system', 'content': '其中基本信息包含用户的个人信息, 周围人物信息包含他人的基本信息以及用户对该人物的了解'},
-            {'role': 'system', 'content': '你只需要提供一个整数(该整数为对应人物的id)即可(请勿包含其他冗余信息)'},
-            {'role': 'system', 'content': '''你的回答需要严格按照以下格式给出(请勿包含其他冗余信息):
-            {"id": 感兴趣人物的id, "conve": 是否进行对话, 可选集合为[是, 否], 'explaination': 进行或不进行对话的理由}'''}
-        ]
-        """
-        Agent主动打招呼的system role dialog
-        The basic system role dialog used for saying hello
-        """
-
-        self.msg_agent_unhandle = {}  # dict of unhandle agent messages
-        """
-        存储未处理消息
-        Store unhandled agent messages
-        """
-
-        self.msg_agent_still = {}  # still on converse person_id
+        self.Reason = {}
         """
-        存储正在进行对话的person_id
-        Store the target person_id of conversations that still working
+        用于存储Reason结果的buffer: key值为Memory.Reason.out
         """
 
         # * user message related
         self.current_target = None
         """
         当前的目标
         Agent's current target
         """
+
         self.has_user_command = False
         """
         是否有用户指令
         Whether there have user commond
         """
-        self.user_converse_buffer = BASE_CONVERSE_DIALOG+[{'role': 'system', 'content': self._agent.Image.get_profile()}]
+
+        self.user_converse_buffer = BASE_CONVERSE_DIALOG+[{'role': 'system', 'content': ""}]
         """
         存储用户对话信息
         Store user conversation content
         """
+
         self.understanding_prompt = [
             {'role': 'system', 'content': '请你根据用户的输入内容，判断用户向你发起对话的用意并返回结果，返回的结果只能是[对话]或[控制]中的一个'},
             {'role': 'system', 'content': '其中[对话]表示用户只是想与你进行常规对话；[控制]表示用户想要控制你的行动'},
             {'role': 'system', 'content': '例如用户输入: 你好, 你的返回结果为: 对话'},
             {'role': 'system', 'content': '例如用户输入: 你现在立刻去附近买菜, 你的返回结果为: 控制'}
         ]
         """
@@ -252,80 +253,166 @@
         """
 
         self.msg_user_unhandle = []  # unhandle user messages
         """
         存储未处理的用户消息
         Store unhandled user messages
         """
+
         self.msg_user_processing = []  # processing user messages
         """
         存储正在处理的用户信息
         Store working user messages
         """
 
+        # * agent social
+        self.agent_converse_buffer = defaultdict(lambda: BASE_CONVERSE_DIALOG+[
+            {'role': 'system', 'content': f'''[角色基本信息]: {self._agent.Image.get_profile()}'''}, 
+            {'role': 'system', 'content': f'''[角色的空间知识]: {self._agent.Brain.Memory.Spatial.to_dialog_str()}'''},
+            {'role': 'system', 'content': f'''[角色的社交关系]: {self._agent.Brain.Memory.Social.to_dialog_str()}'''}
+        ])
+        """
+        存储当前仍未结束的对话内容
+        Store the content of working conversation
+        """
+
+        self.hello_dialog = [
+            {'role': 'system', 'content': '你将基于用户提供的基本信息以及周围人物信息, 预测用户当前对哪个人最感兴趣, 是否会和该人物进行对话, 以及进行对话的理由'},
+            {'role': 'system', 'content': '其中基本信息包含用户的个人信息, 周围人物信息包含他人的基本信息以及用户对该人物的了解'},
+            {'role': 'system', 'content': '你只需要提供一个整数(该整数为对应人物的id)即可(请勿包含其他冗余信息)'},
+            {'role': 'system', 'content': '''你的回答需要严格按照以下格式给出(请勿包含其他冗余信息):
+            {"id": 感兴趣人物的id, "conve": 是否进行对话, 可选集合为[是, 否], 'explaination': 进行或不进行对话的理由}'''}
+        ]
+        """
+        Agent主动打招呼的system role dialog
+        The basic system role dialog used for saying hello
+        """
+
+        self.msg_agent_unhandle = {}  # dict of unhandle agent messages
+        """
+        存储未处理消息
+        Store unhandled agent messages
+        """
+
+        self.msg_agent_still = {}  # still on converse person_id
+        """
+        存储正在进行对话的person_id
+        Store the target person_id of conversations that still working
+        """
+
         # * config
         self.enable_user_interaction = True
         self.enable_economy = True
         self.enable_social = True
 
         # * 信息提取
         self.retrive = {
-            'getfamilier': MemoryRetrive('Social', 'familiers', getfamilier)
+            'getfamilier': MemoryRetrive('Social', 'familiers', getfamilier, "source: social(LTM), destination: familiers")
         }
         """
         记忆索引模块集合
         The collection of MemoryRetrive blocks
             - key (str(MemoryRetrive.user_func))
             - value (MemoryRetrive)
         """
 
         # * reason - 推理/判断功能
         self.reason = {
             'idle': [
-                MemoryReason("hasUserControl", hasUserControl),
-                MemoryReason("startTrip", startTrip),
-                MemoryReason("agent_message_handle_resp", handleConve, [self.retrive['getfamilier']]),
-                MemoryReason("startConve", startConve),
-                MemoryReason("startShop", startShop)
+                MemoryReason("hasUserControl", hasUserControl, "(idle) weather has user control"),
+                MemoryReason("startTrip", startTrip, "(idle) weather to start trip"),
+                MemoryReason("agent_message_handle_resp", handleConve, "(idle) reason the responce for agent messages", [self.retrive['getfamilier']]),
+                MemoryReason("startConve", startConve, "(idle) weather start conversing with other agent"),
+                MemoryReason("startShop", startShop, "(idle) weather start shopping")
             ],
             'trip': [
-                MemoryReason("hasUserControl", hasUserControl),
-                MemoryReason("routeFailed", routeFailed),
-                MemoryReason("tripArrived", tripArrived)
+                MemoryReason("hasUserControl", hasUserControl, "(trip) weather has user control"),
+                MemoryReason("routeFailed", routeFailed, "(trip) weather route failed"),
+                MemoryReason("tripArrived", tripArrived, "(trip) weather arrived at the destination of current trip")
             ],
             'conve': [
-                MemoryReason("hasUserControl", hasUserControl),
-                MemoryReason("agent_message_handle_resp", handleConve, [self.retrive['getfamilier']]),
-                MemoryReason("endConve", endConve),
+                MemoryReason("hasUserControl", hasUserControl, "(conve) weather has user control"),
+                MemoryReason("agent_message_handle_resp", handleConve, "(conve) reason reason the responce for agent messages", [self.retrive['getfamilier']]),
+                MemoryReason("endConve", endConve, "(conve) weather end conversation"),
             ],
             'shop': [
-                 MemoryReason("hasUserControl", hasUserControl),
-                 MemoryReason("endShop", endShop)
+                 MemoryReason("hasUserControl", hasUserControl, "(shop) weather has user control"),
+                 MemoryReason("endShop", endShop, "(shop) weather end shop")
             ],
             'controled': [
-                MemoryReason("endUserControl", endUserControl)
+                MemoryReason("endUserControl", endUserControl, "(controled) weather end user control")
             ]
         }
         """
         记忆推理模块集合
         The collection of MemoryReason blocks
             - key (str): state
             - value (list[MemoryReason])
         Notice: 根据Agent当前状态执行对应列表中的MemoryReason. Execute those corresponding MemoryReason blocks based on Agent's state
         """
 
         # * persistence - 记忆持久化
         self.persistence = [
-            MemoryPersistence('Spatial', spacialPersistence)
+            MemoryPersistence('Spatial', spacialPersistence, "source: WM, destination: spatial(LTM)")
         ]
         """
         记忆持久化模块集合
         The collection of MemoryPersistence blocks
         """
 
+    def reset_retrive(self):
+        """
+        重置WM的retrive模块
+        """
+        self.retrive = {}
+
+    def add_retrive(self, name:str, retrive:MemoryRetrive):
+        """
+        添加索引模块
+
+        Args:
+        - name (str): the name of the retrive module
+        - retrive (MemoryRetrive)
+        """
+        self.retrive[name] = retrive
+
+    def reset_reason(self):
+        """
+        重置WM的推理模块
+        """
+        self.reason = {}
+
+    def add_reason(self, state:str, reason:MemoryReason):
+        """
+        添加Reason模块
+
+        Args:
+        - state (str): 该推理模块会在什么状态下被激活
+        - reason (MemoryReason)
+        """
+        if state in self.reason.keys():
+            self.reason[state].append(reason)
+        else:
+            self.reason[state] = [reason]
+
+    def reset_persistence(self):
+        """
+        重置WM的persistence模块
+        """
+        self.persistence = []
+
+    def add_persistence(self, persistence:MemoryPersistence):
+        """
+        添加持久化模块
+
+        Args:
+        - persistence (MemoryPersistence)
+        """
+        self.persistence.append(persistence)
+
     async def Forward(self):
         """
         WM主工作流
         The main workflow of WM
             - Reason
             - Persistence
             - (if need) Schedule
@@ -365,52 +452,59 @@
                     'content': content
                 }]
         # * user message
         self.msg_user_unhandle = sence['user_messages']
 
     async def runReason(self):
         '''推理模块执行'''
-        reason_line = self.reason[self._agent.state]
-        for reason in reason_line:
-            if reason.retrives == None:
-                self.Reason[reason.out] = await reason.user_func(self)
-            else:
-                retrives = {}
-                for retrive in reason.retrives:
-                    retrives[retrive.out] = await retrive.user_func(getattr(self.LTM, retrive.source))
-                self.Reason[reason.out] = await reason.user_func(self, retrives)
+        if self._agent.state in self.reason:
+            reason_line = self.reason[self._agent.state]
+            for reason in reason_line:
+                if reason.retrives == None:
+                    self.Reason[reason.out] = await reason.user_func(self)
+                else:
+                    retrives = {}
+                    for retrive in reason.retrives:
+                        retrives[retrive.out] = await retrive.user_func(getattr(self.LTM, retrive.source))
+                    self.Reason[reason.out] = await reason.user_func(self, retrives)
+        else:
+            print("Warning: No reason line for current agent's state")
 
     async def runPersistence(self):
         '''持久化模块执行'''
         for persis in self.persistence:
             mem = getattr(self._agent.Brain.Memory, persis.target)
             await persis.user_func(self, mem)
 
     def set_user_converse_background(self):
-        self.user_converse_buffer[2]['content'] = self._agent.Image.get_profile()
+        self.user_converse_buffer[3]['content'] = self._agent.Image.get_profile()
 
     @property
     def LTM(self):
         return self._agent.Brain.Memory
+    
+    @property
+    def Image(self):
+        return self._agent.Image
 
-class SpatialMemory(Memory):
+class SpatialMemory(LTMemory):
     """
     空间记忆 (LTM)
     SpatialMemory (LTM)
 
     空间记忆以location_node为基本组织单位, 每一个node被组织为一个dict, 包含以下属性
     The based unit of Spatial Memory is location_node, each node is presented as a dict, including following attributes:
         - id (int): the id of target location, '700426179' for instance
         - name (str): the name of target location, '清华大学' for instance
         - category (str): the category of target location, '教育学校' for instance
         - aoi_id (int): the related AOI's id, '500000011' for instance
         - relation (str): the relation between Agent and the location, '我在这里任职' for instance
     """
     def __init__(self, agent) -> None:
-        super().__init__(agent, MemoryType.LTM)
+        super().__init__(agent)
         self.constant = []
         """
         以列表形式存储的空间记忆: 基于文件载入的
         Spatial Memory in list: based on the MemoryLoad
         list[location_node]
         """
         self.sence = []
@@ -476,28 +570,28 @@
         """
         将空间信息转换为LLM可理解的文本
         Transfer Spatial Memory to LLM unstandable text
         """
         temp = self.constant + self.sence
         return json.dumps(temp, indent=0)
 
-class SocialMemory(Memory):
+class SocialMemory(LTMemory):
     """
     社交记忆 (LTM)
     Social Memory (LTM)
 
     社交记忆以person_node为基本组织单位, 每一个node被组织为一个dict, 包含以下属性
     The based unit of Social Memory is person_node, each node is presented as a dict, including following attributes:
         - id (int): person_id, '8' for instance
         - name (str): the name of person, '张三' for instance
         - relation (str): the relation between Agent and the target person, '亲密朋友' for instance
         - learned (str): the information that Agent learned about the target person, '他最近在学习AI' for instance
     """
     def __init__(self, agent) -> None:
-        super().__init__(agent, MemoryType.LTM)
+        super().__init__(agent)
         self.familiers = []
         """
         以列表形式存储社交记忆
         The Social Memory in list collection
         list[person_node]
         """
         self.familiers_dict = {}
```

### Comparing `pycityagent-1.0.0/pycityagent/brain/persistence/spatial.py` & `pycityagent-1.1.0/pycityagent/brain/persistence/spatial.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.0.0/pycityagent/brain/reason/shop.py` & `pycityagent-1.1.0/pycityagent/brain/reason/shop.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.0.0/pycityagent/brain/reason/social.py` & `pycityagent-1.1.0/pycityagent/brain/reason/social.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.0.0/pycityagent/brain/reason/trip.py` & `pycityagent-1.1.0/pycityagent/brain/reason/trip.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.0.0/pycityagent/brain/reason/user.py` & `pycityagent-1.1.0/pycityagent/brain/reason/user.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.0.0/pycityagent/brain/scheduler.py` & `pycityagent-1.1.0/pycityagent/brain/scheduler.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.0.0/pycityagent/brain/static.py` & `pycityagent-1.1.0/pycityagent/brain/static.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.0.0/pycityagent/cc/cc.py` & `pycityagent-1.1.0/pycityagent/cc/cc.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,102 +1,106 @@
 from typing import Any
 from .idle import *
 from .shop import *
 from .trip import *
 from .conve import *
 from .user import *
 
-class Commond:
+class Command:
     """
     BrainCommond: 即脑部发出的指令; The commond from Agent's Brain
 
     Args:
     - target (str): 即指令目标(状态转移指令). The commond target(state transformer)
     - user_func (func):
         - 自定义函数, 返回结果为bool类型, 如果返回True, 则表示执行target指令. Self-defined function, the return type is bool, if this function returns 'True', then forward the target commond.
     """
     def __init__(self, target:str, user_func) -> None:
         self.target = target
         self.user_func = user_func
 
-class CommondController:
+class CommandController:
     """
     Commond控制器模组: 连接Brain以及StateTranformer
     Commond Controller module: Used to connect the Brain module and StateTransformer module
     """
-    def __init__(self, agent, config=None) -> None:
+    def __init__(self, agent) -> None:
         '''默认初始化'''
         # TODO: config配置
         self._agent = agent
         self._brain = agent._brain
-        self.commond_control = {}
+        self.command_line = {}
         """
-        控制序列: 与state关联的BrainCommond集合
+        默认控制序列: 与state关联的BrainCommond集合
         Control Hub: connect the state with a BrainCommond collection
         Type: dict[str, list[BrainCommond]]
         Default:
             - idle: [whetherUserControl, whetherGoTrip, whetherGoShop, whetherGoConverse]
             - trip: [whetherUserControl, whetherRouteFailed, whetherTripArrived]
             - shop: [whetherUserControl, whetherShopFinished]
             - conve: [whetherUserControl, whetherStopConverse]
             - controled: [whetherEndControl]
         """
-        if config != None:
-            pass
-        else:
-            self.commond_control['idle'] = [
-                Commond('gousercontrol', whetherUserControl),
-                Commond('gotrip', whetherGoTrip),
-                Commond('goshop', whetherGoShop),
-                Commond('goconverse', whetherGoConverse)
-            ]
-            self.commond_control['trip'] = [
-                Commond('gousercontrol', whetherUserControl),
-                Commond('routefailed', whetherRouteFailed),
-                Commond('arrived', whetherTripArrived)
-            ]
-            self.commond_control['shop'] = [
-                Commond('gousercontrol', whetherUserControl),
-                Commond('shopdone', whetherShopFinished)
-            ]
-            self.commond_control['conve'] = [
-                Commond('gousercontrol', whetherUserControl),
-                Commond('convedone', whetherStopConverse)
-            ]
-            self.commond_control['controled'] = [
-                Commond('controlback', whetherEndControl)
-            ]
 
-    def insertCommond(self, target_state:list[str], commond:Commond):
+        self.command_line['idle'] = [
+            Command('gousercontrol', whetherUserControl),
+            Command('gotrip', whetherGoTrip),
+            Command('goshop', whetherGoShop),
+            Command('goconverse', whetherGoConverse)
+        ]
+        self.command_line['trip'] = [
+            Command('gousercontrol', whetherUserControl),
+            Command('routefailed', whetherRouteFailed),
+            Command('arrived', whetherTripArrived)
+        ]
+        self.command_line['shop'] = [
+            Command('gousercontrol', whetherUserControl),
+            Command('shopdone', whetherShopFinished)
+        ]
+        self.command_line['conve'] = [
+            Command('gousercontrol', whetherUserControl),
+            Command('convedone', whetherStopConverse)
+        ]
+        self.command_line['controled'] = [
+            Command('controlback', whetherEndControl)
+        ]
+
+    def reset_cc(self):
+        """
+        重置命令控制器
+        """
+        self.command_line = {}
+
+    def insert_command(self, target_state:list[str], command:Command):
         """
         插入指令
         Insert Commond: This function will insert the commond to those control sequences show in target_state
 
         Args:
         - target_state (list[str]): the list of state names
         - commond (Comond): the commond to be inserted
         """
         for target in target_state:
-            if target in self.commond_control.keys():
-                self.commond_control.append(commond)
+            if target in self.command_line.keys():
+                self.command_line[target].append(command)
             else:
-                self.commond_control[target] = [commond]
+                self.command_line[target] = [command]
 
     async def Run(self):
         """
         AC主执行函数
         The main function of AC
         Note: By now, AC do not support priority invoke. You can manipulate the sequnce of Commond to create fake priority
 
         Basic Logic: 
             - Based on the current state of Agent, AC invoke those functions in sequence
             - If there is a 'True' of function, returns the target commond
             - Else, return 'nothing' commond
         """
-        if self._agent.state not in self.commond_control.keys():
+        if self._agent.state not in self.command_line.keys():
             print(f"No commond control line match with current state: {self._agent.state}")
-        control_line = self.commond_control[self._agent.state]  # 获取agent状态对应的控制链
+        control_line = self.command_line[self._agent.state]  # 获取agent状态对应的控制链
         for control in control_line:
             result = await control.user_func(self._agent.Brain.Memory.Working)
             if result:
                 return control.target
         return 'nothing'
```

### Comparing `pycityagent-1.0.0/pycityagent/hubconnector/hubconnector.py` & `pycityagent-1.1.0/pycityagent/hubconnector/hubconnector.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,29 +14,17 @@
             self._client = None
         else:
             self._client = AppHubClient(
                             app_hub_url=hub_url,
                             app_id=app_id,
                             app_secret=app_secret
                         )
-        if agent == None:
-            self._agent = None
-            self._agent_id = None
-        else:
-            self._agent = agent
-            try:
-                self._agent_id = self._client.bind_person(
-                    self._agent.base['id'], 
-                    self._agent.agent_name, 
-                    Image.open(profile_img)
-                )
-            except Exception as e:
-                traceback.print_exc()
-                print(e)
-                self._agent_id = 7
+        self._agent = agent
+        self._agent_id = None
+        self._profile_img = profile_img
         self.messageBuffer:list[AgentMessage] = []
         """
         用于存储历史前端交互信息
         Used to store the history message in frontend
         """
 
     def ConnectToHub(self, hub_url:str, app_id:int, app_secret:str):
@@ -51,34 +39,37 @@
         """
         self._client = AppHubClient(
             app_hub_url=hub_url,
             app_id=app_id,
             app_secret=app_secret
         )
 
-    def BindAgent(self, agent, profile_img:str):
+    def BindCitizenAgent(self):
         """
-        绑定Agent
+        将CitizenAgent绑定到绑定Agent
         Bind an Agent through AppHub
-
-        Args:
-        - agent (Agent): the Agent needs to be bind with
-        - profile_img (str) : the path of profile_img, which will be shown in frontend and dashboard
         """
-        if self._client == None:
-            print("Not Connect To AppHub Yet")
-            return
-        self._agent = agent
         self._agent_id = self._client.bind_person(
-            self._agent.base['id'], 
-            self._agent.agent_name, 
-            Image.open(profile_img)
+            self._agent._id, 
+            self._agent._name, 
+            Image.open(self._profile_img)
+        )
+
+    def InsertFuncAgent(self):
+        """
+        将FuncAgent插入到AppHub中
+        Insert the Func Agent to AppHub
+        """
+        self._agent_id = self._client.bind_func(
+            self._agent._id,
+            self._agent._name,
+            Image.open(self._profile_img)
         )
 
-    def Update(self, messages:Optional[list[AgentMessage]]=None, streetview:Image=None, longlat:list[float]=None, pop:str=None):
+    def Update(self, messages:Optional[list[AgentMessage]]=None, streetview:Image.Image=None, longlat:list[float]=None, pop:str=None):
         """
         交互更新
         FrontEnd Related Update
         Note: This function is used by the lib developer. Normally, the user has no need to use this function
 
         Default Action: no message, no streetview, locate based on the Agent's position, Agent's name as pop
 
@@ -96,20 +87,21 @@
             - 气泡信息. The pop message
             - 默认为None(即没有气泡信息). Default: None(i.e. No pop message)
         """
         if self._client == None:
             print("AppHub: Not Bind Agent Yet")
             return
         else:
-            pop_ = self._agent.agent_name
+            pop_ = self._agent._name
             if pop != None:
                 pop_ = self._agent.agent_name + ": " + pop
-            longlat_ = [self._agent.motion['position']['longlat_position']['longitude'], self._agent.motion['position']['longlat_position']['latitude']]
             if longlat != None:
                 longlat_ = longlat
+            else:
+                longlat_ = [self._agent.motion['position']['longlat_position']['longitude'], self._agent.motion['position']['longlat_position']['latitude']]
             
             self._client.update_agent_map(
                 agent_id = self._agent_id, 
                 lnglat = longlat_,
                 street_view=streetview,
                 popup=pop_
             )
```

### Comparing `pycityagent-1.0.0/pycityagent/image/image.py` & `pycityagent-1.1.0/pycityagent/image/image.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,49 @@
 from typing import Optional
 import json
 from abc import ABC, abstractclassmethod
 
-class ProfileTemplate:
+
+class Image:
     """
-    profile模板类
-    The template class of Agent Profile
+    Image模块: 智能体画像
+    Agent's Image module: Defines the uniqueness of Agent
     """
-    def __init__(self) -> None:
-        pass
+    def __init__(self, agent) -> None:
+        self._agent = agent
+        self.scratch = Scratch()
+    
+    def get_profile(self):
+        """
+        获取Agent的Scratch Profile信息
+        Get the Scratch Profile message
 
-    @abstractclassmethod
-    def to_dialog(self) -> list[dict]:
+        Returns:
+        - (str)
         """
-        将Profile转化为LLM可用的dialog的抽象函数
-        The abstract method that turns Agent's profile to LLM standard dialog
+        return self.scratch.get_profile_content()
+    
+    def load_scratch(self, scratch_file:str):
         """
+        加载基于文件的Profile加载
+        Load Profile based on file
 
-class AgentImage:
+        Args:
+        - scratch_file (str): the path of scratch_file
+        """
+        self.scratch.load(scratch_file)
+
+class CitizenImage(Image):
     """
     Agent Image模块: 用户画像控制
     Agent's Image module: Defines the uniqueness of Agent
     """
     def __init__(self, agent, scratch_file:str=None, selfie:bool=False) -> None:
         self._agent = agent
-        self.scratch = AgentScratch()
+        self.scratch = CitizenScratch()
         """
         Agent的Scratch信息: 用于描述Agent的基本属性
         Scratch: Used to describe the basic info of Agent
         - name (str): the name of Agent
         - age (int): the age of Agent
         - education (str): the education level, ['低等教育水平', '中等教育水平', '高等教育水平']
         - gender (str): the gender of Agent, ['男', '女']
@@ -44,15 +59,15 @@
         Selfie of Agent
         Not implement yet!!!
         """
         profile = self._agent.base['profile']
         if scratch_file != None:
             self.scratch.load(scratch_file)
         else:
-            self.scratch.name = self._agent.agent_name
+            self.scratch.name = self._agent._name
             self.scratch.age = profile['age']
             education = profile['education']
             if education < 3:
                 self.scratch.education = '低等教育水平'
             elif education < 5:
                 self.scratch.education = '中等教育水平'
             else:
@@ -68,56 +83,27 @@
                 self.scratch.consumption = '高等消费水平'
             else:
                 self.scratch.consumption = '高等消费水平'
         if selfie:
             # TODO: 补充自拍
             pass
 
-    def get_profile(self):
-        """
-        获取Agent的Scratch Profile信息
-        Get the Scratch Profile message
-
-        Returns:
-        - (str)
-        """
-        return self.scratch.get_profile_content()
-    
-    def load_scratch(self, scratch_file:str):
-        """
-        加载基于文件的Profile加载
-        Load Profile based on file
-
-        Args:
-        - scratch_file (str): the path of scratch_file
-        """
-        self.scratch.load(scratch_file)
-
     def load_selfie(self, selfie_file:str):
         """
         基于图像的Selfie加载
         Load Selfie based on selfie file
         Not implemented yet!!!
 
         Args:
         - selfie_file (str): the path of selfie_file
         """
         print("Not Implemented")
 
-class AgentScratch():
-    def __init__(self, scratch:Optional[dict]=None) -> None:
-        self.name = None
-        self.age = None
-        self.education = None
-        self.gender = None
-        self.consumption = None
-        self.innate = ''
-        self.learned = ''
-        self.currently = ''
-        self.lifestyle = ''
+class Scratch:
+    def __init__(self, scratch: Optional[dict]=None) -> None:
         if scratch != None:
             self.forward(scratch)
 
     def forward(self, x:dict):
         """Scratch记忆更新"""
         for k in x.keys():
             self.__dict__[k] = x[k]
@@ -129,14 +115,33 @@
     
     def load(self, x:str):
         """Scratch记忆恢复"""
         with open(x, 'r') as f:
             json_str = f.read()
             scratch = json.loads(json_str)
             self.forward(scratch)
+
+    def get_profile_content(self):
+        text = ""
+        for attr_name, attr_value in self.__dict__.items():
+            text += f"{attr_name}: {attr_value}\n"
+        return text
+
+class CitizenScratch(Scratch):
+    def __init__(self, scratch:Optional[dict]=None) -> None:
+        super().__init__(scratch=scratch)
+        self.name = None
+        self.age = None
+        self.education = None
+        self.gender = None
+        self.consumption = None
+        self.innate = ''
+        self.learned = ''
+        self.currently = ''
+        self.lifestyle = ''
     
     def get_str_lifestyle(self):
         return self.lifestyle
     
     def get_str_firstname(self):
         return self.first_name
     
@@ -149,10 +154,9 @@
         text += f'消费能力: {self.consumption}\n'
         text += f'性格特点: {self.innate}\n'
         text += f'爱好与习惯: {self.learned}\n'
         text += f'近期状态: {self.currently}\n'
         text += f'生活习惯: {self.lifestyle}\n'
         return text
 
-
     def __str__(self):
         return str(self.__dict__)
```

### Comparing `pycityagent-1.0.0/pycityagent/simulator.py` & `pycityagent-1.1.0/pycityagent/simulator.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from pycitysim import *
-from pycitysim.sidecar import OnlyClientSidecar
+from pycitysim.routing import RoutingClient
 from pycitysim.sim import CityClient
 from typing import Optional, Union
 from datetime import datetime, timedelta
 import asyncio
-from .agent import Agent
+from .agent_citizen import CitizenAgent
+from .agent_func import FuncAgent
 
 class SimPerceive:
     """
     模拟器感知
     Simulator Perceive
     """
     def __init__(self, simualtor) -> None:
@@ -40,14 +41,15 @@
         self._perceive = SimPerceive(self)
         self.map = map.Map(
             mongo_uri = "mongodb://sim:FiblabSim1001@mgo.db.fiblab.tech:8635/",
             mongo_db = "srt",
             mongo_coll = config['map_request']['mongo_coll'],
             cache_dir = config['map_request']['cache_dir'],
         )
+        self.routing = RoutingClient(self.config['route_request']['server'], True)
         self.time = 0
 
     # * Agent相关
     def FindAgentsByArea(self, req: dict, status=None):
         """
         通过区域范围查找agent/person
         Get agents/persons in the provided area
@@ -68,64 +70,62 @@
             motions = []
             for agent in resp.motions:
                 if agent.status in status:
                     motions.append(agent)
             resp.motions = motions
             return resp
 
-    async def GetAgent(self, name:str=None, id:int=None):
+    async def GetCitizenAgent(self, name:str, id:int):
         """
         获取agent
         Get Agent
 
         Args:
         - name str: 你为agent取的名字 the name of your agent
         - id int: 即绑定的person的id the id of person that you try to bind with
         
         Returns:
-        - Agent
+        - CitizenAgent
         """
         await self.GetTime()
-        name_ = "张三"
-        if name != None:
-            name_ = name
-        if id == None:
-            base = self._client.person_service.default_person()
-            agent = Agent(
-                name_, 
-                self.config['simulator']['server'], 
-                simulator=self, 
-                id=id, 
-                base=base,
-            )
-        else:
-            resp = await self._client.person_service.GetPerson({"person_id": id})
-            base = resp['base']
-            motion = resp['motion']
-            agent = Agent(
-                name_, 
-                self.config['simulator']['server'], 
-                simulator=self, 
-                id=id, 
-                base=base,
-                motion=motion,
-            )
-        if 'streetview_request' in self.config.keys():
-            agent.Brain.Sence._streetview_engine = self.config['streetview_request']['engine']
-            if agent.Brain.Sence._streetview_engine == 'baidumap':
-                agent.Brain.Sence._streetviewAK = self.config['streetview_request']['mapAK']
-            elif agent.Brain.Sence._streetview_engine == 'googlemap':
-                if 'proxy' in self.config['streetview_request'].keys():
-                    agent.Brain.Sence._streetviewProxy = self.config['streetview_request']['proxy']
-            else:
-                agent.Brain.Sence._streetview_engine = ""
-                print("Wrong Streetview Engine")
+        resp = await self._client.person_service.GetPerson({"person_id": id})
+        base = resp['base']
+        motion = resp['motion']
+        agent = CitizenAgent(
+            name, 
+            self.config['simulator']['server'], 
+            simulator=self, 
+            id=id, 
+            base=base,
+            motion=motion
+        )
+        agent.set_streetview_config(self.config['streetview_request'])
+        return agent
+
+    async def GetFuncAgent(self, id:int, name:str):
+        """
+        获取一个Func Agent模板
+
+        Args:
+        - name (str): the name of your agent
+        - id (int): the unique id of agent
+
+        Returns:
+        - FuncAgent
+        """
+        agent = FuncAgent(
+                    name,
+                    id+10000000,
+                    self.config['simulator']['server'],
+                    simulator=self
+                )
+        agent.set_streetview_config(self.config['streetview_request'])
         return agent
 
-    def InsertAgent(self, profile):
+    def InsertCitizenAgent(self, profile):
         """
         插入agent
         Insert Agent
         Not implemented yet
         """
         print("Not Implemented Yet")
         pass
```

### Comparing `pycityagent-1.0.0/pycityagent/urbanllm/urbanllm.py` & `pycityagent-1.1.0/pycityagent/urbanllm/urbanllm.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.0.0/pycityagent.egg-info/PKG-INFO` & `pycityagent-1.1.0/pycityagent.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycityagent
-Version: 1.0.0
+Version: 1.1.0
 Summary: LLM-based城市模拟器agent构建库
 Author-email: Yuwei Yan <pinkgranite86@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 FIBLAB
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -35,15 +35,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: dashscope>=1.14.0
 Requires-Dist: geojson>=3.1.0
 Requires-Dist: numpy>=1.26.3
 Requires-Dist: openai>=1.8.0
 Requires-Dist: Pillow>=10.2.0
-Requires-Dist: pycitysim>=1.8.0
+Requires-Dist: pycitysim>=1.12.2
 Requires-Dist: citystreetview>=1.1.0
 Requires-Dist: PyYAML>=6.0.1
 Requires-Dist: Requests>=2.31.0
 Requires-Dist: transitions>=0.9.0
 
 # Pycityagent
 
@@ -88,53 +88,80 @@
 
 citysim_request:
   simulator: 
     server: https://api-opencity-2x.fiblab.net:58081
   map_request:
     mongo_coll: map_beijing_extend_20240205
     cache_dir: ./cache
+  route_request: 
+    server: http://api-opencity-2x.fiblab.net:58082
   streetview_request:
     engine: baidumap / googlemap
-    mapAK: your baidumap AK (if baidumap)
-    proxy: your googlemap proxy (if googlemap, optional)
+    mapAK: baidumap api-key (if you use baidumap engine)
+    proxy: googlemap proxy (if you use googlemap engine)
 
 apphub_request:
   hub_url: https://api-opencity-2x.fiblab.net:58080
   app_id: your APP ID
   app_secret: your APP Secret
   profile_image: the profile image of your agent
 ```
 - Forget about **citysim_request**, let's focus on the other two.
 
 #### LLM_REQUEST
-- As you can tell, the whole CityAgent is based on the LLM, by now, there are three different parts of config items: **text_request**, **img_understand_request** and **img_generate_request**
+- As you can see, the whole CityAgent is based on the LLM, by now, there are three different parts of config items: **text_request**, **img_understand_request** and **img_generate_request**
 - By now, we support [**qwen**](https://tongyi.aliyun.com/) and [**openai**](https://openai.com/)
     - `Notice: Our environments are basically conducted with qwen. If you prefer to use openai, then you may encounter hardships. AND fell free to issue us.`
 - Get your **api_key** and chooce your **model**s
 
-### CITYSIM_REQUEST
-- There are no need to change the 'simulator' and 'map_request' config
-- 'streetview_request': this is the config used for streetview
-  - By now, we support 'baidumap' and 'googlemap'
-  - If you use 'baidumap', then you need to apply for a mapAK
-  - If you use 'googlemap', then you can config your own proxy by 'proxy' attribute
+#### CITYSIM_REQUEST
+- Most of the configuration options in this part are determined, such as **simulator.server**, **map_request.mongo_coll**, **route_request.server**
+- **map_request.cache_dir**: used for storing map data your machine, you can justify the target dir as you wish (**create the dir first**)
+- **streetview_request**: used for obtaining streetview images, by now, we support baidumap engine and googlemap engine
+  - if you choose baidumap engine, you need to get a baidumap api-key
+    ``` yaml
+    streetview_request:
+      engine: baidumap
+      mapAK: xxxx
+    ```
+  - if you choose googlemap engine, you need to provide your proxy address, for example:
+    ``` yaml
+    streetview_request:
+      engine: googlemap
+      proxy: 
+        http: http://xxxx
+        https: https://xxxx
+    ```
 
 #### APPHUB_REQUEST
-- This is basically used to connect with the backend.
+- Used for creating the connection between backend server and client.
 - Put your **app_id** and **app_secret** here.
+  - Create your account and apply in [Opencity website](https://opencity.fiblab.net/)
 
 ### Installation
-- Install from **pip** easily.
-```shell
-pip install pycityagent
-```
+#### PyPI Installation
+  - Install from **pip** easily.
+  ```shell
+  pip install pycityagent
+  ```
+
+#### Install from source code
+- Clone this repo
+- Install required packages
+  ``` shell
+  pip install -r requirements.txt
+  ```
+- Install **libGL.so.1**, if you ara using Linux with a suitable package manager: (apt for instance)
+  ``` shell
+  apt-get install libgl1
+  ```
 
 ### CODE and RUN
 - Check the **example** folder and copy files from it (`Remember replace the config file`)
-- Look at the Demo:
+- Look at the Demo: (A citizen Agent demo)
 ```python
 import yaml
 from pycityagent.simulator import Simulator
 from pycityagent.urbanllm import LLMConfig, UrbanLLM
 import asyncio
 import time
 
@@ -143,25 +170,26 @@
     with open('config_template.yaml', 'r') as file:
         config = yaml.safe_load(file)
     
     # get the simulator object
     smi = Simulator(config['citysim_request'])
     
     # get the person by person_id, return agent
-    agent = await smi.GetAgent("name_of_agent", 8)
+    agent = await smi.GetCitizenAgent("name_of_agent", 8)
 
     # Help you build unique agent by scratch/profile
     agent.Image.load_scratch('scratch_template.json')
 
     # Load Memory and assist the agent to understand "Opencity"
     agent.Brain.Memory.Spatial.MemoryLoad('spatial_knowledge_template.json')
     agent.Brain.Memory.Social.MemoryLoad('social_background_template.json')
 
     # Connect to apphub so you can interact with your agent in front end
     agent.ConnectToHub(config['apphub_request'])
+    agent.Bind()
 
     # Creat the soul (a LLM processor actually)
     llmConfig = LLMConfig(config['llm_request'])
     soul = UrbanLLM(llmConfig)
 
     # Add the soul to your agent
     agent.add_soul(soul)
```

### Comparing `pycityagent-1.0.0/pycityagent.egg-info/SOURCES.txt` & `pycityagent-1.1.0/pycityagent.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 LICENSE
 README.md
 pyproject.toml
 pycityagent/__init__.py
 pycityagent/agent.py
+pycityagent/agent_citizen.py
+pycityagent/agent_func.py
 pycityagent/simulator.py
 pycityagent.egg-info/PKG-INFO
 pycityagent.egg-info/SOURCES.txt
 pycityagent.egg-info/dependency_links.txt
 pycityagent.egg-info/requires.txt
 pycityagent.egg-info/top_level.txt
 pycityagent/ac/__init__.py
 pycityagent/ac/ac.py
 pycityagent/ac/action.py
+pycityagent/ac/action_stream.py
 pycityagent/ac/controled.py
 pycityagent/ac/converse.py
+pycityagent/ac/hub_actions.py
 pycityagent/ac/idle.py
 pycityagent/ac/shop.py
+pycityagent/ac/sim_actions.py
 pycityagent/ac/trip.py
+pycityagent/ac/citizen_actions/controled.py
+pycityagent/ac/citizen_actions/converse.py
+pycityagent/ac/citizen_actions/idle.py
+pycityagent/ac/citizen_actions/shop.py
+pycityagent/ac/citizen_actions/trip.py
 pycityagent/brain/__init__.py
 pycityagent/brain/brain.py
 pycityagent/brain/brainfc.py
 pycityagent/brain/memory.py
 pycityagent/brain/scheduler.py
 pycityagent/brain/sence.py
 pycityagent/brain/static.py
```

### Comparing `pycityagent-1.0.0/pyproject.toml` & `pycityagent-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 requires-python = ">=3.8"
 dependencies = [
     "dashscope >= 1.14.0",
     "geojson >= 3.1.0",
     "numpy >= 1.26.3",
     "openai >= 1.8.0",
     "Pillow >= 10.2.0",
-    "pycitysim >= 1.8.0",
+    "pycitysim >= 1.12.2",
     "citystreetview >= 1.1.0",
     "PyYAML >= 6.0.1",
     "Requests >= 2.31.0",
     "transitions >= 0.9.0"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
```

