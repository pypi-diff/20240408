# Comparing `tmp/manipulation-2024.3.28.tar.gz` & `tmp/manipulation-2024.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manipulation-2024.3.28.tar", max compression
+gzip compressed data, was "manipulation-2024.4.8.tar", max compression
```

## Comparing `manipulation-2024.3.28.tar` & `manipulation-2024.4.8.tar`

### file list

```diff
@@ -1,146 +1,146 @@
--rw-r--r--   0        0        0     1561 2024-02-22 14:57:44.046800 manipulation-2024.3.28/LICENSE.TXT
--rw-r--r--   0        0        0      464 2024-02-22 14:57:44.046800 manipulation-2024.3.28/README.md
--rw-r--r--   0        0        0      167 2024-02-22 14:57:44.110801 manipulation-2024.3.28/manipulation/__init__.py
--rw-r--r--   0        0        0      846 2024-02-22 14:57:44.110801 manipulation-2024.3.28/manipulation/_static/custom.css
--rw-r--r--   0        0        0     6481 2024-02-22 14:57:44.114801 manipulation-2024.3.28/manipulation/clutter.py
--rw-r--r--   0        0        0      891 2024-02-22 14:57:44.114801 manipulation-2024.3.28/manipulation/conf.py
--rw-r--r--   0        0        0    16339 2024-02-22 14:57:44.114801 manipulation-2024.3.28/manipulation/create_sdf_from_mesh.py
--rw-r--r--   0        0        0      211 2024-02-22 14:57:44.114801 manipulation-2024.3.28/manipulation/drake_gym.py
--rw-r--r--   0        0        0     9221 2024-02-22 14:57:44.114801 manipulation-2024.3.28/manipulation/envs/box_flipup.py
--rw-r--r--   0        0        0     8482 2024-02-22 14:57:44.114801 manipulation-2024.3.28/manipulation/envs/planar_gripper_pushing_a_box.py
--rw-r--r--   0        0        0    32464 2024-02-22 14:57:44.114801 manipulation-2024.3.28/manipulation/exercises/clutter/normal_solution.npy
--rw-r--r--   0        0        0     1724 2024-02-22 14:57:44.114801 manipulation-2024.3.28/manipulation/exercises/clutter/test_analytic_grasp.py
--rw-r--r--   0        0        0     6751 2024-02-22 14:57:44.114801 manipulation-2024.3.28/manipulation/exercises/clutter/test_grasp_candidate.py
--rw-r--r--   0        0        0     1768 2024-02-22 14:57:44.114801 manipulation-2024.3.28/manipulation/exercises/clutter/test_normal.py
--rw-r--r--   0        0        0     3978 2024-02-22 14:57:44.114801 manipulation-2024.3.28/manipulation/exercises/clutter/test_simulation_tuning.py
--rw-r--r--   0        0        0     3598 2024-02-22 14:57:44.114801 manipulation-2024.3.28/manipulation/exercises/deep_perception/test_contrastive.py
--rw-r--r--   0        0        0     1563 2024-02-22 14:57:44.114801 manipulation-2024.3.28/manipulation/exercises/force/test_hybrid.py
--rw-r--r--   0        0        0     4758 2024-02-22 14:57:44.114801 manipulation-2024.3.28/manipulation/exercises/grader.py
--rw-r--r--   0        0        0     3934 2024-02-22 14:57:44.114801 manipulation-2024.3.28/manipulation/exercises/mobile/test_mobile_base_ik.py
--rw-r--r--   0        0        0     1188 2024-02-22 14:57:44.114801 manipulation-2024.3.28/manipulation/exercises/pick/plot_planar_manipulator.py
--rw-r--r--   0        0        0    26806 2024-02-22 14:57:44.114801 manipulation-2024.3.28/manipulation/exercises/pick/test_differential_ik.py
--rw-r--r--   0        0        0     3585 2024-02-22 14:57:44.114801 manipulation-2024.3.28/manipulation/exercises/pick/test_planar_manipulator.py
--rw-r--r--   0        0        0     2874 2024-02-22 14:57:44.114801 manipulation-2024.3.28/manipulation/exercises/pick/test_rigid_transforms.py
--rw-r--r--   0        0        0     1881 2024-02-22 14:57:44.114801 manipulation-2024.3.28/manipulation/exercises/pick/test_robot_painter.py
--rw-r--r--   0        0        0     1139 2024-02-22 14:57:44.114801 manipulation-2024.3.28/manipulation/exercises/pick/test_simple_qp.py
--rw-r--r--   0        0        0     3642 2024-02-22 14:57:44.114801 manipulation-2024.3.28/manipulation/exercises/pose/test_icp.py
--rw-r--r--   0        0        0     1445 2024-02-22 14:57:44.114801 manipulation-2024.3.28/manipulation/exercises/pose/test_pose_estimation.py
--rw-r--r--   0        0        0     3240 2024-02-22 14:57:44.114801 manipulation-2024.3.28/manipulation/exercises/pose/test_ransac.py
--rw-r--r--   0        0        0     3380 2024-02-22 14:57:44.114801 manipulation-2024.3.28/manipulation/exercises/rl/test_stochastic_optimization.py
--rw-r--r--   0        0        0     2825 2024-02-22 14:57:44.114801 manipulation-2024.3.28/manipulation/exercises/rl/test_vpg.py
--rw-r--r--   0        0        0      870 2024-02-22 14:57:44.114801 manipulation-2024.3.28/manipulation/exercises/robot/test_direct_joint_control.py
--rw-r--r--   0        0        0     1184 2024-02-22 14:57:44.114801 manipulation-2024.3.28/manipulation/exercises/robot/test_hardware_station_io.py
--rw-r--r--   0        0        0     2261 2024-02-22 14:57:44.114801 manipulation-2024.3.28/manipulation/exercises/robot/test_reflected_inertia.py
--rw-r--r--   0        0        0      672 2024-02-22 14:57:44.118801 manipulation-2024.3.28/manipulation/exercises/robot/test_survey.py
--rw-r--r--   0        0        0     1372 2024-02-22 14:57:44.118801 manipulation-2024.3.28/manipulation/exercises/segmentation/test_mask.py
--rw-r--r--   0        0        0     2271 2024-02-22 14:57:44.118801 manipulation-2024.3.28/manipulation/exercises/segmentation/test_segmentation_and_grasp.py
--rw-r--r--   0        0        0        0 2024-02-22 14:57:44.118801 manipulation-2024.3.28/manipulation/exercises/trajectories/rrt_planner/__init__.py
--rw-r--r--   0        0        0    23490 2024-02-22 14:57:44.118801 manipulation-2024.3.28/manipulation/exercises/trajectories/rrt_planner/geometry.py
--rw-r--r--   0        0        0     3711 2024-02-22 14:57:44.118801 manipulation-2024.3.28/manipulation/exercises/trajectories/rrt_planner/iiwa_rrt_problem.py
--rw-r--r--   0        0        0     6529 2024-02-22 14:57:44.118801 manipulation-2024.3.28/manipulation/exercises/trajectories/rrt_planner/robot.py
--rw-r--r--   0        0        0    14614 2024-02-22 14:57:44.118801 manipulation-2024.3.28/manipulation/exercises/trajectories/rrt_planner/rrt_planning.py
--rw-r--r--   0        0        0     1464 2024-02-22 14:57:44.118801 manipulation-2024.3.28/manipulation/exercises/trajectories/test_door_opening.py
--rw-r--r--   0        0        0     2391 2024-02-22 14:57:44.118801 manipulation-2024.3.28/manipulation/exercises/trajectories/test_rrt_planning.py
--rw-r--r--   0        0        0     5489 2024-02-22 14:57:44.118801 manipulation-2024.3.28/manipulation/exercises/trajectories/test_taskspace_iris.py
--rw-r--r--   0        0        0     3764 2024-02-22 14:57:44.118801 manipulation-2024.3.28/manipulation/icp.py
--rw-r--r--   0        0        0      243 2024-02-22 14:57:44.118801 manipulation-2024.3.28/manipulation/index.md
--rw-r--r--   0        0        0      256 2024-02-22 14:57:44.118801 manipulation-2024.3.28/manipulation/meshcat_cpp_utils.py
--rw-r--r--   0        0        0      102 2024-02-22 14:57:44.118801 manipulation-2024.3.28/manipulation/meshcat_utils.md
--rw-r--r--   0        0        0    17872 2024-02-22 14:57:44.118801 manipulation-2024.3.28/manipulation/meshcat_utils.py
--rw-r--r--   0        0        0     5938 2024-02-22 14:57:44.118801 manipulation-2024.3.28/manipulation/models/061_foam_brick_w_visual_contact_spheres.sdf
--rw-r--r--   0        0        0     1656 2024-02-22 14:57:44.118801 manipulation-2024.3.28/manipulation/models/book.sdf
--rw-r--r--   0        0        0     1280 2024-02-22 14:57:44.118801 manipulation-2024.3.28/manipulation/models/bunny/README
--rw-r--r--   0        0        0   658744 2024-02-22 14:57:44.122801 manipulation-2024.3.28/manipulation/models/bunny/bun_zipper_res2.ply
--rw-r--r--   0        0        0   196232 2024-02-22 14:57:44.126801 manipulation-2024.3.28/manipulation/models/bunny/bunny.npy
--rw-r--r--   0        0        0     1496 2024-02-22 14:57:44.126801 manipulation-2024.3.28/manipulation/models/camera_box.sdf
--rw-r--r--   0        0        0      155 2024-02-22 14:57:44.126801 manipulation-2024.3.28/manipulation/models/clutter.dmd.yaml
--rw-r--r--   0        0        0     1508 2024-02-22 14:57:44.126801 manipulation-2024.3.28/manipulation/models/clutter.scenarios.yaml
--rw-r--r--   0        0        0      367 2024-02-22 14:57:44.126801 manipulation-2024.3.28/manipulation/models/clutter_mustard.dmd.yaml
--rw-r--r--   0        0        0      183 2024-02-22 14:57:44.126801 manipulation-2024.3.28/manipulation/models/clutter_planning.dmd.yaml
--rw-r--r--   0        0        0      165 2024-02-22 14:57:44.126801 manipulation-2024.3.28/manipulation/models/clutter_w_cameras.dmd.yaml
--rw-r--r--   0        0        0     1966 2024-02-22 14:57:44.126801 manipulation-2024.3.28/manipulation/models/cupboard.scenario.yaml
--rw-r--r--   0        0        0     2485 2024-02-22 14:57:44.126801 manipulation-2024.3.28/manipulation/models/double_pendulum.urdf
--rw-r--r--   0        0        0      215 2024-02-22 14:57:44.126801 manipulation-2024.3.28/manipulation/models/floating_joint.urdf
--rw-r--r--   0        0        0     1407 2024-02-22 14:57:44.126801 manipulation-2024.3.28/manipulation/models/floor.sdf
--rw-r--r--   0        0        0     1471 2024-02-22 14:57:44.126801 manipulation-2024.3.28/manipulation/models/hydro/003_cracker_box.sdf
--rw-r--r--   0        0        0     1469 2024-02-22 14:57:44.126801 manipulation-2024.3.28/manipulation/models/hydro/004_sugar_box.sdf
--rw-r--r--   0        0        0     1630 2024-02-22 14:57:44.126801 manipulation-2024.3.28/manipulation/models/hydro/005_tomato_soup_can.sdf
--rw-r--r--   0        0        0     4990 2024-02-22 14:57:44.126801 manipulation-2024.3.28/manipulation/models/hydro/006_mustard_bottle.sdf
--rw-r--r--   0        0        0     1479 2024-02-22 14:57:44.126801 manipulation-2024.3.28/manipulation/models/hydro/009_gelatin_box.sdf
--rw-r--r--   0        0        0     1475 2024-02-22 14:57:44.126801 manipulation-2024.3.28/manipulation/models/hydro/010_potted_meat_can.sdf
--rw-r--r--   0        0        0     1104 2024-02-22 14:57:44.126801 manipulation-2024.3.28/manipulation/models/hydro/061_foam_brick.sdf
--rw-r--r--   0        0        0      246 2024-02-22 14:57:44.126801 manipulation-2024.3.28/manipulation/models/hydro/README.md
--rw-r--r--   0        0        0     4709 2024-02-22 14:57:44.126801 manipulation-2024.3.28/manipulation/models/hydro/bin.sdf
--rw-r--r--   0        0        0     9110 2024-02-22 14:57:44.126801 manipulation-2024.3.28/manipulation/models/hydro/cupboard.sdf
--rw-r--r--   0        0        0     6069 2024-02-22 14:57:44.126801 manipulation-2024.3.28/manipulation/models/hydro/extra_heavy_duty_table_surface_only_collision.sdf
--rw-r--r--   0        0        0     5708 2024-02-22 14:57:44.126801 manipulation-2024.3.28/manipulation/models/hydro/schunk_wsg_50_with_tip.sdf
--rw-r--r--   0        0        0    21069 2024-02-22 14:57:44.126801 manipulation-2024.3.28/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_000.obj
--rw-r--r--   0        0        0    21659 2024-02-22 14:57:44.126801 manipulation-2024.3.28/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_001.obj
--rw-r--r--   0        0        0    23842 2024-02-22 14:57:44.126801 manipulation-2024.3.28/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_002.obj
--rw-r--r--   0        0        0    24252 2024-02-22 14:57:44.126801 manipulation-2024.3.28/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_003.obj
--rw-r--r--   0        0        0    26183 2024-02-22 14:57:44.126801 manipulation-2024.3.28/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_004.obj
--rw-r--r--   0        0        0    15215 2024-02-22 14:57:44.126801 manipulation-2024.3.28/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_005.obj
--rw-r--r--   0        0        0    18773 2024-02-22 14:57:44.126801 manipulation-2024.3.28/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_006.obj
--rw-r--r--   0        0        0    23818 2024-02-22 14:57:44.126801 manipulation-2024.3.28/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_007.obj
--rw-r--r--   0        0        0    24964 2024-02-22 14:57:44.126801 manipulation-2024.3.28/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_008.obj
--rw-r--r--   0        0        0      658 2024-02-22 14:57:44.126801 manipulation-2024.3.28/manipulation/models/iiwa_and_wsg.dmd.yaml
--rw-r--r--   0        0        0      943 2024-02-22 14:57:44.126801 manipulation-2024.3.28/manipulation/models/mecanum/README.md
--rw-r--r--   0        0        0     1126 2024-02-22 14:57:44.126801 manipulation-2024.3.28/manipulation/models/mecanum/drake_obstacles.dmd.yaml
--rw-r--r--   0        0        0     3138 2024-02-22 14:57:44.126801 manipulation-2024.3.28/manipulation/models/mecanum/ground.sdf
--rw-r--r--   0        0        0    61205 2024-02-22 14:57:44.126801 manipulation-2024.3.28/manipulation/models/mecanum/mecanum_base.urdf
--rw-r--r--   0        0        0      673 2024-02-22 14:57:44.126801 manipulation-2024.3.28/manipulation/models/mecanum/obstacle_boxes.sdf
--rw-r--r--   0        0        0      663 2024-02-22 14:57:44.126801 manipulation-2024.3.28/manipulation/models/mecanum/obstacles.sdf
--rw-r--r--   0        0        0    19599 2024-02-22 14:57:44.126801 manipulation-2024.3.28/manipulation/models/mobile_iiwa14_primitive_collision.urdf
--rw-r--r--   0        0        0     1662 2024-02-22 14:57:44.126801 manipulation-2024.3.28/manipulation/models/mustard_w_cameras.dmd.yaml
--rw-r--r--   0        0        0      374 2024-02-22 14:57:44.126801 manipulation-2024.3.28/manipulation/models/package.xml
--rw-r--r--   0        0        0     2574 2024-02-22 14:57:44.126801 manipulation-2024.3.28/manipulation/models/planar_bin.sdf
--rw-r--r--   0        0        0     3716 2024-02-22 14:57:44.126801 manipulation-2024.3.28/manipulation/models/planar_foam_brick_collision_as_visual.sdf
--rw-r--r--   0        0        0    12684 2024-02-22 14:57:44.126801 manipulation-2024.3.28/manipulation/models/planar_iiwa14_no_collision.urdf
--rw-r--r--   0        0        0     1185 2024-02-22 14:57:44.126801 manipulation-2024.3.28/manipulation/models/planar_joint.sdf
--rw-r--r--   0        0        0     1074 2024-02-22 14:57:44.126801 manipulation-2024.3.28/manipulation/models/planar_manipulation_station.scenario.yaml
--rw-r--r--   0        0        0   141408 2024-02-22 14:57:44.126801 manipulation-2024.3.28/manipulation/models/pr2_collision_fixed.urdf
--rw-r--r--   0        0        0     1836 2024-02-22 14:57:44.126801 manipulation-2024.3.28/manipulation/models/pr2_shelves.dmd.yaml
--rw-r--r--   0        0        0    49209 2024-03-17 12:35:12.475299 manipulation-2024.3.28/manipulation/models/rubiks_cube.sdf
--rw-r--r--   0        0        0    15864 2024-02-22 14:57:44.130802 manipulation-2024.3.28/manipulation/models/rubiks_cube_2_by_2.sdf
--rw-r--r--   0        0        0      111 2024-02-22 14:57:44.130802 manipulation-2024.3.28/manipulation/models/schunk_wsg_50_welded_fingers.dmd.yaml
--rw-r--r--   0        0        0     2963 2024-02-22 14:57:44.130802 manipulation-2024.3.28/manipulation/models/schunk_wsg_50_welded_fingers.sdf
--rw-r--r--   0        0        0     2660 2024-02-22 14:57:44.130802 manipulation-2024.3.28/manipulation/models/schunk_wsg_50_welded_fingers_sphere.sdf
--rw-r--r--   0        0        0     2350 2024-02-22 14:57:44.130802 manipulation-2024.3.28/manipulation/models/segmentation_and_grasp_scene.dmd.yaml
--rw-r--r--   0        0        0     2784 2024-02-22 14:57:44.130802 manipulation-2024.3.28/manipulation/models/shelves.sdf
--rw-r--r--   0        0        0     2876 2024-02-22 14:57:44.130802 manipulation-2024.3.28/manipulation/models/shelves_w_ellipsoid_collision.sdf
--rw-r--r--   0        0        0     1388 2024-03-27 11:26:12.916327 manipulation-2024.3.28/manipulation/models/simple_2d_cspace.xml
--rw-r--r--   0        0        0      462 2024-03-27 10:57:46.553239 manipulation-2024.3.28/manipulation/models/simple_2d_obstacle.obj
--rw-r--r--   0        0        0      778 2024-02-22 14:57:44.130802 manipulation-2024.3.28/manipulation/models/spot/README.md
--rw-r--r--   0        0        0     4816 2024-02-22 14:57:44.130802 manipulation-2024.3.28/manipulation/models/spot/read_spot_camera_intrinsics.py
--rw-r--r--   0        0        0       21 2024-02-22 14:57:44.130802 manipulation-2024.3.28/manipulation/models/spot/requirements.txt
--rw-r--r--   0        0        0    27982 2024-02-22 14:57:44.130802 manipulation-2024.3.28/manipulation/models/spot/spot_with_arm.urdf
--rw-r--r--   0        0        0     3548 2024-02-22 14:57:44.130802 manipulation-2024.3.28/manipulation/models/spot/spot_with_arm_and_floating_base_actuators.scenario.yaml
--rw-r--r--   0        0        0    30003 2024-02-22 14:57:44.130802 manipulation-2024.3.28/manipulation/models/spot/spot_with_arm_and_floating_base_actuators.urdf
--rw-r--r--   0        0        0      390 2024-02-22 14:57:44.130802 manipulation-2024.3.28/manipulation/models/suction/README.md
--rw-r--r--   0        0        0     6386 2024-02-22 14:57:44.130802 manipulation-2024.3.28/manipulation/models/suction/base.obj
--rw-r--r--   0        0        0     6203 2024-02-22 14:57:44.130802 manipulation-2024.3.28/manipulation/models/suction/head.obj
--rw-r--r--   0        0        0    40367 2024-02-22 14:57:44.130802 manipulation-2024.3.28/manipulation/models/suction/mid.obj
--rw-r--r--   0        0        0     1382 2024-02-22 14:57:44.130802 manipulation-2024.3.28/manipulation/models/suction/suction-base.urdf
--rw-r--r--   0        0        0     3060 2024-02-22 14:57:44.130802 manipulation-2024.3.28/manipulation/models/suction/suction-head.urdf
--rw-r--r--   0        0        0    82673 2024-02-22 14:57:44.130802 manipulation-2024.3.28/manipulation/models/suction/tip.obj
--rw-r--r--   0        0        0      642 2024-02-22 14:57:44.130802 manipulation-2024.3.28/manipulation/models/two_bins.dmd.yaml
--rw-r--r--   0        0        0      686 2024-02-22 14:57:44.130802 manipulation-2024.3.28/manipulation/models/two_bins.sdf
--rw-r--r--   0        0        0     1915 2024-02-22 14:57:44.130802 manipulation-2024.3.28/manipulation/models/two_bins_w_cameras.dmd.yaml
--rw-r--r--   0        0        0     2459 2024-02-22 14:57:44.130802 manipulation-2024.3.28/manipulation/models/two_bins_w_cameras.sdf
--rw-r--r--   0        0        0    16331 2024-02-22 14:57:44.130802 manipulation-2024.3.28/manipulation/models/two_link_iiwa14.urdf
--rw-r--r--   0        0        0     2148 2024-02-22 14:57:44.130802 manipulation-2024.3.28/manipulation/mustard_depth_camera_example.py
--rw-r--r--   0        0        0     4190 2024-02-22 14:57:44.130802 manipulation-2024.3.28/manipulation/pick.py
--rw-r--r--   0        0        0    26643 2024-02-25 11:58:26.839161 manipulation-2024.3.28/manipulation/scenarios.py
--rw-r--r--   0        0        0       90 2024-02-22 14:57:44.130802 manipulation-2024.3.28/manipulation/station.md
--rw-r--r--   0        0        0    51234 2024-03-26 10:53:46.560515 manipulation-2024.3.28/manipulation/station.py
--rw-r--r--   0        0        0       90 2024-02-22 14:57:44.130802 manipulation-2024.3.28/manipulation/systems.md
--rw-r--r--   0        0        0     4801 2024-02-22 14:57:44.130802 manipulation-2024.3.28/manipulation/systems.py
--rw-r--r--   0        0        0     1547 2024-02-22 14:57:44.130802 manipulation-2024.3.28/manipulation/test/test_create_sdf_from_mesh.py
--rw-r--r--   0        0        0     2292 2024-02-22 14:57:44.130802 manipulation-2024.3.28/manipulation/test/test_gym.py
--rw-r--r--   0        0        0      425 2024-02-22 14:57:44.130802 manipulation-2024.3.28/manipulation/test/test_meshcat_utils.py
--rw-r--r--   0        0        0      561 2024-02-22 14:57:44.130802 manipulation-2024.3.28/manipulation/test/test_model_directives.py
--rw-r--r--   0        0        0      314 2024-02-22 14:57:44.130802 manipulation-2024.3.28/manipulation/test/test_utils.py
--rw-r--r--   0        0        0       86 2024-02-22 14:57:44.130802 manipulation-2024.3.28/manipulation/utils.md
--rw-r--r--   0        0        0     7226 2024-02-22 14:57:44.130802 manipulation-2024.3.28/manipulation/utils.py
--rw-r--r--   0        0        0     3284 2024-03-28 09:15:55.161340 manipulation-2024.3.28/pyproject.toml
--rw-r--r--   0        0        0     1517 1970-01-01 00:00:00.000000 manipulation-2024.3.28/PKG-INFO
+-rw-r--r--   0        0        0     1561 2024-02-22 14:57:44.046800 manipulation-2024.4.8/LICENSE.TXT
+-rw-r--r--   0        0        0      464 2024-02-22 14:57:44.046800 manipulation-2024.4.8/README.md
+-rw-r--r--   0        0        0      167 2024-02-22 14:57:44.110801 manipulation-2024.4.8/manipulation/__init__.py
+-rw-r--r--   0        0        0      846 2024-02-22 14:57:44.110801 manipulation-2024.4.8/manipulation/_static/custom.css
+-rw-r--r--   0        0        0     6481 2024-02-22 14:57:44.114801 manipulation-2024.4.8/manipulation/clutter.py
+-rw-r--r--   0        0        0      891 2024-02-22 14:57:44.114801 manipulation-2024.4.8/manipulation/conf.py
+-rw-r--r--   0        0        0    16339 2024-02-22 14:57:44.114801 manipulation-2024.4.8/manipulation/create_sdf_from_mesh.py
+-rw-r--r--   0        0        0      211 2024-02-22 14:57:44.114801 manipulation-2024.4.8/manipulation/drake_gym.py
+-rw-r--r--   0        0        0     9221 2024-02-22 14:57:44.114801 manipulation-2024.4.8/manipulation/envs/box_flipup.py
+-rw-r--r--   0        0        0     8482 2024-02-22 14:57:44.114801 manipulation-2024.4.8/manipulation/envs/planar_gripper_pushing_a_box.py
+-rw-r--r--   0        0        0    32464 2024-02-22 14:57:44.114801 manipulation-2024.4.8/manipulation/exercises/clutter/normal_solution.npy
+-rw-r--r--   0        0        0     1724 2024-02-22 14:57:44.114801 manipulation-2024.4.8/manipulation/exercises/clutter/test_analytic_grasp.py
+-rw-r--r--   0        0        0     6751 2024-02-22 14:57:44.114801 manipulation-2024.4.8/manipulation/exercises/clutter/test_grasp_candidate.py
+-rw-r--r--   0        0        0     1768 2024-02-22 14:57:44.114801 manipulation-2024.4.8/manipulation/exercises/clutter/test_normal.py
+-rw-r--r--   0        0        0     3978 2024-02-22 14:57:44.114801 manipulation-2024.4.8/manipulation/exercises/clutter/test_simulation_tuning.py
+-rw-r--r--   0        0        0     3598 2024-02-22 14:57:44.114801 manipulation-2024.4.8/manipulation/exercises/deep_perception/test_contrastive.py
+-rw-r--r--   0        0        0     1563 2024-02-22 14:57:44.114801 manipulation-2024.4.8/manipulation/exercises/force/test_hybrid.py
+-rw-r--r--   0        0        0     4758 2024-02-22 14:57:44.114801 manipulation-2024.4.8/manipulation/exercises/grader.py
+-rw-r--r--   0        0        0     3934 2024-02-22 14:57:44.114801 manipulation-2024.4.8/manipulation/exercises/mobile/test_mobile_base_ik.py
+-rw-r--r--   0        0        0     1188 2024-02-22 14:57:44.114801 manipulation-2024.4.8/manipulation/exercises/pick/plot_planar_manipulator.py
+-rw-r--r--   0        0        0    26806 2024-02-22 14:57:44.114801 manipulation-2024.4.8/manipulation/exercises/pick/test_differential_ik.py
+-rw-r--r--   0        0        0     3585 2024-02-22 14:57:44.114801 manipulation-2024.4.8/manipulation/exercises/pick/test_planar_manipulator.py
+-rw-r--r--   0        0        0     2874 2024-02-22 14:57:44.114801 manipulation-2024.4.8/manipulation/exercises/pick/test_rigid_transforms.py
+-rw-r--r--   0        0        0     1881 2024-02-22 14:57:44.114801 manipulation-2024.4.8/manipulation/exercises/pick/test_robot_painter.py
+-rw-r--r--   0        0        0     1139 2024-02-22 14:57:44.114801 manipulation-2024.4.8/manipulation/exercises/pick/test_simple_qp.py
+-rw-r--r--   0        0        0     3642 2024-02-22 14:57:44.114801 manipulation-2024.4.8/manipulation/exercises/pose/test_icp.py
+-rw-r--r--   0        0        0     1445 2024-02-22 14:57:44.114801 manipulation-2024.4.8/manipulation/exercises/pose/test_pose_estimation.py
+-rw-r--r--   0        0        0     3240 2024-02-22 14:57:44.114801 manipulation-2024.4.8/manipulation/exercises/pose/test_ransac.py
+-rw-r--r--   0        0        0     3380 2024-02-22 14:57:44.114801 manipulation-2024.4.8/manipulation/exercises/rl/test_stochastic_optimization.py
+-rw-r--r--   0        0        0     2825 2024-02-22 14:57:44.114801 manipulation-2024.4.8/manipulation/exercises/rl/test_vpg.py
+-rw-r--r--   0        0        0      870 2024-02-22 14:57:44.114801 manipulation-2024.4.8/manipulation/exercises/robot/test_direct_joint_control.py
+-rw-r--r--   0        0        0     1184 2024-02-22 14:57:44.114801 manipulation-2024.4.8/manipulation/exercises/robot/test_hardware_station_io.py
+-rw-r--r--   0        0        0     2261 2024-02-22 14:57:44.114801 manipulation-2024.4.8/manipulation/exercises/robot/test_reflected_inertia.py
+-rw-r--r--   0        0        0      672 2024-02-22 14:57:44.118801 manipulation-2024.4.8/manipulation/exercises/robot/test_survey.py
+-rw-r--r--   0        0        0     1372 2024-02-22 14:57:44.118801 manipulation-2024.4.8/manipulation/exercises/segmentation/test_mask.py
+-rw-r--r--   0        0        0     2271 2024-02-22 14:57:44.118801 manipulation-2024.4.8/manipulation/exercises/segmentation/test_segmentation_and_grasp.py
+-rw-r--r--   0        0        0        0 2024-02-22 14:57:44.118801 manipulation-2024.4.8/manipulation/exercises/trajectories/rrt_planner/__init__.py
+-rw-r--r--   0        0        0    23490 2024-02-22 14:57:44.118801 manipulation-2024.4.8/manipulation/exercises/trajectories/rrt_planner/geometry.py
+-rw-r--r--   0        0        0     3711 2024-02-22 14:57:44.118801 manipulation-2024.4.8/manipulation/exercises/trajectories/rrt_planner/iiwa_rrt_problem.py
+-rw-r--r--   0        0        0     6529 2024-02-22 14:57:44.118801 manipulation-2024.4.8/manipulation/exercises/trajectories/rrt_planner/robot.py
+-rw-r--r--   0        0        0    14614 2024-02-22 14:57:44.118801 manipulation-2024.4.8/manipulation/exercises/trajectories/rrt_planner/rrt_planning.py
+-rw-r--r--   0        0        0     1464 2024-02-22 14:57:44.118801 manipulation-2024.4.8/manipulation/exercises/trajectories/test_door_opening.py
+-rw-r--r--   0        0        0     2391 2024-02-22 14:57:44.118801 manipulation-2024.4.8/manipulation/exercises/trajectories/test_rrt_planning.py
+-rw-r--r--   0        0        0     5489 2024-02-22 14:57:44.118801 manipulation-2024.4.8/manipulation/exercises/trajectories/test_taskspace_iris.py
+-rw-r--r--   0        0        0     3764 2024-02-22 14:57:44.118801 manipulation-2024.4.8/manipulation/icp.py
+-rw-r--r--   0        0        0      243 2024-02-22 14:57:44.118801 manipulation-2024.4.8/manipulation/index.md
+-rw-r--r--   0        0        0      256 2024-02-22 14:57:44.118801 manipulation-2024.4.8/manipulation/meshcat_cpp_utils.py
+-rw-r--r--   0        0        0      102 2024-02-22 14:57:44.118801 manipulation-2024.4.8/manipulation/meshcat_utils.md
+-rw-r--r--   0        0        0    17872 2024-02-22 14:57:44.118801 manipulation-2024.4.8/manipulation/meshcat_utils.py
+-rw-r--r--   0        0        0     5938 2024-02-22 14:57:44.118801 manipulation-2024.4.8/manipulation/models/061_foam_brick_w_visual_contact_spheres.sdf
+-rw-r--r--   0        0        0     1656 2024-02-22 14:57:44.118801 manipulation-2024.4.8/manipulation/models/book.sdf
+-rw-r--r--   0        0        0     1280 2024-02-22 14:57:44.118801 manipulation-2024.4.8/manipulation/models/bunny/README
+-rw-r--r--   0        0        0   658744 2024-02-22 14:57:44.122801 manipulation-2024.4.8/manipulation/models/bunny/bun_zipper_res2.ply
+-rw-r--r--   0        0        0   196232 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/bunny/bunny.npy
+-rw-r--r--   0        0        0     1496 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/camera_box.sdf
+-rw-r--r--   0        0        0      155 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/clutter.dmd.yaml
+-rw-r--r--   0        0        0     1544 2024-04-08 12:21:31.612057 manipulation-2024.4.8/manipulation/models/clutter.scenarios.yaml
+-rw-r--r--   0        0        0      367 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/clutter_mustard.dmd.yaml
+-rw-r--r--   0        0        0      183 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/clutter_planning.dmd.yaml
+-rw-r--r--   0        0        0      165 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/clutter_w_cameras.dmd.yaml
+-rw-r--r--   0        0        0     2000 2024-04-08 12:21:31.612057 manipulation-2024.4.8/manipulation/models/cupboard.scenario.yaml
+-rw-r--r--   0        0        0     2485 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/double_pendulum.urdf
+-rw-r--r--   0        0        0      215 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/floating_joint.urdf
+-rw-r--r--   0        0        0     1407 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/floor.sdf
+-rw-r--r--   0        0        0     1471 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/hydro/003_cracker_box.sdf
+-rw-r--r--   0        0        0     1469 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/hydro/004_sugar_box.sdf
+-rw-r--r--   0        0        0     1630 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/hydro/005_tomato_soup_can.sdf
+-rw-r--r--   0        0        0     4990 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/hydro/006_mustard_bottle.sdf
+-rw-r--r--   0        0        0     1479 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/hydro/009_gelatin_box.sdf
+-rw-r--r--   0        0        0     1475 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/hydro/010_potted_meat_can.sdf
+-rw-r--r--   0        0        0     1104 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/hydro/061_foam_brick.sdf
+-rw-r--r--   0        0        0      246 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/hydro/README.md
+-rw-r--r--   0        0        0     4709 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/hydro/bin.sdf
+-rw-r--r--   0        0        0     9110 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/hydro/cupboard.sdf
+-rw-r--r--   0        0        0     6069 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/hydro/extra_heavy_duty_table_surface_only_collision.sdf
+-rw-r--r--   0        0        0     5708 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/hydro/schunk_wsg_50_with_tip.sdf
+-rw-r--r--   0        0        0    21069 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_000.obj
+-rw-r--r--   0        0        0    21659 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_001.obj
+-rw-r--r--   0        0        0    23842 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_002.obj
+-rw-r--r--   0        0        0    24252 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_003.obj
+-rw-r--r--   0        0        0    26183 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_004.obj
+-rw-r--r--   0        0        0    15215 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_005.obj
+-rw-r--r--   0        0        0    18773 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_006.obj
+-rw-r--r--   0        0        0    23818 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_007.obj
+-rw-r--r--   0        0        0    24964 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_008.obj
+-rw-r--r--   0        0        0      658 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/iiwa_and_wsg.dmd.yaml
+-rw-r--r--   0        0        0      943 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/mecanum/README.md
+-rw-r--r--   0        0        0     1126 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/mecanum/drake_obstacles.dmd.yaml
+-rw-r--r--   0        0        0     3138 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/mecanum/ground.sdf
+-rw-r--r--   0        0        0    61205 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/mecanum/mecanum_base.urdf
+-rw-r--r--   0        0        0      673 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/mecanum/obstacle_boxes.sdf
+-rw-r--r--   0        0        0      663 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/mecanum/obstacles.sdf
+-rw-r--r--   0        0        0    19599 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/mobile_iiwa14_primitive_collision.urdf
+-rw-r--r--   0        0        0     1662 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/mustard_w_cameras.dmd.yaml
+-rw-r--r--   0        0        0      374 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/package.xml
+-rw-r--r--   0        0        0     2574 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/planar_bin.sdf
+-rw-r--r--   0        0        0     3716 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/planar_foam_brick_collision_as_visual.sdf
+-rw-r--r--   0        0        0    12684 2024-03-29 13:38:05.672171 manipulation-2024.4.8/manipulation/models/planar_iiwa14_no_collision.urdf
+-rw-r--r--   0        0        0     1185 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/planar_joint.sdf
+-rw-r--r--   0        0        0     1114 2024-04-08 12:21:31.612057 manipulation-2024.4.8/manipulation/models/planar_manipulation_station.scenario.yaml
+-rw-r--r--   0        0        0   141408 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/pr2_collision_fixed.urdf
+-rw-r--r--   0        0        0     1836 2024-02-22 14:57:44.126801 manipulation-2024.4.8/manipulation/models/pr2_shelves.dmd.yaml
+-rw-r--r--   0        0        0    49209 2024-03-17 12:35:12.475299 manipulation-2024.4.8/manipulation/models/rubiks_cube.sdf
+-rw-r--r--   0        0        0    15864 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/models/rubiks_cube_2_by_2.sdf
+-rw-r--r--   0        0        0      111 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/models/schunk_wsg_50_welded_fingers.dmd.yaml
+-rw-r--r--   0        0        0     2963 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/models/schunk_wsg_50_welded_fingers.sdf
+-rw-r--r--   0        0        0     2660 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/models/schunk_wsg_50_welded_fingers_sphere.sdf
+-rw-r--r--   0        0        0     2350 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/models/segmentation_and_grasp_scene.dmd.yaml
+-rw-r--r--   0        0        0     2784 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/models/shelves.sdf
+-rw-r--r--   0        0        0     2876 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/models/shelves_w_ellipsoid_collision.sdf
+-rw-r--r--   0        0        0     1388 2024-03-27 11:26:12.916327 manipulation-2024.4.8/manipulation/models/simple_2d_cspace.xml
+-rw-r--r--   0        0        0      462 2024-03-27 10:57:46.553239 manipulation-2024.4.8/manipulation/models/simple_2d_obstacle.obj
+-rw-r--r--   0        0        0      778 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/models/spot/README.md
+-rw-r--r--   0        0        0     4816 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/models/spot/read_spot_camera_intrinsics.py
+-rw-r--r--   0        0        0       21 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/models/spot/requirements.txt
+-rw-r--r--   0        0        0    27982 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/models/spot/spot_with_arm.urdf
+-rw-r--r--   0        0        0     3548 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/models/spot/spot_with_arm_and_floating_base_actuators.scenario.yaml
+-rw-r--r--   0        0        0    30003 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/models/spot/spot_with_arm_and_floating_base_actuators.urdf
+-rw-r--r--   0        0        0      390 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/models/suction/README.md
+-rw-r--r--   0        0        0     6386 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/models/suction/base.obj
+-rw-r--r--   0        0        0     6203 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/models/suction/head.obj
+-rw-r--r--   0        0        0    40367 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/models/suction/mid.obj
+-rw-r--r--   0        0        0     1382 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/models/suction/suction-base.urdf
+-rw-r--r--   0        0        0     3060 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/models/suction/suction-head.urdf
+-rw-r--r--   0        0        0    82673 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/models/suction/tip.obj
+-rw-r--r--   0        0        0      642 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/models/two_bins.dmd.yaml
+-rw-r--r--   0        0        0      686 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/models/two_bins.sdf
+-rw-r--r--   0        0        0     1915 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/models/two_bins_w_cameras.dmd.yaml
+-rw-r--r--   0        0        0     2459 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/models/two_bins_w_cameras.sdf
+-rw-r--r--   0        0        0    16331 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/models/two_link_iiwa14.urdf
+-rw-r--r--   0        0        0     2148 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/mustard_depth_camera_example.py
+-rw-r--r--   0        0        0     4190 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/pick.py
+-rw-r--r--   0        0        0    26555 2024-04-08 12:21:31.612057 manipulation-2024.4.8/manipulation/scenarios.py
+-rw-r--r--   0        0        0       90 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/station.md
+-rw-r--r--   0        0        0    50383 2024-04-08 12:21:31.612057 manipulation-2024.4.8/manipulation/station.py
+-rw-r--r--   0        0        0       90 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/systems.md
+-rw-r--r--   0        0        0     4801 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/systems.py
+-rw-r--r--   0        0        0     1547 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/test/test_create_sdf_from_mesh.py
+-rw-r--r--   0        0        0     2292 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/test/test_gym.py
+-rw-r--r--   0        0        0      425 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/test/test_meshcat_utils.py
+-rw-r--r--   0        0        0      561 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/test/test_model_directives.py
+-rw-r--r--   0        0        0      314 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/test/test_utils.py
+-rw-r--r--   0        0        0       86 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/utils.md
+-rw-r--r--   0        0        0     7226 2024-02-22 14:57:44.130802 manipulation-2024.4.8/manipulation/utils.py
+-rw-r--r--   0        0        0     3284 2024-04-08 12:21:57.004494 manipulation-2024.4.8/pyproject.toml
+-rw-r--r--   0        0        0     1516 1970-01-01 00:00:00.000000 manipulation-2024.4.8/PKG-INFO
```

### Comparing `manipulation-2024.3.28/LICENSE.TXT` & `manipulation-2024.4.8/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/_static/custom.css` & `manipulation-2024.4.8/manipulation/_static/custom.css`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/clutter.py` & `manipulation-2024.4.8/manipulation/clutter.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/conf.py` & `manipulation-2024.4.8/manipulation/conf.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/create_sdf_from_mesh.py` & `manipulation-2024.4.8/manipulation/create_sdf_from_mesh.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/envs/box_flipup.py` & `manipulation-2024.4.8/manipulation/envs/box_flipup.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/envs/planar_gripper_pushing_a_box.py` & `manipulation-2024.4.8/manipulation/envs/planar_gripper_pushing_a_box.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/exercises/clutter/normal_solution.npy` & `manipulation-2024.4.8/manipulation/exercises/clutter/normal_solution.npy`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/exercises/clutter/test_analytic_grasp.py` & `manipulation-2024.4.8/manipulation/exercises/clutter/test_analytic_grasp.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/exercises/clutter/test_grasp_candidate.py` & `manipulation-2024.4.8/manipulation/exercises/clutter/test_grasp_candidate.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/exercises/clutter/test_normal.py` & `manipulation-2024.4.8/manipulation/exercises/clutter/test_normal.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/exercises/clutter/test_simulation_tuning.py` & `manipulation-2024.4.8/manipulation/exercises/clutter/test_simulation_tuning.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/exercises/deep_perception/test_contrastive.py` & `manipulation-2024.4.8/manipulation/exercises/deep_perception/test_contrastive.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/exercises/force/test_hybrid.py` & `manipulation-2024.4.8/manipulation/exercises/force/test_hybrid.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/exercises/grader.py` & `manipulation-2024.4.8/manipulation/exercises/grader.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/exercises/mobile/test_mobile_base_ik.py` & `manipulation-2024.4.8/manipulation/exercises/mobile/test_mobile_base_ik.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/exercises/pick/plot_planar_manipulator.py` & `manipulation-2024.4.8/manipulation/exercises/pick/plot_planar_manipulator.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/exercises/pick/test_differential_ik.py` & `manipulation-2024.4.8/manipulation/exercises/pick/test_differential_ik.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/exercises/pick/test_planar_manipulator.py` & `manipulation-2024.4.8/manipulation/exercises/pick/test_planar_manipulator.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/exercises/pick/test_rigid_transforms.py` & `manipulation-2024.4.8/manipulation/exercises/pick/test_rigid_transforms.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/exercises/pick/test_robot_painter.py` & `manipulation-2024.4.8/manipulation/exercises/pick/test_robot_painter.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/exercises/pick/test_simple_qp.py` & `manipulation-2024.4.8/manipulation/exercises/pick/test_simple_qp.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/exercises/pose/test_icp.py` & `manipulation-2024.4.8/manipulation/exercises/pose/test_icp.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/exercises/pose/test_pose_estimation.py` & `manipulation-2024.4.8/manipulation/exercises/pose/test_pose_estimation.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/exercises/pose/test_ransac.py` & `manipulation-2024.4.8/manipulation/exercises/pose/test_ransac.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/exercises/rl/test_stochastic_optimization.py` & `manipulation-2024.4.8/manipulation/exercises/rl/test_stochastic_optimization.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/exercises/rl/test_vpg.py` & `manipulation-2024.4.8/manipulation/exercises/rl/test_vpg.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/exercises/robot/test_direct_joint_control.py` & `manipulation-2024.4.8/manipulation/exercises/robot/test_direct_joint_control.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/exercises/robot/test_hardware_station_io.py` & `manipulation-2024.4.8/manipulation/exercises/robot/test_hardware_station_io.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/exercises/robot/test_reflected_inertia.py` & `manipulation-2024.4.8/manipulation/exercises/robot/test_reflected_inertia.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/exercises/robot/test_survey.py` & `manipulation-2024.4.8/manipulation/exercises/robot/test_survey.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/exercises/segmentation/test_mask.py` & `manipulation-2024.4.8/manipulation/exercises/segmentation/test_mask.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/exercises/segmentation/test_segmentation_and_grasp.py` & `manipulation-2024.4.8/manipulation/exercises/segmentation/test_segmentation_and_grasp.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/exercises/trajectories/rrt_planner/geometry.py` & `manipulation-2024.4.8/manipulation/exercises/trajectories/rrt_planner/geometry.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/exercises/trajectories/rrt_planner/iiwa_rrt_problem.py` & `manipulation-2024.4.8/manipulation/exercises/trajectories/rrt_planner/iiwa_rrt_problem.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/exercises/trajectories/rrt_planner/robot.py` & `manipulation-2024.4.8/manipulation/exercises/trajectories/rrt_planner/robot.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/exercises/trajectories/rrt_planner/rrt_planning.py` & `manipulation-2024.4.8/manipulation/exercises/trajectories/rrt_planner/rrt_planning.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/exercises/trajectories/test_door_opening.py` & `manipulation-2024.4.8/manipulation/exercises/trajectories/test_door_opening.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/exercises/trajectories/test_rrt_planning.py` & `manipulation-2024.4.8/manipulation/exercises/trajectories/test_rrt_planning.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/exercises/trajectories/test_taskspace_iris.py` & `manipulation-2024.4.8/manipulation/exercises/trajectories/test_taskspace_iris.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/icp.py` & `manipulation-2024.4.8/manipulation/icp.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/meshcat_utils.py` & `manipulation-2024.4.8/manipulation/meshcat_utils.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/061_foam_brick_w_visual_contact_spheres.sdf` & `manipulation-2024.4.8/manipulation/models/061_foam_brick_w_visual_contact_spheres.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/book.sdf` & `manipulation-2024.4.8/manipulation/models/book.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/bunny/README` & `manipulation-2024.4.8/manipulation/models/bunny/README`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/bunny/bun_zipper_res2.ply` & `manipulation-2024.4.8/manipulation/models/bunny/bun_zipper_res2.ply`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/bunny/bunny.npy` & `manipulation-2024.4.8/manipulation/models/bunny/bunny.npy`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/camera_box.sdf` & `manipulation-2024.4.8/manipulation/models/camera_box.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/clutter.scenarios.yaml` & `manipulation-2024.4.8/manipulation/models/clutter.scenarios.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
       name: camera5
       depth: True
       X_PB:
         base_frame: camera5::base
 
   model_drivers:
       iiwa: !IiwaDriver
+        control_mode: position_only
         hand_model_name: wsg
       wsg: !SchunkWsgDriver {}
 
 Mustard:
   <<: *Clutter
   directives:
   - add_directives:
```

