# Comparing `tmp/taipy-templates-3.1.0.tar.gz` & `tmp/taipy-templates-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taipy-templates-3.1.0.tar", last modified: Mon Mar  4 15:26:58 2024, max compression
+gzip compressed data, was "taipy-templates-3.1.1.tar", last modified: Mon Apr  8 13:10:38 2024, max compression
```

## Comparing `taipy-templates-3.1.0.tar` & `taipy-templates-3.1.1.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:26:58.796400 taipy-templates-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-04 15:26:44.000000 taipy-templates-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-04 15:26:56.000000 taipy-templates-3.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-03-04 15:26:58.796400 taipy-templates-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-03-04 15:26:44.000000 taipy-templates-3.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-04 15:26:58.796400 taipy-templates-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-03-04 15:26:56.000000 taipy-templates-3.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:26:58.788400 taipy-templates-3.1.0/taipy/
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-03-04 15:26:56.000000 taipy-templates-3.1.0/taipy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:26:58.788400 taipy-templates-3.1.0/taipy/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:26:58.788400 taipy-templates-3.1.0/taipy/templates/default/
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-03-04 15:26:44.000000 taipy-templates-3.1.0/taipy/templates/default/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:26:58.788400 taipy-templates-3.1.0/taipy/templates/default/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)     7818 2024-03-04 15:26:44.000000 taipy-templates-3.1.0/taipy/templates/default/hooks/post_gen_project.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-03-04 15:26:44.000000 taipy-templates-3.1.0/taipy/templates/default/hooks/pre_gen_project.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:26:58.788400 taipy-templates-3.1.0/taipy/templates/default/{{cookiecutter.__root_folder_name}}/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:26:58.788400 taipy-templates-3.1.0/taipy/templates/default/{{cookiecutter.__root_folder_name}}/algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-03-04 15:26:44.000000 taipy-templates-3.1.0/taipy/templates/default/{{cookiecutter.__root_folder_name}}/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-03-04 15:26:44.000000 taipy-templates-3.1.0/taipy/templates/default/{{cookiecutter.__root_folder_name}}/algorithms/algorithms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:26:58.788400 taipy-templates-3.1.0/taipy/templates/default/{{cookiecutter.__root_folder_name}}/configuration/
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-03-04 15:26:44.000000 taipy-templates-3.1.0/taipy/templates/default/{{cookiecutter.__root_folder_name}}/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-03-04 15:26:44.000000 taipy-templates-3.1.0/taipy/templates/default/{{cookiecutter.__root_folder_name}}/configuration/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:26:58.788400 taipy-templates-3.1.0/taipy/templates/default/{{cookiecutter.__root_folder_name}}/pages/
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-03-04 15:26:44.000000 taipy-templates-3.1.0/taipy/templates/default/{{cookiecutter.__root_folder_name}}/pages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:26:58.788400 taipy-templates-3.1.0/taipy/templates/default/{{cookiecutter.__root_folder_name}}/pages/page_example/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-04 15:26:44.000000 taipy-templates-3.1.0/taipy/templates/default/{{cookiecutter.__root_folder_name}}/pages/page_example/page_example.md
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-03-04 15:26:44.000000 taipy-templates-3.1.0/taipy/templates/default/{{cookiecutter.__root_folder_name}}/pages/page_example/page_example.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-04 15:26:44.000000 taipy-templates-3.1.0/taipy/templates/default/{{cookiecutter.__root_folder_name}}/pages/root.md
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-03-04 15:26:44.000000 taipy-templates-3.1.0/taipy/templates/default/{{cookiecutter.__root_folder_name}}/pages/root.py
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-04 15:26:44.000000 taipy-templates-3.1.0/taipy/templates/default/{{cookiecutter.__root_folder_name}}/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:26:58.788400 taipy-templates-3.1.0/taipy/templates/default/{{cookiecutter.__root_folder_name}}/sections/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-04 15:26:44.000000 taipy-templates-3.1.0/taipy/templates/default/{{cookiecutter.__root_folder_name}}/sections/import.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-04 15:26:44.000000 taipy-templates-3.1.0/taipy/templates/default/{{cookiecutter.__root_folder_name}}/sections/main.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 15:26:44.000000 taipy-templates-3.1.0/taipy/templates/default/{{cookiecutter.__root_folder_name}}/sections/page_content.txt
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-04 15:26:44.000000 taipy-templates-3.1.0/taipy/templates/default/{{cookiecutter.__root_folder_name}}/{{cookiecutter.__main_file}}.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:26:58.792400 taipy-templates-3.1.0/taipy/templates/scenario-management/
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-03-04 15:26:44.000000 taipy-templates-3.1.0/taipy/templates/scenario-management/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:26:58.792400 taipy-templates-3.1.0/taipy/templates/scenario-management/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-03-04 15:26:44.000000 taipy-templates-3.1.0/taipy/templates/scenario-management/hooks/post_gen_project.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:26:58.792400 taipy-templates-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-04 15:26:44.000000 taipy-templates-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 15:26:44.000000 taipy-templates-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/.taipyignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:26:58.792400 taipy-templates-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/algos/
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-03-04 15:26:44.000000 taipy-templates-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/algos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-03-04 15:26:44.000000 taipy-templates-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/algos/algos.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:26:58.792400 taipy-templates-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/config/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-04 15:26:44.000000 taipy-templates-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-03-04 15:26:44.000000 taipy-templates-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/config/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-04 15:26:44.000000 taipy-templates-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/config/config.toml
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-03-04 15:26:44.000000 taipy-templates-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/config/config_with_toml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:26:58.792400 taipy-templates-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-03-04 15:26:44.000000 taipy-templates-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:26:58.792400 taipy-templates-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/job_page/
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-03-04 15:26:44.000000 taipy-templates-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/job_page/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-04 15:26:44.000000 taipy-templates-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/job_page/job_page.md
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-03-04 15:26:44.000000 taipy-templates-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/job_page/job_page.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-03-04 15:26:44.000000 taipy-templates-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/root.md
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-03-04 15:26:44.000000 taipy-templates-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/root.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:26:58.792400 taipy-templates-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/scenario_page/
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-03-04 15:26:44.000000 taipy-templates-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/scenario_page/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-03-04 15:26:44.000000 taipy-templates-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/scenario_page/data_node_management.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-03-04 15:26:44.000000 taipy-templates-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/scenario_page/scenario_page.md
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-03-04 15:26:44.000000 taipy-templates-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/scenario_page/scenario_page.py
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-04 15:26:44.000000 taipy-templates-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-03-04 15:26:44.000000 taipy-templates-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/{{cookiecutter.__main_file}}.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 15:26:56.000000 taipy-templates-3.1.0/taipy/templates/setup.requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-04 15:26:44.000000 taipy-templates-3.1.0/taipy/templates/version.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:26:58.796400 taipy-templates-3.1.0/taipy_templates.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-03-04 15:26:58.000000 taipy-templates-3.1.0/taipy_templates.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-03-04 15:26:58.000000 taipy-templates-3.1.0/taipy_templates.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 15:26:58.000000 taipy-templates-3.1.0/taipy_templates.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 15:26:56.000000 taipy-templates-3.1.0/taipy_templates.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-04 15:26:58.000000 taipy-templates-3.1.0/taipy_templates.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:10:38.085880 taipy-templates-3.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-08 13:10:25.000000 taipy-templates-3.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-08 13:10:36.000000 taipy-templates-3.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-04-08 13:10:38.085880 taipy-templates-3.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-04-08 13:10:25.000000 taipy-templates-3.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 13:10:38.085880 taipy-templates-3.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-08 13:10:36.000000 taipy-templates-3.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:10:38.077880 taipy-templates-3.1.1/taipy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-08 13:10:36.000000 taipy-templates-3.1.1/taipy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:10:38.077880 taipy-templates-3.1.1/taipy/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:10:38.077880 taipy-templates-3.1.1/taipy/templates/default/
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-08 13:10:25.000000 taipy-templates-3.1.1/taipy/templates/default/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:10:38.077880 taipy-templates-3.1.1/taipy/templates/default/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     7818 2024-04-08 13:10:25.000000 taipy-templates-3.1.1/taipy/templates/default/hooks/post_gen_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-08 13:10:25.000000 taipy-templates-3.1.1/taipy/templates/default/hooks/pre_gen_project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:10:38.077880 taipy-templates-3.1.1/taipy/templates/default/{{cookiecutter.__root_folder_name}}/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:10:38.077880 taipy-templates-3.1.1/taipy/templates/default/{{cookiecutter.__root_folder_name}}/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-08 13:10:25.000000 taipy-templates-3.1.1/taipy/templates/default/{{cookiecutter.__root_folder_name}}/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-08 13:10:25.000000 taipy-templates-3.1.1/taipy/templates/default/{{cookiecutter.__root_folder_name}}/algorithms/algorithms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:10:38.077880 taipy-templates-3.1.1/taipy/templates/default/{{cookiecutter.__root_folder_name}}/configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-08 13:10:25.000000 taipy-templates-3.1.1/taipy/templates/default/{{cookiecutter.__root_folder_name}}/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-08 13:10:25.000000 taipy-templates-3.1.1/taipy/templates/default/{{cookiecutter.__root_folder_name}}/configuration/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:10:38.077880 taipy-templates-3.1.1/taipy/templates/default/{{cookiecutter.__root_folder_name}}/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-08 13:10:25.000000 taipy-templates-3.1.1/taipy/templates/default/{{cookiecutter.__root_folder_name}}/pages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:10:38.077880 taipy-templates-3.1.1/taipy/templates/default/{{cookiecutter.__root_folder_name}}/pages/page_example/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-08 13:10:25.000000 taipy-templates-3.1.1/taipy/templates/default/{{cookiecutter.__root_folder_name}}/pages/page_example/page_example.md
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-08 13:10:25.000000 taipy-templates-3.1.1/taipy/templates/default/{{cookiecutter.__root_folder_name}}/pages/page_example/page_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-08 13:10:25.000000 taipy-templates-3.1.1/taipy/templates/default/{{cookiecutter.__root_folder_name}}/pages/root.md
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-08 13:10:25.000000 taipy-templates-3.1.1/taipy/templates/default/{{cookiecutter.__root_folder_name}}/pages/root.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-08 13:10:25.000000 taipy-templates-3.1.1/taipy/templates/default/{{cookiecutter.__root_folder_name}}/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:10:38.081879 taipy-templates-3.1.1/taipy/templates/default/{{cookiecutter.__root_folder_name}}/sections/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-08 13:10:25.000000 taipy-templates-3.1.1/taipy/templates/default/{{cookiecutter.__root_folder_name}}/sections/import.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-08 13:10:25.000000 taipy-templates-3.1.1/taipy/templates/default/{{cookiecutter.__root_folder_name}}/sections/main.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 13:10:25.000000 taipy-templates-3.1.1/taipy/templates/default/{{cookiecutter.__root_folder_name}}/sections/page_content.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-08 13:10:25.000000 taipy-templates-3.1.1/taipy/templates/default/{{cookiecutter.__root_folder_name}}/{{cookiecutter.__main_file}}.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:10:38.081879 taipy-templates-3.1.1/taipy/templates/scenario-management/
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-08 13:10:25.000000 taipy-templates-3.1.1/taipy/templates/scenario-management/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:10:38.081879 taipy-templates-3.1.1/taipy/templates/scenario-management/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-08 13:10:25.000000 taipy-templates-3.1.1/taipy/templates/scenario-management/hooks/post_gen_project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:10:38.081879 taipy-templates-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-08 13:10:25.000000 taipy-templates-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 13:10:25.000000 taipy-templates-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/.taipyignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:10:38.081879 taipy-templates-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/algos/
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-08 13:10:25.000000 taipy-templates-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/algos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-08 13:10:25.000000 taipy-templates-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/algos/algos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:10:38.081879 taipy-templates-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-08 13:10:25.000000 taipy-templates-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-04-08 13:10:25.000000 taipy-templates-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-08 13:10:25.000000 taipy-templates-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/config/config.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-08 13:10:25.000000 taipy-templates-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/config/config_with_toml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:10:38.081879 taipy-templates-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-08 13:10:25.000000 taipy-templates-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:10:38.081879 taipy-templates-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/job_page/
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-08 13:10:25.000000 taipy-templates-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/job_page/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-08 13:10:25.000000 taipy-templates-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/job_page/job_page.md
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-08 13:10:25.000000 taipy-templates-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/job_page/job_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-08 13:10:25.000000 taipy-templates-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/root.md
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-08 13:10:25.000000 taipy-templates-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/root.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:10:38.081879 taipy-templates-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/scenario_page/
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-08 13:10:25.000000 taipy-templates-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/scenario_page/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-04-08 13:10:25.000000 taipy-templates-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/scenario_page/data_node_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-08 13:10:25.000000 taipy-templates-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/scenario_page/scenario_page.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-08 13:10:25.000000 taipy-templates-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/scenario_page/scenario_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-08 13:10:25.000000 taipy-templates-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-08 13:10:25.000000 taipy-templates-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/{{cookiecutter.__main_file}}.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 13:10:36.000000 taipy-templates-3.1.1/taipy/templates/setup.requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-08 13:10:25.000000 taipy-templates-3.1.1/taipy/templates/version.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:10:38.085880 taipy-templates-3.1.1/taipy_templates.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-04-08 13:10:38.000000 taipy-templates-3.1.1/taipy_templates.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-04-08 13:10:38.000000 taipy-templates-3.1.1/taipy_templates.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 13:10:38.000000 taipy-templates-3.1.1/taipy_templates.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 13:10:36.000000 taipy-templates-3.1.1/taipy_templates.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-08 13:10:38.000000 taipy-templates-3.1.1/taipy_templates.egg-info/top_level.txt
```

### Comparing `taipy-templates-3.1.0/LICENSE` & `taipy-templates-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `taipy-templates-3.1.0/PKG-INFO` & `taipy-templates-3.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy-templates
-Version: 3.1.0
+Version: 3.1.1
 Summary: An open-source package holding Taipy application templates.
 Home-page: https://github.com/avaiga/taipy-templates
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy-templates
 Classifier: Intended Audience :: Developers
```

