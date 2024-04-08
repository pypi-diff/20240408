# Comparing `tmp/brainglobe-atlasapi-2.0.4.tar.gz` & `tmp/brainglobe-atlasapi-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainglobe-atlasapi-2.0.4.tar", last modified: Tue Mar 19 11:43:09 2024, max compression
+gzip compressed data, was "brainglobe-atlasapi-2.0.5.tar", last modified: Mon Apr  8 16:12:23 2024, max compression
```

## Comparing `brainglobe-atlasapi-2.0.4.tar` & `brainglobe-atlasapi-2.0.5.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 11:43:09.167647 brainglobe-atlasapi-2.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 11:43:09.155647 brainglobe-atlasapi-2.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 11:43:09.159647 brainglobe-atlasapi-2.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-03-19 11:43:03.000000 brainglobe-atlasapi-2.0.4/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-03-19 11:43:03.000000 brainglobe-atlasapi-2.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-03-19 11:43:03.000000 brainglobe-atlasapi-2.0.4/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-03-19 11:43:03.000000 brainglobe-atlasapi-2.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-03-19 11:43:03.000000 brainglobe-atlasapi-2.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    14967 2024-03-19 11:43:09.167647 brainglobe-atlasapi-2.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11220 2024-03-19 11:43:03.000000 brainglobe-atlasapi-2.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 11:43:09.159647 brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-03-19 11:43:03.000000 brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 11:43:09.163648 brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/atlas_generation/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-03-19 11:43:03.000000 brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/atlas_generation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 11:43:09.167647 brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/atlas_generation/atlas_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 11:43:03.000000 brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/atlas_generation/atlas_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13805 2024-03-19 11:43:03.000000 brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/atlas_generation/atlas_scripts/admba_3d_dev_mouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     8861 2024-03-19 11:43:03.000000 brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/atlas_generation/atlas_scripts/allen_cord.py
--rw-r--r--   0 runner    (1001) docker     (127)     3629 2024-03-19 11:43:03.000000 brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/atlas_generation/atlas_scripts/allen_mouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     7610 2024-03-19 11:43:03.000000 brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/atlas_generation/atlas_scripts/azba_zfish.py
--rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-03-19 11:43:03.000000 brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/atlas_generation/atlas_scripts/example_mouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     8893 2024-03-19 11:43:03.000000 brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/atlas_generation/atlas_scripts/humanatlas.py
--rw-r--r--   0 runner    (1001) docker     (127)    10747 2024-03-19 11:43:03.000000 brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/atlas_generation/atlas_scripts/kim_developmental_ccf_mouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     7352 2024-03-19 11:43:03.000000 brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/atlas_generation/atlas_scripts/kim_mouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     8373 2024-03-19 11:43:03.000000 brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/atlas_generation/atlas_scripts/mpin_zfish.py
--rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-03-19 11:43:03.000000 brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/atlas_generation/atlas_scripts/osten_mouse.py
--rw-r--r--   0 runner    (1001) docker     (127)    10296 2024-03-19 11:43:03.000000 brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/atlas_generation/atlas_scripts/perens_lsfm_mouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     7868 2024-03-19 11:43:03.000000 brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/atlas_generation/atlas_scripts/princeton_mouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-03-19 11:43:03.000000 brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/atlas_generation/atlas_scripts/template_script.py
--rw-r--r--   0 runner    (1001) docker     (127)     9586 2024-03-19 11:43:03.000000 brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/atlas_generation/atlas_scripts/whs_sd_rat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-03-19 11:43:03.000000 brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/atlas_generation/main_script.py
--rw-r--r--   0 runner    (1001) docker     (127)     9320 2024-03-19 11:43:03.000000 brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/atlas_generation/mesh_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-03-19 11:43:03.000000 brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/atlas_generation/metadata_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-03-19 11:43:03.000000 brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/atlas_generation/stacks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-03-19 11:43:03.000000 brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/atlas_generation/structure_json_to_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-03-19 11:43:03.000000 brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/atlas_generation/structures.py
--rw-r--r--   0 runner    (1001) docker     (127)     7786 2024-03-19 11:43:03.000000 brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/atlas_generation/validate_atlases.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-03-19 11:43:03.000000 brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/atlas_generation/volume_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7388 2024-03-19 11:43:03.000000 brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/atlas_generation/wrapup.py
--rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-03-19 11:43:03.000000 brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/bg_atlas.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-03-19 11:43:03.000000 brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-03-19 11:43:03.000000 brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    10797 2024-03-19 11:43:03.000000 brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-03-19 11:43:03.000000 brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/descriptors.py
--rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-03-19 11:43:03.000000 brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/list_atlases.py
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-03-19 11:43:03.000000 brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/structure_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-03-19 11:43:03.000000 brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/structure_tree_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-03-19 11:43:03.000000 brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/update_atlases.py
--rw-r--r--   0 runner    (1001) docker     (127)     8018 2024-03-19 11:43:03.000000 brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 11:43:09.167647 brainglobe-atlasapi-2.0.4/brainglobe_atlasapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14967 2024-03-19 11:43:09.000000 brainglobe-atlasapi-2.0.4/brainglobe_atlasapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-03-19 11:43:09.000000 brainglobe-atlasapi-2.0.4/brainglobe_atlasapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 11:43:09.000000 brainglobe-atlasapi-2.0.4/brainglobe_atlasapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-03-19 11:43:09.000000 brainglobe-atlasapi-2.0.4/brainglobe_atlasapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-19 11:43:09.000000 brainglobe-atlasapi-2.0.4/brainglobe_atlasapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-03-19 11:43:03.000000 brainglobe-atlasapi-2.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 11:43:09.167647 brainglobe-atlasapi-2.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:12:23.504845 brainglobe-atlasapi-2.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:12:23.496846 brainglobe-atlasapi-2.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:12:23.496846 brainglobe-atlasapi-2.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    14967 2024-04-08 16:12:23.504845 brainglobe-atlasapi-2.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11220 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:12:23.496846 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:12:23.500846 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:12:23.504845 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/atlas_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/atlas_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13805 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/atlas_scripts/admba_3d_dev_mouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8861 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/atlas_scripts/allen_cord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3629 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/atlas_scripts/allen_mouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7610 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/atlas_scripts/azba_zfish.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/atlas_scripts/example_mouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8893 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/atlas_scripts/humanatlas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10747 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/atlas_scripts/kim_developmental_ccf_mouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7352 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/atlas_scripts/kim_mouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8373 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/atlas_scripts/mpin_zfish.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/atlas_scripts/osten_mouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10296 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/atlas_scripts/perens_lsfm_mouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7868 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/atlas_scripts/princeton_mouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/atlas_scripts/template_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9586 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/atlas_scripts/whs_sd_rat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/main_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9320 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/mesh_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/metadata_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/stacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/structure_json_to_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8831 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/validate_atlases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/volume_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7388 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/wrapup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/bg_atlas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10797 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/list_atlases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/structure_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/structure_tree_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/update_atlases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8018 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:12:23.504845 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14967 2024-04-08 16:12:23.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-04-08 16:12:23.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 16:12:23.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-08 16:12:23.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-08 16:12:23.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-08 16:12:23.000000 brainglobe-atlasapi-2.0.5/brainglobe_atlasapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-04-08 16:12:17.000000 brainglobe-atlasapi-2.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 16:12:23.504845 brainglobe-atlasapi-2.0.5/setup.cfg
```

### Comparing `brainglobe-atlasapi-2.0.4/.github/workflows/test_and_deploy.yml` & `brainglobe-atlasapi-2.0.5/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.4/.gitignore` & `brainglobe-atlasapi-2.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.4/CITATION.cff` & `brainglobe-atlasapi-2.0.5/CITATION.cff`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.4/LICENSE` & `brainglobe-atlasapi-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.4/PKG-INFO` & `brainglobe-atlasapi-2.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainglobe-atlasapi
-Version: 2.0.4
+Version: 2.0.5
 Summary: A lightweight python module to interact with and generate atlases for systems neuroscience.
 Author-email: "Luigi Petrucco, Federico Claudi, Adam Tyson" <code@adamltyson.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2020, BrainGlobe
         All rights reserved.
```