### Comparing `manipulation-2024.3.28/manipulation/models/cupboard.scenario.yaml` & `manipulation-2024.4.8/manipulation/models/cupboard.scenario.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -64,9 +64,10 @@
     parent: world
     child: camera2::base
     X_PC:
         translation: [0.786258, -0.048422, 1.043315]
         rotation: !Rpy { deg: [150.0, 1.3, 88]}
 model_drivers:
     iiwa: !IiwaDriver
+      control_mode: position_only
       hand_model_name: wsg
     wsg: !SchunkWsgDriver {}
```

### Comparing `manipulation-2024.3.28/manipulation/models/double_pendulum.urdf` & `manipulation-2024.4.8/manipulation/models/double_pendulum.urdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/floor.sdf` & `manipulation-2024.4.8/manipulation/models/floor.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/hydro/003_cracker_box.sdf` & `manipulation-2024.4.8/manipulation/models/hydro/003_cracker_box.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/hydro/004_sugar_box.sdf` & `manipulation-2024.4.8/manipulation/models/hydro/004_sugar_box.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/hydro/005_tomato_soup_can.sdf` & `manipulation-2024.4.8/manipulation/models/hydro/005_tomato_soup_can.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/hydro/006_mustard_bottle.sdf` & `manipulation-2024.4.8/manipulation/models/hydro/006_mustard_bottle.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/hydro/009_gelatin_box.sdf` & `manipulation-2024.4.8/manipulation/models/hydro/009_gelatin_box.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/hydro/010_potted_meat_can.sdf` & `manipulation-2024.4.8/manipulation/models/hydro/010_potted_meat_can.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/hydro/061_foam_brick.sdf` & `manipulation-2024.4.8/manipulation/models/hydro/061_foam_brick.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/hydro/bin.sdf` & `manipulation-2024.4.8/manipulation/models/hydro/bin.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/hydro/cupboard.sdf` & `manipulation-2024.4.8/manipulation/models/hydro/cupboard.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/hydro/extra_heavy_duty_table_surface_only_collision.sdf` & `manipulation-2024.4.8/manipulation/models/hydro/extra_heavy_duty_table_surface_only_collision.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/hydro/schunk_wsg_50_with_tip.sdf` & `manipulation-2024.4.8/manipulation/models/hydro/schunk_wsg_50_with_tip.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_000.obj` & `manipulation-2024.4.8/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_000.obj`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_001.obj` & `manipulation-2024.4.8/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_001.obj`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_002.obj` & `manipulation-2024.4.8/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_002.obj`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_003.obj` & `manipulation-2024.4.8/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_003.obj`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_004.obj` & `manipulation-2024.4.8/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_004.obj`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_005.obj` & `manipulation-2024.4.8/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_005.obj`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_006.obj` & `manipulation-2024.4.8/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_006.obj`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_007.obj` & `manipulation-2024.4.8/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_007.obj`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_008.obj` & `manipulation-2024.4.8/manipulation/models/hydro/ycb_mustard_bottle_mesh_pieces/mesh_piece_008.obj`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/iiwa_and_wsg.dmd.yaml` & `manipulation-2024.4.8/manipulation/models/iiwa_and_wsg.dmd.yaml`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/mecanum/README.md` & `manipulation-2024.4.8/manipulation/models/mecanum/README.md`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/mecanum/drake_obstacles.dmd.yaml` & `manipulation-2024.4.8/manipulation/models/mecanum/drake_obstacles.dmd.yaml`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/mecanum/ground.sdf` & `manipulation-2024.4.8/manipulation/models/mecanum/ground.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/mecanum/mecanum_base.urdf` & `manipulation-2024.4.8/manipulation/models/mecanum/mecanum_base.urdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/mecanum/obstacle_boxes.sdf` & `manipulation-2024.4.8/manipulation/models/mecanum/obstacle_boxes.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/mecanum/obstacles.sdf` & `manipulation-2024.4.8/manipulation/models/mecanum/obstacles.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/mobile_iiwa14_primitive_collision.urdf` & `manipulation-2024.4.8/manipulation/models/mobile_iiwa14_primitive_collision.urdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/mustard_w_cameras.dmd.yaml` & `manipulation-2024.4.8/manipulation/models/mustard_w_cameras.dmd.yaml`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/planar_bin.sdf` & `manipulation-2024.4.8/manipulation/models/planar_bin.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/planar_foam_brick_collision_as_visual.sdf` & `manipulation-2024.4.8/manipulation/models/planar_foam_brick_collision_as_visual.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/planar_iiwa14_no_collision.urdf` & `manipulation-2024.4.8/manipulation/models/planar_iiwa14_no_collision.urdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/planar_joint.sdf` & `manipulation-2024.4.8/manipulation/models/planar_joint.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/planar_manipulation_station.scenario.yaml` & `manipulation-2024.4.8/manipulation/models/planar_manipulation_station.scenario.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -32,9 +32,10 @@
 - add_weld:
     parent: world
     child: work_table::link
     X_PC:
         translation: [0.75, 0, -0.7645]
 model_drivers:
     iiwa: !IiwaDriver
+      control_mode: position_and_torque
       hand_model_name: wsg
     wsg: !SchunkWsgDriver {}
```