### Comparing `taipy-templates-3.1.0/README.md` & `taipy-templates-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `taipy-templates-3.1.0/setup.py` & `taipy-templates-3.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `taipy-templates-3.1.0/taipy/__init__.py` & `taipy-templates-3.1.1/taipy/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-templates-3.1.0/taipy/templates/default/cookiecutter.json` & `taipy-templates-3.1.1/taipy/templates/default/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `taipy-templates-3.1.0/taipy/templates/default/hooks/post_gen_project.py` & `taipy-templates-3.1.1/taipy/templates/default/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `taipy-templates-3.1.0/taipy/templates/default/hooks/pre_gen_project.py` & `taipy-templates-3.1.1/taipy/templates/default/hooks/pre_gen_project.py`

 * *Files identical despite different names*

### Comparing `taipy-templates-3.1.0/taipy/templates/default/{{cookiecutter.__root_folder_name}}/algorithms/__init__.py` & `taipy-templates-3.1.1/taipy/templates/default/{{cookiecutter.__root_folder_name}}/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-templates-3.1.0/taipy/templates/default/{{cookiecutter.__root_folder_name}}/algorithms/algorithms.py` & `taipy-templates-3.1.1/taipy/templates/default/{{cookiecutter.__root_folder_name}}/algorithms/algorithms.py`

 * *Files identical despite different names*