### Comparing `brainglobe-atlasapi-2.0.4/README.md` & `brainglobe-atlasapi-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/atlas_generation/atlas_scripts/admba_3d_dev_mouse.py` & `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/atlas_scripts/admba_3d_dev_mouse.py`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/atlas_generation/atlas_scripts/allen_cord.py` & `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/atlas_scripts/allen_cord.py`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/atlas_generation/atlas_scripts/allen_mouse.py` & `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/atlas_scripts/allen_mouse.py`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/atlas_generation/atlas_scripts/azba_zfish.py` & `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/atlas_scripts/azba_zfish.py`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/atlas_generation/atlas_scripts/example_mouse.py` & `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/atlas_scripts/example_mouse.py`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/atlas_generation/atlas_scripts/humanatlas.py` & `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/atlas_scripts/humanatlas.py`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/atlas_generation/atlas_scripts/kim_developmental_ccf_mouse.py` & `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/atlas_scripts/kim_developmental_ccf_mouse.py`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/atlas_generation/atlas_scripts/kim_mouse.py` & `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/atlas_scripts/kim_mouse.py`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/atlas_generation/atlas_scripts/mpin_zfish.py` & `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/atlas_scripts/mpin_zfish.py`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/atlas_generation/atlas_scripts/osten_mouse.py` & `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/atlas_scripts/osten_mouse.py`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/atlas_generation/atlas_scripts/perens_lsfm_mouse.py` & `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/atlas_scripts/perens_lsfm_mouse.py`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/atlas_generation/atlas_scripts/princeton_mouse.py` & `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/atlas_scripts/princeton_mouse.py`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/atlas_generation/atlas_scripts/template_script.py` & `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/atlas_scripts/template_script.py`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/atlas_generation/atlas_scripts/whs_sd_rat.py` & `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/atlas_scripts/whs_sd_rat.py`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/atlas_generation/main_script.py` & `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/main_script.py`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/atlas_generation/mesh_utils.py` & `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/mesh_utils.py`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/atlas_generation/metadata_utils.py` & `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/metadata_utils.py`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/atlas_generation/stacks.py` & `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/stacks.py`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/atlas_generation/structure_json_to_csv.py` & `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/structure_json_to_csv.py`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/atlas_generation/structures.py` & `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/structures.py`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/atlas_generation/validate_atlases.py` & `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/validate_atlases.py`

 * *Files 12% similar despite different names*