### Comparing `manipulation-2024.3.28/manipulation/models/pr2_collision_fixed.urdf` & `manipulation-2024.4.8/manipulation/models/pr2_collision_fixed.urdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/pr2_shelves.dmd.yaml` & `manipulation-2024.4.8/manipulation/models/pr2_shelves.dmd.yaml`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/rubiks_cube.sdf` & `manipulation-2024.4.8/manipulation/models/rubiks_cube.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/rubiks_cube_2_by_2.sdf` & `manipulation-2024.4.8/manipulation/models/rubiks_cube_2_by_2.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/schunk_wsg_50_welded_fingers.sdf` & `manipulation-2024.4.8/manipulation/models/schunk_wsg_50_welded_fingers.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/schunk_wsg_50_welded_fingers_sphere.sdf` & `manipulation-2024.4.8/manipulation/models/schunk_wsg_50_welded_fingers_sphere.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/segmentation_and_grasp_scene.dmd.yaml` & `manipulation-2024.4.8/manipulation/models/segmentation_and_grasp_scene.dmd.yaml`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/shelves.sdf` & `manipulation-2024.4.8/manipulation/models/shelves.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/shelves_w_ellipsoid_collision.sdf` & `manipulation-2024.4.8/manipulation/models/shelves_w_ellipsoid_collision.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/simple_2d_cspace.xml` & `manipulation-2024.4.8/manipulation/models/simple_2d_cspace.xml`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/spot/README.md` & `manipulation-2024.4.8/manipulation/models/spot/README.md`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/spot/read_spot_camera_intrinsics.py` & `manipulation-2024.4.8/manipulation/models/spot/read_spot_camera_intrinsics.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/spot/spot_with_arm.urdf` & `manipulation-2024.4.8/manipulation/models/spot/spot_with_arm.urdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/spot/spot_with_arm_and_floating_base_actuators.scenario.yaml` & `manipulation-2024.4.8/manipulation/models/spot/spot_with_arm_and_floating_base_actuators.scenario.yaml`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/spot/spot_with_arm_and_floating_base_actuators.urdf` & `manipulation-2024.4.8/manipulation/models/spot/spot_with_arm_and_floating_base_actuators.urdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/suction/base.obj` & `manipulation-2024.4.8/manipulation/models/suction/base.obj`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/suction/head.obj` & `manipulation-2024.4.8/manipulation/models/suction/head.obj`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/suction/mid.obj` & `manipulation-2024.4.8/manipulation/models/suction/mid.obj`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/suction/suction-base.urdf` & `manipulation-2024.4.8/manipulation/models/suction/suction-base.urdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/suction/suction-head.urdf` & `manipulation-2024.4.8/manipulation/models/suction/suction-head.urdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/suction/tip.obj` & `manipulation-2024.4.8/manipulation/models/suction/tip.obj`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/two_bins.dmd.yaml` & `manipulation-2024.4.8/manipulation/models/two_bins.dmd.yaml`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/two_bins.sdf` & `manipulation-2024.4.8/manipulation/models/two_bins.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/two_bins_w_cameras.dmd.yaml` & `manipulation-2024.4.8/manipulation/models/two_bins_w_cameras.dmd.yaml`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/two_bins_w_cameras.sdf` & `manipulation-2024.4.8/manipulation/models/two_bins_w_cameras.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/models/two_link_iiwa14.urdf` & `manipulation-2024.4.8/manipulation/models/two_link_iiwa14.urdf`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/mustard_depth_camera_example.py` & `manipulation-2024.4.8/manipulation/mustard_depth_camera_example.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/pick.py` & `manipulation-2024.4.8/manipulation/pick.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/scenarios.py` & `manipulation-2024.4.8/manipulation/scenarios.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,14 @@
 
 
 class WsgPositions(Enum):
     OPEN = 0.107
     CLOSED = 0.002
 
 