### Comparing `taipy-templates-3.1.0/taipy/templates/default/{{cookiecutter.__root_folder_name}}/configuration/__init__.py` & `taipy-templates-3.1.1/taipy/templates/default/{{cookiecutter.__root_folder_name}}/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-templates-3.1.0/taipy/templates/default/{{cookiecutter.__root_folder_name}}/configuration/config.py` & `taipy-templates-3.1.1/taipy/templates/default/{{cookiecutter.__root_folder_name}}/configuration/config.py`

 * *Files identical despite different names*

### Comparing `taipy-templates-3.1.0/taipy/templates/default/{{cookiecutter.__root_folder_name}}/pages/__init__.py` & `taipy-templates-3.1.1/taipy/templates/default/{{cookiecutter.__root_folder_name}}/pages/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-templates-3.1.0/taipy/templates/default/{{cookiecutter.__root_folder_name}}/pages/page_example/page_example.py` & `taipy-templates-3.1.1/taipy/templates/default/{{cookiecutter.__root_folder_name}}/pages/page_example/page_example.py`

 * *Files identical despite different names*

### Comparing `taipy-templates-3.1.0/taipy/templates/default/{{cookiecutter.__root_folder_name}}/pages/root.py` & `taipy-templates-3.1.1/taipy/templates/default/{{cookiecutter.__root_folder_name}}/pages/root.py`

 * *Files identical despite different names*

