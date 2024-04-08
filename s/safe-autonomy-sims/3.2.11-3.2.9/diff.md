# Comparing `tmp/safe_autonomy_sims-3.2.11.tar.gz` & `tmp/safe_autonomy_sims-3.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safe_autonomy_sims-3.2.11.tar", max compression
+gzip compressed data, was "safe_autonomy_sims-3.2.9.tar", max compression
```

## Comparing `safe_autonomy_sims-3.2.11.tar` & `safe_autonomy_sims-3.2.9.tar`

### file list

```diff
@@ -1,92 +1,92 @@
--rw-r--r--   0        0        0       34 2024-04-08 16:33:39.647180 safe_autonomy_sims-3.2.11/LICENSE
--rw-r--r--   0        0        0     6533 2024-04-08 16:33:39.647180 safe_autonomy_sims-3.2.11/README.md
--rw-r--r--   0        0        0    11104 2024-04-08 16:33:39.651180 safe_autonomy_sims-3.2.11/docs/configuration.md
--rw-r--r--   0        0        0      282 2024-04-08 16:33:39.651180 safe_autonomy_sims-3.2.11/docs/css/images.css
--rw-r--r--   0        0        0       90 2024-04-08 16:33:39.651180 safe_autonomy_sims-3.2.11/docs/css/material.css
--rw-r--r--   0        0        0      263 2024-04-08 16:33:39.651180 safe_autonomy_sims-3.2.11/docs/css/mkdocstrings.css
--rw-r--r--   0        0        0      895 2024-04-08 16:33:39.651180 safe_autonomy_sims-3.2.11/docs/css/style.css
--rw-r--r--   0        0        0    36430 2024-04-08 16:33:39.651180 safe_autonomy_sims-3.2.11/docs/experiments.md
--rw-r--r--   0        0        0     1005 2024-04-08 16:33:39.651180 safe_autonomy_sims-3.2.11/docs/gen_ref_nav.py
--rw-r--r--   0        0        0   129349 2024-04-08 16:33:40.867179 safe_autonomy_sims-3.2.11/docs/images/HillsFrame2.png
--rw-r--r--   0        0        0   130401 2024-04-08 16:33:40.871179 safe_autonomy_sims-3.2.11/docs/images/HillsFrame3.png
--rw-r--r--   0        0        0    50311 2024-04-08 16:33:40.871179 safe_autonomy_sims-3.2.11/docs/images/inspection_problem.png
--rw-r--r--   0        0        0    41425 2024-04-08 16:33:40.871179 safe_autonomy_sims-3.2.11/docs/images/linear.png
--rw-r--r--   0        0        0    31143 2024-04-08 16:33:40.871179 safe_autonomy_sims-3.2.11/docs/images/relu.png
--rw-r--r--   0        0        0    33502 2024-04-08 16:33:40.871179 safe_autonomy_sims-3.2.11/docs/images/tanh.png
--rw-r--r--   0        0        0     6407 2024-04-08 16:33:40.871179 safe_autonomy_sims-3.2.11/docs/index.md
--rw-r--r--   0        0        0     1393 2024-04-08 16:33:40.871179 safe_autonomy_sims-3.2.11/docs/install.md
--rw-r--r--   0        0        0      392 2024-04-08 16:33:40.871179 safe_autonomy_sims-3.2.11/docs/javascripts/mathjax.js
--rw-r--r--   0        0        0    22587 2024-04-08 16:33:40.871179 safe_autonomy_sims-3.2.11/docs/tasks/CWH/docking.md
--rw-r--r--   0        0        0     2650 2024-04-08 16:33:40.871179 safe_autonomy_sims-3.2.11/docs/tasks/CWH/index.md
--rw-r--r--   0        0        0    23806 2024-04-08 16:33:40.871179 safe_autonomy_sims-3.2.11/docs/tasks/CWH/multiagent_docking.md
--rw-r--r--   0        0        0    27267 2024-04-08 16:33:40.871179 safe_autonomy_sims-3.2.11/docs/tasks/CWH/multiagent_translational_inspection.md
--rw-r--r--   0        0        0    34877 2024-04-08 16:33:40.875179 safe_autonomy_sims-3.2.11/docs/tasks/CWH/multiagent_weighted_six_dof_inspection.md
--rw-r--r--   0        0        0    28120 2024-04-08 16:33:40.875179 safe_autonomy_sims-3.2.11/docs/tasks/CWH/multiagent_weighted_translational_inspection.md
--rw-r--r--   0        0        0    26682 2024-04-08 16:33:40.875179 safe_autonomy_sims-3.2.11/docs/tasks/CWH/translational_inspection.md
--rw-r--r--   0        0        0    30735 2024-04-08 16:33:40.875179 safe_autonomy_sims-3.2.11/docs/tasks/CWH/weighted_six_dof_inspection.md
--rw-r--r--   0        0        0    27367 2024-04-08 16:33:40.875179 safe_autonomy_sims-3.2.11/docs/tasks/CWH/weighted_translational_inspection.md
--rw-r--r--   0        0        0     1207 2024-04-08 16:33:40.875179 safe_autonomy_sims-3.2.11/docs/tasks/index.md
--rw-r--r--   0        0        0     2324 2024-04-08 16:33:40.875179 safe_autonomy_sims-3.2.11/pyproject.toml
--rw-r--r--   0        0        0      826 2024-04-08 16:33:40.875179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/__init__.py
--rw-r--r--   0        0        0      839 2024-04-08 16:33:40.875179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/agents/__init__.py
--rw-r--r--   0        0        0     2828 2024-04-08 16:33:40.875179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/agents/rta_agent.py
--rw-r--r--   0        0        0      935 2024-04-08 16:33:40.875179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/dones/__init__.py
--rw-r--r--   0        0        0    12175 2024-04-08 16:33:40.875179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/dones/common_dones.py
--rw-r--r--   0        0        0      627 2024-04-08 16:33:40.879179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/dones/cwh/__init__.py
--rw-r--r--   0        0        0    11159 2024-04-08 16:33:40.879179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/dones/cwh/common.py
--rw-r--r--   0        0        0    13464 2024-04-08 16:33:40.879179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/dones/cwh/docking_dones.py
--rw-r--r--   0        0        0    12337 2024-04-08 16:33:40.879179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/dones/cwh/inspection_dones.py
--rw-r--r--   0        0        0      673 2024-04-08 16:33:40.879179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/evaluation/__init__.py
--rw-r--r--   0        0        0      642 2024-04-08 16:33:40.879179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/evaluation/animation/__init__.py
--rw-r--r--   0        0        0     8202 2024-04-08 16:33:40.879179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/evaluation/animation/base_animation.py
--rw-r--r--   0        0        0    19448 2024-04-08 16:33:40.879179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/evaluation/animation/inspection_animation.py
--rw-r--r--   0        0        0    10705 2024-04-08 16:33:40.879179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/evaluation/animation/six_dof_animation.py
--rw-r--r--   0        0        0    38230 2024-04-08 16:33:40.879179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/evaluation/evaluation_api.py
--rw-r--r--   0        0        0     4992 2024-04-08 16:33:40.879179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/evaluation/general_metrics.py
--rw-r--r--   0        0        0     6725 2024-04-08 16:33:40.879179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/evaluation/inspection_metrics.py
--rw-r--r--   0        0        0      660 2024-04-08 16:33:40.879179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/evaluation/launch/__init__.py
--rw-r--r--   0        0        0     1824 2024-04-08 16:33:40.879179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/evaluation/launch/serialize_cwh3d.py
--rw-r--r--   0        0        0      786 2024-04-08 16:33:40.879179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/experiments/__init__.py
--rw-r--r--   0        0        0     7087 2024-04-08 16:33:40.879179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/experiments/rllib_api_experiment.py
--rw-r--r--   0        0        0    20658 2024-04-08 16:33:40.879179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/experiments/safe_autonomy_rllib_api_experiment.py
--rw-r--r--   0        0        0     1265 2024-04-08 16:33:40.879179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/glues/__init__.py
--rw-r--r--   0        0        0     3174 2024-04-08 16:33:40.879179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/glues/coordinate_axis_glue.py
--rw-r--r--   0        0        0     3348 2024-04-08 16:33:40.879179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/glues/dot_product_glue.py
--rw-r--r--   0        0        0      983 2024-04-08 16:33:40.879179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/glues/magnitude_glue.py
--rw-r--r--   0        0        0    10361 2024-04-08 16:33:40.879179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/glues/rta_glue.py
--rw-r--r--   0        0        0     7716 2024-04-08 16:33:40.879179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/glues/six_dof_glues.py
--rw-r--r--   0        0        0     3928 2024-04-08 16:33:40.879179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/glues/vel_limit_glue.py
--rw-r--r--   0        0        0     1063 2024-04-08 16:33:40.879179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/platforms/__init__.py
--rw-r--r--   0        0        0      614 2024-04-08 16:33:40.879179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/platforms/common/__init__.py
--rw-r--r--   0        0        0     3895 2024-04-08 16:33:40.879179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/platforms/common/controllers.py
--rw-r--r--   0        0        0     1757 2024-04-08 16:33:40.879179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/platforms/common/platform.py
--rw-r--r--   0        0        0     2085 2024-04-08 16:33:40.879179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/platforms/common/sensors.py
--rw-r--r--   0        0        0      612 2024-04-08 16:33:40.879179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/platforms/cwh/__init__.py
--rw-r--r--   0        0        0     1499 2024-04-08 16:33:40.879179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/platforms/cwh/cwh_available_platforms.py
--rw-r--r--   0        0        0     7656 2024-04-08 16:33:40.879179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/platforms/cwh/cwh_platform.py
--rw-r--r--   0        0        0    15755 2024-04-08 16:33:40.879179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/platforms/cwh/cwh_properties.py
--rw-r--r--   0        0        0    21104 2024-04-08 16:33:40.879179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/platforms/cwh/cwh_sensors.py
--rw-r--r--   0        0        0     5449 2024-04-08 16:33:40.879179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/platforms/cwh/rotation_sensors.py
--rw-r--r--   0        0        0      970 2024-04-08 16:33:40.879179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/rewards/__init__.py
--rw-r--r--   0        0        0      597 2024-04-08 16:33:40.879179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/rewards/cwh/__init__.py
--rw-r--r--   0        0        0    21575 2024-04-08 16:33:40.879179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/rewards/cwh/docking_rewards.py
--rw-r--r--   0        0        0     3976 2024-04-08 16:33:40.879179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/rewards/cwh/done_state_rewards.py
--rw-r--r--   0        0        0     4320 2024-04-08 16:33:40.879179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/rewards/cwh/gaussian_decay_from_target_value.py
--rw-r--r--   0        0        0    15636 2024-04-08 16:33:40.879179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/rewards/cwh/inspection_rewards.py
--rw-r--r--   0        0        0     2097 2024-04-08 16:33:40.879179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/rewards/cwh/live_timestep_reward.py
--rw-r--r--   0        0        0     1820 2024-04-08 16:33:40.879179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/rewards/rta_rewards.py
--rw-r--r--   0        0        0     1016 2024-04-08 16:33:40.883179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/rta/__init__.py
--rw-r--r--   0        0        0      602 2024-04-08 16:33:40.883179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/rta/cwh/__init__.py
--rw-r--r--   0        0        0     9407 2024-04-08 16:33:40.883179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/rta/cwh/cwh_rta.py
--rw-r--r--   0        0        0     5785 2024-04-08 16:33:40.883179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/rta/cwh/inspection_rta_1v1.py
--rw-r--r--   0        0        0     8226 2024-04-08 16:33:40.883179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/rta/rta_rejection_sampler.py
--rw-r--r--   0        0        0     1122 2024-04-08 16:33:40.883179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/simulators/__init__.py
--rw-r--r--   0        0        0     1262 2024-04-08 16:33:40.883179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/simulators/cwh_simulator.py
--rw-r--r--   0        0        0    22988 2024-04-08 16:33:40.883179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/simulators/illumination_functions.py
--rw-r--r--   0        0        0      830 2024-04-08 16:33:40.883179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/simulators/initializers/__init__.py
--rw-r--r--   0        0        0    15278 2024-04-08 16:33:40.883179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/simulators/initializers/cwh.py
--rw-r--r--   0        0        0     7033 2024-04-08 16:33:40.883179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/simulators/initializers/initializer.py
--rw-r--r--   0        0        0    31944 2024-04-08 16:33:40.883179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/simulators/inspection_simulator.py
--rw-r--r--   0        0        0    16947 2024-04-08 16:33:40.883179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/simulators/saferl_simulator.py
--rw-r--r--   0        0        0     9010 2024-04-08 16:33:40.883179 safe_autonomy_sims-3.2.11/safe_autonomy_sims/utils.py
--rw-r--r--   0        0        0     7697 1970-01-01 00:00:00.000000 safe_autonomy_sims-3.2.11/PKG-INFO
+-rw-r--r--   0        0        0       34 2024-03-26 22:05:54.676286 safe_autonomy_sims-3.2.9/LICENSE
+-rw-r--r--   0        0        0     6533 2024-03-26 22:05:54.676286 safe_autonomy_sims-3.2.9/README.md
+-rw-r--r--   0        0        0    11104 2024-03-26 22:05:54.680286 safe_autonomy_sims-3.2.9/docs/configuration.md
+-rw-r--r--   0        0        0      282 2024-03-26 22:05:54.680286 safe_autonomy_sims-3.2.9/docs/css/images.css
+-rw-r--r--   0        0        0       90 2024-03-26 22:05:54.680286 safe_autonomy_sims-3.2.9/docs/css/material.css
+-rw-r--r--   0        0        0      263 2024-03-26 22:05:54.680286 safe_autonomy_sims-3.2.9/docs/css/mkdocstrings.css
+-rw-r--r--   0        0        0      895 2024-03-26 22:05:54.680286 safe_autonomy_sims-3.2.9/docs/css/style.css
+-rw-r--r--   0        0        0    36430 2024-03-26 22:05:54.680286 safe_autonomy_sims-3.2.9/docs/experiments.md
+-rw-r--r--   0        0        0     1005 2024-03-26 22:05:54.680286 safe_autonomy_sims-3.2.9/docs/gen_ref_nav.py
+-rw-r--r--   0        0        0   129349 2024-03-26 22:05:56.080272 safe_autonomy_sims-3.2.9/docs/images/HillsFrame2.png
+-rw-r--r--   0        0        0   130401 2024-03-26 22:05:56.084272 safe_autonomy_sims-3.2.9/docs/images/HillsFrame3.png
+-rw-r--r--   0        0        0    50311 2024-03-26 22:05:56.084272 safe_autonomy_sims-3.2.9/docs/images/inspection_problem.png
+-rw-r--r--   0        0        0    41425 2024-03-26 22:05:56.084272 safe_autonomy_sims-3.2.9/docs/images/linear.png
+-rw-r--r--   0        0        0    31143 2024-03-26 22:05:56.084272 safe_autonomy_sims-3.2.9/docs/images/relu.png
+-rw-r--r--   0        0        0    33502 2024-03-26 22:05:56.084272 safe_autonomy_sims-3.2.9/docs/images/tanh.png
+-rw-r--r--   0        0        0     6407 2024-03-26 22:05:56.084272 safe_autonomy_sims-3.2.9/docs/index.md
+-rw-r--r--   0        0        0     1393 2024-03-26 22:05:56.084272 safe_autonomy_sims-3.2.9/docs/install.md
+-rw-r--r--   0        0        0      392 2024-03-26 22:05:56.084272 safe_autonomy_sims-3.2.9/docs/javascripts/mathjax.js
+-rw-r--r--   0        0        0    22587 2024-03-26 22:05:56.084272 safe_autonomy_sims-3.2.9/docs/tasks/CWH/docking.md
+-rw-r--r--   0        0        0     2650 2024-03-26 22:05:56.084272 safe_autonomy_sims-3.2.9/docs/tasks/CWH/index.md
+-rw-r--r--   0        0        0    23806 2024-03-26 22:05:56.084272 safe_autonomy_sims-3.2.9/docs/tasks/CWH/multiagent_docking.md
+-rw-r--r--   0        0        0    27267 2024-03-26 22:05:56.088272 safe_autonomy_sims-3.2.9/docs/tasks/CWH/multiagent_translational_inspection.md
+-rw-r--r--   0        0        0    34877 2024-03-26 22:05:56.088272 safe_autonomy_sims-3.2.9/docs/tasks/CWH/multiagent_weighted_six_dof_inspection.md
+-rw-r--r--   0        0        0    28120 2024-03-26 22:05:56.088272 safe_autonomy_sims-3.2.9/docs/tasks/CWH/multiagent_weighted_translational_inspection.md
+-rw-r--r--   0        0        0    26682 2024-03-26 22:05:56.088272 safe_autonomy_sims-3.2.9/docs/tasks/CWH/translational_inspection.md
+-rw-r--r--   0        0        0    30735 2024-03-26 22:05:56.088272 safe_autonomy_sims-3.2.9/docs/tasks/CWH/weighted_six_dof_inspection.md
+-rw-r--r--   0        0        0    27367 2024-03-26 22:05:56.088272 safe_autonomy_sims-3.2.9/docs/tasks/CWH/weighted_translational_inspection.md
+-rw-r--r--   0        0        0     1207 2024-03-26 22:05:56.088272 safe_autonomy_sims-3.2.9/docs/tasks/index.md
+-rw-r--r--   0        0        0     2323 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/pyproject.toml
+-rw-r--r--   0        0        0      826 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/__init__.py
+-rw-r--r--   0        0        0      839 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/agents/__init__.py
+-rw-r--r--   0        0        0     2828 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/agents/rta_agent.py
+-rw-r--r--   0        0        0      935 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/dones/__init__.py
+-rw-r--r--   0        0        0    12175 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/dones/common_dones.py
+-rw-r--r--   0        0        0      627 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/dones/cwh/__init__.py
+-rw-r--r--   0        0        0    11159 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/dones/cwh/common.py
+-rw-r--r--   0        0        0    13464 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/dones/cwh/docking_dones.py
+-rw-r--r--   0        0        0    12337 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/dones/cwh/inspection_dones.py
+-rw-r--r--   0        0        0      673 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/evaluation/__init__.py
+-rw-r--r--   0        0        0      642 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/evaluation/animation/__init__.py
+-rw-r--r--   0        0        0     8202 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/evaluation/animation/base_animation.py
+-rw-r--r--   0        0        0    19448 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/evaluation/animation/inspection_animation.py
+-rw-r--r--   0        0        0    10705 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/evaluation/animation/six_dof_animation.py
+-rw-r--r--   0        0        0    38230 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/evaluation/evaluation_api.py
+-rw-r--r--   0        0        0     4992 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/evaluation/general_metrics.py
+-rw-r--r--   0        0        0     6725 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/evaluation/inspection_metrics.py
+-rw-r--r--   0        0        0      660 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/evaluation/launch/__init__.py
+-rw-r--r--   0        0        0     1824 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/evaluation/launch/serialize_cwh3d.py
+-rw-r--r--   0        0        0      786 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/experiments/__init__.py
+-rw-r--r--   0        0        0     7087 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/experiments/rllib_api_experiment.py
+-rw-r--r--   0        0        0    20658 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/experiments/safe_autonomy_rllib_api_experiment.py
+-rw-r--r--   0        0        0     1265 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/glues/__init__.py
+-rw-r--r--   0        0        0     3174 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/glues/coordinate_axis_glue.py
+-rw-r--r--   0        0        0     3348 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/glues/dot_product_glue.py
+-rw-r--r--   0        0        0      983 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/glues/magnitude_glue.py
+-rw-r--r--   0        0        0    10361 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/glues/rta_glue.py
+-rw-r--r--   0        0        0     7716 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/glues/six_dof_glues.py
+-rw-r--r--   0        0        0     3928 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/glues/vel_limit_glue.py
+-rw-r--r--   0        0        0     1063 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/platforms/__init__.py
+-rw-r--r--   0        0        0      614 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/platforms/common/__init__.py
+-rw-r--r--   0        0        0     3895 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/platforms/common/controllers.py
+-rw-r--r--   0        0        0     1757 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/platforms/common/platform.py
+-rw-r--r--   0        0        0     2085 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/platforms/common/sensors.py
+-rw-r--r--   0        0        0      612 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/platforms/cwh/__init__.py
+-rw-r--r--   0        0        0     1499 2024-03-26 22:05:56.092272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/platforms/cwh/cwh_available_platforms.py
+-rw-r--r--   0        0        0     7656 2024-03-26 22:05:56.096272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/platforms/cwh/cwh_platform.py
+-rw-r--r--   0        0        0    15755 2024-03-26 22:05:56.096272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/platforms/cwh/cwh_properties.py
+-rw-r--r--   0        0        0    21104 2024-03-26 22:05:56.096272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/platforms/cwh/cwh_sensors.py
+-rw-r--r--   0        0        0     5449 2024-03-26 22:05:56.096272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/platforms/cwh/rotation_sensors.py
+-rw-r--r--   0        0        0      970 2024-03-26 22:05:56.096272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/rewards/__init__.py
+-rw-r--r--   0        0        0      597 2024-03-26 22:05:56.096272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/rewards/cwh/__init__.py
+-rw-r--r--   0        0        0    21575 2024-03-26 22:05:56.096272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/rewards/cwh/docking_rewards.py
+-rw-r--r--   0        0        0     3976 2024-03-26 22:05:56.096272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/rewards/cwh/done_state_rewards.py
+-rw-r--r--   0        0        0     4320 2024-03-26 22:05:56.096272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/rewards/cwh/gaussian_decay_from_target_value.py
+-rw-r--r--   0        0        0    15636 2024-03-26 22:05:56.096272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/rewards/cwh/inspection_rewards.py
+-rw-r--r--   0        0        0     2097 2024-03-26 22:05:56.096272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/rewards/cwh/live_timestep_reward.py
+-rw-r--r--   0        0        0     1820 2024-03-26 22:05:56.096272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/rewards/rta_rewards.py
+-rw-r--r--   0        0        0     1016 2024-03-26 22:05:56.096272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/rta/__init__.py
+-rw-r--r--   0        0        0      602 2024-03-26 22:05:56.096272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/rta/cwh/__init__.py
+-rw-r--r--   0        0        0     9407 2024-03-26 22:05:56.096272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/rta/cwh/cwh_rta.py
+-rw-r--r--   0        0        0     5785 2024-03-26 22:05:56.096272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/rta/cwh/inspection_rta_1v1.py
+-rw-r--r--   0        0        0     8206 2024-03-26 22:05:56.096272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/rta/rta_rejection_sampler.py
+-rw-r--r--   0        0        0     1122 2024-03-26 22:05:56.096272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/simulators/__init__.py
+-rw-r--r--   0        0        0     1262 2024-03-26 22:05:56.096272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/simulators/cwh_simulator.py
+-rw-r--r--   0        0        0    22988 2024-03-26 22:05:56.096272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/simulators/illumination_functions.py
+-rw-r--r--   0        0        0      830 2024-03-26 22:05:56.096272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/simulators/initializers/__init__.py
+-rw-r--r--   0        0        0    15278 2024-03-26 22:05:56.096272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/simulators/initializers/cwh.py
+-rw-r--r--   0        0        0     7033 2024-03-26 22:05:56.096272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/simulators/initializers/initializer.py
+-rw-r--r--   0        0        0    31944 2024-03-26 22:05:56.096272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/simulators/inspection_simulator.py
+-rw-r--r--   0        0        0    16947 2024-03-26 22:05:56.096272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/simulators/saferl_simulator.py
+-rw-r--r--   0        0        0     9010 2024-03-26 22:05:56.096272 safe_autonomy_sims-3.2.9/safe_autonomy_sims/utils.py
+-rw-r--r--   0        0        0     7696 1970-01-01 00:00:00.000000 safe_autonomy_sims-3.2.9/PKG-INFO
```

### Comparing `safe_autonomy_sims-3.2.11/README.md` & `safe_autonomy_sims-3.2.9/README.md`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/docs/configuration.md` & `safe_autonomy_sims-3.2.9/docs/configuration.md`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/docs/css/style.css` & `safe_autonomy_sims-3.2.9/docs/css/style.css`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/docs/experiments.md` & `safe_autonomy_sims-3.2.9/docs/experiments.md`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/docs/gen_ref_nav.py` & `safe_autonomy_sims-3.2.9/docs/gen_ref_nav.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/docs/images/HillsFrame2.png` & `safe_autonomy_sims-3.2.9/docs/images/HillsFrame2.png`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/docs/images/HillsFrame3.png` & `safe_autonomy_sims-3.2.9/docs/images/HillsFrame3.png`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/docs/images/inspection_problem.png` & `safe_autonomy_sims-3.2.9/docs/images/inspection_problem.png`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/docs/images/linear.png` & `safe_autonomy_sims-3.2.9/docs/images/linear.png`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/docs/images/relu.png` & `safe_autonomy_sims-3.2.9/docs/images/relu.png`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/docs/images/tanh.png` & `safe_autonomy_sims-3.2.9/docs/images/tanh.png`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/docs/index.md` & `safe_autonomy_sims-3.2.9/docs/index.md`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/docs/install.md` & `safe_autonomy_sims-3.2.9/docs/install.md`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/docs/tasks/CWH/docking.md` & `safe_autonomy_sims-3.2.9/docs/tasks/CWH/docking.md`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/docs/tasks/CWH/index.md` & `safe_autonomy_sims-3.2.9/docs/tasks/CWH/index.md`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/docs/tasks/CWH/multiagent_docking.md` & `safe_autonomy_sims-3.2.9/docs/tasks/CWH/multiagent_docking.md`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/docs/tasks/CWH/multiagent_translational_inspection.md` & `safe_autonomy_sims-3.2.9/docs/tasks/CWH/multiagent_translational_inspection.md`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/docs/tasks/CWH/multiagent_weighted_six_dof_inspection.md` & `safe_autonomy_sims-3.2.9/docs/tasks/CWH/multiagent_weighted_six_dof_inspection.md`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/docs/tasks/CWH/multiagent_weighted_translational_inspection.md` & `safe_autonomy_sims-3.2.9/docs/tasks/CWH/multiagent_weighted_translational_inspection.md`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/docs/tasks/CWH/translational_inspection.md` & `safe_autonomy_sims-3.2.9/docs/tasks/CWH/translational_inspection.md`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/docs/tasks/CWH/weighted_six_dof_inspection.md` & `safe_autonomy_sims-3.2.9/docs/tasks/CWH/weighted_six_dof_inspection.md`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/docs/tasks/CWH/weighted_translational_inspection.md` & `safe_autonomy_sims-3.2.9/docs/tasks/CWH/weighted_translational_inspection.md`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/docs/tasks/index.md` & `safe_autonomy_sims-3.2.9/docs/tasks/index.md`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/pyproject.toml` & `safe_autonomy_sims-3.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "safe-autonomy-sims"
-version = "3.2.11"
+version = "3.2.9"
 description = "The Safe-Autonomy-Sims library provides the components and tools to build modular, integration-focused Reinforcement Learning environments with Run Time Assurance (RTA)"
 authors = [
     "Charles Keating <Charles.Keating@udri.udayton.edu>",
 ]
 license = ""
 readme = "README.md"
 homepage = "https://github.com/act3-ace/safe-autonomy-sims.git"
