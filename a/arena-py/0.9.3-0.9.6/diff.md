# Comparing `tmp/arena-py-0.9.3.tar.gz` & `tmp/arena-py-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arena-py-0.9.3.tar", last modified: Fri Feb 23 19:43:02 2024, max compression
+gzip compressed data, was "arena-py-0.9.6.tar", last modified: Mon Apr  8 15:58:00 2024, max compression
```

## Comparing `arena-py-0.9.3.tar` & `arena-py-0.9.6.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 19:43:02.299580 arena-py-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-02-23 19:42:52.000000 arena-py-0.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-02-23 19:43:02.299580 arena-py-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-02-23 19:42:52.000000 arena-py-0.9.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 19:43:02.283580 arena-py-0.9.3/arena/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3148 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13453 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/arena_mqtt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 19:43:02.291580 arena-py-0.9.3/arena/attributes/
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/attributes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/attributes/animation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/attributes/animation_mixer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/attributes/armarker.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/attributes/attribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/attributes/attribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/attributes/blip.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/attributes/box_collision_listener.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/attributes/click_listener.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/attributes/color.py
--rw-r--r--   0 runner    (1001) docker     (127)     9947 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/attributes/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/attributes/dynamic_body.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/attributes/gltf_model_lod.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/attributes/gltf_morph.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/attributes/goto_landmark.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/attributes/goto_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/attributes/impulse.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/attributes/jitsi_video.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/attributes/landmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/attributes/material.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/attributes/material_extras.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/attributes/model_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/attributes/multisrc.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/attributes/position.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/attributes/remote_render.py
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/attributes/rotation.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/attributes/scale.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/attributes/shadow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/attributes/sound.py
--rw-r--r--   0 runner    (1001) docker     (127)     9349 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/attributes/spe_particles.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/attributes/static_body.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/attributes/textinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/attributes/translate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/attributes/video_control.py
--rw-r--r--   0 runner    (1001) docker     (127)    15849 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/base_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     4526 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 19:43:02.291580 arena-py-0.9.3/arena/event_loop/
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/event_loop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/event_loop/async_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/event_loop/asyncio_mqtt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/event_loop/event_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/event_loop/lazy_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/event_loop/persistent_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/event_loop/single_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/event_loop/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 19:43:02.291580 arena-py-0.9.3/arena/events/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/events/event.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 19:43:02.295580 arena-py-0.9.3/arena/objects/
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7182 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/objects/arena_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/objects/arenaui_button_panel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/objects/arenaui_card.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/objects/arenaui_prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/objects/box.py
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/objects/camera.py
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/objects/capsule.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/objects/circle.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/objects/cone.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/objects/cylinder.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/objects/dodecahedron.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/objects/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/objects/gaussian_splatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/objects/gltf_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/objects/hand_left.py
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/objects/hand_right.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/objects/icosahedron.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/objects/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/objects/light.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/objects/line.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/objects/ocean.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/objects/octahedron.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/objects/pcd_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/objects/plane.py
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/objects/program.py
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/objects/ring.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/objects/roundedbox.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/objects/sphere.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/objects/tetrahedron.py
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/objects/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/objects/thickline.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/objects/threejs_scene.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/objects/torus.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/objects/torus_knot.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/objects/triangle.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/objects/videosphere.py
--rw-r--r--   0 runner    (1001) docker     (127)    26972 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/scene.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 19:43:02.299580 arena-py-0.9.3/arena/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      122 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/scripts/arena_py_permissions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      557 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/scripts/arena_py_pub.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      118 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/scripts/arena_py_signout.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      559 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/scripts/arena_py_sub.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      229 2024-02-23 19:42:52.000000 arena-py-0.9.3/arena/scripts/arena_py_token.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 19:43:02.299580 arena-py-0.9.3/arena/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-02-23 19:42:53.000000 arena-py-0.9.3/arena/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6740 2024-02-23 19:42:53.000000 arena-py-0.9.3/arena/utils/arena_telemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-02-23 19:42:53.000000 arena-py-0.9.3/arena/utils/cmd_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5249 2024-02-23 19:42:53.000000 arena-py-0.9.3/arena/utils/program_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-02-23 19:42:53.000000 arena-py-0.9.3/arena/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-23 19:42:53.000000 arena-py-0.9.3/arena/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 19:43:02.299580 arena-py-0.9.3/arena_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-02-23 19:43:02.000000 arena-py-0.9.3/arena_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-02-23 19:43:02.000000 arena-py-0.9.3/arena_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 19:43:02.000000 arena-py-0.9.3/arena_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-02-23 19:43:02.000000 arena-py-0.9.3/arena_py.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-02-23 19:43:02.000000 arena-py-0.9.3/arena_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-23 19:43:02.000000 arena-py-0.9.3/arena_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-23 19:43:02.299580 arena-py-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-02-23 19:42:53.000000 arena-py-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:00.495318 arena-py-0.9.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-08 15:57:56.000000 arena-py-0.9.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-04-08 15:58:00.495318 arena-py-0.9.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-04-08 15:57:56.000000 arena-py-0.9.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:00.479318 arena-py-0.9.6/arena/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3147 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11638 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/arena_mqtt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:00.483318 arena-py-0.9.6/arena/attributes/
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/attributes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/attributes/animation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/attributes/animation_mixer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/attributes/armarker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/attributes/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/attributes/attribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/attributes/blip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/attributes/box_collision_listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/attributes/click_listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/attributes/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11351 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/attributes/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/attributes/dynamic_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/attributes/gltf_model_lod.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/attributes/gltf_morph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/attributes/goto_landmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/attributes/goto_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/attributes/impulse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/attributes/jitsi_video.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/attributes/landmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5350 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/attributes/material.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/attributes/material_extras.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/attributes/model_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/attributes/multisrc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/attributes/position.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/attributes/remote_render.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/attributes/rotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/attributes/scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/attributes/shadow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/attributes/sound.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9348 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/attributes/spe_particles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/attributes/static_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/attributes/textinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/attributes/translate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/attributes/video_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15550 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/base_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4526 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:00.487318 arena-py-0.9.6/arena/event_loop/
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/event_loop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/event_loop/async_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/event_loop/asyncio_mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/event_loop/event_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/event_loop/lazy_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/event_loop/persistent_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/event_loop/single_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/event_loop/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:00.487318 arena-py-0.9.6/arena/events/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/events/event.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:00.491318 arena-py-0.9.6/arena/objects/
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7182 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/objects/arena_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/objects/arenaui_button_panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/objects/arenaui_card.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/objects/arenaui_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/objects/box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/objects/camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/objects/capsule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/objects/circle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/objects/cone.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/objects/cylinder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/objects/dodecahedron.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/objects/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/objects/gaussian_splatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/objects/gltf_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/objects/hand_left.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/objects/hand_right.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/objects/icosahedron.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/objects/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/objects/light.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/objects/line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/objects/ocean.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/objects/octahedron.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/objects/pcd_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/objects/plane.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/objects/program.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/objects/ring.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/objects/roundedbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/objects/sphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/objects/tetrahedron.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/objects/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/objects/thickline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/objects/threejs_scene.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/objects/torus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/objects/torus_knot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/objects/triangle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/objects/videosphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30122 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/scene.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:00.495318 arena-py-0.9.6/arena/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      122 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/scripts/arena_py_permissions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      557 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/scripts/arena_py_pub.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      118 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/scripts/arena_py_signout.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      559 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/scripts/arena_py_sub.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      229 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/scripts/arena_py_token.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:00.495318 arena-py-0.9.6/arena/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6740 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/utils/arena_telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/utils/cmd_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5249 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/utils/program_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-08 15:57:56.000000 arena-py-0.9.6/arena/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:58:00.495318 arena-py-0.9.6/arena_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-04-08 15:58:00.000000 arena-py-0.9.6/arena_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-04-08 15:58:00.000000 arena-py-0.9.6/arena_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 15:58:00.000000 arena-py-0.9.6/arena_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-08 15:58:00.000000 arena-py-0.9.6/arena_py.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-08 15:58:00.000000 arena-py-0.9.6/arena_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-08 15:58:00.000000 arena-py-0.9.6/arena_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 15:58:00.495318 arena-py-0.9.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-08 15:57:56.000000 arena-py-0.9.6/setup.py
```

### Comparing `arena-py-0.9.3/LICENSE` & `arena-py-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `arena-py-0.9.3/PKG-INFO` & `arena-py-0.9.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: arena-py
-Version: 0.9.3
+Version: 0.9.6
 Summary: Draw objects and run programs in the ARENA using Python!
 Home-page: https://github.com/arenaxr/arena-py
-Author: Conix Research Center
-Author-email: info@conix.io
+Author: Carnegie Mellon University
+Author-email: arenaxr@andrew.cmu.edu
 License: BSD 3-clause "New" or "Revised License"
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -16,14 +16,15 @@
 Requires-Dist: paho-mqtt~=1.5.1
 Requires-Dist: requests~=2.28.1
 Requires-Dist: webcolors~=1.3
 Requires-Dist: google_auth_oauthlib~=1.0.0
 Requires-Dist: google-auth~=2.22.0
 Requires-Dist: PyJWT~=2.4.0
 Requires-Dist: opentelemetry-exporter-otlp-proto-grpc==1.21.*
+Requires-Dist: numpy>=1.22.0
 
 # arena-py
 Draw objects and run programs in the ARENA using Python!
 
 ## Documentation
 The ARENA Python library user guide and tutorials:
 [ARENA Documentation: Python](https://docs.arenaxr.org/content/python/).
```

### Comparing `arena-py-0.9.3/README.md` & `arena-py-0.9.6/README.md`

 * *Files identical despite different names*

### Comparing `arena-py-0.9.3/arena/__main__.py` & `arena-py-0.9.6/arena/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
     parser.add_argument("-a", "--action",
                         help=f"Action to do ({PUBLISH} or {SUBSCRIBE})",
                         choices=(PUBLISH, SUBSCRIBE),
                         required=True)
 
     parser.add_argument("-t", "--topic",
                         type=str,
-                        help=f"Custom topic to publish/subscribe to")
+                        help="Custom topic to publish/subscribe to")
     parser.add_argument("-m", "--message",
                         type=str,
                         help=f"Message to send (ignored when action={SUBSCRIBE})")
 
     args = parser.parse_args()
 
     main(**vars(args))
```

### Comparing `arena-py-0.9.3/arena/arena_mqtt.py` & `arena-py-0.9.6/arena/arena_mqtt.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,23 @@
-import argparse
 import asyncio
 import json
 import os
 import random
 import socket
 import ssl
 import sys
 from datetime import datetime
 
 import paho.mqtt.client as mqtt
 
 from .auth import ArenaAuth
+from .env import (ARENA_PASSWORD, ARENA_USERNAME, MQTTH, NAMESPACE, REALM,
+                  _get_env)
 from .event_loop import *
 
-from .env import (
-    MQTTH,
-    REALM,
-    ARENA_USERNAME,
-    ARENA_PASSWORD,
-    NAMESPACE,
-    _get_env
-)
 
 class ArenaMQTT(object):
     """
     Wrapper around Paho MQTT client and EventLoop.
     """
 
     scene = None
@@ -104,18 +97,18 @@
         self.config_url = f"https://{self.web_host}/conf/defaults.json"
         self.config_data = json.loads(self.auth.urlopen(self.config_url))
 
         self.mqtt_host = self.config_data["ARENADefaults"]["mqttHost"]
 
         # set up topic variables
         if self.scene:
-            self.namespaced_target =  f"{self.namespace}/{self.scene}"
+            self.namespaced_target = f"{self.namespace}/{self.scene}"
             self.root_topic = f"{self.realm}/s/{self.namespaced_target}"
         elif self.device:
-            self.namespaced_target =  f"{self.namespace}/{self.device}"
+            self.namespaced_target = f"{self.namespace}/{self.device}"
             self.root_topic = f"{self.realm}/d/{self.namespaced_target}"
         self.subscribe_topic = f"{self.root_topic}/#"   # main topic for entire target
         self.latency_topic = self.config_data["ARENADefaults"]["latencyTopic"] # network graph latency update
         self.ignore_topic = f"{self.root_topic}/{self.mqttc_id}/#" # ignore own messages
 
         self.mqttc = mqtt.Client(
             self.mqttc_id, clean_session=True
@@ -162,61 +155,26 @@
 
         self.msg_queue = asyncio.Queue()
 
         # connect to mqtt broker
         if "port" in kwargs:
             port = kwargs["port"]
         else:
-            port = 8883 # ARENA broker TLS 1.2 connection port
+            port = 8883  # ARENA broker TLS 1.2 connection port
         if self.auth.verify(self.web_host):
             self.mqttc.tls_set()
         else:
             self.mqttc.tls_set_context(ssl._create_unverified_context())
             self.mqttc.tls_insecure_set(True)
         try:
             self.mqttc.connect(self.mqtt_host, port=port, keepalive=60)
         except Exception as err:
             print(f'MQTT connect error to {self.mqtt_host}, port={port}: Result Code={err}')
         self.mqttc.socket().setsockopt(socket.SOL_SOCKET, socket.SO_SNDBUF, 2048)
 
-    def parse_cli(self):
-        """
-        Reusable command-line options to give apps flexible options to avoid hard-coding locations.
-        """
-        parser = argparse.ArgumentParser(description=("arena-py Application CLI"))
-        parser.add_argument("-mh", "--host", type=str,
-                            help="ARENA webserver main host to connect to")
-        parser.add_argument("-n", "--namespace", type=str,
-                            help="Namespace of scene")
-        parser.add_argument("-s", "--scene", type=str,
-                            help="Scene to publish and listen to")
-        parser.add_argument("-d", "--device", type=str,
-                            help="Device to publish and listen to")
-        parser.add_argument("-p", "--position", nargs=3, type=float, default=(0, 0, 0),
-                            help="App position as cartesian.x cartesian.y cartesian.z")
-        parser.add_argument("-r", "--rotation", nargs=3, type=float, default=(0, 0, 0),
-                            help="App rotation as euler.x euler.y euler.z")
-        parser.add_argument("-c", "--scale", nargs=3, type=float, default=(1, 1, 1),
-                            help="App scale in meters")
-        parser.add_argument("-D", "--debug", action='store_true', help='Debug mode.', default=False)
-        args = parser.parse_args()
-        app_position = tuple(args.position)
-        app_rotation = tuple(args.rotation)
-        app_scale = tuple(args.scale)
-        return {
-            "host": args.host,
-            "namespace": args.namespace,
-            "scene": args.scene,
-            "device": args.device,
-            "position": app_position,
-            "rotation": app_rotation,
-            "scale": app_scale,
-            "debug": args.debug,
-        }
-
     def generate_client_id(self):
         """Returns a random 6 digit id"""
         return str(random.randrange(100000, 999999))
 
     def network_latency_update(self):
         """Update client latency in $NETWORK/latency"""
         # publish empty message with QoS of 2 to update latency
@@ -335,19 +293,18 @@
         self.mqttc.message_callback_add(sub, callback)
 
     def message_callback_remove(self, sub):
         """Unsubscribes to topic and removes callback"""
         self.mqttc.unsubscribe(sub)
         self.mqttc.message_callback_remove(sub)
 
-    def rcv_queue_len(self): 
+    def rcv_queue_len(self):
         """Return receive queue length"""
         self.msg_queue.qsize()
-        
-    def pub_queue_len(self): 
+
+    def pub_queue_len(self):
         """Return publish queue length"""
         return self.mqttc._out_packet
 
-    def client_id(self): 
+    def client_id(self):
         """Return client id"""
         return self.mqttc_id
-
```

### Comparing `arena-py-0.9.3/arena/attributes/__init__.py` & `arena-py-0.9.6/arena/attributes/__init__.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.9.3/arena/attributes/animation.py` & `arena-py-0.9.6/arena/attributes/animation.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,32 +2,32 @@
 from .attribute import Attribute
 from .position import Position
 from .rotation import Rotation
 from .scale import Scale
 
 class Animation(Attribute):
     """
-    Animation attribute class to manage its properties in the ARENA: Animate and tween values.  More properties at (https://aframe.io/docs/1.5.0/components/animation.html) A-Frame Animation component. Easing properties are detailed at (https://easings.net) easings.net.
-    Usage: animation=Animation(...)
-    
+    Animation attribute class to manage its properties in the ARENA: Animate and tween values. More properties at <https://aframe.io/docs/1.5.0/components/animation.html> A-Frame Animation component. Easing properties are detailed at <https://easings.net> easings.net.
+    Usage: `animation=Animation(...)`
+
     :param bool autoplay: Whether or not the animation should autoplay. Should be specified if the animation is defined for the animation-timeline component (currently not supported). Defaults to 'True' (optional)
     :param float delay: How long (milliseconds) to wait before starting. (optional)
     :param str dir: Which dir to go from from to to. Allows [normal, alternate, reverse] Defaults to 'normal' (optional)
     :param float dur: How long (milliseconds) each cycle of the animation is. Defaults to '1000' (optional)
     :param str easing: Easing function of animation. To ease in, ease out, ease in and out. See easings.net for more. Allows [easeInQuad, easeInCubic, easeInQuart, easeInQuint, easeInSine, easeInExpo, easeInCirc, easeInBack, easeInElastic, easeOutQuad, easeOutCubic, easeOutQuart, easeOutQuint, easeOutSine, easeOutExpo, easeOutCirc, easeOutBack, easeOutElastic, easeInOutQuad, easeInOutCubic, easeInOutQuart, easeInOutQuint, easeInOutSine, easeInOutExpo, easeInOutCirc, easeInOutBack, easeInOutElastic, linear] Defaults to 'easeInQuad' (optional)
     :param float elasticity: How much to bounce (higher is stronger). Defaults to '400' (optional)
     :param bool enabled: If disabled, animation will stop and startEvents will not trigger animation start. Defaults to 'True' (optional)
     :param str from: Initial value at start of animation. If not specified, the current property value of the entity will be used (will be sampled on each animation start). It is best to specify a from value when possible for stability. (optional)
     :param bool isRawProperty: Flag to animate an arbitrary object property outside of A-Frame components for better performance. If set to true, for example, we can set property to like components.material.material.opacity. If property starts with components or object3D, this will be inferred to true. (optional)
     :param str loop: How many times the animation should repeat. If the value is true, the animation will repeat infinitely. (optional)
-    :param list[dict] pauseEvents: Comma-separated list of events to listen to trigger pause. Can be resumed with resumeEvents. (optional)
+    :param list[str] pauseEvents: Comma-separated list of events to listen to trigger pause. Can be resumed with resumeEvents. (optional)
     :param str property: Property to animate. Can be a component name, a dot-delimited property of a component (e.g., material.color), or a plain attribute. (optional)
-    :param list[dict] resumeEvents: Comma-separated list of events to listen to trigger resume after pausing. (optional)
+    :param list[str] resumeEvents: Comma-separated list of events to listen to trigger resume after pausing. (optional)
     :param bool round: Whether to round values. (optional)
-    :param list[dict] startEvents: Comma-separated list of events to listen to trigger a restart and play. Animation will not autoplay if specified. startEvents will restart the animation, use pauseEvents to resume it. If there are other animation components on the entity animating the same property, those animations will be automatically paused to not conflict. (optional)
+    :param list[str] startEvents: Comma-separated list of events to listen to trigger a restart and play. Animation will not autoplay if specified. startEvents will restart the animation, use pauseEvents to resume it. If there are other animation components on the entity animating the same property, those animations will be automatically paused to not conflict. (optional)
     :param str to: Target value at end of animation. (optional)
     :param str type: Right now only supports color for tweening isRawProperty color XYZ/RGB vector values. (optional)
     """
     def __init__(self, **kwargs):
         if "start" in kwargs:
             if isinstance(kwargs["start"], tuple) or isinstance(kwargs["start"], list):
                 kwargs["start"] = Utils.tuple_to_string(kwargs["start"])
```

### Comparing `arena-py-0.9.3/arena/attributes/animation_mixer.py` & `arena-py-0.9.6/arena/attributes/animation_mixer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .animation import Animation
 
 class AnimationMixer(Animation):
     """
-    AnimationMixer attribute class to manage its properties in the ARENA: A list of available animations can usually be found by inspecting the model file or its documentation. All animations will play by default. To play only a specific set of animations, use wildcards: animation-mixer='clip: run_*'.  More properties at (https://github.com/n5ro/aframe-extras/tree/master/src/loaders#animation) A-Frame Extras Animation.
-    Usage: animation_mixer=AnimationMixer(...)
-    
+    AnimationMixer attribute class to manage its properties in the ARENA: A list of available animations can usually be found by inspecting the model file or its documentation. All animations will play by default. To play only a specific set of animations, use wildcards: animation-mixer='clip: run_*'. More properties at <https://github.com/n5ro/aframe-extras/tree/master/src/loaders#animation> A-Frame Extras Animation.
+    Usage: `animation_mixer=AnimationMixer(...)`
+
     :param bool clampWhenFinished: If true, halts the animation at the last frame. (optional)
     :param str clip: Name of the animation clip(s) to play. Accepts wildcards. Defaults to '*' (optional)
     :param float crossFadeDuration: Duration of cross-fades between clips, in seconds. (optional)
     :param float duration: Duration of the animation, in seconds (0 = auto). (optional)
     :param str loop: In repeat and pingpong modes, the clip plays once plus the specified number of repetitions. For pingpong, every second clip plays in reverse. Allows [once, repeat, pingpong] Defaults to 'repeat' (optional)
     :param str repetitions: Number of times to play the clip, in addition to the first play (empty string = Infinity). Repetitions are ignored for loop: once. (optional)
     :param float startAt: Sets the start of an animation to a specific time (in milliseconds). This is useful when you need to jump to an exact time in an animation. The input parameter will be scaled by the mixer's timeScale. (optional)
```

### Comparing `arena-py-0.9.3/arena/attributes/armarker.py` & `arena-py-0.9.6/arena/attributes/armarker.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from .attribute import Attribute
 
 
 class Armarker(Attribute):
     """
     Armarker attribute class to manage its properties in the ARENA: A location marker (such as an AprilTag, a lightAnchor, or an UWB tag), used to anchor scenes, or scene objects, in the real world.
-    Usage: armarker=Armarker(...)
-    
+    Usage: `armarker=Armarker(...)`
+
     :param bool buildable: Whether tag has 'dynamic' toggled on click. Used to position a tag, then lock into position. (optional)
     :param bool dynamic: Dynamic tag, not used for localization. E.g., to move object to which this ARMarker component is attached to. Requires permissions to update the scene (if dynamic=true). (optional)
     :param float ele: Tag elevation in meters. (optional)
     :param float lat: Tag latitude. (optional)
     :param float long: Tag longitude. (optional)
     :param str markerid: The marker id (e.g. for AprilTag 36h11 family, an integer in the range [0, 586]). Defaults to '0' (optional)
     :param str markertype: The marker type, technology-based. Allows [apriltag_36h11, lightanchor, uwb, vive, optitrack] Defaults to 'apriltag_36h11' (optional)
```

### Comparing `arena-py-0.9.3/arena/attributes/attribution.py` & `arena-py-0.9.6/arena/attributes/attribution.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from .attribute import Attribute
 
 
 class Attribution(Attribute):
     """
     Attribution attribute class to manage its properties in the ARENA: Attribution Component. Saves attribution data in any entity.
-    Usage: attribution=Attribution(...)
-    
+    Usage: `attribution=Attribution(...)`
+
     :param str author: Author name; e.g. 'Vaptor-Studio'. Defaults to 'Unknown' (optional)
     :param str authorURL: Author homepage/profile; e.g. https://sketchfab.com/VapTor. (optional)
     :param bool extractAssetExtras: Extract attribution info from asset extras; will override attribution info given (default: true). Defaults to 'True' (optional)
     :param str license: License summary/short name; e.g. 'CC-BY-4.0'. Defaults to 'Unknown' (optional)
     :param str licenseURL: License URL; e.g. http://creativecommons.org/licenses/by/4.0/. (optional)
     :param str source: Model source e.g. 'Sketchfab'. Defaults to 'Unknown' (optional)
     :param str sourceURL: Model source URL; e.g. https://sketchfab.com/models/2135501583704537907645bf723685e7. (optional)
```

### Comparing `arena-py-0.9.3/arena/attributes/blip.py` & `arena-py-0.9.6/arena/attributes/blip.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from .attribute import Attribute
 
 
 class Blip(Attribute):
     """
     Blip attribute class to manage its properties in the ARENA: When the object is created or deleted, it will animate in/out of the scene instead of appearing/disappearing instantly. Must have a geometric mesh.
-    Usage: blip=Blip(...)
-    
+    Usage: `blip=Blip(...)`
+
     :param bool applyDescendants: Apply blipout effect to include all descendents. Does not work for blipin. (optional)
     :param bool blipin: Animate in on create, set false to disable. Defaults to 'True' (optional)
     :param bool blipout: Animate out on delete, set false to disable. Defaults to 'True' (optional)
     :param float duration: Animation duration in milliseconds. Defaults to '750' (optional)
     :param str geometry: Geometry of the blipout plane. Allows [rect, disk, ring] Defaults to 'rect' (optional)
     :param str planes: Which which clipping planes to use for effect. A top plane clips above it, bottom clips below it. Allows [both, top, bottom] Defaults to 'both' (optional)
     """
```

### Comparing `arena-py-0.9.3/arena/attributes/box_collision_listener.py` & `arena-py-0.9.6/arena/attributes/box_collision_listener.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .attribute import Attribute
 
 
 class BoxCollisionListener(Attribute):
     """
     BoxCollisionListener attribute class to manage its properties in the ARENA: Listen for bounding-box collisions with user camera and hands. Must be applied to an object or model with geometric mesh. Collisions are determined by course bounding-box overlaps.
-    Usage: box_collision_listener=BoxCollisionListener(...)
-    
+    Usage: `box_collision_listener=BoxCollisionListener(...)`
+
     :param bool dynamic: Set true for a moving object, which should have its bounding box recalculated regularly to determine proper collision. (optional)
     :param bool enabled: Publish detections, set `false` to disable. Defaults to 'True' (optional)
     """
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
```

### Comparing `arena-py-0.9.3/arena/attributes/click_listener.py` & `arena-py-0.9.6/arena/attributes/click_listener.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .attribute import Attribute
 
 
 class ClickListener(Attribute):
     """
-    ClickListener attribute class to manage its properties in the ARENA: Object will listen for clicks.
-    Usage: click_listener=ClickListener(...) or clickable=ClickListener(...)  or clickable=True
+    ClickListener attribute class to manage its properties in the ARENA: Object will listen for mouse events like clicks.
+    Usage: `click_listener=ClickListener(...)` or `clickable=True`
 
-    :param bool bubble: Set false to prevent click events from bubbling up to parent objects. See <a href='https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Events#event_bubbling'>Event Bubbling</a>. Defaults to 'True' (optional)
+    :param bool bubble: Set false to prevent click events from bubbling up to parent objects. See <https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Events#event_bubbling> Event Bubbling. Defaults to 'True' (optional)
     :param bool enabled: Publish events, set false to disable. Defaults to 'True' (optional)
     """
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
```

### Comparing `arena-py-0.9.3/arena/attributes/color.py` & `arena-py-0.9.6/arena/attributes/color.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import re
+
 import webcolors
+
 from .attribute import Attribute
 
+
 class Color(Attribute):
     """
     Color Attribute.
-    Usage: color=Color(red,green,blue)
+    Usage: `color=Color(red,green,blue)` or `color=(red,green,blue)`
     """
     def __init__(self, red=0, green=0, blue=0):
         if isinstance(red, str):
             # hex to tuple to Color
             color = red.lstrip("#")
             hexcolor = re.search(r"^(?:[0-9a-fA-F]{3}){1,2}$", color)
             wcrgb = None
```

### Comparing `arena-py-0.9.3/arena/attributes/data.py` & `arena-py-0.9.6/arena/attributes/data.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,65 +1,67 @@
 from ..utils import *
 from .attribute import Attribute
-from .position import Position
-from .rotation import Rotation
+from .color import Color
+from .dynamic_body import Physics
 from .goto_url import GotoUrl
 from .jitsi_video import JitsiVideo
-from .dynamic_body import Physics
-from .scale import Scale
 from .material import Material
-from .color import Color
+from .position import Position
+from .rotation import Rotation
+from .scale import Scale
+from .translate import (ATTRIBUTE_CLASS_TRANSLATION,
+                        KEYWORD_ATTRIBUTE_TRANSLATION)
 from .video_control import VideoControl
-from .translate import ATTRIBUTE_CLASS_TRANSLATION, KEYWORD_ATTRIBUTE_TRANSLATION
+
 
 class Data(Attribute):
     """
     Data attribute class to manage its properties in the ARENA: Wraps all attributes in JSON.
-    Usage: data=Data(...)
-    
-    :param dict animation: Animate and tween values. (optional)
-    :param dict animation_mixer: A list of available animations can usually be found by inspecting the model file or its documentation. All animations will play by default. To play only a specific set of animations, use wildcards: animation-mixer='clip: run_*'. (optional)
+    Usage: `data=Data(...)`
+
+    :param dict animation: Animate and tween values. More properties at <https://aframe.io/docs/1.5.0/components/animation.html> A-Frame Animation component. Easing properties are detailed at <https://easings.net> easings.net. (optional)
+    :param dict animation_mixer: A list of available animations can usually be found by inspecting the model file or its documentation. All animations will play by default. To play only a specific set of animations, use wildcards: animation-mixer='clip: run_*'. More properties at <https://github.com/n5ro/aframe-extras/tree/master/src/loaders#animation> A-Frame Extras Animation. (optional)
     :param dict armarker: A location marker (such as an AprilTag, a lightAnchor, or an UWB tag), used to anchor scenes, or scene objects, in the real world. (optional)
     :param dict attribution: Attribution Component. Saves attribution data in any entity. (optional)
     :param dict blip: When the object is created or deleted, it will animate in/out of the scene instead of appearing/disappearing instantly. Must have a geometric mesh. (optional)
     :param dict box_collision_listener: Listen for bounding-box collisions with user camera and hands. Must be applied to an object or model with geometric mesh. Collisions are determined by course bounding-box overlaps. (optional)
     :param bool buffer: Transform geometry into a BufferGeometry to reduce memory usage at the cost of being harder to manipulate (geometries only: box, circle, cone, ...). Defaults to 'True' (optional)
-    :param dict click_listener: Object will listen for clicks. (optional)
+    :param dict click_listener: Object will listen for mouse events like clicks. (optional)
     :param str collision_listener: Name of the collision-listener, default can be empty string. Collisions trigger click events. (optional)
-    :param dict dynamic_body: A freely-moving object. Dynamic bodies have mass, collide with other objects, bounce or slow during collisions, and fall if gravity is enabled. (optional)
+    :param dict dynamic_body: A freely-moving object. Dynamic bodies have mass, collide with other objects, bounce or slow during collisions, and fall if gravity is enabled. More properties at <https://github.com/c-frame/aframe-physics-system/blob/master/CannonDriver.md> A-Frame Physics System. (optional)
     :param dict gltf_model_lod: Simple switch between the default gltf-model and a detailed one when a user camera is within specified distance (optional)
-    :param dict gltf_morph: Allows you to target and control a gltf model's morphTargets created in Blender. (optional)
-    :param dict goto_landmark: Teleports user to the landmark with the given name; Requires click-listener. (optional)
-    :param dict goto_url: Goto given URL; Requires click-listener. (optional)
+    :param dict gltf_morph: Allows you to target and control a gltf model's morphTargets created in Blender. More properties at <https://github.com/elbobo/aframe-gltf-morph-component> A-Frame GLTF Morph component. (optional)
+    :param dict goto_landmark: Teleports user to the landmark with the given name. Requires click-listener. (optional)
+    :param dict goto_url: Load new URL when object is clicked. Requires click-listener. (optional)
     :param bool hide_on_enter_ar: Hide object when entering AR. Remove component to *not* hide. (optional)
     :param bool hide_on_enter_vr: Hide object when entering VR. Remove component to *not* hide. (optional)
     :param dict impulse: Apply an impulse to an object to set it in motion. This happens in conjunction with an event. Requires click-listener and physics. (optional)
     :param dict jitsi_video: Apply a jitsi video source to the geometry. (optional)
     :param dict landmark: Define entities as a landmark; Landmarks appears in the landmark list and you can move (teleport) to them; You can define the behavior of the teleport: if you will be at a fixed or random distance, looking at the landmark, fixed offset or if it is constrained by a navmesh (when it exists). (optional)
     :param str look_at: The look-at component defines the behavior for an entity to dynamically rotate or face towards another entity or position. Use '#my-camera' to face the user camera, otherwise can take either a vec3 position or a query selector to another entity. (optional)
-    :param dict material: The material properties of the object's surface. (optional)
-    :param dict material_extras: Define extra material properties, namely texture encoding, whether to render the material's color and render order. (optional)
+    :param dict material: The material properties of the object's surface. More properties at <https://aframe.io/docs/1.5.0/components/material.html> A-Frame Material. (optional)
+    :param dict material_extras: Define extra material properties, namely texture encoding, whether to render the material's color and render order. The properties set here access directly Three.js material component.  More properties at <https://threejs.org/docs/#api/en/materials/Material> THREE.js Material. (optional)
     :param dict modelUpdate: The GLTF-specific `modelUpdate` attribute is an object with child component names as keys. The top-level keys are the names of the child components to be updated. The values of each are nested `position` and `rotation` attributes to set as new values, respectively. Either `position` or `rotation` can be omitted if unchanged. (optional)
     :param dict multisrc: Define multiple visual sources applied to an object. (optional)
     :param str parent: Parent's object_id. Child objects inherit attributes of their parent, for example scale and translation. (optional)
     :param dict position: 3D object position. (optional)
     :param dict remote_render: Whether or not an object should be remote rendered [Experimental]. (optional)
     :param dict rotation: 3D object rotation in quaternion representation; Right-handed coordinate system. Euler degrees are deprecated in wire message format. (optional)
     :param dict scale: 3D object scale. (optional)
     :param bool screenshareable: Whether or not a user can screenshare on an object. Defaults to 'True' (optional)
-    :param dict shadow: Shadow (optional)
+    :param dict shadow: The shadow component enables shadows for an entity and its children. Adding the shadow component alone is not enough to display shadows in your scene. We must have at least one light with castShadow: true enabled. (optional)
     :param bool show_on_enter_ar: Show object when entering AR. Hidden otherwise. (optional)
     :param bool show_on_enter_vr: Show object when entering VR. Hidden otherwise. (optional)
     :param bool skipCache: Disable retrieving the shared geometry object from the cache. (geometries only: box, circle, cone, ...). (optional)
-    :param dict sound: The sound component defines the entity as a source of sound or audio. The sound component is positional and is thus affected by the component's position. (optional)
-    :param dict spe_particles: GPU based particle systems in A-Frame. (optional)
-    :param dict static_body: A fixed-position or animated object. Other objects may collide with static bodies, but static bodies themselves are unaffected by gravity and collisions. (optional)
+    :param dict sound: The sound component defines the entity as a source of sound or audio. The sound component is positional and is thus affected by the component's position. More properties at <https://aframe.io/docs/1.5.0/components/sound.html> A-Frame Sound. (optional)
+    :param dict spe_particles: GPU based particle systems in A-Frame. More properties at <https://github.com/harlyq/aframe-spe-particles-component> A-Frame SPE Particles component. (optional)
+    :param dict static_body: A fixed-position or animated object. Other objects may collide with static bodies, but static bodies themselves are unaffected by gravity and collisions. More properties at <https://github.com/c-frame/aframe-physics-system/blob/master/CannonDriver.md> A-Frame Physics System. (optional)
     :param dict textinput: Opens an HTML prompt when clicked. Sends text input as an event on MQTT. Requires click-listener. (optional)
     :param str url: Use File Store paths under 'store/users/username', see CDN and other storage options in the description above. (optional)
-    :param dict video_control: Video Control. (optional)
+    :param dict video_control: Adds a video to an entity and controls its playback. (optional)
     """
     def __init__(self, **kwargs):
         data = {}
         data = Data.update_data(data, kwargs)
         super().__init__(**data)
 
     @classmethod
```

### Comparing `arena-py-0.9.3/arena/attributes/dynamic_body.py` & `arena-py-0.9.6/arena/attributes/dynamic_body.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .attribute import Attribute
 
 
 class DynamicBody(Attribute):
     """
-    DynamicBody attribute class to manage its properties in the ARENA: A freely-moving object. Dynamic bodies have mass, collide with other objects, bounce or slow during collisions, and fall if gravity is enabled.  More properties at (https://github.com/c-frame/aframe-physics-system/blob/master/CannonDriver.md) A-Frame Physics System.
-    Usage: dynamic_body=DynamicBody(...)
+    DynamicBody attribute class to manage its properties in the ARENA: A freely-moving object. Dynamic bodies have mass, collide with other objects, bounce or slow during collisions, and fall if gravity is enabled. More properties at <https://github.com/c-frame/aframe-physics-system/blob/master/CannonDriver.md> A-Frame Physics System.
+    Usage: `dynamic_body=DynamicBody(...)`
 
     :param float angularDamping: Resistance to rotation. Defaults to '0.01' (optional)
     :param str cylinderAxis: Override default axis of bounding cylinder. Requires shape:cylinder. Allows [x, y, z] Defaults to 'y' (optional)
     :param float linearDamping: Resistance to movement. Defaults to '0.01' (optional)
     :param float mass: Simulated mass of the object, > 0. Defaults to '5' (optional)
     :param str shape: Body components will attempt to find an appropriate CANNON.js shape to fit your model. When defining an object you may choose a shape or leave the default, auto. Select a shape carefully, as there are performance implications with different choices. Allows [auto, box, cylinder, sphere, hull, none] Defaults to 'auto' (optional)
     :param float sphereRadius: Override default radius of bounding sphere. Requires shape:sphere. NaN by default. (optional)
@@ -21,9 +21,9 @@
             _type = "none"
         super().__init__(type=_type, **kwargs)
 
 
 class Physics(DynamicBody):
     """
     Alternate name for DynamicBody.
-    Usage: dynamic_body=Physics(...) or physics=Physics(...)
+    Usage: `physics=Physics(...)`
     """
```

### Comparing `arena-py-0.9.3/arena/attributes/gltf_morph.py` & `arena-py-0.9.6/arena/attributes/gltf_morph.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from .attribute import Attribute
 
 
 class GltfMorph(Attribute):
     """
-    GltfMorph attribute class to manage its properties in the ARENA: Allows you to target and control a gltf model's morphTargets created in Blender.  More properties at (https://github.com/elbobo/aframe-gltf-morph-component) A-Frame GLTF Morph component.
-    Usage: gltf_morph=GltfMorph(...)
+    GltfMorph attribute class to manage its properties in the ARENA: Allows you to target and control a gltf model's morphTargets created in Blender. More properties at <https://github.com/elbobo/aframe-gltf-morph-component> A-Frame GLTF Morph component.
+    Usage: `gltf_morph=GltfMorph(...)`
 
     :param str morphtarget: Name of morphTarget, can be found as part of the GLTF model. (optional)
     :param float value: Value that you want to set that morphTarget to (0 - 1). (optional)
     """
 
     def __init__(self, morphtarget, value):
         self.morphtarget = str(morphtarget)
         self.value = str(value)
 
 
 class Morph(GltfMorph):
     """
     Alternate name for GltfMorph.
-    Usage: gltf_morph=Morph(...)
+    Usage: `gltf_morph=Morph(...)`
     """
```

### Comparing `arena-py-0.9.3/arena/attributes/goto_landmark.py` & `arena-py-0.9.6/arena/attributes/goto_landmark.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .attribute import Attribute
 
 
 class GotoLandmark(Attribute):
     """
-    GotoLandmark attribute class to manage its properties in the ARENA: Teleports user to the landmark with the given name; Requires click-listener.
-    Usage: goto_landmark=GotoLandmark(...)
-    
+    GotoLandmark attribute class to manage its properties in the ARENA: Teleports user to the landmark with the given name. Requires click-listener.
+    Usage: `goto_landmark=GotoLandmark(...)`
+
     :param str landmark: Id of landmark to teleport to. (optional)
     :param str on: Event to listen 'on'. Allows [mousedown, mouseup] Defaults to 'mousedown' (optional)
     """
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
```

### Comparing `arena-py-0.9.3/arena/attributes/impulse.py` & `arena-py-0.9.6/arena/attributes/impulse.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from ..utils import Utils
 from .attribute import Attribute
 from .position import Position
 
 class Impulse(Attribute):
     """
     Impulse attribute class to manage its properties in the ARENA: Apply an impulse to an object to set it in motion. This happens in conjunction with an event. Requires click-listener and physics.
-    Usage: impulse=Impulse(...)
-    
+    Usage: `impulse=Impulse(...)`
+
     :param dict force: Impulse vector. Defaults to '{'x': 1, 'y': 1, 'z': 1}' (optional)
-    :param str on: Event to listen 'on'. (optional)
+    :param str on: Event to listen 'on'. Allows [mousedown, mouseup] Defaults to 'mousedown' (optional)
     :param dict position: World position. Defaults to '{'x': 1, 'y': 1, 'z': 1}' (optional)
     """
     def __init__(self, on="mousedown", force=Position(0,0,0), position=Position(0,0,0), **kwargs):
         if isinstance(force, Position):
             force = force.to_str()
         elif isinstance(force, tuple) or isinstance(force, list):
             force = Utils.tuple_to_string(force)
```

### Comparing `arena-py-0.9.3/arena/attributes/jitsi_video.py` & `arena-py-0.9.6/arena/attributes/jitsi_video.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .attribute import Attribute
 
 class JitsiVideo(Attribute):
     """
     JitsiVideo attribute class to manage its properties in the ARENA: Apply a jitsi video source to the geometry.
-    Usage: jitsi_video=JitsiVideo(...)
-    
+    Usage: `jitsi_video=JitsiVideo(...)`
+
     :param str displayName: ARENA or Jitsi display name of the video source; Will be ignored if jitsiId is given. (* change requires reload* ). (optional)
     :param str jitsiId: JitsiId of the video source; If defined will override displayName. (optional)
     """
     def __init__(self, jitsiId=None, displayName=None):
         # Since jitsiId overrides displayName, do not set None arguments
         kwargs = {}
         if jitsiId is not None:
```

### Comparing `arena-py-0.9.3/arena/attributes/landmark.py` & `arena-py-0.9.6/arena/attributes/landmark.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from ..utils import Utils
 from .attribute import Attribute
 from .position import Position
 
 class Landmark(Attribute):
     """
     Landmark attribute class to manage its properties in the ARENA: Define entities as a landmark; Landmarks appears in the landmark list and you can move (teleport) to them; You can define the behavior of the teleport: if you will be at a fixed or random distance, looking at the landmark, fixed offset or if it is constrained by a navmesh (when it exists).
-    Usage: landmark=Landmark(...)
-    
+    Usage: `landmark=Landmark(...)`
+
     :param str constrainToNavMesh: Teleports should snap to navmesh. Allows [false, any, coplanar] Defaults to 'false' (optional)
     :param str label: Landmark description to display in the landmark list. (optional)
     :param bool lookAtLandmark: Set to true to make users face the landmark when teleported to it. Defaults to 'True' (optional)
     :param dict offsetPosition: Use as a static teleport x,y,z offset. Defaults to '{'x': 0, 'y': 1.6, 'z': 0}' (optional)
     :param float randomRadiusMax: Maximum radius from the landmark to teleport to. (optional)
     :param float randomRadiusMin: Minimum radius from the landmark to teleport to. (randomRadiusMax must > 0). (optional)
     :param bool startingPosition: Set to true to use this landmark as a scene start (spawn) position. If several landmarks with startingPosition=true exist in a scene, one will be randomly selected. (optional)
```

### Comparing `arena-py-0.9.3/arena/attributes/material.py` & `arena-py-0.9.6/arena/objects/text.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,36 @@
-from .attribute import Attribute
+from .arena_object import Object
 
-class Material(Attribute):
+
+class Text(Object):
     """
-    Material attribute class to manage its properties in the ARENA: The material properties of the object's surface.  More properties at (https://aframe.io/docs/1.5.0/components/material.html) A-Frame Material.
-    Usage: material=Material(...)
-    
-    :param float alphaTest: Alpha test threshold for transparency. (optional)
-    :param str blending: The blending mode for the material's RGB and Alpha sent to the WebGLRenderer. Allows [none, normal, additive, subtractive, multiply] Defaults to 'normal' (optional)
-    :param str color: Base diffuse color. Defaults to '#7f7f7f' (optional)
-    :param bool depthTest: Whether depth testing is enabled when rendering the material. Defaults to 'True' (optional)
-    :param bool dithering: Whether material is dithered with noise. Removes banding from gradients like ones produced by lighting. Defaults to 'True' (optional)
-    :param bool flatShading: Use THREE.FlatShading rather than THREE.StandardShading. (optional)
-    :param bool npot: Use settings for non-power-of-two (NPOT) texture. (optional)
-    :param dict offset: Texture offset to be used. Defaults to '{'x': 1, 'y': 1}' (optional)
-    :param float opacity: Extent of transparency. If the transparent property is not true, then the material will remain opaque and opacity will only affect color. Defaults to '1' (optional)
-    :param dict repeat: Texture repeat to be used. Defaults to '{'x': 1, 'y': 1}' (optional)
-    :param str shader: Which material to use. Defaults to the standard material. Can be set to the flat material or to a registered custom shader material. Defaults to 'standard' (optional)
-    :param str side: Which sides of the mesh to render. Allows [front, back, double] Defaults to 'front' (optional)
-    :param str src: URI, relative or full path of an image/video file. e.g. 'store/users/wiselab/images/360falls.mp4'. (optional)
-    :param bool transparent: Whether material is transparent. Transparent entities are rendered after non-transparent entities. (optional)
-    :param str vertexColors: Whether to use vertex or face colors to shade the material. Allows [none, vertex, face] Defaults to 'none' (optional)
-    :param bool visible: Whether material is visible. Raycasters will ignore invisible materials. Defaults to 'True' (optional)
+    Text object class to manage its properties in the ARENA: Display text. More properties at <https://aframe.io/docs/1.5.0/components/text.html> A-Frame Text.
+
+    :param str align: Multi-line text alignment. Allows [left, center, right] Defaults to 'left' (optional)
+    :param float alphaTest: Discard text pixels if alpha is less than this value. Defaults to '0.5' (optional)
+    :param str anchor: Horizontal positioning. Allows [left, right, center, align] Defaults to 'center' (optional)
+    :param str baseline: Vertical positioning. Allows [top, center, bottom] Defaults to 'center' (optional)
+    :param str color: Text color. Defaults to '#000000' (optional)
+    :param str font: Font to render text, either the name of one of A-Frame's stock fonts or a URL to a font file. Allows [aileronsemibold, dejavu, exo2bold, exo2semibold, kelsonsans, monoid, mozillavr, roboto, sourcecodepro] Defaults to 'roboto' (optional)
+    :param str fontImage: Font image texture path to render text. Defaults to the font's name with extension replaced to .png. Don't need to specify if using a stock font. (derived from font name). (optional)
+    :param float height: Height of text block. (derived from text size). (optional)
+    :param float letterSpacing: Letter spacing in pixels. (optional)
+    :param float lineHeight: Line height in pixels. (derived from font file). (optional)
+    :param float opacity: Opacity, on a scale from 0 to 1, where 0 means fully transparent and 1 means fully opaque. Defaults to '1' (optional)
+    :param str shader: Shader used to render text. Allows [portal, flat, standard, sdf, msdf, ios10hls, skyshader, gradientshader] Defaults to 'sdf' (optional)
+    :param str side: Side to render. Allows [front, back, double] Defaults to 'double' (optional)
+    :param float tabSize: Tab size in spaces. Defaults to '4' (optional)
+    :param bool transparent: Whether text is transparent. Defaults to 'True' (optional)
+    :param str value: The actual content of the text. Line breaks and tabs are supported with `\\n` and `\\t`. (optional)
+    :param str whiteSpace: How whitespace should be handled. Allows [normal, pre, nowrap] Defaults to 'normal' (optional)
+    :param float width: Width in meters. (derived from geometry if exists). Defaults to '5' (optional)
+    :param float wrapCount: Number of characters before wrapping text (more or less). Defaults to '40' (optional)
+    :param float wrapPixels: Number of pixels before wrapping text. (derived from wrapCount). (optional)
+    :param float xOffset: X-offset to apply to add padding. (optional)
+    :param float zOffset: Z-offset to apply to avoid Z-fighting if using with a geometry as a background. Defaults to '0.001' (optional)
     """
-    def __init__(self, **kwargs):
-        if "opacity" in kwargs:
-            # kwargs["transparent"] = True # need to be transparent to be opaque
-            if kwargs["opacity"] > 1.0: # keep opacity between 0.0 and 1.0
-                kwargs["opacity"] = float(kwargs["opacity"]) / 100
-            kwargs["opacity"] = max(0.0, kwargs["opacity"])
-            kwargs["opacity"] = min(kwargs["opacity"], 1.0)
+    object_type = "text"
 
-        super().__init__(**kwargs)
+    def __init__(self, **kwargs):
+        # NOTE: Don't require parameter 'text' or 'value' we won't know which one users
+        #       used downstream into persist
+        super().__init__(object_type=Text.object_type, **kwargs)
```

### Comparing `arena-py-0.9.3/arena/attributes/material_extras.py` & `arena-py-0.9.6/arena/attributes/material_extras.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from .attribute import Attribute
 
 
 class MaterialExtras(Attribute):
     """
-    MaterialExtras attribute class to manage its properties in the ARENA: Define extra material properties, namely texture encoding, whether to render the material's color and render order.  The properties set here access directly Three.js material component.   More properties at (https://threejs.org/docs/#api/en/materials/Material) THREE.js Material.
-    Usage: material_extras=MaterialExtras(...)
-    
+    MaterialExtras attribute class to manage its properties in the ARENA: Define extra material properties, namely texture encoding, whether to render the material's color and render order. The properties set here access directly Three.js material component.  More properties at <https://threejs.org/docs/#api/en/materials/Material> THREE.js Material.
+    Usage: `material_extras=MaterialExtras(...)`
+
+    :param str colorSpace: The material colorspace. Allows [SRGBColorSpace, LinearSRGBColorSpace, DisplayP3ColorSpace, NoColorSpace] Defaults to 'SRGBColorSpace' (optional)
     :param bool colorWrite: Whether to render the material's color. Defaults to 'True' (optional)
-    :param str encoding:  Allows [LinearEncoding, sRGBEncoding, GammaEncoding, RGBEEncoding, LogLuvEncoding, RGBM7Encoding, RGBM16Encoding, RGBDEncoding, BasicDepthPacking, RGBADepthPacking] Defaults to 'sRGBEncoding' (optional)
     :param float gltfOpacity: Opacity value to apply to the model. 1 is fully opaque, 0 is fully transparent. Defaults to '1' (optional)
     :param str overrideSrc: Overrides the material source in all meshes of an object (e.g. a basic shape or a GLTF); Use, for example, to change the texture of a GLTF. (optional)
     :param float renderOrder: Allows the default rendering order of scene graph objects to be overridden. Defaults to '1' (optional)
     :param bool transparentOccluder: If `true`, will set `colorWrite=false` and `renderOrder=0` to make the material a transparent occluder. (optional)
     """
 
     def __init__(self, **kwargs):
```

### Comparing `arena-py-0.9.3/arena/attributes/model_update.py` & `arena-py-0.9.6/arena/attributes/model_update.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from .attribute import Attribute
 
 
 class ModelUpdate(Attribute):
     """
     ModelUpdate attribute class to manage its properties in the ARENA: The GLTF-specific `modelUpdate` attribute is an object with child component names as keys. The top-level keys are the names of the child components to be updated. The values of each are nested `position` and `rotation` attributes to set as new values, respectively. Either `position` or `rotation` can be omitted if unchanged.
-    Usage: modelUpdate=ModelUpdate(...)
+    Usage: `modelUpdate=ModelUpdate(...)`
 
     """
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
```

### Comparing `arena-py-0.9.3/arena/attributes/multisrc.py` & `arena-py-0.9.6/arena/attributes/multisrc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .attribute import Attribute
 
 
 class Multisrc(Attribute):
     """
     Multisrc attribute class to manage its properties in the ARENA: Define multiple visual sources applied to an object.
-    Usage: multisrc=Multisrc(...)
-    
+    Usage: `multisrc=Multisrc(...)`
+
     :param str srcs: A comma-delimited list if URIs, e.g. 'side1.png, side2.png, side3.png, side4.png, side5.png, side6.png' (required). (optional)
     :param str srcspath: URI, relative or full path of a directory containing srcs, e.g. 'store/users/wiselab/images/dice/' (required). (optional)
     """
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
```

### Comparing `arena-py-0.9.3/arena/attributes/position.py` & `arena-py-0.9.6/arena/attributes/position.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 from .attribute import Attribute
 from collections.abc import Iterable
 
 
 class Position(Attribute):
     """
     Position attribute class to manage its properties in the ARENA: 3D object position.
-    Usage: position=Position(x,y,z)
+    Usage: `position=Position(...)` or `position=Position(x,y,z)` or `position=(x,y,z)`
 
-    :param float x:  (optional)
-    :param float y:  (optional)
-    :param float z:  (optional)
+    :param float x: x (optional)
+    :param float y: y (optional)
+    :param float z: z (optional)
     """
 
     def __init__(self, x=None, y=None, z=None):
         if x is not None and (y is None or z is None or isinstance(x, Iterable)):
             raise ValueError("Position takes x,y,z")
         x = x or 0
         y = y or 0
@@ -25,7 +25,11 @@
     def to_str(self):
         return Utils.tuple_to_string((self.x, self.y, self.z))
 
     def distance_to(self, pos):
         return math.sqrt(
             (self.x - pos.x) ** 2 + (self.y - pos.y) ** 2 + (self.z - pos.z) ** 2
         )
+
+    @property
+    def array(self):
+        return [self.x, self.y, self.z]
```

### Comparing `arena-py-0.9.3/arena/attributes/rotation.py` & `arena-py-0.9.6/arena/attributes/rotation.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 from .attribute import Attribute
 from collections.abc import Iterable
 
 
 class Rotation(Attribute):
     """
     Rotation attribute class to manage its properties in the ARENA: 3D object rotation in quaternion representation; Right-handed coordinate system. Euler degrees are deprecated in wire message format.
-    Usage: rotation=Rotation(x,y,z,w) or rotation=Rotation(x,y,z)
+    Usage: `rotation=Rotation(...)` or `rotation=Rotation(x,y,z,w)` or `rotation=Rotation(x,y,z)` or `rotation=(x,y,z,w)` or `rotation=(x,y,z)`
 
-    :param float w:  Defaults to '1' (optional)
-    :param float x:  (optional)
-    :param float y:  (optional)
-    :param float z:  (optional)
+    :param float w: w Defaults to '1' (optional)
+    :param float x: x (optional)
+    :param float y: y (optional)
+    :param float z: z (optional)
     """
 
     def __init__(self, x=None, y=None, z=None, w=None):
         if x is not None and (y is None or z is None or isinstance(x, Iterable)):
             raise ValueError("Rotation takes x,y,z or x,y,z,w")
         x = x or 0
         y = y or 0
@@ -54,14 +54,19 @@
     def quaternion(self):
         if self.is_quaternion:  # quaternions
             return self
         else:  # euler
             quat = Rotation.e2q((self.x, self.y, self.z))
             return Rotation(*quat)
 
+    @property
+    def array(self):
+        q = self.quaternion
+        return [q.x, q.y, q.z, q.w]
+
     @classmethod
     def q2e(cls, q):
         """quaternions to euler (degrees)"""
         x, y, z, w = q
 
         # Roll (x-axis rotation)
         sinr_cosp = 2.0 * (w * x + y * z)
```

### Comparing `arena-py-0.9.3/arena/attributes/scale.py` & `arena-py-0.9.6/arena/attributes/scale.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,24 +2,28 @@
 from .attribute import Attribute
 from collections.abc import Iterable
 
 
 class Scale(Attribute):
     """
     Scale attribute class to manage its properties in the ARENA: 3D object scale.
-    Usage: scale=Scale(x,y,z)
+    Usage: `scale=Scale(...)` or `scale=Scale(x,y,z)` or `scale=(x,y,z)`
 
-    :param float x:  Defaults to '1' (optional)
-    :param float y:  Defaults to '1' (optional)
-    :param float z:  Defaults to '1' (optional)
+    :param float x: x Defaults to '1' (optional)
+    :param float y: y Defaults to '1' (optional)
+    :param float z: z Defaults to '1' (optional)
     """
 
     def __init__(self, x=None, y=None, z=None):
         if x is not None and (y is None or z is None or isinstance(x, Iterable)):
             raise ValueError("Scale takes x,y,z")
         x = x or 1
         y = y or 1
         z = z or 1
         super().__init__(x=Utils.agran(x), y=Utils.agran(y), z=Utils.agran(z))
 
     def to_str(self):
         return Utils.tuple_to_string((self.x, self.y, self.z))
+
+    @property
+    def array(self):
+        return [self.x, self.y, self.z]
```

### Comparing `arena-py-0.9.3/arena/attributes/sound.py` & `arena-py-0.9.6/arena/attributes/sound.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .attribute import Attribute
 
 class Sound(Attribute):
     """
-    Sound attribute class to manage its properties in the ARENA: The sound component defines the entity as a source of sound or audio. The sound component is positional and is thus affected by the component's position.  More properties at (https://aframe.io/docs/1.5.0/components/sound.html) A-Frame Sound.
-    Usage: sound=Sound(...)
-    
+    Sound attribute class to manage its properties in the ARENA: The sound component defines the entity as a source of sound or audio. The sound component is positional and is thus affected by the component's position. More properties at <https://aframe.io/docs/1.5.0/components/sound.html> A-Frame Sound.
+    Usage: `sound=Sound(...)`
+
     :param bool autoplay: Whether to automatically play sound once set. (optional)
     :param str distanceModel: Sound model. Allows [linear, inverse, exponential] Defaults to 'inverse' (optional)
     :param bool loop: Whether to loop the sound once the sound finishes playing. (optional)
     :param float maxDistance: Maximum distance between the audio source and the listener, after which the volume is not reduced any further. Defaults to '10000' (optional)
     :param str on: An event for the entity to listen to before playing sound. Allows [mousedown, mouseup, mouseenter, mouseleave, triggerdown, triggerup, gripdown, gripup, menudown, menuup, systemdown, systemup, trackpaddown, trackpadup] Defaults to 'mousedown' (optional)
     :param float poolSize: Numbers of simultaneous instances of this sound that can be playing at the same time. Defaults to '1' (optional)
     :param bool positional: Whether or not the audio is positional (movable). Defaults to 'True' (optional)
```

### Comparing `arena-py-0.9.3/arena/attributes/spe_particles.py` & `arena-py-0.9.6/arena/attributes/spe_particles.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from .attribute import Attribute
 
+
 class SpeParticles(Attribute):
     """
-    SpeParticles attribute class to manage its properties in the ARENA: GPU based particle systems in A-Frame.  More properties at (https://github.com/harlyq/aframe-spe-particles-component) A-Frame SPE Particles component.
-    Usage: spe_particles=SpeParticles(...)
-    
+    SpeParticles attribute class to manage its properties in the ARENA: GPU based particle systems in A-Frame. More properties at <https://github.com/harlyq/aframe-spe-particles-component> A-Frame SPE Particles component.
+    Usage: `spe_particles=SpeParticles(...)`
+
     :param dict acceleration: For sphere and disc distributions, only the x axis is used. Defaults to '{'x': 0, 'y': 0, 'z': 0}' (optional)
     :param str accelerationDistribution: Distribution of particle acceleration, for disc and sphere, only the x component will be used. if set to NONE use the 'distribution' attribute for accelerationDistribution. Allows [none, box, sphere, disc] Defaults to 'none' (optional)
     :param dict accelerationSpread: Spread of the particle's acceleration. for sphere and disc distributions, only the x axis is used. Defaults to '{'x': 0, 'y': 0, 'z': 0}' (optional)
     :param float activeMultiplier: Multiply the rate of particles emission, if larger than 1 then the particles will be emitted in bursts. note, very large numbers will emit all particles at once. Defaults to '1' (optional)
     :param bool affectedByFog: If true, the particles are affected by THREE js fog. Defaults to 'True' (optional)
     :param float alphaTest: Alpha values below the alphaTest threshold are considered invisible. Defaults to '0' (optional)
     :param list[float] angle: 2D rotation of the particle over the particle's lifetime, max 4 elements. Defaults to '[0]' (optional)
@@ -51,15 +52,15 @@
     :param float rotation: Rotation in degrees. Defaults to '0' (optional)
     :param dict rotationAxis: Local axis when using rotation. Defaults to '{'x': 0, 'y': 0, 'z': 0}' (optional)
     :param dict rotationAxisSpread: Variance in the axis of rotation. Defaults to '{'x': 0, 'y': 0, 'z': 0}' (optional)
     :param float rotationSpread: Rotation variance in degrees. Defaults to '0' (optional)
     :param bool rotationStatic: If true, the particles are fixed at their initial rotation value. if false, the particle will rotate from 0 to the 'rotation' value. (optional)
     :param list[float] size: Array of sizes over the particle's lifetime, max 4 elements. Defaults to '[1]' (optional)
     :param list[float] sizeSpread: Spread in size over the particle's lifetime, max 4 elements. Defaults to '[0]' (optional)
-    :param str texture: Texture to be used for each particle, may be a spritesheet.  Examples: [blob.png, fog.png, square.png, explosion_sheet.png, fireworks_sheet.png], like path 'static/images/textures/blob.png'. (optional)
+    :param str texture: Texture to be used for each particle, may be a spritesheet. Examples: [blob.png, fog.png, square.png, explosion_sheet.png, fireworks_sheet.png], like path 'static/images/textures/blob.png'. (optional)
     :param int textureFrameCount: Number of frames in the spritesheet, negative numbers default to textureFrames.x * textureFrames.y. Defaults to '-1' (optional)
     :param int textureFrameLoop: Number of times the spritesheet should be looped over the lifetime of a particle. Defaults to '1' (optional)
     :param dict textureFrames: X and Y frames for a spritesheet. each particle will transition through every frame of the spritesheet over its lifetime (see textureFramesLoop). Defaults to '{'x': 1, 'y': 1}' (optional)
     :param bool useTransparency: Should the particles be rendered with transparency? Defaults to 'True' (optional)
     :param dict velocity: For sphere and disc distributions, only the x axis is used. Defaults to '{'x': 0, 'y': 0, 'z': 0}' (optional)
     :param str velocityDistribution: Distribution of particle velocities, for disc and sphere, only the x component will be used. if set to NONE use the 'distribution' attribute for velocityDistribution. Allows [none, box, sphere, disc] Defaults to 'none' (optional)
     :param dict velocitySpread: Variance for the velocity. Defaults to '{'x': 0, 'y': 0, 'z': 0}' (optional)
@@ -70,9 +71,9 @@
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
 
 class Particles(SpeParticles):
     """
     Alternate name for SpeParticles.
-    Usage: spe_particles=Particles(...)
+    Usage: `spe_particles=Particles(...)`
     """
```

### Comparing `arena-py-0.9.3/arena/attributes/static_body.py` & `arena-py-0.9.6/arena/attributes/static_body.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from .attribute import Attribute
 
 
 class StaticBody(Attribute):
     """
-    StaticBody attribute class to manage its properties in the ARENA: A fixed-position or animated object. Other objects may collide with static bodies, but static bodies themselves are unaffected by gravity and collisions.  More properties at (https://github.com/c-frame/aframe-physics-system/blob/master/CannonDriver.md) A-Frame Physics System.
-    Usage: static_body=StaticBody(...)
-    
+    StaticBody attribute class to manage its properties in the ARENA: A fixed-position or animated object. Other objects may collide with static bodies, but static bodies themselves are unaffected by gravity and collisions. More properties at <https://github.com/c-frame/aframe-physics-system/blob/master/CannonDriver.md> A-Frame Physics System.
+    Usage: `static_body=StaticBody(...)`
+
     :param str cylinderAxis: Override default axis of bounding cylinder. Requires shape:cylinder. Allows [x, y, z] Defaults to 'y' (optional)
     :param str shape: Body components will attempt to find an appropriate CANNON.js shape to fit your model. When defining an object you may choose a shape or leave the default, auto. Select a shape carefully, as there are performance implications with different choices. Allows [auto, box, cylinder, sphere, hull, none] Defaults to 'auto' (optional)
     :param float sphereRadius: Override default radius of bounding sphere. Requires shape:sphere. NaN by default. (optional)
     :param str type: Define the result of collisions. Dynamic can be moved, Static cannot be moved. Allows [dynamic, static] Defaults to 'static' (optional)
     """
 
     def __init__(self, **kwargs):
```

### Comparing `arena-py-0.9.3/arena/attributes/textinput.py` & `arena-py-0.9.6/arena/attributes/textinput.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from .attribute import Attribute
 
 
 class Textinput(Attribute):
     """
     Textinput attribute class to manage its properties in the ARENA: Opens an HTML prompt when clicked. Sends text input as an event on MQTT. Requires click-listener.
-    Usage: textinput=Textinput(...)
-    
+    Usage: `textinput=Textinput(...)`
+
     :param str label: Text prompt label Defaults to 'Input text below (max is 140 characters).' (optional)
-    :param str on: A case-sensitive string representing the event type to listen for, e.g. 'mousedown', 'mouseup'. See <a href='https://developer.mozilla.org/en-US/docs/Web/Events'>Web Events</a> Allows [mousedown, mouseup, mouseenter, mouseleave, triggerdown, triggerup, gripdown, gripup, menudown, menuup, systemdown, systemup, trackpaddown, trackpadup] Defaults to 'mousedown' (optional)
+    :param str on: A case-sensitive string representing the event type to listen for. See <https://developer.mozilla.org/en-US/docs/Web/Events> Web Events Allows [mousedown, mouseup, mouseenter, mouseleave, triggerdown, triggerup, gripdown, gripup, menudown, menuup, systemdown, systemup, trackpaddown, trackpadup] Defaults to 'mousedown' (optional)
     :param str placeholder: Text input place holder. Defaults to 'Type here' (optional)
     :param str title: The prompt title. Defaults to 'Text Input' (optional)
     """
 
     def __init__(self,
                  title="Text Input",
                  label="Input text below (max is 140 characters)",
@@ -21,9 +21,9 @@
         super().__init__(title=title[:140], label=label[:140],
                          placeholder=placeholder[:140], on=on, **kwargs)
 
 
 class TextInput(Textinput):
     """
     Alternate name for Textinput.
-    Usage: textinput=TextInput(...)
+    Usage: `textinput=TextInput(...)`
     """
```

### Comparing `arena-py-0.9.3/arena/attributes/translate.py` & `arena-py-0.9.6/arena/attributes/translate.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.9.3/arena/attributes/video_control.py` & `arena-py-0.9.6/arena/attributes/video_control.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .attribute import Attribute
 
 class VideoControl(Attribute):
     """
-    VideoControl attribute class to manage its properties in the ARENA: Video Control.
-    Usage: video_control=VideoControl(...)
-    
+    VideoControl attribute class to manage its properties in the ARENA: Adds a video to an entity and controls its playback.
+    Usage: `video_control=VideoControl(...)`
+
     :param bool anyone_clicks: Responds to clicks from any user. Defaults to 'True' (optional)
     :param bool autoplay: Video starts playing automatically. (optional)
     :param bool cleanup: Automatically remove HTML5 video and img assets from DOM on object removal. Defaults to 'True' (optional)
     :param str frame_object: URL of a thumbnail image, e.g. 'store/users/wiselab/images/conix-face-white.jpg'. (optional)
     :param bool video_loop: Video automatically loops. Defaults to 'True' (optional)
     :param str video_object: Name of object where to put the video, e.g. 'square_vid6'. (optional)
     :param str video_path: URL of the video file, e.g. 'store/users/wiselab/videos/kungfu.mp4'. (optional)
```

### Comparing `arena-py-0.9.3/arena/auth.py` & `arena-py-0.9.6/arena/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -303,24 +303,25 @@
             else:
                 context = ssl.create_default_context()
                 context.check_hostname = False
                 context.verify_mode = ssl.CERT_NONE
                 res = request.urlopen(req, data=data, context=context)
             return res.read().decode("utf-8")
         except (requests.exceptions.ConnectionError, ConnectionError, URLError, HTTPError) as err:
-            print("{0}: ".format(err)+url)
+            print(f"{err}: {url}")
             if isinstance(err, HTTPError) and round(err.code, -2) == 400:
                 # user not authorized on website yet, they don"t have an ARENA username
-                base_url = "{0.scheme}://{0.netloc}".format(urlsplit(url))
+                us = urlsplit(url)
+                base_url = f"{us.scheme}://{us.netloc}"
                 print("Login with this account on the website first:")
                 print(f"Trying to open login page: {base_url}/user")
                 try:
                     webbrowser.open_new_tab(f"{base_url}/user")
-                except (webbrowser.Error) as err:
-                    print("Console-only login. {0}".format(err))
+                except (webbrowser.Error) as error:
+                    print(f"Console-only login. {error}")
             sys.exit("Terminating...")
 
 
 def signout():
     for root, dirs, files in os.walk(_arena_user_dir):
         if _mqtt_token_file in files:
             _remove_credentials(root)
@@ -328,28 +329,18 @@
         _remove_credentials(_local_mqtt_path)
     print("Signed out of the ARENA.")
 
 
 def _print_mqtt_token(storage_str, mqtt_claims):
     print("\nARENA MQTT/Video Permissions")
     print("----------------------")
-    print(f"Storage: {storage_str}")
-    print(f"User: {mqtt_claims['sub']}")
     exp_str = time.strftime("%c", time.localtime(mqtt_claims["exp"]))
     print(f"Expires: {exp_str}")
-    if "room" in mqtt_claims:
-        print("Video Conference: enabled")
-    else:
-        print("Video Conference: disabled")
-    print("Publish topics:")
-    for pub in mqtt_claims["publ"]:
-        print(f"- {pub}")
-    print("Subscribe topics:")
-    for sub in mqtt_claims["subs"]:
-        print(f"- {sub}")
+    print(f"Storage: {storage_str}")
+    print(f"{json.dumps(mqtt_claims, indent=4)}")
 
 
 def permissions():
     mqtt_claims = None
     # env storage auth
     if os.environ.get("ARENA_USERNAME") and os.environ.get("ARENA_PASSWORD"):
         mqtt_token = os.environ["ARENA_PASSWORD"]
```

### Comparing `arena-py-0.9.3/arena/base_object.py` & `arena-py-0.9.6/arena/base_object.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.9.3/arena/device.py` & `arena-py-0.9.6/arena/device.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,36 @@
 import json
 import os
 import re
 import sys
 
 from .arena_mqtt import ArenaMQTT
+from .env import DEVICE, _get_env
 
-from .env import (
-    DEVICE,
-    _get_env
-)
 
 class Device(ArenaMQTT):
     """
     Gives access to an ARENA device.
     Can create and execute various user-defined functions/tasks.
 
     :param str host: Hostname of the ARENA webserver (required).
     :param str realm: Reserved topic fork for future use (optional).
     :param str namespace: Username of authenticated user or other namespace (automatic).
     :param str device: The name of the device, without namespace (required).
     """
 
-    def __init__(
-                self,
-                host = "arenaxr.org",
-                realm = "realm",
-                network_latency_interval = 10000,  # run network latency update every 10s
-                on_msg_callback = None,
-                end_program_callback = None,
-                debug = False,
-                cli_args = False,
-                **kwargs
-            ):
-        if cli_args:
-            self.args = self.parse_cli()
-            if self.args["host"]:
-                kwargs["host"] = self.args["host"]
-            if self.args["namespace"]:
-                kwargs["namespace"] = self.args["namespace"]
-            if self.args["device"]:
-                kwargs["device"] = self.args["device"]
-            if self.args["debug"]:
-                debug = self.args["debug"]
+    def __init__(self,
+                 host="arenaxr.org",
+                 realm="realm",
+                 network_latency_interval=10000,  # run network latency update every 10s
+                 on_msg_callback=None,
+                 end_program_callback=None,
+                 debug=False,
+                 **kwargs
+                 ):
 
         if os.environ.get(DEVICE):
             self.device = _get_env(DEVICE)
             print(f"Using Device from 'DEVICE' env variable: {self.device}")
         elif "device" in kwargs and kwargs["device"]:
             if re.search("/", kwargs["device"]):
                 sys.exit("Device argument (device) cannot include '/', aborting...")
@@ -79,10 +64,10 @@
 
     def publish(self, topic, payload_obj):
         """Publishes to mqtt broker."""
         payload = json.dumps(payload_obj)
         self.mqttc.publish(topic, payload, qos=0)
         if self.debug: print("[publish]", topic, payload)
         return payload
-    
+
     def on_publish(self, client, userdata, mid):
-        pass
+        pass
```

### Comparing `arena-py-0.9.3/arena/env.py` & `arena-py-0.9.6/arena/env.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.9.3/arena/event_loop/asyncio_mqtt.py` & `arena-py-0.9.6/arena/event_loop/asyncio_mqtt.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.9.3/arena/event_loop/event_loop.py` & `arena-py-0.9.6/arena/event_loop/event_loop.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.9.3/arena/event_loop/lazy_worker.py` & `arena-py-0.9.6/arena/event_loop/lazy_worker.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.9.3/arena/event_loop/persistent_worker.py` & `arena-py-0.9.6/arena/event_loop/persistent_worker.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.9.3/arena/event_loop/worker.py` & `arena-py-0.9.6/arena/event_loop/worker.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.9.3/arena/events/event.py` & `arena-py-0.9.6/arena/events/event.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.9.3/arena/objects/__init__.py` & `arena-py-0.9.6/arena/objects/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # This file is auto-generated from github.com/arenaxr/arena-schema, changes here may be overwritten.
 
 from .arena_object import *
+from .program import *
 from .arenaui_button_panel import *
 from .arenaui_card import *
 from .arenaui_prompt import *
 from .box import *
 from .camera import *
 from .capsule import *
 from .circle import *
@@ -31,15 +32,14 @@
 from .text import *
 from .thickline import *
 from .threejs_scene import *
 from .torus import *
 from .torus_knot import *
 from .triangle import *
 from .videosphere import *
-from .program import *
 
 OBJECT_TYPE_MAP = {
     Object.object_type: Object,
     ArenauiButtonPanel.object_type: ArenauiButtonPanel,
     ArenauiCard.object_type: ArenauiCard,
     ArenauiPrompt.object_type: ArenauiPrompt,
     Box.object_type: Box,
@@ -69,8 +69,8 @@
     Text.object_type: Text,
     Thickline.object_type: Thickline,
     ThreejsScene.object_type: ThreejsScene,
     Torus.object_type: Torus,
     TorusKnot.object_type: TorusKnot,
     Triangle.object_type: Triangle,
     Videosphere.object_type: Videosphere,
-}
+}
```

### Comparing `arena-py-0.9.3/arena/objects/arena_object.py` & `arena-py-0.9.6/arena/objects/arena_object.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.9.3/arena/objects/arenaui_button_panel.py` & `arena-py-0.9.6/arena/objects/arenaui_button_panel.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from .arena_object import Object
 
 class ArenauiButtonPanel(Object):
     """
     ArenauiButtonPanel object class to manage its properties in the ARENA: ARENAUI element which displays a vertical or horizontal panel of buttons.
-    
+
     :param list[dict] buttons: Buttons Defaults to '[{'name': 'Option 1'}, {'name': 'Option 2'}]' (optional)
     :param str font: Font to use for button text. Allows [Roboto, Roboto-Mono] Defaults to 'Roboto' (optional)
+    :param str materialSides: Which sides display the rendered UI material Allows [both, front] Defaults to 'both' (optional)
     :param str theme: Color Theme Allows [light, dark] Defaults to 'light' (optional)
     :param str title: Title to display above buttons (optional). (optional)
     :param bool vertical: Vertical button layout (optional)
     """
     object_type = "arenaui-button-panel"
 
     def __init__(self, **kwargs):
```

### Comparing `arena-py-0.9.3/arena/objects/arenaui_card.py` & `arena-py-0.9.6/arena/objects/arenaui_card.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from .arena_object import Object
 
 class ArenauiCard(Object):
     """
     ArenauiCard object class to manage its properties in the ARENA: ARENAUI element which displays text and optionally an image.
-    
+
     :param str body: This is the text body of the card. (optional)
     :param str bodyAlign: Body Text Alignment Allows [left, center, right, justify] Defaults to 'left' (optional)
     :param bool closeButton: Show close button (optional)
     :param str font: Font to use for button text. Allows [Roboto, Roboto-Mono] Defaults to 'Roboto' (optional)
     :param float fontSize: Font Size Defaults to '0.035' (optional)
     :param str img: This image will be embedded alongside the body text. (optional)
     :param str imgCaption: This will caption the image. (optional)
     :param str imgDirection: Image Direction Allows [left, right] Defaults to 'right' (optional)
     :param str imgSize: Image sizing Allows [cover, contain, stretch] Defaults to 'cover' (optional)
+    :param str materialSides: Which sides display the rendered UI material Allows [both, front] Defaults to 'both' (optional)
     :param float textImageRatio: Text to Image Width Ratio Defaults to '0.5' (optional)
     :param str theme: Color Theme Allows [light, dark] Defaults to 'light' (optional)
     :param str title: Title (optional)
     :param float widthScale: Width scale multiplier Defaults to '1' (optional)
     """
     object_type = "arenaui-card"
```

### Comparing `arena-py-0.9.3/arena/objects/arenaui_prompt.py` & `arena-py-0.9.6/arena/objects/arenaui_prompt.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from .arena_object import Object
 
 class ArenauiPrompt(Object):
     """
     ArenauiPrompt object class to manage its properties in the ARENA: ARENAUI element which displays prompt with button actions.
-    
+
     :param list[str] buttons: Buttons Defaults to '['Confirm', 'Cancel']' (optional)
     :param str description: Description Defaults to 'This is a prompt. Please confirm or cancel.' (optional)
     :param str font: Font to use for button text. Allows [Roboto, Roboto-Mono] Defaults to 'Roboto' (optional)
+    :param str materialSides: Which sides display the rendered UI material Allows [both, front] Defaults to 'both' (optional)
     :param str theme: Color Theme Allows [light, dark] Defaults to 'light' (optional)
     :param str title: Title Defaults to 'Prompt' (optional)
     :param float width: Override width Defaults to '1.5' (optional)
     """
     object_type = "arenaui-prompt"
 
     def __init__(self, **kwargs):
```

### Comparing `arena-py-0.9.3/arena/objects/box.py` & `arena-py-0.9.6/arena/objects/box.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .arena_object import Object
 
 class Box(Object):
     """
     Box object class to manage its properties in the ARENA: Box Geometry.
-    
+
     :param float depth: depth Defaults to '1' (optional)
     :param float height: height Defaults to '1' (optional)
     :param int segmentsDepth: segments depth Defaults to '1' (optional)
     :param int segmentsHeight: segments height Defaults to '1' (optional)
     :param int segmentsWidth: segments width Defaults to '1' (optional)
     :param float width: width Defaults to '1' (optional)
     """
```

### Comparing `arena-py-0.9.3/arena/objects/camera.py` & `arena-py-0.9.6/arena/objects/camera.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from .arena_object import Object
 from ..attributes import Position, Rotation
 
 
 class Camera(Object):
     """
     Camera object class to manage its properties in the ARENA: Camera is the pose and arena-user component data representing a user avatar.
-    
-    :param dict arena_user:  (optional)
+
+    :param dict arena_user: arena-user (optional)
     """
 
     object_type = "camera"
 
     def __init__(self, object_id, **kwargs):
         data = kwargs.get("data", {})
         arena_user = data.get("arena-user", {})
```

### Comparing `arena-py-0.9.3/arena/objects/capsule.py` & `arena-py-0.9.6/arena/objects/capsule.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .arena_object import Object
 
 class Capsule(Object):
     """
     Capsule object class to manage its properties in the ARENA: Capsule Geometry.
-    
+
     :param float length: length Defaults to '1' (optional)
     :param float radius: radius Defaults to '1' (optional)
     :param int segmentsCap: segments capsule Defaults to '18' (optional)
     :param int segmentsRadial: segments radial Defaults to '36' (optional)
     """
     object_type = "capsule"
```

### Comparing `arena-py-0.9.3/arena/objects/circle.py` & `arena-py-0.9.6/arena/objects/circle.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .arena_object import Object
 
 class Circle(Object):
     """
     Circle object class to manage its properties in the ARENA: Circle Geometry.
-    
+
     :param float radius: radius Defaults to '1' (optional)
     :param int segments: segments Defaults to '32' (optional)
     :param float thetaLength: theta length Defaults to '360' (optional)
     :param float thetaStart: theta start (optional)
     """
     object_type = "circle"
```

### Comparing `arena-py-0.9.3/arena/objects/cone.py` & `arena-py-0.9.6/arena/objects/cone.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .arena_object import Object
 
 class Cone(Object):
     """
     Cone object class to manage its properties in the ARENA: Cone Geometry.
-    
+
     :param float height: height Defaults to '1' (optional)
     :param bool openEnded: open ended (optional)
     :param float radiusBottom: radius bottom Defaults to '1' (optional)
     :param float radiusTop: radius top Defaults to '0.01' (optional)
     :param int segmentsHeight: segments height Defaults to '18' (optional)
     :param int segmentsRadial: segments radial Defaults to '36' (optional)
     :param float thetaLength: theta length Defaults to '360' (optional)
```

### Comparing `arena-py-0.9.3/arena/objects/cylinder.py` & `arena-py-0.9.6/arena/objects/cylinder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .arena_object import Object
 
 class Cylinder(Object):
     """
     Cylinder object class to manage its properties in the ARENA: Cylinder Geometry.
-    
+
     :param float height: height Defaults to '1' (optional)
     :param bool openEnded: open ended (optional)
     :param float radius: radius Defaults to '1' (optional)
     :param int segmentsHeight: segments height Defaults to '18' (optional)
     :param int segmentsRadial: segments radial Defaults to '36' (optional)
     :param float thetaLength: theta length Defaults to '360' (optional)
     :param float thetaStart: theta start (optional)
```

### Comparing `arena-py-0.9.3/arena/objects/gaussian_splatting.py` & `arena-py-0.9.6/arena/objects/gaussian_splatting.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from .arena_object import Object
 
+
 class GaussianSplatting(Object):
     """
-    GaussianSplatting object class to manage its properties in the ARENA: Load a 3D Gaussian Splat for Real-Time Radiance Field Rendering.  More information : (https://github.com/quadjr/aframe-gaussian-splatting) A-Frame Gaussian Splatting. See guidance to store paths under (https://docs.arenaxr.org/content/interface/filestore.html) ARENA File Store, CDN, or DropBox.
-    
+    GaussianSplatting object class to manage its properties in the ARENA: Load a 3D Gaussian Splat for Real-Time Radiance Field Rendering. More information: <https://github.com/quadjr/aframe-gaussian-splatting> A-Frame Gaussian Splatting. See guidance to store paths under <https://docs.arenaxr.org/content/interface/filestore.html> ARENA File Store, CDN, or DropBox.
+
     :param str cutoutEntity: Selector to a box primitive that uses scale and position to define the bounds of splat points to render. (optional)
     :param float pixelRatio: Pixel ratio for rendering. Reducing the value decreases the resolution and improves performance. If a negative value is set, the device's native value will be applied. Defaults to '1.0' (optional)
     :param str src: Use File Store paths under 'store/users/username', see CDN and other storage options in the description above. (optional)
     :param float xrPixelRatio: Same as pixelRatio. Applied to XR devices. Defaults to '0.5' (optional)
     """
     object_type = "gaussian_splatting"
```

### Comparing `arena-py-0.9.3/arena/objects/gltf_model.py` & `arena-py-0.9.6/arena/objects/gltf_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 from .arena_object import Object
 from ..attributes import Morph
 
 class GltfModel(Object):
     """
-    GltfModel object class to manage its properties in the ARENA: Load a GLTF model.   Besides applying standard rotation and position attributes to the center-point of the GLTF model, the individual child components can also be manually manipulated. See format details in the `modelUpdate` data attribute. See guidance to store paths under (https://docs.arenaxr.org/content/interface/filestore.html) ARENA File Store, CDN, or DropBox.
-    
+    GltfModel object class to manage its properties in the ARENA: Load a GLTF model.  Besides applying standard rotation and position attributes to the center-point of the GLTF model, the individual child components can also be manually manipulated. See format details in the `modelUpdate` data attribute. See guidance to store paths under <https://docs.arenaxr.org/content/interface/filestore.html> ARENA File Store, CDN, or DropBox.
+
     :param str url: Use File Store paths under 'store/users/username', see CDN and other storage options in the description above. (optional)
     """
     object_type = "gltf-model"
 
     def __init__(self, url="", **kwargs):
         self.morphs = {}
         super().__init__(object_type=GLTF.object_type, url=url, **kwargs)
```

### Comparing `arena-py-0.9.3/arena/objects/hand_left.py` & `arena-py-0.9.6/arena/objects/hand_left.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .arena_object import Object
 
 class HandLeft(Object):
     """
     HandLeft object class to manage its properties in the ARENA: Hand is the (left or right) hand metadata pose and controller type of the user avatar.
-    
+
     :param str dep: Camera object_id this hand belongs to. (optional)
     :param str url: Path to user avatar hand model. Defaults to 'static/models/hands/valve_index_left.gltf' (optional)
     """
     object_type = "handLeft"
 
     def __init__(self,**kwargs):
         self.camera = None
```

### Comparing `arena-py-0.9.3/arena/objects/hand_right.py` & `arena-py-0.9.6/arena/objects/hand_right.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .arena_object import Object
 
 class HandRight(Object):
     """
     HandRight object class to manage its properties in the ARENA: Hand is the (left or right) hand metadata pose and controller type of the user avatar.
-    
+
     :param str dep: Camera object_id this hand belongs to. (optional)
     :param str url: Path to user avatar hand model. Defaults to 'static/models/hands/valve_index_left.gltf' (optional)
     """
     object_type = "handRight"
 
     def __init__(self,**kwargs):
         self.camera = None
```

### Comparing `arena-py-0.9.3/arena/objects/image.py` & `arena-py-0.9.6/arena/objects/image.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .arena_object import Object
 
 class Image(Object):
     """
-    Image object class to manage its properties in the ARENA: Display an image on a plane.  See guidance to store paths under (https://docs.arenaxr.org/content/interface/filestore.html) ARENA File Store, CDN, or DropBox.
-    
+    Image object class to manage its properties in the ARENA: Display an image on a plane. See guidance to store paths under <https://docs.arenaxr.org/content/interface/filestore.html> ARENA File Store, CDN, or DropBox.
+
     :param float height: height Defaults to '1' (optional)
     :param int segmentsHeight: segments height Defaults to '1' (optional)
     :param int segmentsWidth: segments width Defaults to '1' (optional)
     :param str url: Use File Store paths under 'store/users/username', see CDN and other storage options in the description above. (optional)
     :param float width: width Defaults to '1' (optional)
     """
     object_type = "image"
```

### Comparing `arena-py-0.9.3/arena/objects/light.py` & `arena-py-0.9.6/arena/objects/light.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from .arena_object import Object
 
 class Light(Object):
     """
-    Light object class to manage its properties in the ARENA: A light.  More properties at (https://aframe.io/docs/1.5.0/components/light.html) A-Frame Light.
-    
+    Light object class to manage its properties in the ARENA: A light. More properties at <https://aframe.io/docs/1.5.0/components/light.html> A-Frame Light.
+
     :param float angle: Maximum extent of spot light from its direction (in degrees). Requires type:spot. Defaults to '60' (optional)
     :param bool castShadow: Whether this light casts shadows on the scene. (optional)
     :param str color: Light color. For 'hemisphere', light color from above. Defaults to '#ffffff' (optional)
     :param float decay: Amount the light dims along the distance of the light. Requires type:point or type:spot. Defaults to '1' (optional)
     :param float distance: Distance where intensity becomes 0. If distance is 0, then the point light does not decay with distance. Requires type:point or type:spot. (optional)
     :param str envMap: Cube Map to load. (optional)
     :param str groundColor: Light color from below. Requires type:hemisphere. Defaults to '#ffffff' (optional)
     :param float intensity: Amount of light provided. Defaults to '1' (optional)
-    :param dict light:  (optional)
+    :param dict light: light (optional)
     :param float penumbra: Percent of the spotlight cone that is attenuated due to penumbra. Requires type:spot. (optional)
     :param float shadowBias: Offset depth when deciding whether a surface is in shadow. Tiny adjustments here (in the order of +/-0.0001) may reduce artifacts in shadows. (optional)
     :param float shadowCameraBottom: Bottom plane of shadow camera frustum. Requires type:directional. Defaults to '-5' (optional)
     :param float shadowCameraFar: Far plane of shadow camera frustum. Defaults to '500' (optional)
     :param float shadowCameraFov: Shadow camera's FOV. Requires type:point or spot. Defaults to '50' (optional)
     :param float shadowCameraLeft: Left plane of shadow camera frustum. Requires type:directional. Defaults to '-5' (optional)
     :param float shadowCameraNear: Near plane of shadow camera frustum. Defaults to '0.5' (optional)
```

### Comparing `arena-py-0.9.3/arena/objects/line.py` & `arena-py-0.9.6/arena/objects/line.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .arena_object import Object
 from ..attributes import Position
 
 class Line(Object):
     """
     Line object class to manage its properties in the ARENA: Draw a line.
-    
+
     :param str color: Line color. Defaults to '#74BEC1' (optional)
     :param dict end: End coordinate. Defaults to '{'x': -0.5, 'y': -0.5, 'z': 0}' (optional)
     :param float opacity: Line opacity. Defaults to '1' (optional)
     :param dict start: Start point coordinate. Defaults to '{'x': 0, 'y': 0.5, 'z': 0}' (optional)
     :param bool visible: Whether the material is visible. Defaults to 'True' (optional)
     """
     object_type = "line"
```

### Comparing `arena-py-0.9.3/arena/objects/ocean.py` & `arena-py-0.9.6/arena/objects/ocean.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.9.3/arena/objects/pcd_model.py` & `arena-py-0.9.6/arena/objects/pcd_model.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .arena_object import Object
 
 class PcdModel(Object):
     """
-    PcdModel object class to manage its properties in the ARENA: Load a PCD model.  Format: (https://pointclouds.org/documentation/tutorials/index.html) Point Clouds. See guidance to store paths under (https://docs.arenaxr.org/content/interface/filestore.html) ARENA File Store, CDN, or DropBox.
-    
+    PcdModel object class to manage its properties in the ARENA: Load a PCD model. Format: <https://pointclouds.org/documentation/tutorials/index.html> Point Clouds. See guidance to store paths under <https://docs.arenaxr.org/content/interface/filestore.html> ARENA File Store, CDN, or DropBox.
+
     :param str pointColor: Color of the points. Defaults to '#7f7f7f' (optional)
     :param float pointSize: Size of the points. Defaults to '0.01' (optional)
     :param str url: Use File Store paths under 'store/users/username', see CDN and other storage options in the description above. (optional)
     """
     object_type = "pcd-model"
 
     def __init__(self, **kwargs):
```

### Comparing `arena-py-0.9.3/arena/objects/plane.py` & `arena-py-0.9.6/arena/objects/plane.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .arena_object import Object
 
 class Plane(Object):
     """
     Plane object class to manage its properties in the ARENA: Plane Geometry.
-    
+
     :param float height: height Defaults to '1' (optional)
     :param int segmentsHeight: segments height Defaults to '1' (optional)
     :param int segmentsWidth: segments width Defaults to '1' (optional)
     :param float width: width Defaults to '1' (optional)
     """
     object_type = "plane"
```

### Comparing `arena-py-0.9.3/arena/objects/program.py` & `arena-py-0.9.6/arena/objects/program.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.9.3/arena/objects/ring.py` & `arena-py-0.9.6/arena/objects/ring.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .arena_object import Object
 
 class Ring(Object):
     """
     Ring object class to manage its properties in the ARENA: Ring Geometry.
-    
+
     :param float radiusInner: radius inner Defaults to '0.8' (optional)
     :param float radiusOuter: radius outer Defaults to '1.2' (optional)
     :param int segmentsPhi: segments phi Defaults to '10' (optional)
     :param int segmentsTheta: segments theta Defaults to '32' (optional)
     :param float thetaLength: theta length Defaults to '360' (optional)
     :param float thetaStart: theta start (optional)
     """
```

### Comparing `arena-py-0.9.3/arena/objects/roundedbox.py` & `arena-py-0.9.6/arena/objects/torus.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from .arena_object import Object
 
-class Roundedbox(Object):
+class Torus(Object):
     """
-    Roundedbox object class to manage its properties in the ARENA: Rounded Box Geometry.
-    
-    :param float depth: depth Defaults to '1' (optional)
-    :param float height: height Defaults to '1' (optional)
-    :param float radius: radius of edge Defaults to '0.15' (optional)
-    :param int radiusSegments: segments radius Defaults to '10' (optional)
-    :param float width: width Defaults to '1' (optional)
+    Torus object class to manage its properties in the ARENA: Torus Geometry.
+
+    :param float arc: Arc Defaults to '360' (optional)
+    :param float radius: radius Defaults to '1' (optional)
+    :param float radiusTubular: radius tubular Defaults to '0.2' (optional)
+    :param int segmentsRadial: segments radial Defaults to '36' (optional)
+    :param int segmentsTubular: segments tubular Defaults to '32' (optional)
     """
-    object_type = "roundedbox"
+    object_type = "torus"
 
     def __init__(self, **kwargs):
-        super().__init__(object_type=Roundedbox.object_type, **kwargs)
+        super().__init__(object_type=Torus.object_type, **kwargs)
```

### Comparing `arena-py-0.9.3/arena/objects/sphere.py` & `arena-py-0.9.6/arena/objects/sphere.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .arena_object import Object
 
 class Sphere(Object):
     """
     Sphere object class to manage its properties in the ARENA: Sphere Geometry.
-    
+
     :param float phiLength: phi length Defaults to '360' (optional)
     :param float phiStart: phi start (optional)
     :param float radius: radius Defaults to '1' (optional)
     :param int segmentsHeight: segments height Defaults to '18' (optional)
     :param int segmentsWidth: segments width Defaults to '36' (optional)
     :param float thetaLength: theta length Defaults to '180' (optional)
     :param float thetaStart: theta start (optional)
```

### Comparing `arena-py-0.9.3/arena/objects/thickline.py` & `arena-py-0.9.6/arena/objects/thickline.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from ..utils import Utils
 from .arena_object import Object
 from ..attributes import Attribute, Position
 
 class Thickline(Object):
     """
     Thickline object class to manage its properties in the ARENA: Draw a line that can have a custom width.
-    
+
     :param str color: Line color. Defaults to '#000000' (optional)
     :param float lineWidth: Width of line in px. Defaults to '1' (optional)
     :param str lineWidthStyler: Allows defining the line width as a function of relative position p along the path of the line. By default it is set to a constant 1. You may also choose one of the preset functions. Allows [default, grow, shrink, center-sharp, center-smooth, sine-wave] Defaults to 'default' (optional)
     :param str path: Comma-separated list of x y z coordinates of the line vertices. Defaults to '-2 -1 0, 0 20 0, 10 -1 10' (optional)
     """
     object_type = "thickline"
```

### Comparing `arena-py-0.9.3/arena/objects/threejs_scene.py` & `arena-py-0.9.6/arena/objects/threejs_scene.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from .arena_object import Object
 
 class ThreejsScene(Object):
     """
-    ThreejsScene object class to manage its properties in the ARENA: Load a Three.js Scene.  Could be THREE.js version-specific; you can see the THREE.js version in the JS console once you open ARENA; using glTF is preferred. Format: (https://threejs.org/docs/#api/en/scenes/Scene) THREE.js Scene. See guidance to store paths under (https://docs.arenaxr.org/content/interface/filestore.html) ARENA File Store, CDN, or DropBox.
-    
+    ThreejsScene object class to manage its properties in the ARENA: Load a Three.js Scene. Could be THREE.js version-specific; you can see the THREE.js version in the JS console once you open ARENA; using glTF is preferred. Format: <https://threejs.org/docs/#api/en/scenes/Scene> THREE.js Scene. See guidance to store paths under <https://docs.arenaxr.org/content/interface/filestore.html> ARENA File Store, CDN, or DropBox.
+
     :param str url: Use File Store paths under 'store/users/username', see CDN and other storage options in the description above. (optional)
     """
     object_type = "threejs-scene"
 
     def __init__(self, **kwargs):
         super().__init__(object_type=ThreejsScene.object_type, **kwargs)
```

### Comparing `arena-py-0.9.3/arena/objects/torus.py` & `arena-py-0.9.6/arena/objects/torus_knot.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from .arena_object import Object
 
-class Torus(Object):
+class TorusKnot(Object):
     """
-    Torus object class to manage its properties in the ARENA: Torus Geometry.
-    
-    :param float arc: Arc Defaults to '360' (optional)
+    TorusKnot object class to manage its properties in the ARENA: Torus Knot Geometry.
+
+    :param float p: P Defaults to '2' (optional)
+    :param float q: Q Defaults to '3' (optional)
     :param float radius: radius Defaults to '1' (optional)
     :param float radiusTubular: radius tubular Defaults to '0.2' (optional)
-    :param int segmentsRadial: segments radial Defaults to '36' (optional)
-    :param int segmentsTubular: segments tubular Defaults to '32' (optional)
+    :param int segmentsRadial: segments radial Defaults to '8' (optional)
+    :param int segmentsTubular: segments tubular Defaults to '100' (optional)
     """
-    object_type = "torus"
+    object_type = "torusKnot"
 
     def __init__(self, **kwargs):
-        super().__init__(object_type=Torus.object_type, **kwargs)
+        super().__init__(object_type=TorusKnot.object_type, **kwargs)
```

### Comparing `arena-py-0.9.3/arena/objects/torus_knot.py` & `arena-py-0.9.6/arena/objects/roundedbox.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from .arena_object import Object
 
-class TorusKnot(Object):
+class Roundedbox(Object):
     """
-    TorusKnot object class to manage its properties in the ARENA: Torus Knot Geometry.
-    
-    :param float p: P Defaults to '2' (optional)
-    :param float q: Q Defaults to '3' (optional)
-    :param float radius: radius Defaults to '1' (optional)
-    :param float radiusTubular: radius tubular Defaults to '0.2' (optional)
-    :param int segmentsRadial: segments radial Defaults to '8' (optional)
-    :param int segmentsTubular: segments tubular Defaults to '100' (optional)
+    Roundedbox object class to manage its properties in the ARENA: Rounded Box Geometry.
+
+    :param float depth: depth Defaults to '1' (optional)
+    :param float height: height Defaults to '1' (optional)
+    :param float radius: radius of edge Defaults to '0.15' (optional)
+    :param int radiusSegments: segments radius Defaults to '10' (optional)
+    :param float width: width Defaults to '1' (optional)
     """
-    object_type = "torusKnot"
+    object_type = "roundedbox"
 
     def __init__(self, **kwargs):
-        super().__init__(object_type=TorusKnot.object_type, **kwargs)
+        super().__init__(object_type=Roundedbox.object_type, **kwargs)
```

### Comparing `arena-py-0.9.3/arena/objects/triangle.py` & `arena-py-0.9.6/arena/objects/triangle.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .arena_object import Object
 
 class Triangle(Object):
     """
     Triangle object class to manage its properties in the ARENA: Triangle Geometry.
-    
+
     :param dict vertexA: vertex A Defaults to '{'x': 0, 'y': 0.5, 'z': 0}' (optional)
     :param dict vertexB: vertex B Defaults to '{'x': -0.5, 'y': -0.5, 'z': 0}' (optional)
     :param dict vertexC: vertex C Defaults to '{'x': 0.5, 'y': -0.5, 'z': 0}' (optional)
     """
     object_type = "triangle"
 
     def __init__(self, **kwargs):
```

### Comparing `arena-py-0.9.3/arena/objects/videosphere.py` & `arena-py-0.9.6/arena/objects/videosphere.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from .arena_object import Object
 
 class Videosphere(Object):
     """
     Videosphere object class to manage its properties in the ARENA: Videosphere Geometry.
-    
+
     :param bool autoplay: Autoplay Defaults to 'True' (optional)
     :param str crossOrigin: Cross Origin Defaults to 'anonymous' (optional)
     :param bool loop: Loop Defaults to 'True' (optional)
-    :param float radius: Radius Defaults to '5000' (optional)
-    :param int segmentsHeight: Segments Height Defaults to '64' (optional)
+    :param float radius: Radius Defaults to '500' (optional)
+    :param int segmentsHeight: Segments Height Defaults to '32' (optional)
     :param int segmentsWidth: Segments Width Defaults to '64' (optional)
     :param str src: URI, relative or full path of an image/video file. e.g. 'store/users/wiselab/images/360falls.mp4'. (optional)
     """
     object_type = "videosphere"
 
     def __init__(self, **kwargs):
         super().__init__(object_type=Videosphere.object_type, **kwargs)
```

### Comparing `arena-py-0.9.3/arena/scene.py` & `arena-py-0.9.6/arena/scene.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,70 +1,70 @@
+import argparse
 import asyncio
 import json
 import os
 import re
 import sys
-from datetime import datetime
-from inspect import signature
 import threading
 import uuid
+from datetime import datetime
+from inspect import signature
+from pathlib import Path
+
+import __main__ as main
 
 from .arena_mqtt import ArenaMQTT
 from .attributes import *
+from .env import PROGRAM_OBJECT_ID, SCENE, _get_env
 from .events import *
 from .objects import *
-from .utils import Utils, ArenaTelemetry, ArenaCmdInterpreter, ProgramRunInfo, QueueStats
+from .utils import (ArenaCmdInterpreter, ArenaTelemetry, ProgramRunInfo,
+                    QueueStats, Utils)
 
-from .env import (
-    SCENE,
-    PROGRAM_OBJECT_ID,
-    _get_env
-)
 
 class Scene(ArenaMQTT):
     """
     Gives access to an ARENA scene.
     Can create and execute various user-defined functions/tasks.
 
     :param str host: Hostname of the ARENA webserver (required).
     :param str realm: Reserved topic fork for future use (optional).
     :param str namespace: Username of authenticated user or other namespace (automatic).
     :param str scene: The name of the scene, without namespace (required).
     """
 
-    def __init__(
-                self,
-                host = "arenaxr.org",
-                realm = "realm",
-                network_latency_interval = 10000,  # run network latency update every 10s
-                on_msg_callback = None,
-                new_obj_callback = None,
-                user_join_callback = None,
-                user_left_callback = None,
-                delete_obj_callback = None,
-                end_program_callback = None,
-                video = False,
-                debug = False,
-                cli_args = False,
-                **kwargs
-            ):
+    def __init__(self,
+                 host="arenaxr.org",
+                 realm="realm",
+                 network_latency_interval=10000,  # run network latency update every 10s
+                 on_msg_callback=None,
+                 new_obj_callback=None,
+                 user_join_callback=None,
+                 user_left_callback=None,
+                 delete_obj_callback=None,
+                 end_program_callback=None,
+                 video=False,
+                 debug=False,
+                 cli_args=False,
+                 **kwargs
+                 ):
 
         # init telemetry
         self.telemetry = ArenaTelemetry()
 
         # setup event to let others wait on connection
         self.connected_evt = threading.Event()
 
         # start the command interpreter (if enabled by env variable)
         self.cmd_interpreter = ArenaCmdInterpreter(self, show_attrs=('config_data', 'scene', 'users', 'all_objects', 'run_info'),
                                     get_callables=('persisted_objs', 'persisted_scene_option', 'writable_scenes', 'user_list'),
                                     start_cmd_event=self.connected_evt)
 
         if cli_args:
-            self.args = self.parse_cli()
+            self.args = self.parse_cli(cli_args)
             if self.args["host"]:
                 kwargs["host"] = self.args["host"]
             if self.args["namespace"]:
                 kwargs["namespace"] = self.args["namespace"]
             if self.args["scene"]:
                 kwargs["scene"] = self.args["scene"]
             if self.args["debug"]:
@@ -131,14 +131,56 @@
                                            )
 
             # Always use the the hostname specified by the user, or defaults.
             print(f"Loading: https://{self.web_host}/{self.namespace}/{self.scene}, realm={self.realm}")
 
             span.add_event(f"Loading: https://{self.web_host}/{self.namespace}/{self.scene}, realm={self.realm}")
 
+    def parse_cli(self, cli_args=False):
+        """
+        Reusable command-line options to give apps flexible options to avoid hard-coding locations.
+        """
+        parser = argparse.ArgumentParser(description=(f"{Path(main.__file__).name} (arena-py) Application CLI"),
+                                         epilog="Additional user-defined args are possible, see docs at https://docs.arenaxr.org/content/python/scenes for usage.")
+        parser.add_argument("-mh", "--host", type=str,
+                            help="ARENA webserver main host to connect to")
+        parser.add_argument("-n", "--namespace", type=str,
+                            help="Namespace of scene")
+        parser.add_argument("-s", "--scene", type=str,
+                            help="Scene to publish and listen to")
+        parser.add_argument("-d", "--device", type=str,
+                            help="Device to publish and listen to")
+        parser.add_argument("-p", "--position", nargs=3, type=float, default=(0, 0, 0),
+                            help="App position as cartesian.x cartesian.y cartesian.z")
+        parser.add_argument("-r", "--rotation", nargs=3, type=float, default=(0, 0, 0),
+                            help="App rotation as euler.x euler.y euler.z")
+        parser.add_argument("-c", "--scale", nargs=3, type=float, default=(1, 1, 1),
+                            help="App scale as cartesian.x cartesian.y cartesian.z")
+        parser.add_argument("-D", "--debug", action='store_true',
+                            help='Debug mode.', default=False)
+
+        # add known help descriptions
+        if isinstance(cli_args, dict):
+            for k in cli_args:
+                parser.add_argument(
+                    f"-{k}", f"--{k}", help=cli_args[k], required=False)
+
+        # add unknown arguments for users to pull as strings
+        parsed, unknown = parser.parse_known_args()
+        for arg in unknown:
+            if arg.startswith(("-", "--")):
+                parser.add_argument(arg.split('=')[0])
+
+        args = parser.parse_args()
+        argdict = vars(args)
+        argdict["position"] = tuple(args.position)
+        argdict["rotation"] = tuple(args.rotation)
+        argdict["scale"] = tuple(args.scale)
+        return argdict
+
     def exit(self, arg=0):
         """Custom exit to push errors to telemetry"""
         error_msg=None
         if arg != 0:
             error_msg = f"Exiting with sys.exit('{arg}')"
         self.telemetry.exit(error_msg)
         os._exit(arg)
@@ -356,14 +398,36 @@
             object_id = cam
         evt = Event(object_id=object_id,
                     type="camera-override",
                     object_type="look-at",
                     target=target)
         return self.generate_custom_event(evt, action="update")
 
+    def teleport_to_landmark(self, cam, target):
+        """Publishes a camera manipulation event"""
+        if isinstance(target, Object):
+            target_id = target.object_id
+        elif type(target) is str:
+            target_id = target
+        else:
+            raise ValueError("target must be an ARENA object or string object_id")
+
+        if isinstance(cam, Object):
+            object_id = cam.object_id
+        elif type(target) is str:
+            object_id = cam
+        else:
+            raise ValueError("cam must be an ARENA object or string object_id")
+
+        evt = Event(object_id=object_id,
+                    type="camera-override",
+                    object_type="teleport-to-landmark",
+                    landmarkObj=target_id)
+        return self.generate_custom_event(evt, action="update")
+
     @property
     def all_objects(self):
         """Returns all the objects in a scene"""
         return Object.all_objects
 
     def add_object(self, obj):
         """Public function to create an object"""
@@ -608,15 +672,15 @@
         return self.users.values()
 
     def get_rcv_pub_queue_len(self):
         """Return QueueStats object with receive and publish queue length"""
         return QueueStats(super().rcv_queue_len(),  super().pub_queue_len())
 
     def run_info_update(self, run_info):
-        """Callbak when program stats are updated; publish program object update"""
+        """Callback when program stats are updated; publish program object update"""
         # Add run info to program data object and publish program object update
         run_info.add_program_info(self.program.data)
         self._publish(self.program, "update")
 
 class Arena(Scene):
     """
     Another name for Scene.
```

### Comparing `arena-py-0.9.3/arena/scripts/arena_py_pub.py` & `arena-py-0.9.6/arena/scripts/arena_py_pub.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.9.3/arena/scripts/arena_py_sub.py` & `arena-py-0.9.6/arena/scripts/arena_py_sub.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.9.3/arena/utils/arena_telemetry.py` & `arena-py-0.9.6/arena/utils/arena_telemetry.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.9.3/arena/utils/cmd_interpreter.py` & `arena-py-0.9.6/arena/utils/cmd_interpreter.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.9.3/arena/utils/program_info.py` & `arena-py-0.9.6/arena/utils/program_info.py`

 * *Files identical despite different names*

### Comparing `arena-py-0.9.3/arena_py.egg-info/PKG-INFO` & `arena-py-0.9.6/arena_py.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: arena-py
-Version: 0.9.3
+Version: 0.9.6
 Summary: Draw objects and run programs in the ARENA using Python!
 Home-page: https://github.com/arenaxr/arena-py
-Author: Conix Research Center
-Author-email: info@conix.io
+Author: Carnegie Mellon University
+Author-email: arenaxr@andrew.cmu.edu
 License: BSD 3-clause "New" or "Revised License"
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -16,14 +16,15 @@
 Requires-Dist: paho-mqtt~=1.5.1
 Requires-Dist: requests~=2.28.1
 Requires-Dist: webcolors~=1.3
 Requires-Dist: google_auth_oauthlib~=1.0.0
 Requires-Dist: google-auth~=2.22.0
 Requires-Dist: PyJWT~=2.4.0
 Requires-Dist: opentelemetry-exporter-otlp-proto-grpc==1.21.*
+Requires-Dist: numpy>=1.22.0
 
 # arena-py
 Draw objects and run programs in the ARENA using Python!
 
 ## Documentation
 The ARENA Python library user guide and tutorials:
 [ARENA Documentation: Python](https://docs.arenaxr.org/content/python/).
```

### Comparing `arena-py-0.9.3/arena_py.egg-info/SOURCES.txt` & `arena-py-0.9.6/arena_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arena-py-0.9.3/setup.py` & `arena-py-0.9.6/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import os
+
 import setuptools
 
 with open("README.md", "r") as readme:
     long_description = readme.read()
 
 # package_root = os.path.abspath(os.path.dirname(__file__))
 
 # version = {}
 # with open(os.path.join(package_root, "arena/version.py")) as fp:
 #     exec(fp.read(), version)
 # version = version["__version__"]
 
 setuptools.setup(
     name="arena-py",
-    version="0.9.3",
-    author="Conix Research Center",
-    author_email="info@conix.io",
+    version="0.9.6",
+    author="Carnegie Mellon University",
+    author_email="arenaxr@andrew.cmu.edu",
     license="BSD 3-clause \"New\" or \"Revised License\"",
     description="Draw objects and run programs in the ARENA using Python!",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/arenaxr/arena-py",
     packages=setuptools.find_packages(),
     entry_points={
@@ -36,15 +37,16 @@
         "aiohttp>=3.7.4",
         "paho-mqtt~=1.5.1",
         "requests~=2.28.1",
         "webcolors~=1.3",
         "google_auth_oauthlib~=1.0.0",
         "google-auth~=2.22.0",
         "PyJWT~=2.4.0",
-        "opentelemetry-exporter-otlp-proto-grpc==1.21.*"
+        "opentelemetry-exporter-otlp-proto-grpc==1.21.*",
+        "numpy>=1.22.0",
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.8',
```