### Comparing `taipy-templates-3.1.0/taipy/templates/default/{{cookiecutter.__root_folder_name}}/{{cookiecutter.__main_file}}.py` & `taipy-templates-3.1.1/taipy/templates/default/{{cookiecutter.__root_folder_name}}/{{cookiecutter.__main_file}}.py`

 * *Files identical despite different names*

### Comparing `taipy-templates-3.1.0/taipy/templates/scenario-management/cookiecutter.json` & `taipy-templates-3.1.1/taipy/templates/scenario-management/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `taipy-templates-3.1.0/taipy/templates/scenario-management/hooks/post_gen_project.py` & `taipy-templates-3.1.1/taipy/templates/scenario-management/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `taipy-templates-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/algos/__init__.py` & `taipy-templates-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/algos/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-templates-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/algos/algos.py` & `taipy-templates-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/algos/algos.py`

 * *Files identical despite different names*

### Comparing `taipy-templates-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/config/__init__.py` & `taipy-templates-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/config/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-templates-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/config/config.py` & `taipy-templates-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/config/config.py`

 * *Files identical despite different names*

### Comparing `taipy-templates-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/config/config.toml` & `taipy-templates-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/config/config.toml`

 * *Files identical despite different names*

### Comparing `taipy-templates-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/config/config_with_toml.py` & `taipy-templates-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/config/config_with_toml.py`

 * *Files identical despite different names*