@@ -26,16 +26,16 @@
 tqdm = "^4.66.1"
 scikit-learn = "1.2.1"
 seaborn = "^0.12.0"
 torch = "1.13.0"
 imageio = "2.25.0"
 imageio-ffmpeg = "0.4.8"
 pint = "^0.22"
-safe-autonomy-dynamics = "1.2.3"
-run-time-assurance = "1.16.1"
+safe-autonomy-dynamics = "1.2.2"
+run-time-assurance = "1.15.3"
 corl = "3.14.13"
 
 [tool.poetry.group.lint.dependencies]
 pylint = "2.15.4"
 flake8 = "3.9.2"
 yapf = "^0.40.0"
 isort = "5.9.3"
```

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/__init__.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/__init__.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/agents/__init__.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/agents/rta_agent.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/agents/rta_agent.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/dones/__init__.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/dones/__init__.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/dones/common_dones.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/dones/common_dones.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/dones/cwh/__init__.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/dones/cwh/__init__.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/dones/cwh/common.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/dones/cwh/common.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/dones/cwh/docking_dones.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/dones/cwh/docking_dones.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/dones/cwh/inspection_dones.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/dones/cwh/inspection_dones.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/evaluation/__init__.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/evaluation/animation/__init__.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/evaluation/animation/__init__.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/evaluation/animation/base_animation.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/evaluation/animation/base_animation.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/evaluation/animation/inspection_animation.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/evaluation/animation/inspection_animation.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/evaluation/animation/six_dof_animation.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/evaluation/animation/six_dof_animation.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/evaluation/evaluation_api.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/evaluation/evaluation_api.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/evaluation/general_metrics.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/evaluation/general_metrics.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/evaluation/inspection_metrics.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/evaluation/inspection_metrics.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/evaluation/launch/__init__.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/evaluation/launch/__init__.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/evaluation/launch/serialize_cwh3d.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/evaluation/launch/serialize_cwh3d.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/experiments/__init__.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/experiments/__init__.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/experiments/rllib_api_experiment.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/experiments/rllib_api_experiment.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/experiments/safe_autonomy_rllib_api_experiment.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/experiments/safe_autonomy_rllib_api_experiment.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/glues/__init__.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/glues/__init__.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/glues/coordinate_axis_glue.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/glues/coordinate_axis_glue.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/glues/dot_product_glue.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/glues/dot_product_glue.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/glues/magnitude_glue.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/glues/magnitude_glue.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/glues/rta_glue.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/glues/rta_glue.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/glues/six_dof_glues.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/glues/six_dof_glues.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/glues/vel_limit_glue.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/glues/vel_limit_glue.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/platforms/__init__.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/platforms/__init__.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/platforms/common/__init__.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/platforms/common/__init__.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/platforms/common/controllers.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/platforms/common/controllers.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/platforms/common/platform.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/platforms/common/platform.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/platforms/common/sensors.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/platforms/common/sensors.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/platforms/cwh/__init__.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/platforms/cwh/__init__.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/platforms/cwh/cwh_available_platforms.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/platforms/cwh/cwh_available_platforms.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/platforms/cwh/cwh_platform.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/platforms/cwh/cwh_platform.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/platforms/cwh/cwh_properties.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/platforms/cwh/cwh_properties.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/platforms/cwh/cwh_sensors.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/platforms/cwh/cwh_sensors.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/platforms/cwh/rotation_sensors.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/platforms/cwh/rotation_sensors.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/rewards/__init__.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/rewards/__init__.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/rewards/cwh/__init__.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/rewards/cwh/__init__.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/rewards/cwh/docking_rewards.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/rewards/cwh/docking_rewards.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/rewards/cwh/done_state_rewards.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/rewards/cwh/done_state_rewards.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/rewards/cwh/gaussian_decay_from_target_value.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/rewards/cwh/gaussian_decay_from_target_value.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/rewards/cwh/inspection_rewards.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/rewards/cwh/inspection_rewards.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/rewards/cwh/live_timestep_reward.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/rewards/cwh/live_timestep_reward.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/rewards/rta_rewards.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/rewards/rta_rewards.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/rta/__init__.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/rta/__init__.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/rta/cwh/__init__.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/rta/cwh/__init__.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/rta/cwh/cwh_rta.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/rta/cwh/cwh_rta.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/rta/cwh/inspection_rta_1v1.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/rta/cwh/inspection_rta_1v1.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/rta/rta_rejection_sampler.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/rta/rta_rejection_sampler.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,15 +184,15 @@
         """
         assert isinstance(self.config.rta.functor(**self.config.rta.args).rta,
                           ConstraintBasedRTA), ("Must use constraint based rta for rejection sampling.")
         init_state_safe = True
 
         # For each constraint, check if satisfied
         for c in self.config.rta.functor(**self.config.rta.args).rta.constraints.values():
-            if c.phi(to_jnp_array_jit(state), c.params) < 0 or c(to_jnp_array_jit(state), c.params) < 0:
+            if c.phi(to_jnp_array_jit(state)) < 0 or c(to_jnp_array_jit(state)) < 0:
                 init_state_safe = False
                 break
         return init_state_safe
 
 
 class RejectionSamplerInitializerValidator(InitializerValidator):
     """
```

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/simulators/__init__.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/simulators/__init__.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/simulators/cwh_simulator.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/simulators/cwh_simulator.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/simulators/illumination_functions.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/simulators/illumination_functions.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/simulators/initializers/__init__.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/simulators/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/simulators/initializers/cwh.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/simulators/initializers/cwh.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/simulators/initializers/initializer.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/simulators/initializers/initializer.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/simulators/inspection_simulator.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/simulators/inspection_simulator.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/simulators/saferl_simulator.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/simulators/saferl_simulator.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/safe_autonomy_sims/utils.py` & `safe_autonomy_sims-3.2.9/safe_autonomy_sims/utils.py`

 * *Files identical despite different names*

### Comparing `safe_autonomy_sims-3.2.11/PKG-INFO` & `safe_autonomy_sims-3.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: safe-autonomy-sims
-Version: 3.2.11
+Version: 3.2.9
 Summary: The Safe-Autonomy-Sims library provides the components and tools to build modular, integration-focused Reinforcement Learning environments with Run Time Assurance (RTA)
 Home-page: https://github.com/act3-ace/safe-autonomy-sims.git
 Author: Charles Keating
 Author-email: Charles.Keating@udri.udayton.edu
 Requires-Python: >=3.10,<3.11
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: corl (==3.14.13)
 Requires-Dist: imageio (==2.25.0)
 Requires-Dist: imageio-ffmpeg (==0.4.8)
 Requires-Dist: numpy (==1.24.0)
 Requires-Dist: pint (>=0.22,<0.23)
-Requires-Dist: run-time-assurance (==1.16.1)
-Requires-Dist: safe-autonomy-dynamics (==1.2.3)
+Requires-Dist: run-time-assurance (==1.15.3)
+Requires-Dist: safe-autonomy-dynamics (==1.2.2)
 Requires-Dist: scikit-learn (==1.2.1)
 Requires-Dist: seaborn (>=0.12.0,<0.13.0)
 Requires-Dist: torch (==1.13.0)
 Requires-Dist: tqdm (>=4.66.1,<5.0.0)
 Project-URL: Documentation, https://github.com/act3-ace/safe-autonomy-sims/docs
 Project-URL: Repository, https://github.com/act3-ace/safe-autonomy-sims.git
 Description-Content-Type: text/markdown
```