```diff
@@ -107,17 +107,44 @@
 
 
 def validate_checksum(atlas: BrainGlobeAtlas):
     # implement later
     pass
 
 
-def check_additional_references(atlas: BrainGlobeAtlas):
-    # check additional references are different, but have same dimensions
-    pass
+def validate_image_dimensions(atlas: BrainGlobeAtlas):
+    """
+    Check that annotation and reference image have the same dimensions.
+    """
+    assert atlas.annotation.shape == atlas.reference.shape, (
+        "Annotation and reference image have different dimensions. \n"
+        f"Annotation image has dimension: {atlas.annotation.shape}, "
+        f"while reference image has dimension {atlas.reference.shape}."
+    )
+    return True
+
+
+def validate_additional_references(atlas: BrainGlobeAtlas):
+    """
+    Check that additional references are different, but have same dimensions.
+    """
+    for (
+        additional_reference_name
+    ) in atlas.additional_references.references_list:
+        additional_reference = atlas.additional_references[
+            additional_reference_name
+        ]
+        assert additional_reference.shape == atlas.reference.shape, (
+            f"Additional reference {additional_reference} "
+            "has unexpected dimension."
+        )
+        assert not np.all(
+            additional_reference == atlas.reference
+        ), "Additional reference is not different to main reference."
+    return True
 
 
 def catch_missing_mesh_files(atlas: BrainGlobeAtlas):
     """
     Checks if all the structures in the atlas have a corresponding mesh file
     """
 
@@ -207,15 +234,16 @@
 if __name__ == "__main__":
     # list to store the validation functions
     all_validation_functions = [
         validate_atlas_files,
         validate_mesh_matches_image_extents,
         open_for_visual_check,
         validate_checksum,
-        check_additional_references,
+        validate_image_dimensions,
+        validate_additional_references,
         catch_missing_mesh_files,
         catch_missing_structures,
     ]
 
     valid_atlases = []
     invalid_atlases = []
     validation_results = {}
```