-# TODO: take argument for whether we want the welded fingers version or not
 def AddWsg(plant, iiwa_model_instance, roll=np.pi / 2.0, welded=False, sphere=False):
     parser = Parser(plant)
     ConfigureParser(parser)
     if welded:
         if sphere:
             file = "package://manipulation/schunk_wsg_50_welded_fingers_sphere.sdf"
         else:
@@ -663,15 +662,15 @@
                 PassThrough([0] * num_iiwa_positions)
             )
             builder.Connect(
                 torque_passthrough.get_output_port(), adder.get_input_port(1)
             )
             builder.ExportInput(
                 torque_passthrough.get_input_port(),
-                model_instance_name + "_feedforward_torque",
+                model_instance_name + "_torque",
             )
             builder.Connect(
                 adder.get_output_port(),
                 plant.get_actuation_input_port(model_instance),
             )
 
             # Add discrete derivative to command velocities.
```

### Comparing `manipulation-2024.3.28/manipulation/station.py` & `manipulation-2024.4.8/manipulation/station.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,30 +10,30 @@
 from drake import (
     lcmt_iiwa_command,
     lcmt_iiwa_status,
     lcmt_schunk_wsg_command,
     lcmt_schunk_wsg_status,
 )
 from pydrake.all import (
-    Adder,
     ApplyCameraConfig,
     ApplyLcmBusConfig,
     ApplyMultibodyPlantConfig,
     ApplyVisualizationConfig,
     BaseField,
     CameraConfig,
     CameraInfo,
-    Demultiplexer,
     DepthImageToPointCloud,
     Diagram,
     DiagramBuilder,
     DrakeLcmParams,
     FlattenModelDirectives,
+    Gain,
     GetScopedFrameByName,
     IiwaCommandSender,
+    IiwaControlMode,
     IiwaDriver,
     IiwaStatusReceiver,
     InverseDynamicsController,
     LcmBuses,
     LcmPublisherSystem,
     LcmSubscriberSystem,
     LeafSystem,
@@ -42,31 +42,35 @@
     MeshcatPointCloudVisualizer,
     ModelDirective,
     ModelDirectives,
     ModelInstanceIndex,
     ModelInstanceInfo,
     MultibodyPlant,
     MultibodyPlantConfig,
+    Multiplexer,
     OutputPort,
+    ParseIiwaControlMode,
     Parser,
-    PassThrough,
     PdControllerGains,
     ProcessModelDirectives,
     RobotDiagram,
     RobotDiagramBuilder,
     SceneGraph,
     SchunkWsgCommandSender,
     SchunkWsgDriver,
     SchunkWsgPositionController,
     SchunkWsgStatusReceiver,
     ScopedName,
+    SharedPointerSystem,
+    SimIiwaDriver,
     SimulatorConfig,
-    StateInterpolatorWithDiscreteDerivative,
     VisualizationConfig,
     ZeroForceDriver,
+    position_enabled,
+    torque_enabled,
 )
 from pydrake.common.yaml import yaml_load_typed
 
 from manipulation.scenarios import AddIiwa, AddPlanarIiwa, AddWsg
 from manipulation.systems import ExtractPose
 from manipulation.utils import ConfigureParser
 