### Comparing `taipy-templates-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/__init__.py` & `taipy-templates-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-templates-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/job_page/__init__.py` & `taipy-templates-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/job_page/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-templates-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/job_page/job_page.py` & `taipy-templates-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/job_page/job_page.py`

 * *Files identical despite different names*

### Comparing `taipy-templates-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/root.py` & `taipy-templates-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/root.py`

 * *Files identical despite different names*

### Comparing `taipy-templates-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/scenario_page/__init__.py` & `taipy-templates-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/scenario_page/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-templates-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/scenario_page/data_node_management.py` & `taipy-templates-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/scenario_page/data_node_management.py`

 * *Files identical despite different names*

### Comparing `taipy-templates-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/scenario_page/scenario_page.py` & `taipy-templates-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/pages/scenario_page/scenario_page.py`

 * *Files identical despite different names*

### Comparing `taipy-templates-3.1.0/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/{{cookiecutter.__main_file}}.py` & `taipy-templates-3.1.1/taipy/templates/scenario-management/{{cookiecutter.__root_folder_name}}/{{cookiecutter.__main_file}}.py`

 * *Files identical despite different names*

### Comparing `taipy-templates-3.1.0/taipy_templates.egg-info/PKG-INFO` & `taipy-templates-3.1.1/taipy_templates.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy-templates
-Version: 3.1.0
+Version: 3.1.1
 Summary: An open-source package holding Taipy application templates.
 Home-page: https://github.com/avaiga/taipy-templates
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy-templates
 Classifier: Intended Audience :: Developers
```

### Comparing `taipy-templates-3.1.0/taipy_templates.egg-info/SOURCES.txt` & `taipy-templates-3.1.1/taipy_templates.egg-info/SOURCES.txt`

 * *Files identical despite different names*