### Comparing `brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/atlas_generation/volume_utils.py` & `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/volume_utils.py`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/atlas_generation/wrapup.py` & `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/atlas_generation/wrapup.py`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/bg_atlas.py` & `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/bg_atlas.py`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/cli.py` & `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/cli.py`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/config.py` & `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/config.py`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/core.py` & `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/core.py`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/descriptors.py` & `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/descriptors.py`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/list_atlases.py` & `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/list_atlases.py`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/structure_class.py` & `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/structure_class.py`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/structure_tree_util.py` & `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/structure_tree_util.py`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/update_atlases.py` & `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/update_atlases.py`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.4/brainglobe_atlasapi/utils.py` & `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi/utils.py`

 * *Files identical despite different names*

### Comparing `brainglobe-atlasapi-2.0.4/brainglobe_atlasapi.egg-info/PKG-INFO` & `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainglobe-atlasapi
-Version: 2.0.4
+Version: 2.0.5
 Summary: A lightweight python module to interact with and generate atlases for systems neuroscience.
 Author-email: "Luigi Petrucco, Federico Claudi, Adam Tyson" <code@adamltyson.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2020, BrainGlobe
         All rights reserved.
```

### Comparing `brainglobe-atlasapi-2.0.4/brainglobe_atlasapi.egg-info/SOURCES.txt` & `brainglobe-atlasapi-2.0.5/brainglobe_atlasapi.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 brainglobe_atlasapi/structure_class.py
 brainglobe_atlasapi/structure_tree_util.py
 brainglobe_atlasapi/update_atlases.py
 brainglobe_atlasapi/utils.py
 brainglobe_atlasapi.egg-info/PKG-INFO
 brainglobe_atlasapi.egg-info/SOURCES.txt
 brainglobe_atlasapi.egg-info/dependency_links.txt
+brainglobe_atlasapi.egg-info/entry_points.txt
 brainglobe_atlasapi.egg-info/requires.txt
 brainglobe_atlasapi.egg-info/top_level.txt
 brainglobe_atlasapi/atlas_generation/__init__.py
 brainglobe_atlasapi/atlas_generation/main_script.py
 brainglobe_atlasapi/atlas_generation/mesh_utils.py
 brainglobe_atlasapi/atlas_generation/metadata_utils.py
 brainglobe_atlasapi/atlas_generation/stacks.py
```

### Comparing `brainglobe-atlasapi-2.0.4/pyproject.toml` & `brainglobe-atlasapi-2.0.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -57,14 +57,18 @@
     "ruff",
     "setuptools_scm",
     "tox",
 ]
 
 allenmouse = ["allensdk"]
 
+
+[project.scripts]
+brainglobe = "brainglobe_atlasapi.cli:bg_cli"
+
 [build-system]
 requires = ["setuptools>=45", "wheel", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 include-package-data = true
```