@@ -359,15 +363,15 @@
     children_to_freeze = set()
     if model_instance_names and add_frozen_child_instances:
         children_to_freeze = _FindChildren(flattened_directives, model_instance_names)
     all_model_instances = children_to_freeze.union(model_instance_names)
 
     directives = []
     for d in flattened_directives:
-        if d.add_model and (d.add_model.name in model_instance_names):
+        if d.add_model and (d.add_model.name in all_model_instances):
             directives.append(d)
         if (
             d.add_weld
             and (
                 ScopedName.Parse(d.add_weld.child).get_namespace()
                 in all_model_instances
             )
@@ -562,135 +566,61 @@
 
 
 # TODO(russt): Use the c++ version pending https://github.com/RobotLocomotion/drake/issues/20055
 def _ApplyDriverConfigSim(
     driver_config,  # See Scenario.model_drivers for typing
     model_instance_name: str,
     sim_plant: MultibodyPlant,
-    directives: typing.List[ModelDirective],
-    models_from_directives_map: typing.Mapping[str, typing.List[ModelInstanceInfo]],
+    scenario: Scenario,
     package_xmls: typing.List[str],
     builder: DiagramBuilder,
 ) -> None:
     if isinstance(driver_config, IiwaDriver):
         model_instance = sim_plant.GetModelInstanceByName(model_instance_name)
         num_iiwa_positions = sim_plant.num_positions(model_instance)
 
-        # I need a PassThrough system so that I can export the input port.
-        iiwa_position = builder.AddSystem(PassThrough(num_iiwa_positions))
-        builder.ExportInput(
-            iiwa_position.get_input_port(),
-            model_instance_name + ".position",
-        )
-        builder.ExportOutput(
-            iiwa_position.get_output_port(),
-            model_instance_name + ".position_commanded",
-        )
-
-        # Export the iiwa "state" outputs.
-        demux = builder.AddSystem(
-            Demultiplexer(2 * num_iiwa_positions, num_iiwa_positions)
-        )
-        builder.Connect(
-            sim_plant.get_state_output_port(model_instance),
-            demux.get_input_port(),
-        )
-        builder.ExportOutput(
-            demux.get_output_port(0),
-            model_instance_name + ".position_measured",
-        )
-        builder.ExportOutput(
-            demux.get_output_port(1),
-            model_instance_name + ".velocity_estimated",
-        )
-        builder.ExportOutput(
-            sim_plant.get_state_output_port(model_instance),
-            model_instance_name + ".state_estimated",
-        )
-
         # Make the plant for the iiwa controller to use.
+        # TODO: The current hardcoded implementation should be replaced with the
+        # MakeMultibodyPlant below, once adding frozen children is supported in Drake.
+        # controller_plant = MakeMultibodyPlant(
+        #     scenario=scenario,
+        #     model_instance_names=[model_instance_name],
+        #     add_frozen_child_instances=True,
+        #     package_xmls=package_xmls,
+        # )
         controller_plant = MultibodyPlant(time_step=sim_plant.time_step())
-        # TODO: Add the correct IIWA model (introspected from MBP). See
-        # build_iiwa_control in Drake for a slightly closer attempt.
         if num_iiwa_positions == 3:
             controller_iiwa = AddPlanarIiwa(controller_plant)
         else:
             controller_iiwa = AddIiwa(controller_plant)
         AddWsg(controller_plant, controller_iiwa, welded=True)
         controller_plant.Finalize()
-
-        # Add the iiwa controller
-        iiwa_controller = builder.AddSystem(
-            InverseDynamicsController(
-                controller_plant,
-                kp=[100] * num_iiwa_positions,
-                ki=[1] * num_iiwa_positions,
-                kd=[20] * num_iiwa_positions,
-                has_reference_acceleration=False,
-            )
-        )
-        iiwa_controller.set_name(model_instance_name + ".controller")
-        builder.Connect(
-            sim_plant.get_state_output_port(model_instance),
-            iiwa_controller.get_input_port_estimated_state(),
-        )
-
-        # Add in the feed-forward torque
-        adder = builder.AddSystem(Adder(2, num_iiwa_positions))
-        builder.Connect(
-            iiwa_controller.get_output_port_control(),
-            adder.get_input_port(0),
-        )
-        # Use a PassThrough to make the port optional (it will provide zero
-        # values if not connected).
-        torque_passthrough = builder.AddSystem(PassThrough([0] * num_iiwa_positions))
-        builder.Connect(torque_passthrough.get_output_port(), adder.get_input_port(1))
-        builder.ExportInput(
-            torque_passthrough.get_input_port(),
-            model_instance_name + ".feedforward_torque",
-        )
-        builder.Connect(
-            adder.get_output_port(),
-            sim_plant.get_actuation_input_port(model_instance),
-        )
-
-        # Add discrete derivative to command velocities.
-        desired_state_from_position = builder.AddSystem(
-            StateInterpolatorWithDiscreteDerivative(
-                num_iiwa_positions,
-                sim_plant.time_step(),
-                suppress_initial_transient=True,
-            )
-        )
-        desired_state_from_position.set_name(
-            model_instance_name + ".desired_state_from_position"
-        )
-        builder.Connect(
-            desired_state_from_position.get_output_port(),
-            iiwa_controller.get_input_port_desired_state(),
-        )
-        builder.Connect(
-            iiwa_position.get_output_port(),
-            desired_state_from_position.get_input_port(),
-        )
-
-        # Export commanded torques.
-        builder.ExportOutput(
-            adder.get_output_port(),
-            model_instance_name + ".torque_commanded",
-        )
-        builder.ExportOutput(
-            adder.get_output_port(),
-            model_instance_name + ".torque_measured",
-        )
-
-        builder.ExportOutput(
-            sim_plant.get_generalized_contact_forces_output_port(model_instance),
-            model_instance_name + ".torque_external",
-        )
+        # Keep the controller plant alive during the Diagram lifespan.
+        builder.AddNamedSystem(
+            f"{model_instance_name}_controller_plant_pointer_system",
+            SharedPointerSystem(controller_plant),
+        )
+
+        control_mode = ParseIiwaControlMode(driver_config.control_mode)
+        sim_iiwa_driver = SimIiwaDriver.AddToBuilder(
+            plant=sim_plant,
+            iiwa_instance=model_instance,
+            controller_plant=controller_plant,
+            builder=builder,
+            ext_joint_filter_tau=0.01,
+            desired_iiwa_kp_gains=np.full(num_iiwa_positions, 100),
+            control_mode=control_mode,
+        )
+        for i in range(sim_iiwa_driver.num_input_ports()):
+            port = sim_iiwa_driver.get_input_port(i)
+            if not builder.IsConnectedOrExported(port):
+                builder.ExportInput(port, f"{model_instance_name}.{port.get_name()}")
+        for i in range(sim_iiwa_driver.num_output_ports()):
+            port = sim_iiwa_driver.get_output_port(i)
+            builder.ExportOutput(port, f"{model_instance_name}.{port.get_name()}")
 
     elif isinstance(driver_config, SchunkWsgDriver):
         model_instance = sim_plant.GetModelInstanceByName(model_instance_name)
         # Wsg controller.
         wsg_controller = builder.AddSystem(SchunkWsgPositionController())
         wsg_controller.set_name(model_instance_name + ".controller")
         builder.Connect(
@@ -736,15 +666,15 @@
         for p in package_xmls:
             parser.package_map().AddPackageXml(p)
         ConfigureParser(parser)
 
         # Make the plant for the iiwa controller to use.
         controller_directives = []
         for d in FlattenModelDirectives(
-            ModelDirectives(directives=directives), parser.package_map()
+            ModelDirectives(directives=scenario.directives), parser.package_map()
         ).directives:
             if d.add_model and (d.add_model.name in model_instance_names):
                 controller_directives.append(d)
             if (
                 d.add_weld
                 and (
                     ScopedName.Parse(d.add_weld.child).get_namespace()
@@ -842,31 +772,26 @@
         )
 
 
 def _ApplyDriverConfigsSim(
     *,
     driver_configs,  # See Scenario.model_drivers for typing
     sim_plant: MultibodyPlant,
-    directives: typing.List[ModelDirective],
-    models_from_directives: typing.Mapping[str, typing.List[ModelInstanceInfo]],
+    scenario: Scenario,
     package_xmls: typing.List[str],
     builder: DiagramBuilder,
 ) -> None:
-    models_from_directives_map = dict(
-        [(info.model_name, info) for info in models_from_directives]
-    )
     for model_instance_name, driver_config in driver_configs.items():
         _ApplyDriverConfigSim(
-            driver_config,
-            model_instance_name,
-            sim_plant,
-            directives,
-            models_from_directives_map,
-            package_xmls,
-            builder,
+            driver_config=driver_config,
+            model_instance_name=model_instance_name,
+            sim_plant=sim_plant,
+            scenario=scenario,
+            package_xmls=package_xmls,
+            builder=builder,
         )
 
 
 def _ApplyPrefinalizeDriverConfigSim(
     driver_config,  # See Scenario.model_drivers for typing
     model_instance_name: str,
     sim_plant: MultibodyPlant,
@@ -1031,16 +956,15 @@
     # messages and dispatching them to the receivers, i.e., "pump" the bus.)
     lcm_buses = ApplyLcmBusConfig(lcm_buses=scenario.lcm_buses, builder=builder)
 
     # Add drivers.
     _ApplyDriverConfigsSim(
         driver_configs=scenario.model_drivers,
         sim_plant=sim_plant,
-        directives=scenario.directives,
-        models_from_directives=added_models,
+        scenario=scenario,
         package_xmls=package_xmls,
         builder=builder,
     )
 
     # Setup a virtual display if needed (for simulating cameras)
     if scenario.cameras and sys.platform == "linux" and os.getenv("DISPLAY") is None:
         from pyvirtualdisplay import Display
@@ -1086,47 +1010,76 @@
         prebuild_callback(builder)
 
     diagram = robot_builder.Build()
     diagram.set_name("station")
     return diagram
 
 
+def NegatedPort(
+    builder: DiagramBuilder, output_port: OutputPort, prefix: str = ""
+) -> OutputPort:
+    """Negates the output of the given port.
+
+    Args:
+        builder: The diagram builder to add the negation system to.
+        output_port: The output port to negate.
+        prefix: The prefix to use for the negation system.
+
+    Returns:
+        The output port of the negation system.
+    """
+    negater = builder.AddNamedSystem(
+        f"sign_flip_{prefix}{output_port.get_name()}", Gain(-1, size=output_port.size())
+    )
+    builder.Connect(output_port, negater.get_input_port())
+    return negater.get_output_port()
+
+
 # TODO(russt): Use the c++ version pending https://github.com/RobotLocomotion/drake/issues/20055
 def _ApplyDriverConfigInterface(
     driver_config,  # See Scenario.model_drivers for typing
     model_instance_name: str,
     plant: MultibodyPlant,
     models_from_directives_map: typing.Mapping[str, typing.List[ModelInstanceInfo]],
     lcm_buses: LcmBuses,
     builder: DiagramBuilder,
 ) -> None:
     if isinstance(driver_config, IiwaDriver):
         lcm = lcm_buses.Find("Driver for " + model_instance_name, driver_config.lcm_bus)
 
         # Publish IIWA command.
-        iiwa_command_sender = builder.AddSystem(IiwaCommandSender())
-        # Note on publish period: IIWA driver won't respond faster than 200Hz
+        # Note on publish period: IIWA driver won't respond faster than 1000Hz in
+        # torque_only mode and 200Hz in other modes
+        control_mode = ParseIiwaControlMode(driver_config.control_mode)
+        publish_period = 0.005
+        if control_mode == IiwaControlMode.kTorqueOnly:
+            publish_period = 0.001
+        iiwa_command_sender = builder.AddSystem(
+            IiwaCommandSender(control_mode=control_mode)
+        )
         iiwa_command_publisher = builder.AddSystem(
             LcmPublisherSystem.Make(
                 channel="IIWA_COMMAND",
                 lcm_type=lcmt_iiwa_command,
                 lcm=lcm,
-                publish_period=0.005,
+                publish_period=publish_period,
                 use_cpp_serializer=True,
             )
         )
         iiwa_command_publisher.set_name(model_instance_name + ".command_publisher")
-        builder.ExportInput(
-            iiwa_command_sender.get_position_input_port(),
-            model_instance_name + ".position",
-        )
-        builder.ExportInput(
-            iiwa_command_sender.get_torque_input_port(),
-            model_instance_name + ".feedforward_torque",
-        )
+        if position_enabled(control_mode):
+            builder.ExportInput(
+                iiwa_command_sender.get_position_input_port(),
+                model_instance_name + ".position",
+            )
+        if torque_enabled(control_mode):
+            builder.ExportInput(
+                iiwa_command_sender.get_torque_input_port(),
+                model_instance_name + ".torque",
+            )
         builder.Connect(
             iiwa_command_sender.get_output_port(),
             iiwa_command_publisher.get_input_port(),
         )
         # Receive IIWA status and populate the output ports.
         iiwa_status_receiver = builder.AddSystem(IiwaStatusReceiver())
         iiwa_status_subscriber = builder.AddSystem(
@@ -1136,43 +1089,62 @@
                 lcm=lcm,
                 use_cpp_serializer=True,
                 wait_for_message_on_initialization_timeout=10,
             )
         )
         iiwa_status_subscriber.set_name(model_instance_name + ".status_subscriber")
 
-        # builder.Connect(
-        #    iiwa_status_receiver.get_position_measured_output_port(),
-        #    to_pose.get_input_port(),
-        # )
-
         builder.ExportOutput(
             iiwa_status_receiver.get_position_commanded_output_port(),
             model_instance_name + ".position_commanded",
         )
         builder.ExportOutput(
             iiwa_status_receiver.get_position_measured_output_port(),
             model_instance_name + ".position_measured",
         )
         builder.ExportOutput(
             iiwa_status_receiver.get_velocity_estimated_output_port(),
             model_instance_name + ".velocity_estimated",
         )
+        # These are *negative* w.r.t. the conventions outlined in
+        # drake/manipulation/README.
         builder.ExportOutput(
-            iiwa_status_receiver.get_torque_commanded_output_port(),
+            NegatedPort(
+                builder=builder,
+                output_port=iiwa_status_receiver.get_torque_commanded_output_port(),
+                prefix=model_instance_name,
+            ),
             model_instance_name + ".torque_commanded",
         )
         builder.ExportOutput(
-            iiwa_status_receiver.get_torque_measured_output_port(),
+            NegatedPort(
+                builder=builder,
+                output_port=iiwa_status_receiver.get_torque_measured_output_port(),
+                prefix=model_instance_name,
+            ),
             model_instance_name + ".torque_measured",
         )
         builder.ExportOutput(
             iiwa_status_receiver.get_torque_external_output_port(),
             model_instance_name + ".torque_external",
         )
+
+        iiwa_state_mux: Multiplexer = builder.AddSystem(Multiplexer([7, 7]))
+        builder.Connect(
+            iiwa_status_receiver.get_position_measured_output_port(),
+            iiwa_state_mux.get_input_port(0),
+        )
+        builder.Connect(
+            iiwa_status_receiver.get_velocity_estimated_output_port(),
+            iiwa_state_mux.get_input_port(1),
+        )
+        builder.ExportOutput(
+            iiwa_state_mux.get_output_port(), model_instance_name + ".state_estimated"
+        )
+
         builder.Connect(
             iiwa_status_subscriber.get_output_port(),
             iiwa_status_receiver.get_input_port(),
         )
     if isinstance(driver_config, SchunkWsgDriver):
         lcm = lcm_buses.Find("Driver for " + model_instance_name, driver_config.lcm_bus)
```

### Comparing `manipulation-2024.3.28/manipulation/systems.py` & `manipulation-2024.4.8/manipulation/systems.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/test/test_create_sdf_from_mesh.py` & `manipulation-2024.4.8/manipulation/test/test_create_sdf_from_mesh.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/test/test_gym.py` & `manipulation-2024.4.8/manipulation/test/test_gym.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/test/test_model_directives.py` & `manipulation-2024.4.8/manipulation/test/test_model_directives.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/manipulation/utils.py` & `manipulation-2024.4.8/manipulation/utils.py`

 * *Files identical despite different names*

### Comparing `manipulation-2024.3.28/pyproject.toml` & `manipulation-2024.4.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "manipulation"
 # Use e.g. 2023.10.4.rc0 if I need to release a release candidate.
 # Use e.g. 2023.10.4.post1 if I need to rerelease on the same day.
-version = "2024.03.28"
+version = "2024.04.08"
 description = "MIT 6.421 - Robotic Manipulation"
 authors = ["Russ Tedrake <russt@mit.edu>"]
 license = "BSD License"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: BSD License"
```

### Comparing `manipulation-2024.3.28/PKG-INFO` & `manipulation-2024.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manipulation
-Version: 2024.3.28
+Version: 2024.4.8
 Summary: MIT 6.421 - Robotic Manipulation
 License: BSD License
 Author: Russ Tedrake
 Author-email: russt@mit.edu
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: License :: Other/Proprietary License
```

