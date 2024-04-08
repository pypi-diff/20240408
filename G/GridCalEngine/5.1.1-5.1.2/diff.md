# Comparing `tmp/GridCalEngine-5.1.1.tar.gz` & `tmp/GridCalEngine-5.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GridCalEngine-5.1.1.tar", last modified: Wed Apr  3 10:11:16 2024, max compression
+gzip compressed data, was "GridCalEngine-5.1.2.tar", last modified: Mon Apr  8 13:35:50 2024, max compression
```

## Comparing `GridCalEngine-5.1.1.tar` & `GridCalEngine-5.1.2.tar`

### file list

```diff
@@ -1,677 +1,678 @@
--rw-rw-r--   0 santi     (1000) santi     (1000)     2270 2024-04-03 10:10:53.840547 GridCalEngine-5.1.1/GridCalEngine/__version__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      790 2024-02-13 14:28:28.615734 GridCalEngine-5.1.1/GridCalEngine/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11585 2024-03-11 19:28:12.203075 GridCalEngine-5.1.1/GridCalEngine/LICENSE.txt
--rw-rw-r--   0 santi     (1000) santi     (1000)    10942 2024-03-14 19:48:07.696505 GridCalEngine-5.1.1/GridCalEngine/data_logger.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    38586 2024-03-28 10:16:48.988877 GridCalEngine-5.1.1/GridCalEngine/enumerations.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    23610 2024-03-14 19:48:07.696505 GridCalEngine-5.1.1/GridCalEngine/basic_structures.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3008 2024-03-11 19:28:12.223075 GridCalEngine-5.1.1/GridCalEngine/api.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.538645 GridCalEngine-5.1.1/GridCalEngine/Utils/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4960 2024-03-28 10:16:48.988877 GridCalEngine-5.1.1/GridCalEngine/Utils/Filtering/objects_filtering.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1037 2024-03-11 19:28:12.223075 GridCalEngine-5.1.1/GridCalEngine/Utils/Filtering/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5922 2024-03-11 19:28:12.223075 GridCalEngine-5.1.1/GridCalEngine/Utils/Filtering/timeseries_filtering.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9710 2024-03-28 10:16:48.988877 GridCalEngine-5.1.1/GridCalEngine/Utils/Filtering/filtering.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    10146 2024-03-14 19:48:07.696505 GridCalEngine-5.1.1/GridCalEngine/Utils/Filtering/results_table_filtering.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3555 2024-02-20 09:29:33.592105 GridCalEngine-5.1.1/GridCalEngine/Utils/NumericalMethods/common.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-02-13 14:28:28.615734 GridCalEngine-5.1.1/GridCalEngine/Utils/NumericalMethods/iwamoto.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6314 2024-02-20 09:29:33.592105 GridCalEngine-5.1.1/GridCalEngine/Utils/NumericalMethods/levenberg_marquadt.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    15007 2024-03-17 11:12:27.697061 GridCalEngine-5.1.1/GridCalEngine/Utils/NumericalMethods/ips.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-02-13 14:28:28.615734 GridCalEngine-5.1.1/GridCalEngine/Utils/NumericalMethods/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6918 2024-03-11 19:28:12.223075 GridCalEngine-5.1.1/GridCalEngine/Utils/NumericalMethods/newton_raphson.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3618 2024-03-11 19:28:12.223075 GridCalEngine-5.1.1/GridCalEngine/Utils/NumericalMethods/weldorf_online_stddev.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7272 2024-02-20 09:29:33.592105 GridCalEngine-5.1.1/GridCalEngine/Utils/NumericalMethods/powell.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-02-13 14:28:28.615734 GridCalEngine-5.1.1/GridCalEngine/Utils/NumericalMethods/newton_raphson_ode.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6454 2024-02-13 14:28:28.615734 GridCalEngine-5.1.1/GridCalEngine/Utils/NumericalMethods/autodiff.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5184 2024-03-11 19:28:12.223075 GridCalEngine-5.1.1/GridCalEngine/Utils/NumericalMethods/sparse_solve.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      898 2024-02-13 14:28:28.615734 GridCalEngine-5.1.1/GridCalEngine/Utils/Sparse/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    35003 2024-03-11 19:28:12.223075 GridCalEngine-5.1.1/GridCalEngine/Utils/Sparse/csc_numba.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    20288 2024-02-20 09:29:33.592105 GridCalEngine-5.1.1/GridCalEngine/Utils/Sparse/csc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2602 2024-02-13 14:28:28.615734 GridCalEngine-5.1.1/GridCalEngine/Utils/Sparse/utils.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.538645 GridCalEngine-5.1.1/GridCalEngine/Utils/ThirdParty/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.538645 GridCalEngine-5.1.1/GridCalEngine/Utils/ThirdParty/SyntheticNetworks/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    16616 2024-03-14 19:48:07.696505 GridCalEngine-5.1.1/GridCalEngine/Utils/ThirdParty/SyntheticNetworks/rpgm_algo.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3271 2024-02-13 14:28:28.615734 GridCalEngine-5.1.1/GridCalEngine/Utils/MIP/selected_interface.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.538645 GridCalEngine-5.1.1/GridCalEngine/Utils/MIP/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11191 2024-04-03 10:10:53.840547 GridCalEngine-5.1.1/GridCalEngine/Utils/MIP/ortools_interface.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8598 2024-02-13 14:28:28.615734 GridCalEngine-5.1.1/GridCalEngine/Utils/MIP/pulp_interface.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      971 2024-02-13 14:28:28.615734 GridCalEngine-5.1.1/GridCalEngine/Utils/MIP/SimpleMip/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    12785 2024-02-13 14:28:28.615734 GridCalEngine-5.1.1/GridCalEngine/Utils/MIP/SimpleMip/lpobjects.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    23363 2024-02-13 14:28:28.615734 GridCalEngine-5.1.1/GridCalEngine/Utils/MIP/SimpleMip/lpmodel.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3095 2024-02-13 14:28:28.615734 GridCalEngine-5.1.1/GridCalEngine/Utils/MIP/SimpleMip/highs.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    12143 2024-03-11 19:28:12.223075 GridCalEngine-5.1.1/GridCalEngine/Topology/topology.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-11 19:28:12.223075 GridCalEngine-5.1.1/GridCalEngine/Topology/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    21011 2024-03-14 19:59:31.536490 GridCalEngine-5.1.1/GridCalEngine/Topology/simulation_indices.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9597 2024-03-14 19:48:07.692505 GridCalEngine-5.1.1/GridCalEngine/Topology/topology_substation_reduction.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    27056 2024-04-01 07:29:23.260927 GridCalEngine-5.1.1/GridCalEngine/Topology/admittance_matrices.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      644 2023-11-16 09:36:26.522645 GridCalEngine-5.1.1/GridCalEngine/IO/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    19662 2024-03-14 19:48:07.688505 GridCalEngine-5.1.1/GridCalEngine/IO/file_handler.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      361 2023-11-16 09:36:26.530645 GridCalEngine-5.1.1/GridCalEngine/IO/file_system.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.522645 GridCalEngine-5.1.1/GridCalEngine/IO/base/base_device.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.522645 GridCalEngine-5.1.1/GridCalEngine/IO/base/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4486 2023-11-16 09:36:26.522645 GridCalEngine-5.1.1/GridCalEngine/IO/base/units.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      200 2023-11-16 09:36:26.522645 GridCalEngine-5.1.1/GridCalEngine/IO/base/base_circuit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2588 2024-03-14 19:48:07.684505 GridCalEngine-5.1.1/GridCalEngine/IO/base/base_property.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.530645 GridCalEngine-5.1.1/GridCalEngine/IO/dgs/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    41779 2024-03-14 19:48:07.688505 GridCalEngine-5.1.1/GridCalEngine/IO/dgs/dgs_parser.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    87374 2024-03-14 19:48:07.688505 GridCalEngine-5.1.1/GridCalEngine/IO/raw/raw_parser_legacy.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.530645 GridCalEngine-5.1.1/GridCalEngine/IO/raw/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2636 2024-03-14 19:48:07.688505 GridCalEngine-5.1.1/GridCalEngine/IO/raw/raw_functions.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4036 2024-03-11 19:28:12.203075 GridCalEngine-5.1.1/GridCalEngine/IO/raw/rawx_parser_writer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    18318 2024-02-13 14:28:28.603734 GridCalEngine-5.1.1/GridCalEngine/IO/raw/raw_parser_writer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      245 2024-03-11 19:28:12.203075 GridCalEngine-5.1.1/GridCalEngine/IO/raw/gridcal_to_raw.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    31801 2024-03-14 19:48:07.688505 GridCalEngine-5.1.1/GridCalEngine/IO/raw/raw_to_gridcal.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    48436 2024-03-14 19:48:07.688505 GridCalEngine-5.1.1/GridCalEngine/IO/raw/rawx_parser_legacy.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1892 2024-03-14 19:48:07.688505 GridCalEngine-5.1.1/GridCalEngine/IO/raw/devices/gne_device.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9804 2024-02-13 14:28:28.603734 GridCalEngine-5.1.1/GridCalEngine/IO/raw/devices/switched_shunt.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1288 2023-11-16 09:36:26.530645 GridCalEngine-5.1.1/GridCalEngine/IO/raw/devices/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5779 2024-02-13 14:28:28.603734 GridCalEngine-5.1.1/GridCalEngine/IO/raw/devices/system_switching_device.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5949 2024-02-13 14:28:28.603734 GridCalEngine-5.1.1/GridCalEngine/IO/raw/devices/psse_object.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    54576 2024-02-13 14:28:28.603734 GridCalEngine-5.1.1/GridCalEngine/IO/raw/devices/transformer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    12199 2024-02-13 14:28:28.603734 GridCalEngine-5.1.1/GridCalEngine/IO/raw/devices/facts.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2338 2024-02-13 14:28:28.603734 GridCalEngine-5.1.1/GridCalEngine/IO/raw/devices/owner.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3520 2024-02-13 14:28:28.603734 GridCalEngine-5.1.1/GridCalEngine/IO/raw/devices/inter_area.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1811 2024-02-13 14:28:28.603734 GridCalEngine-5.1.1/GridCalEngine/IO/raw/devices/psse_property.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    13081 2024-03-11 19:28:12.203075 GridCalEngine-5.1.1/GridCalEngine/IO/raw/devices/generator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    23805 2024-02-13 14:28:28.603734 GridCalEngine-5.1.1/GridCalEngine/IO/raw/devices/two_terminal_dc_line.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7667 2024-02-13 14:28:28.603734 GridCalEngine-5.1.1/GridCalEngine/IO/raw/devices/psse_circuit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7998 2024-02-13 14:28:28.603734 GridCalEngine-5.1.1/GridCalEngine/IO/raw/devices/bus.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    21807 2024-02-13 14:28:28.603734 GridCalEngine-5.1.1/GridCalEngine/IO/raw/devices/vsc_dc_line.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3434 2024-02-13 14:28:28.603734 GridCalEngine-5.1.1/GridCalEngine/IO/raw/devices/area.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    16814 2024-03-11 19:28:12.203075 GridCalEngine-5.1.1/GridCalEngine/IO/raw/devices/induction_machine.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3338 2024-03-11 19:28:12.203075 GridCalEngine-5.1.1/GridCalEngine/IO/raw/devices/fixed_shunt.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    10649 2024-02-13 14:28:28.603734 GridCalEngine-5.1.1/GridCalEngine/IO/raw/devices/load.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4135 2024-02-13 14:28:28.603734 GridCalEngine-5.1.1/GridCalEngine/IO/raw/devices/node.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2335 2024-02-13 14:28:28.603734 GridCalEngine-5.1.1/GridCalEngine/IO/raw/devices/zone.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11887 2024-02-13 14:28:28.603734 GridCalEngine-5.1.1/GridCalEngine/IO/raw/devices/branch.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3486 2024-03-11 19:28:12.203075 GridCalEngine-5.1.1/GridCalEngine/IO/raw/devices/substation.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2238 2024-02-13 14:28:28.603734 GridCalEngine-5.1.1/GridCalEngine/IO/matpower/matpower_storage_definitions.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7498 2023-11-16 09:36:26.530645 GridCalEngine-5.1.1/GridCalEngine/IO/matpower/matpower_gen_definitions.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.530645 GridCalEngine-5.1.1/GridCalEngine/IO/matpower/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8171 2024-03-14 19:48:07.688505 GridCalEngine-5.1.1/GridCalEngine/IO/matpower/matpower_bus_definitions.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    31013 2024-03-14 19:48:07.688505 GridCalEngine-5.1.1/GridCalEngine/IO/matpower/matpower_parser.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6661 2023-11-16 09:36:26.530645 GridCalEngine-5.1.1/GridCalEngine/IO/matpower/matpower_branch_definitions.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.530645 GridCalEngine-5.1.1/GridCalEngine/IO/gridcal/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    54211 2024-04-01 07:29:23.260927 GridCalEngine-5.1.1/GridCalEngine/IO/gridcal/pack_unpack.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    16119 2024-03-11 19:28:12.199075 GridCalEngine-5.1.1/GridCalEngine/IO/gridcal/zip_interface.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    98297 2024-03-28 10:16:48.984877 GridCalEngine-5.1.1/GridCalEngine/IO/gridcal/json_parser.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1966 2024-03-11 19:28:12.199075 GridCalEngine-5.1.1/GridCalEngine/IO/gridcal/generic_io_functions.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2432 2024-03-11 19:28:12.199075 GridCalEngine-5.1.1/GridCalEngine/IO/gridcal/h5_interface.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    47307 2024-03-14 19:48:07.688505 GridCalEngine-5.1.1/GridCalEngine/IO/gridcal/excel_interface.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2365 2024-02-13 14:28:28.599734 GridCalEngine-5.1.1/GridCalEngine/IO/gridcal/sqlite_interface.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2869 2024-03-11 19:28:12.199075 GridCalEngine-5.1.1/GridCalEngine/IO/gridcal/contingency_parser.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.530645 GridCalEngine-5.1.1/GridCalEngine/IO/epc/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    19972 2024-03-11 19:28:12.199075 GridCalEngine-5.1.1/GridCalEngine/IO/epc/epc_parser.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    38780 2024-03-28 10:16:48.984877 GridCalEngine-5.1.1/GridCalEngine/IO/others/dpx_parser.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.530645 GridCalEngine-5.1.1/GridCalEngine/IO/others/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4259 2024-03-14 19:48:07.688505 GridCalEngine-5.1.1/GridCalEngine/IO/others/ipa_parser.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    12272 2024-03-11 19:28:12.203075 GridCalEngine-5.1.1/GridCalEngine/IO/others/pypsa_parser.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    32570 2024-03-28 10:16:48.984877 GridCalEngine-5.1.1/GridCalEngine/IO/others/plx_parser.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.522645 GridCalEngine-5.1.1/GridCalEngine/IO/cim/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    36020 2024-03-11 19:28:12.183075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_enums.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    49322 2024-04-01 07:29:23.260927 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_to_gridcal.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3421 2024-03-11 19:28:12.183075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_poperty.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    15944 2024-03-28 10:16:48.980877 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_data_parser.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-11 19:28:12.183075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2229 2024-03-11 19:28:12.195075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_writer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    18971 2024-04-03 10:10:53.840547 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/gridcal_to_cgmes.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11194 2024-03-28 10:16:48.980877 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/base.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11951 2024-04-01 07:29:23.256927 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_export.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    26145 2024-04-01 07:29:23.260927 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_utils.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8815 2024-03-14 19:59:31.536490 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_data_validator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    81755 2024-04-01 07:29:23.256927 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_circuit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1167 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_switch.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2002 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_non_linear.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2803 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/connectivity_node.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1933 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_equipment_container.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3119 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/identified_object.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3492 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/control_area.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2649 2024-03-14 19:48:07.684505 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/location.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1169 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_chopper.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1201 2024-03-11 19:28:12.195075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/season_day_type_schedule.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1999 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/asynchronous_machine.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4399 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_injection.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1550 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_line.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1616 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/caes_plant.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1607 2024-03-11 19:28:12.195075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/solar_power_plant.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2454 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/curve.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1755 2024-03-11 19:28:12.195075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/regular_interval_schedule.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1121 2024-03-11 19:28:12.195075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/work_location.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1140 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/breaker.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1570 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_topological_island.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1581 2024-03-11 19:28:12.195075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ratio_tap_changer_table_point.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1164 2024-03-11 19:28:12.195075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/surge_arrester.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1912 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/battery_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1117 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/post_line_sensor.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4313 2024-03-11 19:28:12.195075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/shunt_compensator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2394 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/nonlinear_shunt_compensator_point.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2122 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_branch.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1750 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/active_power_limit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1097 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/fuse.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1656 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/nonlinear_shunt_compensator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1707 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_series_device.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3015 2024-03-11 19:28:12.195075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tap_changer_table_point.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1499 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_system_resource.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1147 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/disconnecting_circuit_breaker.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1693 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_shunt.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5175 2024-03-11 19:28:12.195075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/vs_converter.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3482 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/external_network_injection.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3263 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_electronics_connection.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1125 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/current_transformer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2025 2024-03-11 19:28:12.195075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_voltage.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2431 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_node.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1174 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_connection.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1960 2024-03-11 19:28:12.195075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_tap_step.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2689 2024-03-11 19:28:12.195075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/voltage_level.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3356 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_consumer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1838 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/current_limit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1166 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/fault_indicator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2263 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ratio_tap_changer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1187 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/grounding_impedance.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1677 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_ground.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7023 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/acdc_converter.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1113 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/disconnector.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3305 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_transformer_end.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1167 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_busbar.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1977 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/operational_limit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1164 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/nuclear_generating_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1540 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_scheduling_type.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1546 2024-03-11 19:28:12.195075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tap_changer_control.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1569 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_transformer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1500 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/auxiliary_equipment.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2312 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/curve_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1175 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/petersen_coil.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1154 2024-03-11 19:28:12.195075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/wave_trap.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2033 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_table.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2730 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ac_line_segment.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1821 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_table_point.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1217 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_symmetrical.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1521 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3095 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/base_voltage.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3217 2024-03-11 19:28:12.195075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/transformer_end.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1636 2024-03-11 19:28:12.195075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/voltage_limit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1597 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_network.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1101 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/jumper.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3204 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/acdc_terminal.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1567 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_terminal.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1116 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_breaker.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3413 2024-03-11 19:28:12.195075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/switch.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3854 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equipment.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5068 2024-03-11 19:28:12.195075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/topological_node.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2815 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/operational_limit_type.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1931 2024-03-11 19:28:12.195075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/reporting_group.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1735 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/linear_shunt_compensator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3458 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_source.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2228 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_line_segment.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1414 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conductor.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2748 2024-03-11 19:28:12.195075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/thermal_generating_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1117 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/junction.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1574 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_equipment.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2567 2024-03-11 19:28:12.195075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sub_geographical_region.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1617 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/cogeneration_plant.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2186 2024-03-11 19:28:12.195075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_injection.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5616 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/boundary_point.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5089 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_response_characteristic.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1896 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_converter_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1499 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/bay.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1821 2024-03-11 19:28:12.195075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/wind_generating_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1799 2024-03-11 19:28:12.195075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sub_load_area.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2175 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_electronics_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2422 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/hydro_generating_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2421 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conducting_equipment.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1571 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/geographical_region.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1517 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/non_conform_load.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3492 2024-03-11 19:28:12.195075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/synchronous_machine.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1528 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/line.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1504 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_group.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1696 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_shunt.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2807 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_topological_node.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1469 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_area.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2004 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/control_area_generating_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1523 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equipment_container.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2110 2024-03-11 19:28:12.195075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/topological_island.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1129 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/potential_transformer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1955 2024-03-11 19:28:12.195075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_shunt_compensator_sections.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1593 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_tabular.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1150 2024-03-11 19:28:12.195075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sensor.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4996 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/cs_converter.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1501 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conform_load_group.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1597 2024-03-11 19:28:12.195075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/wind_power_plant.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3510 2024-03-11 19:28:12.195075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/rotating_machine.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1195 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_electronics_wind_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1527 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_area.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1986 2024-03-11 19:28:12.195075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/reactive_capability_curve.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2080 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/hydro_pump.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1119 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/protected_switch.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1941 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_linear.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2133 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/acdc_converterdc_terminal.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4941 2024-03-11 19:28:12.195075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tap_changer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1765 2024-03-11 19:28:12.195075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_switch.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1520 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/non_conform_load_group.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2093 2024-03-11 19:28:12.195075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_status.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1156 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_break_switch.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2253 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/bus_name_marker.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1548 2024-03-11 19:28:12.195075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/solar_generating_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1860 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/fossil_fuel.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1184 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/earth_fault_compensator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2249 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/operational_limit_set.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2307 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/hydro_power_plant.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6776 2024-03-14 19:48:07.684505 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/generating_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1144 2024-03-11 19:28:12.195075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/service_location.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5780 2024-03-11 19:28:12.195075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/terminal.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1489 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_asymmetrical.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1621 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/combined_cycle_plant.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1127 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/busbar_section.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1126 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_disconnector.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1160 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/connector.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2404 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/coordinate_system.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1901 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_base_terminal.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2752 2024-03-11 19:28:12.195075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/static_var_compensator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1712 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/apparent_power_limit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1498 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conform_load.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1652 2024-03-11 19:28:12.195075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/series_compensator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2010 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/connectivity_node_container.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2299 2024-03-11 19:28:12.195075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/substation.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2448 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/position_point.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1805 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/clamp.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2302 2024-03-11 19:28:12.195075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tie_flow.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1996 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/basic_interval_schedule.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1744 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/cut.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1125 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ground_disconnector.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1971 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ratio_tap_changer_table.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1740 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_conducting_equipment.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1486 2024-03-11 19:28:12.195075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/vs_capability_curve.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1179 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/photo_voltaic_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1154 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ground.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5088 2024-03-11 19:28:12.195075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/regulating_control.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2095 2024-03-11 19:28:12.195075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_power_flow.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-11 19:28:12.183075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1168 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_switch.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2003 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_non_linear.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2432 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/connectivity_node.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1820 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_equipment_container.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3521 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/identified_object.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3496 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/control_area.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2403 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/location.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1170 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_chopper.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1202 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/season_day_type_schedule.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4118 2024-03-11 19:28:12.183075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/asynchronous_machine.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5617 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_injection.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1507 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_line.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2447 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/curve.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1702 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/regular_interval_schedule.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1141 2024-03-11 19:28:12.183075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/breaker.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1524 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_topological_island.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1583 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ratio_tap_changer_table_point.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3985 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/shunt_compensator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2908 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/nonlinear_shunt_compensator_point.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5115 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_branch.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1457 2024-03-11 19:28:12.183075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/active_power_limit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1658 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/nonlinear_shunt_compensator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1943 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_series_device.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2768 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tap_changer_table_point.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2209 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/power_system_resource.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1694 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_shunt.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4544 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/vs_converter.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6505 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/external_network_injection.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2026 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_voltage.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2246 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_node.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2012 2024-04-01 07:29:23.260927 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1800 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_tap_step.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2693 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/voltage_level.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3370 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_consumer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1497 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/current_limit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2617 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ratio_tap_changer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1444 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/grounding_impedance.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1678 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_ground.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6262 2024-03-11 19:28:12.183075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/acdc_converter.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1114 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/disconnector.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4973 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/power_transformer_end.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1168 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_busbar.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1960 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/operational_limit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1165 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/nuclear_generating_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1531 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_scheduling_type.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1544 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tap_changer_control.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3596 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/power_transformer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2285 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/curve_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3199 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/petersen_coil.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2036 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_table.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3385 2024-03-11 19:28:12.183075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ac_line_segment.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1822 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_table_point.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1218 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_symmetrical.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1522 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3094 2024-03-11 19:28:12.183075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/base_voltage.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3989 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/transformer_end.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1396 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/voltage_limit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1611 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_network.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1768 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/measurement_value.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3786 2024-03-11 19:28:12.183075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/acdc_terminal.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1521 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_terminal.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1117 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_breaker.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2509 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/switch.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2591 2024-03-14 19:48:07.684505 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equipment.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5742 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/quality61850.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5081 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/topological_node.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2424 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/operational_limit_type.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1936 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/reporting_group.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2289 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/linear_shunt_compensator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4321 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_source.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2638 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_line_segment.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1475 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/limit_set.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1393 2024-03-11 19:28:12.183075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conductor.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1533 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/thermal_generating_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4216 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/full_model.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1118 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/junction.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1564 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_equipment.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2534 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sub_geographical_region.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2189 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_injection.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5141 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_response_characteristic.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1776 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_converter_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1501 2024-03-11 19:28:12.183075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/bay.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1441 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/wind_generating_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1141 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/limit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1802 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sub_load_area.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1901 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/hydro_generating_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2431 2024-03-11 19:28:12.183075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conducting_equipment.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1573 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/geographical_region.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1541 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/non_conform_load.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7957 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/synchronous_machine.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1530 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/line.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1506 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_group.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1932 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_shunt.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2608 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_topological_node.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1471 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_area.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2007 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/control_area_generating_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1525 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equipment_container.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2317 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/per_lengthdc_line_parameter.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3599 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/measurement.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2113 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/topological_island.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1852 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_shunt_compensator_sections.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1595 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_tabular.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4958 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/cs_converter.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1503 2024-03-11 19:28:12.183075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conform_load_group.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3430 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/rotating_machine.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1529 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_area.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2013 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/reactive_capability_curve.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2083 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/hydro_pump.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1120 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/protected_switch.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1942 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_linear.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1796 2024-03-11 19:28:12.183075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/acdc_converterdc_terminal.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4341 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tap_changer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1500 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/non_conform_load_group.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1860 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_status.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1157 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_break_switch.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2254 2024-03-11 19:28:12.183075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/bus_name_marker.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1161 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/solar_generating_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1862 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/fossil_fuel.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1417 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/earth_fault_compensator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2226 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/operational_limit_set.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2310 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/hydro_power_plant.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6586 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/generating_unit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6326 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/terminal.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1490 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_asymmetrical.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1470 2024-03-11 19:28:12.183075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/busbar_section.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1127 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_disconnector.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1161 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/connector.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2404 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/coordinate_system.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1823 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_base_terminal.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2744 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/static_var_compensator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1440 2024-03-11 19:28:12.183075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/apparent_power_limit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1500 2024-03-11 19:28:12.183075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conform_load.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3068 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/series_compensator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2013 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/connectivity_node_container.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2257 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/substation.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2449 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/position_point.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2444 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tie_flow.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1943 2024-03-11 19:28:12.183075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/basic_interval_schedule.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4063 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/mutual_coupling.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1126 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ground_disconnector.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1975 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ratio_tap_changer_table.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1894 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/regulating_cond_eq.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1456 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_conducting_equipment.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1650 2024-03-11 19:28:12.183075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/analog_control.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1481 2024-03-11 19:28:12.191075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/vs_capability_curve.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3195 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/control.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1155 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ground.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3782 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/regulating_control.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2096 2024-03-11 19:28:12.187075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_power_flow.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    18126 2024-02-13 14:28:28.599734 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cim16/cim_circuit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)   192495 2024-02-13 14:28:28.599734 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cim16/cim_devices.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.526645 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cim16/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    14224 2024-02-13 14:28:28.599734 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cim16/cim_enums.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    45731 2024-03-11 19:28:12.199075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cim16/cim_parser.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8909 2023-11-16 09:36:26.526645 GridCalEngine-5.1.1/GridCalEngine/IO/cim/cim16/cim_data_parser.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.526645 GridCalEngine-5.1.1/GridCalEngine/IO/cim/db/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2734 2023-11-16 09:36:26.526645 GridCalEngine-5.1.1/GridCalEngine/IO/cim/db/base_db.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1705 2024-03-11 19:28:12.199075 GridCalEngine-5.1.1/GridCalEngine/IO/cim/db/cgmes_lookup_db.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      697 2023-11-16 09:36:26.526645 GridCalEngine-5.1.1/GridCalEngine/IO/cim/db/file_system.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5267 2023-11-16 09:36:26.526645 GridCalEngine-5.1.1/GridCalEngine/IO/cim/db/psse_lookup_db.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      527 2023-11-16 09:36:26.526645 GridCalEngine-5.1.1/GridCalEngine/IO/cim/db/db_handler.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2325 2024-04-03 10:10:53.840547 GridCalEngine-5.1.1/GridCalEngine/Devices/types.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7311 2024-03-14 19:48:07.684505 GridCalEngine-5.1.1/GridCalEngine/Devices/sparse_array.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1463 2024-03-28 10:16:48.980877 GridCalEngine-5.1.1/GridCalEngine/Devices/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)   191901 2024-03-28 10:16:48.980877 GridCalEngine-5.1.1/GridCalEngine/Devices/multi_circuit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5773 2024-03-11 19:28:12.183075 GridCalEngine-5.1.1/GridCalEngine/Devices/measurement.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    14002 2024-03-28 10:16:48.980877 GridCalEngine-5.1.1/GridCalEngine/Devices/profile.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2048 2024-03-14 19:59:31.532490 GridCalEngine-5.1.1/GridCalEngine/Devices/Aggregation/municipality.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1687 2024-03-11 19:28:12.179075 GridCalEngine-5.1.1/GridCalEngine/Devices/Aggregation/contingency_group.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1728 2024-03-14 19:59:31.532490 GridCalEngine-5.1.1/GridCalEngine/Devices/Aggregation/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3005 2024-03-11 19:28:12.179075 GridCalEngine-5.1.1/GridCalEngine/Devices/Aggregation/fuel.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4255 2024-03-11 19:28:12.179075 GridCalEngine-5.1.1/GridCalEngine/Devices/Aggregation/contingency.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3028 2024-03-11 19:28:12.179075 GridCalEngine-5.1.1/GridCalEngine/Devices/Aggregation/emission_gas.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1647 2024-03-11 19:28:12.179075 GridCalEngine-5.1.1/GridCalEngine/Devices/Aggregation/country.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2020 2024-03-14 19:59:31.532490 GridCalEngine-5.1.1/GridCalEngine/Devices/Aggregation/region.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2558 2024-03-28 10:16:48.972877 GridCalEngine-5.1.1/GridCalEngine/Devices/Aggregation/area.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2547 2024-03-11 19:28:12.179075 GridCalEngine-5.1.1/GridCalEngine/Devices/Aggregation/technology.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2008 2024-03-14 19:59:31.532490 GridCalEngine-5.1.1/GridCalEngine/Devices/Aggregation/zone.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2174 2024-03-11 19:28:12.179075 GridCalEngine-5.1.1/GridCalEngine/Devices/Aggregation/investments_group.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3715 2024-03-11 19:28:12.179075 GridCalEngine-5.1.1/GridCalEngine/Devices/Aggregation/investment.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2045 2024-03-14 19:59:31.532490 GridCalEngine-5.1.1/GridCalEngine/Devices/Aggregation/community.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1463 2024-03-14 19:59:31.532490 GridCalEngine-5.1.1/GridCalEngine/Devices/Aggregation/branch_group.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1099 2024-03-11 19:28:12.179075 GridCalEngine-5.1.1/GridCalEngine/Devices/Fluid/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3692 2024-03-28 10:16:48.976877 GridCalEngine-5.1.1/GridCalEngine/Devices/Fluid/fluid_path.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2342 2024-03-11 19:28:12.179075 GridCalEngine-5.1.1/GridCalEngine/Devices/Fluid/fluid_pump.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6083 2024-03-11 19:28:12.179075 GridCalEngine-5.1.1/GridCalEngine/Devices/Fluid/fluid_node.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2352 2024-03-11 19:28:12.179075 GridCalEngine-5.1.1/GridCalEngine/Devices/Fluid/fluid_turbine.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3976 2024-03-11 19:28:12.179075 GridCalEngine-5.1.1/GridCalEngine/Devices/Fluid/fluid_injection_template.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2331 2024-03-11 19:28:12.179075 GridCalEngine-5.1.1/GridCalEngine/Devices/Fluid/fluid_p2x.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    10736 2024-03-28 10:16:48.976877 GridCalEngine-5.1.1/GridCalEngine/Devices/Branches/dc_line.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4278 2024-03-11 19:28:12.179075 GridCalEngine-5.1.1/GridCalEngine/Devices/Branches/underground_line_type.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2005 2024-03-28 10:16:48.972877 GridCalEngine-5.1.1/GridCalEngine/Devices/Branches/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    10226 2024-03-28 10:16:48.976877 GridCalEngine-5.1.1/GridCalEngine/Devices/Branches/series_reactance.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2485 2024-03-11 19:28:12.179075 GridCalEngine-5.1.1/GridCalEngine/Devices/Branches/wire.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5553 2024-03-28 10:16:48.976877 GridCalEngine-5.1.1/GridCalEngine/Devices/Branches/line_locations.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3652 2024-03-11 19:28:12.179075 GridCalEngine-5.1.1/GridCalEngine/Devices/Branches/sequence_line_type.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    18829 2024-03-14 19:48:07.684505 GridCalEngine-5.1.1/GridCalEngine/Devices/Branches/overhead_line_type.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7386 2024-03-14 19:59:31.532490 GridCalEngine-5.1.1/GridCalEngine/Devices/Branches/switch.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    12638 2024-03-28 10:16:48.976877 GridCalEngine-5.1.1/GridCalEngine/Devices/Branches/vsc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7628 2024-03-28 10:16:48.976877 GridCalEngine-5.1.1/GridCalEngine/Devices/Branches/upfc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    19502 2024-03-28 10:16:48.976877 GridCalEngine-5.1.1/GridCalEngine/Devices/Branches/transformer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    19989 2024-03-28 10:16:48.976877 GridCalEngine-5.1.1/GridCalEngine/Devices/Branches/hvdc_line.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    15863 2024-03-28 10:16:48.976877 GridCalEngine-5.1.1/GridCalEngine/Devices/Branches/line.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9400 2024-03-28 10:16:48.976877 GridCalEngine-5.1.1/GridCalEngine/Devices/Branches/tap_changer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9196 2024-03-28 10:16:48.976877 GridCalEngine-5.1.1/GridCalEngine/Devices/Branches/winding.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    21848 2024-03-28 10:16:48.976877 GridCalEngine-5.1.1/GridCalEngine/Devices/Branches/branch.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5636 2024-03-11 19:28:12.179075 GridCalEngine-5.1.1/GridCalEngine/Devices/Branches/transformer_type.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11653 2024-03-11 19:28:12.179075 GridCalEngine-5.1.1/GridCalEngine/Devices/Branches/transformer3w.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2136 2024-03-11 19:28:12.183075 GridCalEngine-5.1.1/GridCalEngine/Devices/Injections/static_generator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2325 2024-03-28 10:16:48.976877 GridCalEngine-5.1.1/GridCalEngine/Devices/Injections/shunt.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1419 2024-03-11 19:28:12.179075 GridCalEngine-5.1.1/GridCalEngine/Devices/Injections/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5913 2024-03-28 10:16:48.976877 GridCalEngine-5.1.1/GridCalEngine/Devices/Injections/external_grid.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5261 2024-03-28 10:16:48.976877 GridCalEngine-5.1.1/GridCalEngine/Devices/Injections/current_injection.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6930 2024-03-28 10:16:48.976877 GridCalEngine-5.1.1/GridCalEngine/Devices/Injections/battery.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    15372 2024-03-28 10:16:48.976877 GridCalEngine-5.1.1/GridCalEngine/Devices/Injections/generator.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7856 2024-03-28 10:16:48.976877 GridCalEngine-5.1.1/GridCalEngine/Devices/Injections/generator_q_curve.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6864 2024-03-28 10:16:48.976877 GridCalEngine-5.1.1/GridCalEngine/Devices/Injections/controllable_shunt.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6780 2024-03-28 10:16:48.976877 GridCalEngine-5.1.1/GridCalEngine/Devices/Injections/load.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2203 2024-04-01 07:29:23.256927 GridCalEngine-5.1.1/GridCalEngine/Devices/Diagrams/graphic_location.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3172 2024-03-11 19:28:12.179075 GridCalEngine-5.1.1/GridCalEngine/Devices/Diagrams/map_diagram.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1181 2024-03-11 19:28:12.179075 GridCalEngine-5.1.1/GridCalEngine/Devices/Diagrams/node_breaker_diagram.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1162 2024-03-11 19:28:12.179075 GridCalEngine-5.1.1/GridCalEngine/Devices/Diagrams/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1176 2024-03-11 19:28:12.179075 GridCalEngine-5.1.1/GridCalEngine/Devices/Diagrams/bus_branch_diagram.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1452 2024-03-11 19:28:12.179075 GridCalEngine-5.1.1/GridCalEngine/Devices/Diagrams/map_location.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    12261 2024-04-01 07:29:23.256927 GridCalEngine-5.1.1/GridCalEngine/Devices/Diagrams/base_diagram.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1982 2024-03-11 19:28:12.183075 GridCalEngine-5.1.1/GridCalEngine/Devices/Substation/connectivity_node.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1130 2024-03-14 19:48:07.684505 GridCalEngine-5.1.1/GridCalEngine/Devices/Substation/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2020 2024-03-14 19:48:07.684505 GridCalEngine-5.1.1/GridCalEngine/Devices/Substation/voltage_level.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    14124 2024-03-28 10:16:48.980877 GridCalEngine-5.1.1/GridCalEngine/Devices/Substation/bus.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2648 2024-03-14 19:48:07.684505 GridCalEngine-5.1.1/GridCalEngine/Devices/Substation/busbar.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7724 2024-03-28 10:16:48.980877 GridCalEngine-5.1.1/GridCalEngine/Devices/Substation/substation.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7316 2024-04-03 10:10:53.840547 GridCalEngine-5.1.1/GridCalEngine/Devices/Parents/injection_parent.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    24200 2024-03-28 10:16:48.980877 GridCalEngine-5.1.1/GridCalEngine/Devices/Parents/editable_device.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7700 2024-03-11 19:28:12.183075 GridCalEngine-5.1.1/GridCalEngine/Devices/Parents/generator_parent.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      790 2024-03-11 19:28:12.183075 GridCalEngine-5.1.1/GridCalEngine/Devices/Parents/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    16800 2024-03-28 10:16:48.980877 GridCalEngine-5.1.1/GridCalEngine/Devices/Parents/controllable_branch_parent.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7034 2024-03-11 19:28:12.183075 GridCalEngine-5.1.1/GridCalEngine/Devices/Parents/load_parent.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    17125 2024-03-28 10:16:48.980877 GridCalEngine-5.1.1/GridCalEngine/Devices/Parents/branch_parent.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8463 2024-03-11 19:28:12.183075 GridCalEngine-5.1.1/GridCalEngine/Devices/Parents/shunt_parent.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2829 2024-03-11 19:28:12.179075 GridCalEngine-5.1.1/GridCalEngine/Devices/Associations/generator_emission.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1038 2024-03-11 19:28:12.179075 GridCalEngine-5.1.1/GridCalEngine/Devices/Associations/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2898 2024-03-11 19:28:12.179075 GridCalEngine-5.1.1/GridCalEngine/Devices/Associations/generator_technology.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2741 2024-03-11 19:28:12.179075 GridCalEngine-5.1.1/GridCalEngine/Devices/Associations/generator_fuel.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6558 2024-03-11 19:28:12.175075 GridCalEngine-5.1.1/GridCalEngine/DataStructures/load_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4274 2024-03-14 19:48:07.680505 GridCalEngine-5.1.1/GridCalEngine/DataStructures/bus_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    14793 2024-04-01 07:29:23.256927 GridCalEngine-5.1.1/GridCalEngine/DataStructures/branch_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1588 2024-03-11 19:28:12.175075 GridCalEngine-5.1.1/GridCalEngine/DataStructures/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2088 2024-03-11 19:28:12.175075 GridCalEngine-5.1.1/GridCalEngine/DataStructures/fluid_turbine_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1158 2024-03-11 19:28:12.175075 GridCalEngine-5.1.1/GridCalEngine/DataStructures/fluid_p2x_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    67051 2024-04-03 10:10:53.840547 GridCalEngine-5.1.1/GridCalEngine/DataStructures/numerical_circuit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    10107 2024-03-11 19:28:12.175075 GridCalEngine-5.1.1/GridCalEngine/DataStructures/generator_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1162 2024-03-11 19:28:12.175075 GridCalEngine-5.1.1/GridCalEngine/DataStructures/fluid_pump_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3073 2024-03-11 19:28:12.175075 GridCalEngine-5.1.1/GridCalEngine/DataStructures/battery_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2038 2024-03-11 19:28:12.175075 GridCalEngine-5.1.1/GridCalEngine/DataStructures/fluid_path_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    10968 2024-03-14 19:59:31.532490 GridCalEngine-5.1.1/GridCalEngine/DataStructures/hvdc_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4320 2024-03-11 19:28:12.175075 GridCalEngine-5.1.1/GridCalEngine/DataStructures/shunt_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2224 2024-03-11 19:28:12.175075 GridCalEngine-5.1.1/GridCalEngine/DataStructures/fluid_node_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    70288 2024-03-11 19:28:12.175075 GridCalEngine-5.1.1/GridCalEngine/Compilers/circuit_to_newton_pa.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    27811 2024-03-11 19:28:12.175075 GridCalEngine-5.1.1/GridCalEngine/Compilers/circuit_to_bentayga.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      992 2024-03-11 19:28:12.175075 GridCalEngine-5.1.1/GridCalEngine/Compilers/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    43799 2024-03-28 10:16:48.972877 GridCalEngine-5.1.1/GridCalEngine/Compilers/circuit_to_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3328 2024-03-11 19:28:12.175075 GridCalEngine-5.1.1/GridCalEngine/Compilers/circuit_to_optimods.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    27652 2024-03-14 19:48:07.680505 GridCalEngine-5.1.1/GridCalEngine/Compilers/circuit_to_pgm.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11185 2024-03-14 19:48:07.692505 GridCalEngine-5.1.1/GridCalEngine/Simulations/results_template.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1767 2024-03-11 19:28:12.223075 GridCalEngine-5.1.1/GridCalEngine/Simulations/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    12454 2024-03-11 19:28:12.223075 GridCalEngine-5.1.1/GridCalEngine/Simulations/results_table.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2699 2024-03-11 19:28:12.223075 GridCalEngine-5.1.1/GridCalEngine/Simulations/driver_types.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7963 2024-03-14 19:59:31.536490 GridCalEngine-5.1.1/GridCalEngine/Simulations/driver_template.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      359 2024-01-05 08:44:35.545288 GridCalEngine-5.1.1/GridCalEngine/Simulations/InvestmentsEvaluation/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    17002 2024-03-11 19:28:12.211075 GridCalEngine-5.1.1/GridCalEngine/Simulations/InvestmentsEvaluation/investments_evaluation_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8665 2024-03-14 19:48:07.692505 GridCalEngine-5.1.1/GridCalEngine/Simulations/InvestmentsEvaluation/investments_evaluation_results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2248 2024-02-13 14:28:28.607734 GridCalEngine-5.1.1/GridCalEngine/Simulations/InvestmentsEvaluation/investments_evaluation_options.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3318 2024-03-11 19:28:12.211075 GridCalEngine-5.1.1/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/stop_crits.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    25202 2024-03-14 19:48:07.692505 GridCalEngine-5.1.1/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/MVRSM_mo_pareto.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-11 19:28:12.211075 GridCalEngine-5.1.1/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    24206 2024-03-11 19:28:12.211075 GridCalEngine-5.1.1/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/MVRSM_mo_scaled.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    17532 2024-03-11 19:28:12.211075 GridCalEngine-5.1.1/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/MVRSM_original.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1104 2024-03-11 19:28:12.219075 GridCalEngine-5.1.1/GridCalEngine/Simulations/Topology/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11454 2024-03-14 19:48:07.692505 GridCalEngine-5.1.1/GridCalEngine/Simulations/Topology/topology_reduction_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11519 2024-03-11 19:28:12.219075 GridCalEngine-5.1.1/GridCalEngine/Simulations/Topology/topology_processor_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4832 2024-03-11 19:28:12.219075 GridCalEngine-5.1.1/GridCalEngine/Simulations/Topology/node_groups_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6814 2024-03-11 19:28:12.219075 GridCalEngine-5.1.1/GridCalEngine/Simulations/Stochastic/reliability_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3804 2024-03-14 19:48:07.692505 GridCalEngine-5.1.1/GridCalEngine/Simulations/Stochastic/stochastic_power_flow_input.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1312 2024-02-13 14:28:28.611734 GridCalEngine-5.1.1/GridCalEngine/Simulations/Stochastic/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    19791 2024-03-11 19:28:12.219075 GridCalEngine-5.1.1/GridCalEngine/Simulations/Stochastic/stochastic_power_flow_results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3777 2024-03-11 19:28:12.219075 GridCalEngine-5.1.1/GridCalEngine/Simulations/Stochastic/reliability_iterable.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11634 2024-03-11 19:28:12.219075 GridCalEngine-5.1.1/GridCalEngine/Simulations/Stochastic/blackout_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8063 2024-03-11 19:28:12.219075 GridCalEngine-5.1.1/GridCalEngine/Simulations/Stochastic/stochastic_power_flow_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8210 2024-03-14 19:48:07.692505 GridCalEngine-5.1.1/GridCalEngine/Simulations/Stochastic/latin_hypercube_sampling.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    29913 2024-03-11 19:28:12.219075 GridCalEngine-5.1.1/GridCalEngine/Simulations/PowerFlow/power_flow_ts_results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    10299 2024-03-14 19:59:31.536490 GridCalEngine-5.1.1/GridCalEngine/Simulations/PowerFlow/power_flow_ts_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    33458 2024-03-14 19:48:07.692505 GridCalEngine-5.1.1/GridCalEngine/Simulations/PowerFlow/power_flow_results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9269 2024-03-11 19:28:12.219075 GridCalEngine-5.1.1/GridCalEngine/Simulations/PowerFlow/power_flow_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1474 2024-02-13 14:28:28.611734 GridCalEngine-5.1.1/GridCalEngine/Simulations/PowerFlow/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5534 2024-02-13 14:28:28.611734 GridCalEngine-5.1.1/GridCalEngine/Simulations/PowerFlow/power_flow_ts_input.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4163 2024-03-11 19:28:12.215075 GridCalEngine-5.1.1/GridCalEngine/Simulations/PowerFlow/grid_analysis.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5496 2024-02-20 09:29:33.592105 GridCalEngine-5.1.1/GridCalEngine/Simulations/PowerFlow/power_flow_options.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    31315 2024-03-14 19:48:07.692505 GridCalEngine-5.1.1/GridCalEngine/Simulations/PowerFlow/power_flow_worker.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8754 2024-03-28 10:16:48.988877 GridCalEngine-5.1.1/GridCalEngine/Simulations/PowerFlow/NumericalMethods/common_functions.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1999 2024-02-13 14:28:28.611734 GridCalEngine-5.1.1/GridCalEngine/Simulations/PowerFlow/NumericalMethods/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    32701 2024-02-13 14:28:28.611734 GridCalEngine-5.1.1/GridCalEngine/Simulations/PowerFlow/NumericalMethods/acdc_jacobian.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    18741 2024-03-11 19:28:12.215075 GridCalEngine-5.1.1/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_acdc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8459 2024-03-14 19:48:07.692505 GridCalEngine-5.1.1/GridCalEngine/Simulations/PowerFlow/NumericalMethods/iwamoto_newton_raphson.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9795 2024-02-20 09:29:33.592105 GridCalEngine-5.1.1/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    12948 2024-03-11 19:28:12.215075 GridCalEngine-5.1.1/GridCalEngine/Simulations/PowerFlow/NumericalMethods/levenberg_marquardt_acdc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    33790 2024-03-14 19:48:07.692505 GridCalEngine-5.1.1/GridCalEngine/Simulations/PowerFlow/NumericalMethods/derivatives.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8882 2024-02-20 09:29:33.592105 GridCalEngine-5.1.1/GridCalEngine/Simulations/PowerFlow/NumericalMethods/levenberg_marquardt.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4066 2023-11-16 09:36:26.538645 GridCalEngine-5.1.1/GridCalEngine/Simulations/PowerFlow/NumericalMethods/fast_decoupled.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    25376 2024-03-14 19:48:07.692505 GridCalEngine-5.1.1/GridCalEngine/Simulations/PowerFlow/NumericalMethods/helm_power_flow.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6550 2024-03-14 19:48:07.692505 GridCalEngine-5.1.1/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_decoupled.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4027 2024-02-13 14:28:28.611734 GridCalEngine-5.1.1/GridCalEngine/Simulations/PowerFlow/NumericalMethods/gauss_power_flow.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7630 2024-03-14 19:48:07.692505 GridCalEngine-5.1.1/GridCalEngine/Simulations/PowerFlow/NumericalMethods/linearized_power_flow.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5676 2024-03-14 19:48:07.692505 GridCalEngine-5.1.1/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_ode.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    17875 2023-11-16 09:36:26.538645 GridCalEngine-5.1.1/GridCalEngine/Simulations/PowerFlow/NumericalMethods/ac_jacobian.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    26346 2024-01-05 08:44:35.549288 GridCalEngine-5.1.1/GridCalEngine/Simulations/PowerFlow/NumericalMethods/discrete_controls.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5855 2024-02-13 14:28:28.611734 GridCalEngine-5.1.1/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_current.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      121 2023-11-16 09:36:26.534645 GridCalEngine-5.1.1/GridCalEngine/Simulations/InputsAnalysis/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    20717 2024-03-28 10:16:48.984877 GridCalEngine-5.1.1/GridCalEngine/Simulations/InputsAnalysis/inputs_analysis_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.534645 GridCalEngine-5.1.1/GridCalEngine/Simulations/Dynamics/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3926 2024-03-11 19:28:12.207075 GridCalEngine-5.1.1/GridCalEngine/Simulations/Dynamics/transient_stability_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    48769 2024-03-14 19:48:07.692505 GridCalEngine-5.1.1/GridCalEngine/Simulations/Dynamics/dynamic_modules.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1401 2024-02-13 14:28:28.607734 GridCalEngine-5.1.1/GridCalEngine/Simulations/ContinuationPowerFlow/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7391 2024-03-14 19:48:07.692505 GridCalEngine-5.1.1/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1394 2024-02-13 14:28:28.607734 GridCalEngine-5.1.1/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_input.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    29581 2024-03-14 19:48:07.692505 GridCalEngine-5.1.1/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2390 2024-02-13 14:28:28.607734 GridCalEngine-5.1.1/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_options.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    18392 2024-03-11 19:28:12.207075 GridCalEngine-5.1.1/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4371 2024-02-13 14:28:28.611734 GridCalEngine-5.1.1/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    13984 2024-03-14 19:48:07.692505 GridCalEngine-5.1.1/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1138 2024-02-13 14:28:28.611734 GridCalEngine-5.1.1/GridCalEngine/Simulations/ShortCircuitStudies/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    28931 2024-03-11 19:28:12.219075 GridCalEngine-5.1.1/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit_results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    16615 2024-04-01 07:29:23.260927 GridCalEngine-5.1.1/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit_worker.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      463 2023-11-16 09:36:26.534645 GridCalEngine-5.1.1/GridCalEngine/Simulations/NTC/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    46689 2024-03-28 10:16:48.984877 GridCalEngine-5.1.1/GridCalEngine/Simulations/NTC/ntc_results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    31737 2024-03-28 10:16:48.984877 GridCalEngine-5.1.1/GridCalEngine/Simulations/NTC/ntc_ts_results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7649 2024-03-28 10:16:48.984877 GridCalEngine-5.1.1/GridCalEngine/Simulations/NTC/ntc_ts_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    51043 2024-03-28 10:16:48.984877 GridCalEngine-5.1.1/GridCalEngine/Simulations/NTC/ntc_opf.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8071 2024-03-28 10:16:48.984877 GridCalEngine-5.1.1/GridCalEngine/Simulations/NTC/ntc_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3467 2024-03-28 10:16:48.984877 GridCalEngine-5.1.1/GridCalEngine/Simulations/NTC/ntc_options.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9925 2024-03-14 19:48:07.692505 GridCalEngine-5.1.1/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_ts_results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7552 2024-03-14 19:48:07.692505 GridCalEngine-5.1.1/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1376 2024-02-13 14:28:28.603734 GridCalEngine-5.1.1/GridCalEngine/Simulations/ContingencyAnalysis/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7522 2024-03-14 19:59:31.536490 GridCalEngine-5.1.1/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3522 2024-03-11 19:28:12.207075 GridCalEngine-5.1.1/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_options.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    29395 2024-03-28 10:16:48.984877 GridCalEngine-5.1.1/GridCalEngine/Simulations/ContingencyAnalysis/contingencies_report.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8858 2024-03-14 19:59:31.536490 GridCalEngine-5.1.1/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_ts_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9287 2024-03-14 19:48:07.692505 GridCalEngine-5.1.1/GridCalEngine/Simulations/ContingencyAnalysis/contingency_plan.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-02-13 14:28:28.603734 GridCalEngine-5.1.1/GridCalEngine/Simulations/ContingencyAnalysis/Methods/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8443 2024-03-14 19:59:31.536490 GridCalEngine-5.1.1/GridCalEngine/Simulations/ContingencyAnalysis/Methods/srap.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8773 2024-03-14 19:59:31.536490 GridCalEngine-5.1.1/GridCalEngine/Simulations/ContingencyAnalysis/Methods/optimal_linear_contingency_analysis.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7252 2024-03-14 19:59:31.536490 GridCalEngine-5.1.1/GridCalEngine/Simulations/ContingencyAnalysis/Methods/linear_contingency_analysis.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7518 2024-03-14 19:59:31.536490 GridCalEngine-5.1.1/GridCalEngine/Simulations/ContingencyAnalysis/Methods/nonlinear_contingency_analysis.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5880 2024-03-14 19:59:31.536490 GridCalEngine-5.1.1/GridCalEngine/Simulations/ContingencyAnalysis/Methods/helm_contingency_analysis.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11049 2024-03-11 19:28:12.207075 GridCalEngine-5.1.1/GridCalEngine/Simulations/ContingencyAnalysis/Methods/helm_contingencies.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5386 2024-03-14 19:48:07.692505 GridCalEngine-5.1.1/GridCalEngine/Simulations/Clustering/clustering.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1054 2024-02-13 14:28:28.603734 GridCalEngine-5.1.1/GridCalEngine/Simulations/Clustering/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3158 2024-03-11 19:28:12.207075 GridCalEngine-5.1.1/GridCalEngine/Simulations/Clustering/clustering_results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      984 2024-02-13 14:28:28.603734 GridCalEngine-5.1.1/GridCalEngine/Simulations/Clustering/clustering_options.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2710 2024-03-11 19:28:12.207075 GridCalEngine-5.1.1/GridCalEngine/Simulations/Clustering/clustering_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9311 2024-03-11 19:28:12.219075 GridCalEngine-5.1.1/GridCalEngine/Simulations/StateEstimation/state_stimation_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      215 2023-11-16 09:36:26.538645 GridCalEngine-5.1.1/GridCalEngine/Simulations/StateEstimation/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    12628 2023-11-16 09:36:26.538645 GridCalEngine-5.1.1/GridCalEngine/Simulations/StateEstimation/state_estimation.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    14766 2024-03-28 10:16:48.988877 GridCalEngine-5.1.1/GridCalEngine/Simulations/OPF/opf_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1382 2024-02-13 14:28:28.611734 GridCalEngine-5.1.1/GridCalEngine/Simulations/OPF/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    26711 2024-03-28 10:16:48.988877 GridCalEngine-5.1.1/GridCalEngine/Simulations/OPF/opf_ts_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    33619 2024-03-11 19:28:12.215075 GridCalEngine-5.1.1/GridCalEngine/Simulations/OPF/opf_ts_results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    27247 2024-03-14 19:59:31.536490 GridCalEngine-5.1.1/GridCalEngine/Simulations/OPF/opf_results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4263 2024-03-11 19:28:12.215075 GridCalEngine-5.1.1/GridCalEngine/Simulations/OPF/simple_dispatch_ts.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    78103 2024-03-14 19:59:31.536490 GridCalEngine-5.1.1/GridCalEngine/Simulations/OPF/linear_opf_ts.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4148 2024-03-11 19:28:12.215075 GridCalEngine-5.1.1/GridCalEngine/Simulations/OPF/opf_options.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-02-13 14:28:28.607734 GridCalEngine-5.1.1/GridCalEngine/Simulations/OPF/NumericalMethods/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    44316 2024-03-28 10:16:48.984877 GridCalEngine-5.1.1/GridCalEngine/Simulations/OPF/NumericalMethods/ac_opf.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    15593 2024-02-13 14:28:28.607734 GridCalEngine-5.1.1/GridCalEngine/Simulations/OPF/NumericalMethods/ac_opf_autodif.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    54149 2024-03-28 10:16:48.988877 GridCalEngine-5.1.1/GridCalEngine/Simulations/OPF/NumericalMethods/ac_opf_derivatives.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    12868 2024-03-14 19:48:07.688505 GridCalEngine-5.1.1/GridCalEngine/Simulations/ATC/available_transfer_capacity_ts_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1054 2024-02-13 14:28:28.603734 GridCalEngine-5.1.1/GridCalEngine/Simulations/ATC/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    24852 2024-03-14 19:48:07.688505 GridCalEngine-5.1.1/GridCalEngine/Simulations/ATC/available_transfer_capacity_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      116 2023-11-16 09:36:26.538645 GridCalEngine-5.1.1/GridCalEngine/Simulations/SigmaAnalysis/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    18826 2024-03-11 19:28:12.219075 GridCalEngine-5.1.1/GridCalEngine/Simulations/SigmaAnalysis/sigma_analysis_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1207 2024-02-13 14:28:28.607734 GridCalEngine-5.1.1/GridCalEngine/Simulations/LinearFactors/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6692 2024-03-11 19:28:12.211075 GridCalEngine-5.1.1/GridCalEngine/Simulations/LinearFactors/linear_analysis_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    29516 2024-03-14 19:59:31.536490 GridCalEngine-5.1.1/GridCalEngine/Simulations/LinearFactors/linear_analysis.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6138 2024-03-11 19:28:12.211075 GridCalEngine-5.1.1/GridCalEngine/Simulations/LinearFactors/linear_analysis_ts_results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6497 2024-03-11 19:28:12.211075 GridCalEngine-5.1.1/GridCalEngine/Simulations/LinearFactors/linear_analysis_results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1603 2024-02-13 14:28:28.607734 GridCalEngine-5.1.1/GridCalEngine/Simulations/LinearFactors/linear_analysis_options.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4727 2024-03-11 19:28:12.211075 GridCalEngine-5.1.1/GridCalEngine/Simulations/LinearFactors/linear_analysis_ts_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3501 2024-03-17 12:13:24.384980 GridCalEngine-5.1.1/setup.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1049 2024-04-03 10:11:16.048547 GridCalEngine-5.1.1/PKG-INFO
--rw-rw-r--   0 santi     (1000) santi     (1000)       37 2024-04-03 10:11:16.048547 GridCalEngine-5.1.1/setup.cfg
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2270 2024-04-08 13:34:15.975164 GridCalEngine-5.1.2/GridCalEngine/__version__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      790 2024-02-13 14:28:28.615734 GridCalEngine-5.1.2/GridCalEngine/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11585 2024-03-11 19:28:12.203075 GridCalEngine-5.1.2/GridCalEngine/LICENSE.txt
+-rw-rw-r--   0 santi     (1000) santi     (1000)    10942 2024-03-14 19:48:07.696505 GridCalEngine-5.1.2/GridCalEngine/data_logger.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    38634 2024-04-08 13:34:15.975164 GridCalEngine-5.1.2/GridCalEngine/enumerations.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    23610 2024-03-14 19:48:07.696505 GridCalEngine-5.1.2/GridCalEngine/basic_structures.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3068 2024-04-08 13:34:15.975164 GridCalEngine-5.1.2/GridCalEngine/api.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.538645 GridCalEngine-5.1.2/GridCalEngine/Utils/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4960 2024-03-28 10:16:48.988877 GridCalEngine-5.1.2/GridCalEngine/Utils/Filtering/objects_filtering.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1037 2024-03-11 19:28:12.223075 GridCalEngine-5.1.2/GridCalEngine/Utils/Filtering/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5922 2024-03-11 19:28:12.223075 GridCalEngine-5.1.2/GridCalEngine/Utils/Filtering/timeseries_filtering.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9710 2024-03-28 10:16:48.988877 GridCalEngine-5.1.2/GridCalEngine/Utils/Filtering/filtering.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    10146 2024-03-14 19:48:07.696505 GridCalEngine-5.1.2/GridCalEngine/Utils/Filtering/results_table_filtering.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3555 2024-02-20 09:29:33.592105 GridCalEngine-5.1.2/GridCalEngine/Utils/NumericalMethods/common.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-02-13 14:28:28.615734 GridCalEngine-5.1.2/GridCalEngine/Utils/NumericalMethods/iwamoto.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6314 2024-02-20 09:29:33.592105 GridCalEngine-5.1.2/GridCalEngine/Utils/NumericalMethods/levenberg_marquadt.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    15007 2024-03-17 11:12:27.697061 GridCalEngine-5.1.2/GridCalEngine/Utils/NumericalMethods/ips.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-02-13 14:28:28.615734 GridCalEngine-5.1.2/GridCalEngine/Utils/NumericalMethods/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6918 2024-03-11 19:28:12.223075 GridCalEngine-5.1.2/GridCalEngine/Utils/NumericalMethods/newton_raphson.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3618 2024-03-11 19:28:12.223075 GridCalEngine-5.1.2/GridCalEngine/Utils/NumericalMethods/weldorf_online_stddev.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7272 2024-02-20 09:29:33.592105 GridCalEngine-5.1.2/GridCalEngine/Utils/NumericalMethods/powell.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-02-13 14:28:28.615734 GridCalEngine-5.1.2/GridCalEngine/Utils/NumericalMethods/newton_raphson_ode.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6454 2024-02-13 14:28:28.615734 GridCalEngine-5.1.2/GridCalEngine/Utils/NumericalMethods/autodiff.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5184 2024-03-11 19:28:12.223075 GridCalEngine-5.1.2/GridCalEngine/Utils/NumericalMethods/sparse_solve.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      898 2024-02-13 14:28:28.615734 GridCalEngine-5.1.2/GridCalEngine/Utils/Sparse/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    35003 2024-03-11 19:28:12.223075 GridCalEngine-5.1.2/GridCalEngine/Utils/Sparse/csc_numba.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    20288 2024-02-20 09:29:33.592105 GridCalEngine-5.1.2/GridCalEngine/Utils/Sparse/csc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2602 2024-02-13 14:28:28.615734 GridCalEngine-5.1.2/GridCalEngine/Utils/Sparse/utils.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.538645 GridCalEngine-5.1.2/GridCalEngine/Utils/ThirdParty/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.538645 GridCalEngine-5.1.2/GridCalEngine/Utils/ThirdParty/SyntheticNetworks/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    16616 2024-03-14 19:48:07.696505 GridCalEngine-5.1.2/GridCalEngine/Utils/ThirdParty/SyntheticNetworks/rpgm_algo.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3271 2024-02-13 14:28:28.615734 GridCalEngine-5.1.2/GridCalEngine/Utils/MIP/selected_interface.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.538645 GridCalEngine-5.1.2/GridCalEngine/Utils/MIP/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11191 2024-04-03 10:10:53.840547 GridCalEngine-5.1.2/GridCalEngine/Utils/MIP/ortools_interface.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8598 2024-02-13 14:28:28.615734 GridCalEngine-5.1.2/GridCalEngine/Utils/MIP/pulp_interface.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      971 2024-02-13 14:28:28.615734 GridCalEngine-5.1.2/GridCalEngine/Utils/MIP/SimpleMip/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    12785 2024-02-13 14:28:28.615734 GridCalEngine-5.1.2/GridCalEngine/Utils/MIP/SimpleMip/lpobjects.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    23363 2024-02-13 14:28:28.615734 GridCalEngine-5.1.2/GridCalEngine/Utils/MIP/SimpleMip/lpmodel.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3095 2024-02-13 14:28:28.615734 GridCalEngine-5.1.2/GridCalEngine/Utils/MIP/SimpleMip/highs.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    12143 2024-03-11 19:28:12.223075 GridCalEngine-5.1.2/GridCalEngine/Topology/topology.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-11 19:28:12.223075 GridCalEngine-5.1.2/GridCalEngine/Topology/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    21011 2024-03-14 19:59:31.536490 GridCalEngine-5.1.2/GridCalEngine/Topology/simulation_indices.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9597 2024-03-14 19:48:07.692505 GridCalEngine-5.1.2/GridCalEngine/Topology/topology_substation_reduction.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    27056 2024-04-01 07:29:23.260927 GridCalEngine-5.1.2/GridCalEngine/Topology/admittance_matrices.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      644 2023-11-16 09:36:26.522645 GridCalEngine-5.1.2/GridCalEngine/IO/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    20668 2024-04-08 13:34:15.975164 GridCalEngine-5.1.2/GridCalEngine/IO/file_handler.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      361 2023-11-16 09:36:26.530645 GridCalEngine-5.1.2/GridCalEngine/IO/file_system.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.522645 GridCalEngine-5.1.2/GridCalEngine/IO/base/base_device.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.522645 GridCalEngine-5.1.2/GridCalEngine/IO/base/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4486 2023-11-16 09:36:26.522645 GridCalEngine-5.1.2/GridCalEngine/IO/base/units.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      200 2023-11-16 09:36:26.522645 GridCalEngine-5.1.2/GridCalEngine/IO/base/base_circuit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2588 2024-03-14 19:48:07.684505 GridCalEngine-5.1.2/GridCalEngine/IO/base/base_property.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.530645 GridCalEngine-5.1.2/GridCalEngine/IO/dgs/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    41779 2024-03-14 19:48:07.688505 GridCalEngine-5.1.2/GridCalEngine/IO/dgs/dgs_parser.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    87374 2024-03-14 19:48:07.688505 GridCalEngine-5.1.2/GridCalEngine/IO/raw/raw_parser_legacy.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.530645 GridCalEngine-5.1.2/GridCalEngine/IO/raw/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2636 2024-03-14 19:48:07.688505 GridCalEngine-5.1.2/GridCalEngine/IO/raw/raw_functions.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4036 2024-03-11 19:28:12.203075 GridCalEngine-5.1.2/GridCalEngine/IO/raw/rawx_parser_writer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    18318 2024-02-13 14:28:28.603734 GridCalEngine-5.1.2/GridCalEngine/IO/raw/raw_parser_writer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      245 2024-03-11 19:28:12.203075 GridCalEngine-5.1.2/GridCalEngine/IO/raw/gridcal_to_raw.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    31801 2024-03-14 19:48:07.688505 GridCalEngine-5.1.2/GridCalEngine/IO/raw/raw_to_gridcal.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    48436 2024-03-14 19:48:07.688505 GridCalEngine-5.1.2/GridCalEngine/IO/raw/rawx_parser_legacy.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1892 2024-03-14 19:48:07.688505 GridCalEngine-5.1.2/GridCalEngine/IO/raw/devices/gne_device.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9804 2024-02-13 14:28:28.603734 GridCalEngine-5.1.2/GridCalEngine/IO/raw/devices/switched_shunt.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1288 2023-11-16 09:36:26.530645 GridCalEngine-5.1.2/GridCalEngine/IO/raw/devices/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5779 2024-02-13 14:28:28.603734 GridCalEngine-5.1.2/GridCalEngine/IO/raw/devices/system_switching_device.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5949 2024-02-13 14:28:28.603734 GridCalEngine-5.1.2/GridCalEngine/IO/raw/devices/psse_object.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    54576 2024-02-13 14:28:28.603734 GridCalEngine-5.1.2/GridCalEngine/IO/raw/devices/transformer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    12199 2024-02-13 14:28:28.603734 GridCalEngine-5.1.2/GridCalEngine/IO/raw/devices/facts.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2338 2024-02-13 14:28:28.603734 GridCalEngine-5.1.2/GridCalEngine/IO/raw/devices/owner.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3520 2024-02-13 14:28:28.603734 GridCalEngine-5.1.2/GridCalEngine/IO/raw/devices/inter_area.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1811 2024-02-13 14:28:28.603734 GridCalEngine-5.1.2/GridCalEngine/IO/raw/devices/psse_property.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    13081 2024-03-11 19:28:12.203075 GridCalEngine-5.1.2/GridCalEngine/IO/raw/devices/generator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    23805 2024-02-13 14:28:28.603734 GridCalEngine-5.1.2/GridCalEngine/IO/raw/devices/two_terminal_dc_line.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7667 2024-02-13 14:28:28.603734 GridCalEngine-5.1.2/GridCalEngine/IO/raw/devices/psse_circuit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7998 2024-02-13 14:28:28.603734 GridCalEngine-5.1.2/GridCalEngine/IO/raw/devices/bus.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    21807 2024-02-13 14:28:28.603734 GridCalEngine-5.1.2/GridCalEngine/IO/raw/devices/vsc_dc_line.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3434 2024-02-13 14:28:28.603734 GridCalEngine-5.1.2/GridCalEngine/IO/raw/devices/area.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    16814 2024-03-11 19:28:12.203075 GridCalEngine-5.1.2/GridCalEngine/IO/raw/devices/induction_machine.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3338 2024-03-11 19:28:12.203075 GridCalEngine-5.1.2/GridCalEngine/IO/raw/devices/fixed_shunt.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    10649 2024-02-13 14:28:28.603734 GridCalEngine-5.1.2/GridCalEngine/IO/raw/devices/load.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4135 2024-02-13 14:28:28.603734 GridCalEngine-5.1.2/GridCalEngine/IO/raw/devices/node.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2335 2024-02-13 14:28:28.603734 GridCalEngine-5.1.2/GridCalEngine/IO/raw/devices/zone.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11887 2024-02-13 14:28:28.603734 GridCalEngine-5.1.2/GridCalEngine/IO/raw/devices/branch.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3486 2024-03-11 19:28:12.203075 GridCalEngine-5.1.2/GridCalEngine/IO/raw/devices/substation.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2238 2024-02-13 14:28:28.603734 GridCalEngine-5.1.2/GridCalEngine/IO/matpower/matpower_storage_definitions.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7498 2023-11-16 09:36:26.530645 GridCalEngine-5.1.2/GridCalEngine/IO/matpower/matpower_gen_definitions.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.530645 GridCalEngine-5.1.2/GridCalEngine/IO/matpower/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8171 2024-03-14 19:48:07.688505 GridCalEngine-5.1.2/GridCalEngine/IO/matpower/matpower_bus_definitions.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    31013 2024-03-14 19:48:07.688505 GridCalEngine-5.1.2/GridCalEngine/IO/matpower/matpower_parser.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6661 2023-11-16 09:36:26.530645 GridCalEngine-5.1.2/GridCalEngine/IO/matpower/matpower_branch_definitions.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.530645 GridCalEngine-5.1.2/GridCalEngine/IO/gridcal/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    54302 2024-04-08 13:34:15.975164 GridCalEngine-5.1.2/GridCalEngine/IO/gridcal/pack_unpack.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    16119 2024-03-11 19:28:12.199075 GridCalEngine-5.1.2/GridCalEngine/IO/gridcal/zip_interface.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    98297 2024-03-28 10:16:48.984877 GridCalEngine-5.1.2/GridCalEngine/IO/gridcal/json_parser.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1966 2024-03-11 19:28:12.199075 GridCalEngine-5.1.2/GridCalEngine/IO/gridcal/generic_io_functions.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2432 2024-03-11 19:28:12.199075 GridCalEngine-5.1.2/GridCalEngine/IO/gridcal/h5_interface.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    47307 2024-03-14 19:48:07.688505 GridCalEngine-5.1.2/GridCalEngine/IO/gridcal/excel_interface.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2365 2024-02-13 14:28:28.599734 GridCalEngine-5.1.2/GridCalEngine/IO/gridcal/sqlite_interface.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2869 2024-03-11 19:28:12.199075 GridCalEngine-5.1.2/GridCalEngine/IO/gridcal/contingency_parser.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.530645 GridCalEngine-5.1.2/GridCalEngine/IO/epc/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    19972 2024-03-11 19:28:12.199075 GridCalEngine-5.1.2/GridCalEngine/IO/epc/epc_parser.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    38780 2024-03-28 10:16:48.984877 GridCalEngine-5.1.2/GridCalEngine/IO/others/dpx_parser.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.530645 GridCalEngine-5.1.2/GridCalEngine/IO/others/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4259 2024-03-14 19:48:07.688505 GridCalEngine-5.1.2/GridCalEngine/IO/others/ipa_parser.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    12272 2024-03-11 19:28:12.203075 GridCalEngine-5.1.2/GridCalEngine/IO/others/pypsa_parser.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    32570 2024-03-28 10:16:48.984877 GridCalEngine-5.1.2/GridCalEngine/IO/others/plx_parser.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.522645 GridCalEngine-5.1.2/GridCalEngine/IO/cim/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    36020 2024-03-11 19:28:12.183075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_enums.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    49632 2024-04-08 13:34:15.971164 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_to_gridcal.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3421 2024-03-11 19:28:12.183075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_poperty.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    15944 2024-03-28 10:16:48.980877 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_data_parser.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-11 19:28:12.183075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2229 2024-03-11 19:28:12.195075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_writer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    25093 2024-04-08 13:34:15.971164 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/gridcal_to_cgmes.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11194 2024-03-28 10:16:48.980877 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/base.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11951 2024-04-01 07:29:23.256927 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_export.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    26275 2024-04-08 13:34:15.971164 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_utils.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8815 2024-03-14 19:59:31.536490 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_data_validator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    81740 2024-04-08 13:34:15.971164 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_circuit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1167 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_switch.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2002 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_non_linear.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2803 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/connectivity_node.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1933 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_equipment_container.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3119 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/identified_object.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3492 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/control_area.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2649 2024-03-14 19:48:07.684505 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/location.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1169 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_chopper.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1201 2024-03-11 19:28:12.195075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/season_day_type_schedule.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1999 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/asynchronous_machine.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4399 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_injection.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1550 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_line.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1616 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/caes_plant.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1607 2024-03-11 19:28:12.195075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/solar_power_plant.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2454 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/curve.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1755 2024-03-11 19:28:12.195075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/regular_interval_schedule.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1121 2024-03-11 19:28:12.195075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/work_location.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1140 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/breaker.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1570 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_topological_island.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1581 2024-03-11 19:28:12.195075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ratio_tap_changer_table_point.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1164 2024-03-11 19:28:12.195075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/surge_arrester.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1912 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/battery_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1117 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/post_line_sensor.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4313 2024-03-11 19:28:12.195075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/shunt_compensator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2394 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/nonlinear_shunt_compensator_point.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2122 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_branch.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1750 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/active_power_limit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1097 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/fuse.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1656 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/nonlinear_shunt_compensator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1707 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_series_device.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3015 2024-03-11 19:28:12.195075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tap_changer_table_point.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1499 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_system_resource.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1147 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/disconnecting_circuit_breaker.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1693 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_shunt.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5175 2024-03-11 19:28:12.195075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/vs_converter.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3482 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/external_network_injection.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3263 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_electronics_connection.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1125 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/current_transformer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2025 2024-03-11 19:28:12.195075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_voltage.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2431 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_node.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1174 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_connection.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1960 2024-03-11 19:28:12.195075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_tap_step.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2689 2024-03-11 19:28:12.195075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/voltage_level.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3356 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_consumer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1838 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/current_limit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1166 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/fault_indicator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2263 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ratio_tap_changer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1187 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/grounding_impedance.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1677 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_ground.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7023 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/acdc_converter.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1113 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/disconnector.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3305 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_transformer_end.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1167 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_busbar.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1977 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/operational_limit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1164 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/nuclear_generating_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1540 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_scheduling_type.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1546 2024-03-11 19:28:12.195075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tap_changer_control.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1569 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_transformer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1500 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/auxiliary_equipment.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2312 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/curve_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1175 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/petersen_coil.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1154 2024-03-11 19:28:12.195075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/wave_trap.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2033 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_table.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2730 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ac_line_segment.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1821 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_table_point.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1217 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_symmetrical.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1521 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3095 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/base_voltage.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3217 2024-03-11 19:28:12.195075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/transformer_end.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1636 2024-03-11 19:28:12.195075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/voltage_limit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1597 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_network.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1101 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/jumper.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3204 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/acdc_terminal.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1567 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_terminal.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1116 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_breaker.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3413 2024-03-11 19:28:12.195075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/switch.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3854 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equipment.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5068 2024-03-11 19:28:12.195075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/topological_node.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2815 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/operational_limit_type.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1931 2024-03-11 19:28:12.195075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/reporting_group.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1735 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/linear_shunt_compensator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3458 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_source.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2228 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_line_segment.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1414 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conductor.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2748 2024-03-11 19:28:12.195075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/thermal_generating_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1117 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/junction.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1574 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_equipment.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2567 2024-03-11 19:28:12.195075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sub_geographical_region.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1617 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/cogeneration_plant.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2186 2024-03-11 19:28:12.195075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_injection.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5616 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/boundary_point.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5089 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_response_characteristic.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1896 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_converter_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1499 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/bay.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1821 2024-03-11 19:28:12.195075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/wind_generating_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1799 2024-03-11 19:28:12.195075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sub_load_area.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2175 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_electronics_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2422 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/hydro_generating_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2421 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conducting_equipment.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1571 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/geographical_region.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1517 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/non_conform_load.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3492 2024-03-11 19:28:12.195075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/synchronous_machine.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1528 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/line.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1504 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_group.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1696 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_shunt.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2807 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_topological_node.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1469 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_area.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2004 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/control_area_generating_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1523 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equipment_container.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2110 2024-03-11 19:28:12.195075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/topological_island.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1129 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/potential_transformer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1955 2024-03-11 19:28:12.195075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_shunt_compensator_sections.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1593 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_tabular.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1150 2024-03-11 19:28:12.195075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sensor.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4996 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/cs_converter.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1501 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conform_load_group.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1597 2024-03-11 19:28:12.195075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/wind_power_plant.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3510 2024-03-11 19:28:12.195075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/rotating_machine.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1195 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_electronics_wind_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1527 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_area.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1986 2024-03-11 19:28:12.195075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/reactive_capability_curve.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2080 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/hydro_pump.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1119 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/protected_switch.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1941 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_linear.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2133 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/acdc_converterdc_terminal.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4941 2024-03-11 19:28:12.195075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tap_changer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1765 2024-03-11 19:28:12.195075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_switch.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1520 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/non_conform_load_group.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2093 2024-03-11 19:28:12.195075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_status.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1156 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_break_switch.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2253 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/bus_name_marker.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1548 2024-03-11 19:28:12.195075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/solar_generating_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1860 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/fossil_fuel.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1184 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/earth_fault_compensator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2249 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/operational_limit_set.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2307 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/hydro_power_plant.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6776 2024-03-14 19:48:07.684505 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/generating_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1144 2024-03-11 19:28:12.195075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/service_location.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5780 2024-03-11 19:28:12.195075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/terminal.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1489 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_asymmetrical.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1621 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/combined_cycle_plant.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1127 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/busbar_section.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1126 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_disconnector.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1160 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/connector.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2404 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/coordinate_system.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1901 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_base_terminal.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2752 2024-03-11 19:28:12.195075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/static_var_compensator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1712 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/apparent_power_limit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1498 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conform_load.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1652 2024-03-11 19:28:12.195075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/series_compensator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2010 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/connectivity_node_container.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2299 2024-03-11 19:28:12.195075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/substation.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2448 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/position_point.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1805 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/clamp.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2302 2024-03-11 19:28:12.195075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tie_flow.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1996 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/basic_interval_schedule.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1744 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/cut.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1125 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ground_disconnector.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1971 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ratio_tap_changer_table.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1740 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_conducting_equipment.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1486 2024-03-11 19:28:12.195075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/vs_capability_curve.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1179 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/photo_voltaic_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1154 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ground.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5088 2024-03-11 19:28:12.195075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/regulating_control.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2095 2024-03-11 19:28:12.195075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_power_flow.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-11 19:28:12.183075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1168 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_switch.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2003 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_non_linear.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2432 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/connectivity_node.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1820 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_equipment_container.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3521 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/identified_object.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3496 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/control_area.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2403 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/location.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1170 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_chopper.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1202 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/season_day_type_schedule.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4118 2024-03-11 19:28:12.183075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/asynchronous_machine.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5617 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_injection.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1507 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_line.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2447 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/curve.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1702 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/regular_interval_schedule.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1141 2024-03-11 19:28:12.183075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/breaker.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1524 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_topological_island.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1583 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ratio_tap_changer_table_point.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3985 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/shunt_compensator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2908 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/nonlinear_shunt_compensator_point.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5115 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_branch.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1457 2024-03-11 19:28:12.183075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/active_power_limit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1658 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/nonlinear_shunt_compensator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1943 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_series_device.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2768 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tap_changer_table_point.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2209 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/power_system_resource.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1694 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_shunt.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4544 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/vs_converter.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6505 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/external_network_injection.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2026 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_voltage.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2246 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_node.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2211 2024-04-08 13:34:15.971164 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1800 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_tap_step.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2693 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/voltage_level.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3370 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_consumer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1497 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/current_limit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2617 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ratio_tap_changer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1444 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/grounding_impedance.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1678 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_ground.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6262 2024-03-11 19:28:12.183075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/acdc_converter.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1114 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/disconnector.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4973 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/power_transformer_end.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1168 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_busbar.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1960 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/operational_limit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1165 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/nuclear_generating_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1531 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_scheduling_type.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1544 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tap_changer_control.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3596 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/power_transformer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2285 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/curve_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3199 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/petersen_coil.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2036 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_table.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3385 2024-03-11 19:28:12.183075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ac_line_segment.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1822 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_table_point.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1218 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_symmetrical.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1522 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3094 2024-03-11 19:28:12.183075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/base_voltage.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3989 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/transformer_end.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1396 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/voltage_limit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1611 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_network.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1768 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/measurement_value.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3786 2024-03-11 19:28:12.183075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/acdc_terminal.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1521 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_terminal.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1117 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_breaker.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2509 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/switch.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2591 2024-03-14 19:48:07.684505 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equipment.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5742 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/quality61850.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5081 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/topological_node.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2424 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/operational_limit_type.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1936 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/reporting_group.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2289 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/linear_shunt_compensator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4321 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_source.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2638 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_line_segment.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1475 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/limit_set.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1393 2024-03-11 19:28:12.183075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conductor.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1533 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/thermal_generating_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4216 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/full_model.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1118 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/junction.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1564 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_equipment.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2534 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sub_geographical_region.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2189 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_injection.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5141 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_response_characteristic.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1776 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_converter_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1501 2024-03-11 19:28:12.183075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/bay.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1441 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/wind_generating_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1141 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/limit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1802 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sub_load_area.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1901 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/hydro_generating_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2431 2024-03-11 19:28:12.183075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conducting_equipment.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1573 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/geographical_region.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1541 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/non_conform_load.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7957 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/synchronous_machine.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1530 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/line.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1506 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_group.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1932 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_shunt.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2608 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_topological_node.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1471 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_area.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2007 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/control_area_generating_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1525 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equipment_container.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2317 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/per_lengthdc_line_parameter.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3599 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/measurement.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2113 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/topological_island.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1852 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_shunt_compensator_sections.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1595 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_tabular.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4958 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/cs_converter.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1503 2024-03-11 19:28:12.183075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conform_load_group.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3430 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/rotating_machine.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1529 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_area.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2013 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/reactive_capability_curve.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2083 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/hydro_pump.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1120 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/protected_switch.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1942 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_linear.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1796 2024-03-11 19:28:12.183075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/acdc_converterdc_terminal.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4341 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tap_changer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1500 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/non_conform_load_group.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1860 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_status.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1157 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_break_switch.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2254 2024-03-11 19:28:12.183075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/bus_name_marker.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1161 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/solar_generating_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1862 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/fossil_fuel.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1417 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/earth_fault_compensator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2226 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/operational_limit_set.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2310 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/hydro_power_plant.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6586 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/generating_unit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6326 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/terminal.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1490 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_asymmetrical.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1470 2024-03-11 19:28:12.183075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/busbar_section.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1127 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_disconnector.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1161 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/connector.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2404 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/coordinate_system.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1823 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_base_terminal.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2744 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/static_var_compensator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1440 2024-03-11 19:28:12.183075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/apparent_power_limit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1500 2024-03-11 19:28:12.183075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conform_load.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3068 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/series_compensator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2013 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/connectivity_node_container.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2257 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/substation.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2449 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/position_point.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2444 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tie_flow.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1943 2024-03-11 19:28:12.183075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/basic_interval_schedule.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4063 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/mutual_coupling.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1126 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ground_disconnector.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1975 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ratio_tap_changer_table.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1894 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/regulating_cond_eq.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1456 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_conducting_equipment.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1650 2024-03-11 19:28:12.183075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/analog_control.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1481 2024-03-11 19:28:12.191075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/vs_capability_curve.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3195 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/control.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1155 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ground.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3782 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/regulating_control.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2096 2024-03-11 19:28:12.187075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_power_flow.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    18126 2024-02-13 14:28:28.599734 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cim16/cim_circuit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)   192495 2024-02-13 14:28:28.599734 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cim16/cim_devices.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.526645 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cim16/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    14224 2024-02-13 14:28:28.599734 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cim16/cim_enums.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    45731 2024-03-11 19:28:12.199075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cim16/cim_parser.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8909 2023-11-16 09:36:26.526645 GridCalEngine-5.1.2/GridCalEngine/IO/cim/cim16/cim_data_parser.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.526645 GridCalEngine-5.1.2/GridCalEngine/IO/cim/db/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2734 2023-11-16 09:36:26.526645 GridCalEngine-5.1.2/GridCalEngine/IO/cim/db/base_db.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1705 2024-03-11 19:28:12.199075 GridCalEngine-5.1.2/GridCalEngine/IO/cim/db/cgmes_lookup_db.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      697 2023-11-16 09:36:26.526645 GridCalEngine-5.1.2/GridCalEngine/IO/cim/db/file_system.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5267 2023-11-16 09:36:26.526645 GridCalEngine-5.1.2/GridCalEngine/IO/cim/db/psse_lookup_db.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      527 2023-11-16 09:36:26.526645 GridCalEngine-5.1.2/GridCalEngine/IO/cim/db/db_handler.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2499 2024-04-08 13:34:15.971164 GridCalEngine-5.1.2/GridCalEngine/Devices/types.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7311 2024-03-14 19:48:07.684505 GridCalEngine-5.1.2/GridCalEngine/Devices/sparse_array.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1463 2024-03-28 10:16:48.980877 GridCalEngine-5.1.2/GridCalEngine/Devices/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)   193316 2024-04-08 13:34:15.971164 GridCalEngine-5.1.2/GridCalEngine/Devices/multi_circuit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5773 2024-03-11 19:28:12.183075 GridCalEngine-5.1.2/GridCalEngine/Devices/measurement.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    14002 2024-03-28 10:16:48.980877 GridCalEngine-5.1.2/GridCalEngine/Devices/profile.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2048 2024-03-14 19:59:31.532490 GridCalEngine-5.1.2/GridCalEngine/Devices/Aggregation/municipality.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1687 2024-03-11 19:28:12.179075 GridCalEngine-5.1.2/GridCalEngine/Devices/Aggregation/contingency_group.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1813 2024-04-08 13:34:15.971164 GridCalEngine-5.1.2/GridCalEngine/Devices/Aggregation/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3005 2024-03-11 19:28:12.179075 GridCalEngine-5.1.2/GridCalEngine/Devices/Aggregation/fuel.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4255 2024-03-11 19:28:12.179075 GridCalEngine-5.1.2/GridCalEngine/Devices/Aggregation/contingency.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3028 2024-03-11 19:28:12.179075 GridCalEngine-5.1.2/GridCalEngine/Devices/Aggregation/emission_gas.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1647 2024-03-11 19:28:12.179075 GridCalEngine-5.1.2/GridCalEngine/Devices/Aggregation/country.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1332 2024-04-08 13:34:15.971164 GridCalEngine-5.1.2/GridCalEngine/Devices/Aggregation/modelling_authority.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2020 2024-03-14 19:59:31.532490 GridCalEngine-5.1.2/GridCalEngine/Devices/Aggregation/region.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2558 2024-03-28 10:16:48.972877 GridCalEngine-5.1.2/GridCalEngine/Devices/Aggregation/area.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2547 2024-03-11 19:28:12.179075 GridCalEngine-5.1.2/GridCalEngine/Devices/Aggregation/technology.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2008 2024-03-14 19:59:31.532490 GridCalEngine-5.1.2/GridCalEngine/Devices/Aggregation/zone.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2174 2024-03-11 19:28:12.179075 GridCalEngine-5.1.2/GridCalEngine/Devices/Aggregation/investments_group.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3715 2024-03-11 19:28:12.179075 GridCalEngine-5.1.2/GridCalEngine/Devices/Aggregation/investment.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2045 2024-03-14 19:59:31.532490 GridCalEngine-5.1.2/GridCalEngine/Devices/Aggregation/community.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1463 2024-03-14 19:59:31.532490 GridCalEngine-5.1.2/GridCalEngine/Devices/Aggregation/branch_group.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1099 2024-03-11 19:28:12.179075 GridCalEngine-5.1.2/GridCalEngine/Devices/Fluid/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3692 2024-03-28 10:16:48.976877 GridCalEngine-5.1.2/GridCalEngine/Devices/Fluid/fluid_path.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2342 2024-03-11 19:28:12.179075 GridCalEngine-5.1.2/GridCalEngine/Devices/Fluid/fluid_pump.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8006 2024-04-08 13:34:15.971164 GridCalEngine-5.1.2/GridCalEngine/Devices/Fluid/fluid_node.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2352 2024-03-11 19:28:12.179075 GridCalEngine-5.1.2/GridCalEngine/Devices/Fluid/fluid_turbine.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3976 2024-03-11 19:28:12.179075 GridCalEngine-5.1.2/GridCalEngine/Devices/Fluid/fluid_injection_template.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2331 2024-03-11 19:28:12.179075 GridCalEngine-5.1.2/GridCalEngine/Devices/Fluid/fluid_p2x.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    10736 2024-03-28 10:16:48.976877 GridCalEngine-5.1.2/GridCalEngine/Devices/Branches/dc_line.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4278 2024-03-11 19:28:12.179075 GridCalEngine-5.1.2/GridCalEngine/Devices/Branches/underground_line_type.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2005 2024-03-28 10:16:48.972877 GridCalEngine-5.1.2/GridCalEngine/Devices/Branches/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    10226 2024-03-28 10:16:48.976877 GridCalEngine-5.1.2/GridCalEngine/Devices/Branches/series_reactance.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2485 2024-03-11 19:28:12.179075 GridCalEngine-5.1.2/GridCalEngine/Devices/Branches/wire.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5553 2024-03-28 10:16:48.976877 GridCalEngine-5.1.2/GridCalEngine/Devices/Branches/line_locations.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3652 2024-03-11 19:28:12.179075 GridCalEngine-5.1.2/GridCalEngine/Devices/Branches/sequence_line_type.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    18829 2024-03-14 19:48:07.684505 GridCalEngine-5.1.2/GridCalEngine/Devices/Branches/overhead_line_type.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7386 2024-03-14 19:59:31.532490 GridCalEngine-5.1.2/GridCalEngine/Devices/Branches/switch.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    12638 2024-03-28 10:16:48.976877 GridCalEngine-5.1.2/GridCalEngine/Devices/Branches/vsc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7628 2024-03-28 10:16:48.976877 GridCalEngine-5.1.2/GridCalEngine/Devices/Branches/upfc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    19502 2024-03-28 10:16:48.976877 GridCalEngine-5.1.2/GridCalEngine/Devices/Branches/transformer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    19989 2024-03-28 10:16:48.976877 GridCalEngine-5.1.2/GridCalEngine/Devices/Branches/hvdc_line.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    15863 2024-03-28 10:16:48.976877 GridCalEngine-5.1.2/GridCalEngine/Devices/Branches/line.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9400 2024-03-28 10:16:48.976877 GridCalEngine-5.1.2/GridCalEngine/Devices/Branches/tap_changer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9196 2024-03-28 10:16:48.976877 GridCalEngine-5.1.2/GridCalEngine/Devices/Branches/winding.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    21848 2024-03-28 10:16:48.976877 GridCalEngine-5.1.2/GridCalEngine/Devices/Branches/branch.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5636 2024-03-11 19:28:12.179075 GridCalEngine-5.1.2/GridCalEngine/Devices/Branches/transformer_type.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11752 2024-04-08 13:34:15.971164 GridCalEngine-5.1.2/GridCalEngine/Devices/Branches/transformer3w.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2136 2024-03-11 19:28:12.183075 GridCalEngine-5.1.2/GridCalEngine/Devices/Injections/static_generator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2325 2024-03-28 10:16:48.976877 GridCalEngine-5.1.2/GridCalEngine/Devices/Injections/shunt.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1419 2024-03-11 19:28:12.179075 GridCalEngine-5.1.2/GridCalEngine/Devices/Injections/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5913 2024-03-28 10:16:48.976877 GridCalEngine-5.1.2/GridCalEngine/Devices/Injections/external_grid.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5261 2024-03-28 10:16:48.976877 GridCalEngine-5.1.2/GridCalEngine/Devices/Injections/current_injection.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6930 2024-03-28 10:16:48.976877 GridCalEngine-5.1.2/GridCalEngine/Devices/Injections/battery.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    15372 2024-03-28 10:16:48.976877 GridCalEngine-5.1.2/GridCalEngine/Devices/Injections/generator.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7856 2024-03-28 10:16:48.976877 GridCalEngine-5.1.2/GridCalEngine/Devices/Injections/generator_q_curve.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6864 2024-03-28 10:16:48.976877 GridCalEngine-5.1.2/GridCalEngine/Devices/Injections/controllable_shunt.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6780 2024-03-28 10:16:48.976877 GridCalEngine-5.1.2/GridCalEngine/Devices/Injections/load.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2203 2024-04-01 07:29:23.256927 GridCalEngine-5.1.2/GridCalEngine/Devices/Diagrams/graphic_location.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3172 2024-03-11 19:28:12.179075 GridCalEngine-5.1.2/GridCalEngine/Devices/Diagrams/map_diagram.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1181 2024-03-11 19:28:12.179075 GridCalEngine-5.1.2/GridCalEngine/Devices/Diagrams/node_breaker_diagram.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1162 2024-03-11 19:28:12.179075 GridCalEngine-5.1.2/GridCalEngine/Devices/Diagrams/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1176 2024-03-11 19:28:12.179075 GridCalEngine-5.1.2/GridCalEngine/Devices/Diagrams/bus_branch_diagram.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1452 2024-03-11 19:28:12.179075 GridCalEngine-5.1.2/GridCalEngine/Devices/Diagrams/map_location.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    12261 2024-04-01 07:29:23.256927 GridCalEngine-5.1.2/GridCalEngine/Devices/Diagrams/base_diagram.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1982 2024-03-11 19:28:12.183075 GridCalEngine-5.1.2/GridCalEngine/Devices/Substation/connectivity_node.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1130 2024-03-14 19:48:07.684505 GridCalEngine-5.1.2/GridCalEngine/Devices/Substation/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2020 2024-03-14 19:48:07.684505 GridCalEngine-5.1.2/GridCalEngine/Devices/Substation/voltage_level.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    14124 2024-03-28 10:16:48.980877 GridCalEngine-5.1.2/GridCalEngine/Devices/Substation/bus.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2648 2024-03-14 19:48:07.684505 GridCalEngine-5.1.2/GridCalEngine/Devices/Substation/busbar.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7724 2024-03-28 10:16:48.980877 GridCalEngine-5.1.2/GridCalEngine/Devices/Substation/substation.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7316 2024-04-03 10:10:53.840547 GridCalEngine-5.1.2/GridCalEngine/Devices/Parents/injection_parent.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    24200 2024-03-28 10:16:48.980877 GridCalEngine-5.1.2/GridCalEngine/Devices/Parents/editable_device.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7700 2024-03-11 19:28:12.183075 GridCalEngine-5.1.2/GridCalEngine/Devices/Parents/generator_parent.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      790 2024-03-11 19:28:12.183075 GridCalEngine-5.1.2/GridCalEngine/Devices/Parents/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    16800 2024-03-28 10:16:48.980877 GridCalEngine-5.1.2/GridCalEngine/Devices/Parents/controllable_branch_parent.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7034 2024-03-11 19:28:12.183075 GridCalEngine-5.1.2/GridCalEngine/Devices/Parents/load_parent.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    17125 2024-03-28 10:16:48.980877 GridCalEngine-5.1.2/GridCalEngine/Devices/Parents/branch_parent.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8463 2024-03-11 19:28:12.183075 GridCalEngine-5.1.2/GridCalEngine/Devices/Parents/shunt_parent.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2829 2024-03-11 19:28:12.179075 GridCalEngine-5.1.2/GridCalEngine/Devices/Associations/generator_emission.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1038 2024-03-11 19:28:12.179075 GridCalEngine-5.1.2/GridCalEngine/Devices/Associations/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2898 2024-03-11 19:28:12.179075 GridCalEngine-5.1.2/GridCalEngine/Devices/Associations/generator_technology.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2741 2024-03-11 19:28:12.179075 GridCalEngine-5.1.2/GridCalEngine/Devices/Associations/generator_fuel.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6558 2024-03-11 19:28:12.175075 GridCalEngine-5.1.2/GridCalEngine/DataStructures/load_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4274 2024-03-14 19:48:07.680505 GridCalEngine-5.1.2/GridCalEngine/DataStructures/bus_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    14793 2024-04-01 07:29:23.256927 GridCalEngine-5.1.2/GridCalEngine/DataStructures/branch_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1588 2024-03-11 19:28:12.175075 GridCalEngine-5.1.2/GridCalEngine/DataStructures/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2088 2024-03-11 19:28:12.175075 GridCalEngine-5.1.2/GridCalEngine/DataStructures/fluid_turbine_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1158 2024-03-11 19:28:12.175075 GridCalEngine-5.1.2/GridCalEngine/DataStructures/fluid_p2x_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    67051 2024-04-03 10:10:53.840547 GridCalEngine-5.1.2/GridCalEngine/DataStructures/numerical_circuit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    10107 2024-03-11 19:28:12.175075 GridCalEngine-5.1.2/GridCalEngine/DataStructures/generator_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1162 2024-03-11 19:28:12.175075 GridCalEngine-5.1.2/GridCalEngine/DataStructures/fluid_pump_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3073 2024-03-11 19:28:12.175075 GridCalEngine-5.1.2/GridCalEngine/DataStructures/battery_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2038 2024-03-11 19:28:12.175075 GridCalEngine-5.1.2/GridCalEngine/DataStructures/fluid_path_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    10968 2024-03-14 19:59:31.532490 GridCalEngine-5.1.2/GridCalEngine/DataStructures/hvdc_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4320 2024-03-11 19:28:12.175075 GridCalEngine-5.1.2/GridCalEngine/DataStructures/shunt_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2347 2024-04-08 13:34:15.971164 GridCalEngine-5.1.2/GridCalEngine/DataStructures/fluid_node_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    70288 2024-03-11 19:28:12.175075 GridCalEngine-5.1.2/GridCalEngine/Compilers/circuit_to_newton_pa.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    27811 2024-03-11 19:28:12.175075 GridCalEngine-5.1.2/GridCalEngine/Compilers/circuit_to_bentayga.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      992 2024-03-11 19:28:12.175075 GridCalEngine-5.1.2/GridCalEngine/Compilers/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    43991 2024-04-08 13:34:15.971164 GridCalEngine-5.1.2/GridCalEngine/Compilers/circuit_to_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3328 2024-03-11 19:28:12.175075 GridCalEngine-5.1.2/GridCalEngine/Compilers/circuit_to_optimods.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    27652 2024-03-14 19:48:07.680505 GridCalEngine-5.1.2/GridCalEngine/Compilers/circuit_to_pgm.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11185 2024-03-14 19:48:07.692505 GridCalEngine-5.1.2/GridCalEngine/Simulations/results_template.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1767 2024-03-11 19:28:12.223075 GridCalEngine-5.1.2/GridCalEngine/Simulations/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    12454 2024-03-11 19:28:12.223075 GridCalEngine-5.1.2/GridCalEngine/Simulations/results_table.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2699 2024-03-11 19:28:12.223075 GridCalEngine-5.1.2/GridCalEngine/Simulations/driver_types.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7963 2024-03-14 19:59:31.536490 GridCalEngine-5.1.2/GridCalEngine/Simulations/driver_template.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      359 2024-01-05 08:44:35.545288 GridCalEngine-5.1.2/GridCalEngine/Simulations/InvestmentsEvaluation/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    17002 2024-03-11 19:28:12.211075 GridCalEngine-5.1.2/GridCalEngine/Simulations/InvestmentsEvaluation/investments_evaluation_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8665 2024-03-14 19:48:07.692505 GridCalEngine-5.1.2/GridCalEngine/Simulations/InvestmentsEvaluation/investments_evaluation_results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2248 2024-02-13 14:28:28.607734 GridCalEngine-5.1.2/GridCalEngine/Simulations/InvestmentsEvaluation/investments_evaluation_options.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3318 2024-03-11 19:28:12.211075 GridCalEngine-5.1.2/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/stop_crits.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    25202 2024-03-14 19:48:07.692505 GridCalEngine-5.1.2/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/MVRSM_mo_pareto.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-11 19:28:12.211075 GridCalEngine-5.1.2/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    24206 2024-03-11 19:28:12.211075 GridCalEngine-5.1.2/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/MVRSM_mo_scaled.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    17532 2024-03-11 19:28:12.211075 GridCalEngine-5.1.2/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/MVRSM_original.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1104 2024-03-11 19:28:12.219075 GridCalEngine-5.1.2/GridCalEngine/Simulations/Topology/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11454 2024-03-14 19:48:07.692505 GridCalEngine-5.1.2/GridCalEngine/Simulations/Topology/topology_reduction_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11519 2024-03-11 19:28:12.219075 GridCalEngine-5.1.2/GridCalEngine/Simulations/Topology/topology_processor_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4832 2024-03-11 19:28:12.219075 GridCalEngine-5.1.2/GridCalEngine/Simulations/Topology/node_groups_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6814 2024-03-11 19:28:12.219075 GridCalEngine-5.1.2/GridCalEngine/Simulations/Stochastic/reliability_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3804 2024-03-14 19:48:07.692505 GridCalEngine-5.1.2/GridCalEngine/Simulations/Stochastic/stochastic_power_flow_input.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1312 2024-02-13 14:28:28.611734 GridCalEngine-5.1.2/GridCalEngine/Simulations/Stochastic/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    19791 2024-03-11 19:28:12.219075 GridCalEngine-5.1.2/GridCalEngine/Simulations/Stochastic/stochastic_power_flow_results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3777 2024-03-11 19:28:12.219075 GridCalEngine-5.1.2/GridCalEngine/Simulations/Stochastic/reliability_iterable.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11634 2024-03-11 19:28:12.219075 GridCalEngine-5.1.2/GridCalEngine/Simulations/Stochastic/blackout_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8063 2024-03-11 19:28:12.219075 GridCalEngine-5.1.2/GridCalEngine/Simulations/Stochastic/stochastic_power_flow_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8210 2024-03-14 19:48:07.692505 GridCalEngine-5.1.2/GridCalEngine/Simulations/Stochastic/latin_hypercube_sampling.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    29913 2024-03-11 19:28:12.219075 GridCalEngine-5.1.2/GridCalEngine/Simulations/PowerFlow/power_flow_ts_results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    10299 2024-03-14 19:59:31.536490 GridCalEngine-5.1.2/GridCalEngine/Simulations/PowerFlow/power_flow_ts_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    33458 2024-03-14 19:48:07.692505 GridCalEngine-5.1.2/GridCalEngine/Simulations/PowerFlow/power_flow_results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9269 2024-03-11 19:28:12.219075 GridCalEngine-5.1.2/GridCalEngine/Simulations/PowerFlow/power_flow_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1474 2024-02-13 14:28:28.611734 GridCalEngine-5.1.2/GridCalEngine/Simulations/PowerFlow/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5534 2024-02-13 14:28:28.611734 GridCalEngine-5.1.2/GridCalEngine/Simulations/PowerFlow/power_flow_ts_input.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4163 2024-03-11 19:28:12.215075 GridCalEngine-5.1.2/GridCalEngine/Simulations/PowerFlow/grid_analysis.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5496 2024-02-20 09:29:33.592105 GridCalEngine-5.1.2/GridCalEngine/Simulations/PowerFlow/power_flow_options.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    31315 2024-03-14 19:48:07.692505 GridCalEngine-5.1.2/GridCalEngine/Simulations/PowerFlow/power_flow_worker.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8754 2024-03-28 10:16:48.988877 GridCalEngine-5.1.2/GridCalEngine/Simulations/PowerFlow/NumericalMethods/common_functions.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1999 2024-02-13 14:28:28.611734 GridCalEngine-5.1.2/GridCalEngine/Simulations/PowerFlow/NumericalMethods/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    32701 2024-02-13 14:28:28.611734 GridCalEngine-5.1.2/GridCalEngine/Simulations/PowerFlow/NumericalMethods/acdc_jacobian.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    18741 2024-03-11 19:28:12.215075 GridCalEngine-5.1.2/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_acdc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8459 2024-03-14 19:48:07.692505 GridCalEngine-5.1.2/GridCalEngine/Simulations/PowerFlow/NumericalMethods/iwamoto_newton_raphson.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9795 2024-02-20 09:29:33.592105 GridCalEngine-5.1.2/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    12948 2024-03-11 19:28:12.215075 GridCalEngine-5.1.2/GridCalEngine/Simulations/PowerFlow/NumericalMethods/levenberg_marquardt_acdc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    33790 2024-03-14 19:48:07.692505 GridCalEngine-5.1.2/GridCalEngine/Simulations/PowerFlow/NumericalMethods/derivatives.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8882 2024-02-20 09:29:33.592105 GridCalEngine-5.1.2/GridCalEngine/Simulations/PowerFlow/NumericalMethods/levenberg_marquardt.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4066 2023-11-16 09:36:26.538645 GridCalEngine-5.1.2/GridCalEngine/Simulations/PowerFlow/NumericalMethods/fast_decoupled.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    25376 2024-03-14 19:48:07.692505 GridCalEngine-5.1.2/GridCalEngine/Simulations/PowerFlow/NumericalMethods/helm_power_flow.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6550 2024-03-14 19:48:07.692505 GridCalEngine-5.1.2/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_decoupled.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4027 2024-02-13 14:28:28.611734 GridCalEngine-5.1.2/GridCalEngine/Simulations/PowerFlow/NumericalMethods/gauss_power_flow.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7630 2024-03-14 19:48:07.692505 GridCalEngine-5.1.2/GridCalEngine/Simulations/PowerFlow/NumericalMethods/linearized_power_flow.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5676 2024-03-14 19:48:07.692505 GridCalEngine-5.1.2/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_ode.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    17875 2023-11-16 09:36:26.538645 GridCalEngine-5.1.2/GridCalEngine/Simulations/PowerFlow/NumericalMethods/ac_jacobian.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    26346 2024-01-05 08:44:35.549288 GridCalEngine-5.1.2/GridCalEngine/Simulations/PowerFlow/NumericalMethods/discrete_controls.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5855 2024-02-13 14:28:28.611734 GridCalEngine-5.1.2/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_current.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      121 2023-11-16 09:36:26.534645 GridCalEngine-5.1.2/GridCalEngine/Simulations/InputsAnalysis/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    20717 2024-03-28 10:16:48.984877 GridCalEngine-5.1.2/GridCalEngine/Simulations/InputsAnalysis/inputs_analysis_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.534645 GridCalEngine-5.1.2/GridCalEngine/Simulations/Dynamics/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3926 2024-03-11 19:28:12.207075 GridCalEngine-5.1.2/GridCalEngine/Simulations/Dynamics/transient_stability_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    48769 2024-03-14 19:48:07.692505 GridCalEngine-5.1.2/GridCalEngine/Simulations/Dynamics/dynamic_modules.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1401 2024-02-13 14:28:28.607734 GridCalEngine-5.1.2/GridCalEngine/Simulations/ContinuationPowerFlow/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7391 2024-03-14 19:48:07.692505 GridCalEngine-5.1.2/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1394 2024-02-13 14:28:28.607734 GridCalEngine-5.1.2/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_input.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    29971 2024-04-08 13:34:15.975164 GridCalEngine-5.1.2/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2390 2024-02-13 14:28:28.607734 GridCalEngine-5.1.2/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_options.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    18392 2024-03-11 19:28:12.207075 GridCalEngine-5.1.2/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4371 2024-02-13 14:28:28.611734 GridCalEngine-5.1.2/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    13984 2024-03-14 19:48:07.692505 GridCalEngine-5.1.2/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1138 2024-02-13 14:28:28.611734 GridCalEngine-5.1.2/GridCalEngine/Simulations/ShortCircuitStudies/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    28931 2024-03-11 19:28:12.219075 GridCalEngine-5.1.2/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit_results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    16615 2024-04-01 07:29:23.260927 GridCalEngine-5.1.2/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit_worker.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      463 2023-11-16 09:36:26.534645 GridCalEngine-5.1.2/GridCalEngine/Simulations/NTC/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    46689 2024-03-28 10:16:48.984877 GridCalEngine-5.1.2/GridCalEngine/Simulations/NTC/ntc_results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    31737 2024-03-28 10:16:48.984877 GridCalEngine-5.1.2/GridCalEngine/Simulations/NTC/ntc_ts_results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7649 2024-03-28 10:16:48.984877 GridCalEngine-5.1.2/GridCalEngine/Simulations/NTC/ntc_ts_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    51043 2024-03-28 10:16:48.984877 GridCalEngine-5.1.2/GridCalEngine/Simulations/NTC/ntc_opf.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8071 2024-03-28 10:16:48.984877 GridCalEngine-5.1.2/GridCalEngine/Simulations/NTC/ntc_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3467 2024-03-28 10:16:48.984877 GridCalEngine-5.1.2/GridCalEngine/Simulations/NTC/ntc_options.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9925 2024-03-14 19:48:07.692505 GridCalEngine-5.1.2/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_ts_results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7552 2024-03-14 19:48:07.692505 GridCalEngine-5.1.2/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1376 2024-02-13 14:28:28.603734 GridCalEngine-5.1.2/GridCalEngine/Simulations/ContingencyAnalysis/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7522 2024-03-14 19:59:31.536490 GridCalEngine-5.1.2/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3522 2024-03-11 19:28:12.207075 GridCalEngine-5.1.2/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_options.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    29395 2024-03-28 10:16:48.984877 GridCalEngine-5.1.2/GridCalEngine/Simulations/ContingencyAnalysis/contingencies_report.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8858 2024-03-14 19:59:31.536490 GridCalEngine-5.1.2/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_ts_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9287 2024-03-14 19:48:07.692505 GridCalEngine-5.1.2/GridCalEngine/Simulations/ContingencyAnalysis/contingency_plan.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-02-13 14:28:28.603734 GridCalEngine-5.1.2/GridCalEngine/Simulations/ContingencyAnalysis/Methods/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8443 2024-03-14 19:59:31.536490 GridCalEngine-5.1.2/GridCalEngine/Simulations/ContingencyAnalysis/Methods/srap.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8773 2024-03-14 19:59:31.536490 GridCalEngine-5.1.2/GridCalEngine/Simulations/ContingencyAnalysis/Methods/optimal_linear_contingency_analysis.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7252 2024-03-14 19:59:31.536490 GridCalEngine-5.1.2/GridCalEngine/Simulations/ContingencyAnalysis/Methods/linear_contingency_analysis.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7518 2024-03-14 19:59:31.536490 GridCalEngine-5.1.2/GridCalEngine/Simulations/ContingencyAnalysis/Methods/nonlinear_contingency_analysis.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5880 2024-03-14 19:59:31.536490 GridCalEngine-5.1.2/GridCalEngine/Simulations/ContingencyAnalysis/Methods/helm_contingency_analysis.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11049 2024-03-11 19:28:12.207075 GridCalEngine-5.1.2/GridCalEngine/Simulations/ContingencyAnalysis/Methods/helm_contingencies.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5386 2024-03-14 19:48:07.692505 GridCalEngine-5.1.2/GridCalEngine/Simulations/Clustering/clustering.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1054 2024-02-13 14:28:28.603734 GridCalEngine-5.1.2/GridCalEngine/Simulations/Clustering/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3158 2024-03-11 19:28:12.207075 GridCalEngine-5.1.2/GridCalEngine/Simulations/Clustering/clustering_results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      984 2024-02-13 14:28:28.603734 GridCalEngine-5.1.2/GridCalEngine/Simulations/Clustering/clustering_options.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2710 2024-03-11 19:28:12.207075 GridCalEngine-5.1.2/GridCalEngine/Simulations/Clustering/clustering_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9311 2024-03-11 19:28:12.219075 GridCalEngine-5.1.2/GridCalEngine/Simulations/StateEstimation/state_stimation_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      215 2023-11-16 09:36:26.538645 GridCalEngine-5.1.2/GridCalEngine/Simulations/StateEstimation/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    12628 2023-11-16 09:36:26.538645 GridCalEngine-5.1.2/GridCalEngine/Simulations/StateEstimation/state_estimation.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    14766 2024-03-28 10:16:48.988877 GridCalEngine-5.1.2/GridCalEngine/Simulations/OPF/opf_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1382 2024-02-13 14:28:28.611734 GridCalEngine-5.1.2/GridCalEngine/Simulations/OPF/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    26711 2024-03-28 10:16:48.988877 GridCalEngine-5.1.2/GridCalEngine/Simulations/OPF/opf_ts_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    33619 2024-03-11 19:28:12.215075 GridCalEngine-5.1.2/GridCalEngine/Simulations/OPF/opf_ts_results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    27247 2024-03-14 19:59:31.536490 GridCalEngine-5.1.2/GridCalEngine/Simulations/OPF/opf_results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4263 2024-03-11 19:28:12.215075 GridCalEngine-5.1.2/GridCalEngine/Simulations/OPF/simple_dispatch_ts.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    78572 2024-04-08 13:34:15.975164 GridCalEngine-5.1.2/GridCalEngine/Simulations/OPF/linear_opf_ts.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4148 2024-03-11 19:28:12.215075 GridCalEngine-5.1.2/GridCalEngine/Simulations/OPF/opf_options.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-02-13 14:28:28.607734 GridCalEngine-5.1.2/GridCalEngine/Simulations/OPF/NumericalMethods/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    44335 2024-04-08 13:34:15.975164 GridCalEngine-5.1.2/GridCalEngine/Simulations/OPF/NumericalMethods/ac_opf.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    15593 2024-02-13 14:28:28.607734 GridCalEngine-5.1.2/GridCalEngine/Simulations/OPF/NumericalMethods/ac_opf_autodif.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    54372 2024-04-08 13:34:15.975164 GridCalEngine-5.1.2/GridCalEngine/Simulations/OPF/NumericalMethods/ac_opf_derivatives.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    12868 2024-03-14 19:48:07.688505 GridCalEngine-5.1.2/GridCalEngine/Simulations/ATC/available_transfer_capacity_ts_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1054 2024-02-13 14:28:28.603734 GridCalEngine-5.1.2/GridCalEngine/Simulations/ATC/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    24852 2024-03-14 19:48:07.688505 GridCalEngine-5.1.2/GridCalEngine/Simulations/ATC/available_transfer_capacity_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      116 2023-11-16 09:36:26.538645 GridCalEngine-5.1.2/GridCalEngine/Simulations/SigmaAnalysis/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    18826 2024-03-11 19:28:12.219075 GridCalEngine-5.1.2/GridCalEngine/Simulations/SigmaAnalysis/sigma_analysis_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1207 2024-02-13 14:28:28.607734 GridCalEngine-5.1.2/GridCalEngine/Simulations/LinearFactors/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6692 2024-03-11 19:28:12.211075 GridCalEngine-5.1.2/GridCalEngine/Simulations/LinearFactors/linear_analysis_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    29516 2024-03-14 19:59:31.536490 GridCalEngine-5.1.2/GridCalEngine/Simulations/LinearFactors/linear_analysis.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6138 2024-03-11 19:28:12.211075 GridCalEngine-5.1.2/GridCalEngine/Simulations/LinearFactors/linear_analysis_ts_results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6497 2024-03-11 19:28:12.211075 GridCalEngine-5.1.2/GridCalEngine/Simulations/LinearFactors/linear_analysis_results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1603 2024-02-13 14:28:28.607734 GridCalEngine-5.1.2/GridCalEngine/Simulations/LinearFactors/linear_analysis_options.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4727 2024-03-11 19:28:12.211075 GridCalEngine-5.1.2/GridCalEngine/Simulations/LinearFactors/linear_analysis_ts_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3501 2024-03-17 12:13:24.384980 GridCalEngine-5.1.2/setup.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1049 2024-04-08 13:35:50.475167 GridCalEngine-5.1.2/PKG-INFO
+-rw-rw-r--   0 santi     (1000) santi     (1000)       37 2024-04-08 13:35:50.475167 GridCalEngine-5.1.2/setup.cfg
```

### Comparing `GridCalEngine-5.1.1/GridCalEngine/__version__.py` & `GridCalEngine-5.1.2/GridCalEngine/__version__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with GridCal.  If not, see <http://www.gnu.org/licenses/>.
 import datetime
 _current_year_ = datetime.datetime.now().year
 
 # do not forget to keep a three-number version!!!
-__GridCalEngine_VERSION__ = "5.1.1"
+__GridCalEngine_VERSION__ = "5.1.2"
 
 url = 'https://github.com/SanPen/GridCal'
 
 about_msg = "GridCal v" + str(__GridCalEngine_VERSION__) + '\n\n'
 
 about_msg += """
 GridCal has been carefully crafted since 2015 to
```

### Comparing `GridCalEngine-5.1.1/GridCalEngine/__init__.py` & `GridCalEngine-5.1.2/GridCalEngine/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/LICENSE.txt` & `GridCalEngine-5.1.2/GridCalEngine/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/data_logger.py` & `GridCalEngine-5.1.2/GridCalEngine/data_logger.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/enumerations.py` & `GridCalEngine-5.1.2/GridCalEngine/enumerations.py`

 * *Files 0% similar despite different names*

```diff
@@ -939,14 +939,16 @@
     FluidP2XDevice = 'Fluid P2X'
     FluidPathDevice = 'Fluid path'
     FluidNodeDevice = 'Fluid node'
 
     LineLocation = "Line Location"
     LineLocations = "Line Locations"
 
+    ModellingAuthority = "Modelling Authority"
+
     def __str__(self) -> str:
         return str(self.value)
 
     def __repr__(self):
         return str(self)
 
     @staticmethod
```

### Comparing `GridCalEngine-5.1.1/GridCalEngine/basic_structures.py` & `GridCalEngine-5.1.2/GridCalEngine/basic_structures.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/api.py` & `GridCalEngine-5.1.2/GridCalEngine/api.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,18 +18,18 @@
 from GridCalEngine.Simulations import *
 from GridCalEngine.IO import *
 from GridCalEngine.Devices import *
 from GridCalEngine.DataStructures.numerical_circuit import compile_numerical_circuit_at
 from GridCalEngine.enumerations import *
 
 
-def open_file(filename: str) -> MultiCircuit:
+def open_file(filename: Union[str, List[str]]) -> MultiCircuit:
     """
     Open file
-    :param filename: name of the file (.gridcal, .ejson, .m, etc.)
+    :param filename: name of the file (.gridcal, .ejson, .m, .xml, .zip, etc.) or list of files (.xml, .zip)
     :return: MultiCircuit instance
     """
     return FileOpen(file_name=filename).open()
 
 
 def save_file(grid: MultiCircuit, filename: str):
     """
```

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Utils/Filtering/objects_filtering.py` & `GridCalEngine-5.1.2/GridCalEngine/Utils/Filtering/objects_filtering.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Utils/Filtering/__init__.py` & `GridCalEngine-5.1.2/GridCalEngine/Utils/Filtering/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Utils/Filtering/timeseries_filtering.py` & `GridCalEngine-5.1.2/GridCalEngine/Utils/Filtering/timeseries_filtering.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Utils/Filtering/filtering.py` & `GridCalEngine-5.1.2/GridCalEngine/Utils/Filtering/filtering.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Utils/Filtering/results_table_filtering.py` & `GridCalEngine-5.1.2/GridCalEngine/Utils/Filtering/results_table_filtering.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Utils/NumericalMethods/common.py` & `GridCalEngine-5.1.2/GridCalEngine/Utils/NumericalMethods/common.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Utils/NumericalMethods/levenberg_marquadt.py` & `GridCalEngine-5.1.2/GridCalEngine/Utils/NumericalMethods/levenberg_marquadt.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Utils/NumericalMethods/ips.py` & `GridCalEngine-5.1.2/GridCalEngine/Utils/NumericalMethods/ips.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Utils/NumericalMethods/newton_raphson.py` & `GridCalEngine-5.1.2/GridCalEngine/Utils/NumericalMethods/newton_raphson.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Utils/NumericalMethods/weldorf_online_stddev.py` & `GridCalEngine-5.1.2/GridCalEngine/Utils/NumericalMethods/weldorf_online_stddev.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Utils/NumericalMethods/powell.py` & `GridCalEngine-5.1.2/GridCalEngine/Utils/NumericalMethods/powell.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Utils/NumericalMethods/autodiff.py` & `GridCalEngine-5.1.2/GridCalEngine/Utils/NumericalMethods/autodiff.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Utils/NumericalMethods/sparse_solve.py` & `GridCalEngine-5.1.2/GridCalEngine/Utils/NumericalMethods/sparse_solve.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Utils/Sparse/__init__.py` & `GridCalEngine-5.1.2/GridCalEngine/Utils/Sparse/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Utils/Sparse/csc_numba.py` & `GridCalEngine-5.1.2/GridCalEngine/Utils/Sparse/csc_numba.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Utils/Sparse/csc.py` & `GridCalEngine-5.1.2/GridCalEngine/Utils/Sparse/csc.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Utils/Sparse/utils.py` & `GridCalEngine-5.1.2/GridCalEngine/Utils/Sparse/utils.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Utils/ThirdParty/SyntheticNetworks/rpgm_algo.py` & `GridCalEngine-5.1.2/GridCalEngine/Utils/ThirdParty/SyntheticNetworks/rpgm_algo.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Utils/MIP/selected_interface.py` & `GridCalEngine-5.1.2/GridCalEngine/Utils/MIP/selected_interface.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Utils/MIP/ortools_interface.py` & `GridCalEngine-5.1.2/GridCalEngine/Utils/MIP/ortools_interface.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Utils/MIP/pulp_interface.py` & `GridCalEngine-5.1.2/GridCalEngine/Utils/MIP/pulp_interface.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Utils/MIP/SimpleMip/__init__.py` & `GridCalEngine-5.1.2/GridCalEngine/Utils/MIP/SimpleMip/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Utils/MIP/SimpleMip/lpobjects.py` & `GridCalEngine-5.1.2/GridCalEngine/Utils/MIP/SimpleMip/lpobjects.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Utils/MIP/SimpleMip/lpmodel.py` & `GridCalEngine-5.1.2/GridCalEngine/Utils/MIP/SimpleMip/lpmodel.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Utils/MIP/SimpleMip/highs.py` & `GridCalEngine-5.1.2/GridCalEngine/Utils/MIP/SimpleMip/highs.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Topology/topology.py` & `GridCalEngine-5.1.2/GridCalEngine/Topology/topology.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Topology/simulation_indices.py` & `GridCalEngine-5.1.2/GridCalEngine/Topology/simulation_indices.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Topology/topology_substation_reduction.py` & `GridCalEngine-5.1.2/GridCalEngine/Topology/topology_substation_reduction.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Topology/admittance_matrices.py` & `GridCalEngine-5.1.2/GridCalEngine/Topology/admittance_matrices.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/__init__.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/file_handler.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/file_handler.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,27 +14,27 @@
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 import os
 import json
 
 from collections.abc import Callable
-from typing import Union, List
+from typing import Union, List, Any, Dict
 
+from GridCalEngine.Simulations.driver_template import DriverTemplate
 from GridCalEngine.IO.cim.cgmes.cgmes_data_parser import CgmesDataParser
 from GridCalEngine.basic_structures import Logger
 from GridCalEngine.data_logger import DataLogger
 
 from GridCalEngine.IO.gridcal.json_parser import save_json_file_v3
 from GridCalEngine.IO.cim.cim16.cim_parser import CIMExport
 from GridCalEngine.IO.gridcal.excel_interface import save_excel, load_from_xls, interpret_excel_v3, interprete_excel_v2
 from GridCalEngine.IO.gridcal.pack_unpack import gather_model_as_data_frames, parse_gridcal_data, gather_model_as_jsons
-from GridCalEngine.IO.matpower.matpower_parser import interpret_data_v1
+from GridCalEngine.IO.matpower.matpower_parser import interpret_data_v1, parse_matpower_file
 from GridCalEngine.IO.dgs.dgs_parser import dgs_to_circuit
-from GridCalEngine.IO.matpower.matpower_parser import parse_matpower_file
 from GridCalEngine.IO.others.dpx_parser import load_dpx
 from GridCalEngine.IO.others.ipa_parser import load_iPA
 from GridCalEngine.IO.gridcal.json_parser import parse_json, parse_json_data_v2, parse_json_data_v3
 from GridCalEngine.IO.raw.raw_parser_writer import read_raw, write_raw
 from GridCalEngine.IO.raw.raw_to_gridcal import psse_to_gridcal
 from GridCalEngine.IO.raw.gridcal_to_raw import gridcal_to_raw
 from GridCalEngine.IO.epc.epc_parser import PowerWorldParser
@@ -45,14 +45,40 @@
 from GridCalEngine.IO.gridcal.sqlite_interface import save_data_frames_to_sqlite, open_data_frames_from_sqlite
 from GridCalEngine.IO.gridcal.h5_interface import save_h5, open_h5
 from GridCalEngine.IO.raw.rawx_parser_writer import parse_rawx, write_rawx
 from GridCalEngine.IO.others.pypsa_parser import parse_netcdf, parse_hdf5
 from GridCalEngine.Devices.multi_circuit import MultiCircuit
 
 
+class FileSavingOptions:
+    """
+    This class is to store the extra stuff that needs to be passed to save more complex files
+    """
+    def __init__(self,
+                 cgmes_boundary_set: str = "",
+                 simulation_drivers: List[DriverTemplate] = None,
+                 sessions: List[Any] = None,
+                 dictionary_of_json_files: Dict[str, Dict[str, Any]] = None):
+        """
+        Constructor
+        :param cgmes_boundary_set: CGMES boundary set zip file path
+        :param simulation_drivers: List of Simulation Drivers
+        :param sessions: List of sessions
+        :param dictionary_of_json_files: Dictionary of json files
+        """
+
+        self.cgmes_boundary_set: str = cgmes_boundary_set
+
+        self.simulation_drivers = simulation_drivers if simulation_drivers else list()
+
+        self.sessions = sessions if sessions else list()
+
+        self.dictionary_of_json_files = dictionary_of_json_files if dictionary_of_json_files else dict()
+
+
 class FileOpen:
     """
     File open interface
     """
 
     def __init__(self, file_name: Union[str, List[str]]):
         """
@@ -279,41 +305,39 @@
 
 
 class FileSave:
     """
     FileSave
     """
 
-    def __init__(self, circuit: MultiCircuit, file_name, text_func=None, progress_func=None,
-                 simulation_drivers=list(), sessions=list(), json_files=dict()):
+    def __init__(self,
+                 circuit: MultiCircuit,
+                 file_name: str,
+                 options: FileSavingOptions = FileSavingOptions(),
+                 text_func=None,
+                 progress_func=None):
         """
         File saver
         :param circuit: MultiCircuit
         :param file_name: file name to save to
+        :param options: FileSavingOptions
         :param text_func: Pointer to the text function
         :param progress_func: Pointer to the progress function
-        :param simulation_drivers: List of Simulation Drivers
-        :param sessions: List of sessions
-        :param json_files: Dictionary of json files
         """
         self.circuit = circuit
 
         self.file_name = file_name
 
-        self.simulation_drivers = simulation_drivers
-
-        self.sessions = sessions
-
-        self.json_files = json_files
+        self.options = options
 
         self.text_func = text_func
 
         self.progress_func = progress_func
 
-    def save(self):
+    def save(self) -> Logger:
         """
         Save the file in the corresponding format
         :return: logger with information
         """
         if self.file_name.endswith('.xlsx'):
             logger = self.save_excel()
 
@@ -356,15 +380,15 @@
         :return: logger with information
         """
 
         logger = save_excel(self.circuit, self.file_name)
 
         return logger
 
-    def save_zip(self):
+    def save_zip(self) -> Logger:
         """
         Save the circuit information in zip format
         :return: logger with information
         """
 
         logger = Logger()
 
@@ -372,17 +396,17 @@
                                           legacy=False)
 
         model_data = gather_model_as_jsons(self.circuit)
 
         save_gridcal_data_to_zip(dfs=dfs,
                                  filename_zip=self.file_name,
                                  model_data=model_data,
-                                 sessions=self.sessions,
+                                 sessions=self.options.sessions,
                                  diagrams=self.circuit.diagrams,
-                                 json_files=self.json_files,
+                                 json_files=self.options.dictionary_of_json_files,
                                  text_func=self.text_func,
                                  progress_func=self.progress_func,
                                  logger=logger)
 
         return logger
 
     def save_sqlite(self):
@@ -398,21 +422,23 @@
         save_data_frames_to_sqlite(dfs,
                                    file_path=self.file_name,
                                    text_func=self.text_func,
                                    progress_func=self.progress_func)
 
         return logger
 
-    def save_json_v3(self):
+    def save_json_v3(self) -> Logger:
         """
         Save the circuit information in json format
         :return:logger with information
         """
 
-        logger = save_json_file_v3(self.file_name, self.circuit, self.simulation_drivers)
+        logger = save_json_file_v3(self.file_name,
+                                   self.circuit,
+                                   self.options.simulation_drivers)
         return logger
 
     def save_cim(self):
         """
         Save the circuit information in CIM format
         :return: logger with information
         """
```

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/base/units.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/base/units.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/base/base_property.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/base/base_property.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/dgs/dgs_parser.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/dgs/dgs_parser.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/raw/raw_parser_legacy.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/raw/raw_parser_legacy.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/raw/raw_functions.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/raw/raw_functions.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/raw/rawx_parser_writer.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/raw/rawx_parser_writer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/raw/raw_parser_writer.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/raw/raw_parser_writer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/raw/raw_to_gridcal.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/raw/raw_to_gridcal.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/raw/rawx_parser_legacy.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/raw/rawx_parser_legacy.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/raw/devices/gne_device.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/raw/devices/gne_device.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/raw/devices/switched_shunt.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/raw/devices/switched_shunt.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/raw/devices/__init__.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/raw/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/raw/devices/system_switching_device.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/raw/devices/system_switching_device.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/raw/devices/psse_object.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/raw/devices/psse_object.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/raw/devices/transformer.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/raw/devices/transformer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/raw/devices/facts.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/raw/devices/facts.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/raw/devices/owner.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/raw/devices/owner.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/raw/devices/inter_area.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/raw/devices/inter_area.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/raw/devices/psse_property.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/raw/devices/psse_property.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/raw/devices/generator.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/raw/devices/generator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/raw/devices/two_terminal_dc_line.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/raw/devices/two_terminal_dc_line.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/raw/devices/psse_circuit.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/raw/devices/psse_circuit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/raw/devices/bus.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/raw/devices/bus.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/raw/devices/vsc_dc_line.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/raw/devices/vsc_dc_line.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/raw/devices/area.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/raw/devices/area.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/raw/devices/induction_machine.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/raw/devices/induction_machine.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/raw/devices/fixed_shunt.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/raw/devices/fixed_shunt.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/raw/devices/load.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/raw/devices/load.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/raw/devices/node.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/raw/devices/node.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/raw/devices/zone.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/raw/devices/zone.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/raw/devices/branch.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/raw/devices/branch.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/raw/devices/substation.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/raw/devices/substation.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/matpower/matpower_storage_definitions.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/matpower/matpower_storage_definitions.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/matpower/matpower_gen_definitions.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/matpower/matpower_gen_definitions.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/matpower/matpower_bus_definitions.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/matpower/matpower_bus_definitions.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/matpower/matpower_parser.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/matpower/matpower_parser.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/matpower/matpower_branch_definitions.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/matpower/matpower_branch_definitions.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/gridcal/pack_unpack.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/gridcal/pack_unpack.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,18 @@
     creates a dictionary with the types and the circuit objects
     :return: Dictionary instance
     """
 
     # this list must be sorted in dependency order so that the
     # loading algorithm is able to find the object substitutions
 
-    object_types = {'area': dev.Area(),
+    object_types = {
+                    'modelling_authority': dev.ModellingAuthority(),
+
+                    'area': dev.Area(),
                     'zone': dev.Zone(),
 
                     'substation': dev.Substation(),
 
                     'voltage_level': dev.VoltageLevel(),
 
                     'country': dev.Country(),
```

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/gridcal/zip_interface.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/gridcal/zip_interface.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/gridcal/json_parser.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/gridcal/json_parser.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/gridcal/generic_io_functions.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/gridcal/generic_io_functions.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/gridcal/h5_interface.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/gridcal/h5_interface.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/gridcal/excel_interface.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/gridcal/excel_interface.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/gridcal/sqlite_interface.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/gridcal/sqlite_interface.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/gridcal/contingency_parser.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/gridcal/contingency_parser.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/epc/epc_parser.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/epc/epc_parser.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/others/dpx_parser.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/others/dpx_parser.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/others/ipa_parser.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/others/ipa_parser.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/others/pypsa_parser.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/others/pypsa_parser.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/others/plx_parser.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/others/plx_parser.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_enums.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_enums.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_to_gridcal.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_to_gridcal.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from GridCalEngine.IO.cim.cgmes.cgmes_utils import (get_nominal_voltage,
                                                     get_pu_values_ac_line_segment,
                                                     get_values_shunt,
                                                     get_pu_values_power_transformer, get_pu_values_power_transformer3w,
                                                     get_windings,
                                                     get_regulating_control, get_pu_values_power_transformer_end,
                                                     get_slack_id)
-from GridCalEngine.IO.cim.cgmes.gridcal_to_cgmes import gridcal_to_cgmes    #TODO move them here
+from GridCalEngine.IO.cim.cgmes.gridcal_to_cgmes import gridcal_to_cgmes  # TODO move them here
 from GridCalEngine.data_logger import DataLogger
 from GridCalEngine.IO.cim.cgmes.cgmes_v2_4_15.devices.identified_object import IdentifiedObject
 from GridCalEngine.IO.cim.cgmes.cgmes_v2_4_15.devices.terminal import Terminal
 from GridCalEngine.IO.cim.cgmes.cgmes_v2_4_15.devices.ac_line_segment import ACLineSegment
 from GridCalEngine.IO.cim.cgmes.cgmes_v2_4_15.devices.switch import Switch
 from GridCalEngine.IO.cim.cgmes.cgmes_v2_4_15.devices.disconnector import Disconnector
 from GridCalEngine.IO.cim.cgmes.cgmes_v2_4_15.devices.load_break_switch import LoadBreakSwitch
@@ -158,15 +158,15 @@
         logger.add_error("No terminal for the device",
                          device=cgmes_elm.rdfid,
                          device_class=cgmes_elm.tpe)
 
     return calc_nodes, cns
 
 
-def find_object_by_idtag(object_list, target_idtag):  #TODO move to somewhere
+def find_object_by_idtag(object_list, target_idtag):  # TODO move to somewhere
     """
     Finds an object with the specified idtag
      in the given object_list from a Multi Circuit.
 
     Args:
         object_list (list[MyObject]): List of MyObject instances.
         target_idtag (str): The uuid to search for.
@@ -234,25 +234,24 @@
                               vnom=nominal_voltage,
                               vmin=0.9,
                               vmax=1.1,
                               active=True,
                               is_slack=is_slack,
                               is_dc=False,
                               # is_internal=False,
-                              area=None,    #TODO get tp area
-                              zone=None,    #TODO get tp zone
-                              substation=None,  #TODO
-                              voltage_level=volt_lev,   #TODO
-                              country=None,     #TODO
+                              area=None,  # TODO get tp area
+                              zone=None,  # TODO get tp zone
+                              substation=None,  # TODO
+                              voltage_level=volt_lev,  # TODO
+                              country=None,  # TODO
                               # latitude=0.0,
                               # longitude=0.0,
                               Vm0=vm,
                               Va0=va)
 
-
         gc_model.add_bus(gcdev_elm)
         calc_node_dict[gcdev_elm.idtag] = gcdev_elm
 
     return calc_node_dict
 
 
 def get_gcdev_connectivity_nodes(cgmes_model: CgmesCircuit,
@@ -326,16 +325,16 @@
                 cn = cns[0]
 
                 p, q, i_i, i_r, g, b = 0.0, 0.0, 0.0, 0.0, 0.0, 0.0
                 if cgmes_elm.LoadResponse is not None:
 
                     if cgmes_elm.LoadResponse.exponentModel:
                         print(f'Exponent model True at {cgmes_elm.name}')
-                        pass    #TODO convert exponent to ZIP
-                    else:       # ZIP model
+                        pass  # TODO convert exponent to ZIP
+                    else:  # ZIP model
                         # TODO check all attributes
                         p = cgmes_elm.p * cgmes_elm.LoadResponse.pConstantPower
                         q = cgmes_elm.q * cgmes_elm.LoadResponse.qConstantPower
                         i_r = cgmes_elm.p * cgmes_elm.LoadResponse.pConstantCurrent
                         i_i = cgmes_elm.q * cgmes_elm.LoadResponse.qConstantCurrent
 
                         # g = cgmes_elm.p / cgmes_elm.LoadResponse.pConstantImpedance  # TODO ask Chavdar
@@ -485,15 +484,15 @@
     :param calc_node_dict: Dict[str, gcdev.Bus]
     :param cn_dict: Dict[str, gcdev.ConnectivityNode]
     :param device_to_terminal_dict: Dict[str, Terminal]
     :param logger:
     """
     # convert loads
     for device_list in [cgmes_model.EquivalentInjection_list]:
-        #TODO ExternalNetworkInjection
+        # TODO ExternalNetworkInjection
         for cgmes_elm in device_list:
             calc_nodes, cns = find_connections(cgmes_elm=cgmes_elm,
                                                device_to_terminal_dict=device_to_terminal_dict,
                                                calc_node_dict=calc_node_dict,
                                                cn_dict=cn_dict,
                                                logger=logger)
 
@@ -624,15 +623,21 @@
     """
 
     # convert ac lines
     for device_list in [cgmes_model.PowerTransformer_list]:
 
         for cgmes_elm in device_list:
 
-            windings = get_windings(cgmes_elm)
+            windings = [None, None, None]
+            for pte in list(cgmes_elm.PowerTransformerEnd):
+                if hasattr(pte, "endNumber"):
+                    i = getattr(pte, "endNumber")
+                    windings[i - 1] = pte
+            windings = [x for x in windings if x is not None]
+            # windings = get_windings(cgmes_elm)
             # windings: List[PowerTransformerEnd] = list(cgmes_elm.references_to_me['PowerTransformerEnd'])
 
             if len(windings) == 2:
                 calc_nodes, cns = find_connections(cgmes_elm=cgmes_elm,
                                                    device_to_terminal_dict=device_to_terminal_dict,
                                                    calc_node_dict=calc_node_dict,
                                                    cn_dict=cn_dict,
@@ -759,17 +764,18 @@
                     gcdev_elm.winding3.X = x
                     gcdev_elm.winding3.G = g
                     gcdev_elm.winding3.B = b
                     gcdev_elm.winding3.R0 = r0
                     gcdev_elm.winding3.X0 = x0
                     gcdev_elm.winding3.G0 = g0
                     gcdev_elm.winding3.B0 = b0
-                    gcdev_model.add_transformer3w(gcdev_elm)
                     gcdev_elm.winding3.rate = windings[2].ratedS
 
+                    gcdev_model.add_transformer3w(gcdev_elm)
+
 
                 else:
                     logger.add_error(msg='Not exactly three terminals',
                                      device=cgmes_elm.rdfid,
                                      device_class=cgmes_elm.tpe,
                                      device_property="number of associated terminals",
                                      value=len(calc_nodes),
@@ -903,21 +909,22 @@
                 cn_t = cns[1]
 
                 operational_current_rate = rates_dict.get(cgmes_elm.uuid, None)  # A
                 if operational_current_rate and cgmes_elm.BaseVoltage is not None:
                     # rate in MVA = A / 1000 * kV * sqrt(3)    CORRECTED!
                     op_rate = np.round((operational_current_rate / 1000.0) *
                                        cgmes_elm.BaseVoltage.nominalVoltage * 1.73205080756888,
-                                    4)
+                                       4)
                 else:
                     op_rate = 9999  # Corrected
 
-                if cgmes_elm.ratedCurrent is not None and cgmes_elm.ratedCurrent != 0.0:   # TODO
-                    rated_current = np.round((cgmes_elm.ratedCurrent / 1000.0) * cgmes_elm.BaseVoltage.nominalVoltage * 1.73205080756888,
-                                    4)
+                if cgmes_elm.ratedCurrent is not None and cgmes_elm.ratedCurrent != 0.0:  # TODO
+                    rated_current = np.round(
+                        (cgmes_elm.ratedCurrent / 1000.0) * cgmes_elm.BaseVoltage.nominalVoltage * 1.73205080756888,
+                        4)
                 else:
                     rated_current = op_rate
 
                 gcdev_elm = gcdev.Switch(
                     idtag=cgmes_elm.uuid,
                     code=cgmes_elm.description,
                     name=cgmes_elm.name,
@@ -951,15 +958,14 @@
     :param cgmes_model: CgmesCircuit
     :param gcdev_model: gcdevCircuit
     """
     # convert substations
     for device_list in [cgmes_model.Substation_list]:
 
         for cgmes_elm in device_list:
-
             gcdev_elm = gcdev.Substation(
                 name=cgmes_elm.name,
                 idtag=cgmes_elm.uuid,
                 code=cgmes_elm.description,
                 # latitude=0.0,     # later from GL profile/Location class
                 # longitude=0.0
             )
```

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_poperty.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_poperty.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_data_parser.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_data_parser.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_writer.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_writer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/gridcal_to_cgmes.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/gridcal_to_cgmes.py`

 * *Files 21% similar despite different names*

```diff
@@ -59,14 +59,42 @@
         for obj in object_list:
             obj_attr = getattr(obj, target_attr_name)
             if obj_attr == target_value:
                 return obj
     return None
 
 
+def get_ohm_values_power_transformer(r, x, g, b, r0, x0, g0, b0, nominal_power, rated_voltage):
+    """
+    Get the transformer ohm values
+    :return:
+    """
+    try:
+        Sbase_system = 100
+        Zbase = (rated_voltage * rated_voltage) / nominal_power
+        Ybase = 1.0 / Zbase
+        R, X, G, B = 0, 0, 0, 0
+        R0, X0, G0, B0 = 0, 0, 0, 0
+        machine_to_sys = Sbase_system / nominal_power
+        R = r * Zbase / machine_to_sys
+        X = x * Zbase / machine_to_sys
+        G = g * Ybase / machine_to_sys
+        B = b * Ybase / machine_to_sys
+        R0 = r0 * Zbase / machine_to_sys if r0 is not None else 0
+        X0 = x0 * Zbase / machine_to_sys if x0 is not None else 0
+        G0 = g0 * Ybase / machine_to_sys if g0 is not None else 0
+        B0 = b0 * Ybase / machine_to_sys if b0 is not None else 0
+
+    except KeyError:
+        R, X, G, B = 0, 0, 0, 0
+        R0, X0, G0, B0 = 0, 0, 0, 0
+
+    return R, X, G, B, R0, X0, G0, B0
+
+
 # endregion
 
 # region create new classes for CC
 
 
 def create_cgmes_terminal(bus: Bus,
                           cgmes_model: CgmesCircuit,
@@ -95,15 +123,14 @@
 
     return term
 
 
 def create_cgmes_load_response_char(
         load: gcdev.Load,
         logger: DataLogger) -> cgmes.LoadResponseCharacteristic:
-
     new_rdf_id = get_new_rdfid()
     lrc = cgmes.LoadResponseCharacteristic(rdfid=new_rdf_id)
     # lrc.name =
     lrc.pConstantCurrent = load.Ir / load.P if load.P != 0.0 else 0
     lrc.qConstantCurrent = load.Ii / load.Q if load.Q != 0.0 else 0
     lrc.pConstantImpedance = load.G / load.P if load.P != 0.0 else 0
     lrc.qConstantImpedance = load.B / load.Q if load.Q != 0.0 else 0  # TODO ask Chavdar
@@ -264,15 +291,14 @@
 
         cgmes_model.VoltageLevel_list.append(vl)
 
 
 def get_cgmes_tn_nodes(multi_circuit_model: MultiCircuit,
                        cgmes_model: CgmesCircuit,
                        logger: DataLogger) -> None:
-
     for bus in multi_circuit_model.buses:
 
         tn = cgmes.TopologicalNode(rdfid=bus.idtag)
         tn.name = bus.name
         tn.BaseVoltage = find_object_by_vnom(
             object_list=cgmes_model.BaseVoltage_list,
             target_vnom=bus.Vnom
@@ -295,29 +321,28 @@
 
     return
 
 
 def get_cgmes_cn_nodes(multi_circuit_model: MultiCircuit,
                        cgmes_model: CgmesCircuit,
                        logger: DataLogger) -> None:
-
     for mc_elm in multi_circuit_model.connectivity_nodes:
 
         cn = cgmes.ConnectivityNode(rdfid=form_rdfid(mc_elm.idtag))
         cn.name = mc_elm.name
         tn = None
         if mc_elm.default_bus is not None:
             tn: cgmes.TopologicalNode = find_object_by_uuid(
                 object_list=cgmes_model.TopologicalNode_list,
                 target_uuid=mc_elm.default_bus.idtag
             )
             if tn is not None:
                 cn.TopologicalNode = tn
                 cn.ConnectivityNodeContainer = tn.ConnectivityNodeContainer
-                tn.ConnectivityNodes = cn    # link back
+                tn.ConnectivityNodes = cn  # link back
             else:
                 logger.add_error(msg='No TopologinalNode found',
                                  device=cn,
                                  device_class=cn.tpe)
         else:
             logger.add_error(msg='Connectivity Node has no default bus',
                              device=mc_elm,
@@ -436,15 +461,15 @@
         line = cgmes.ACLineSegment(rdfid=form_rdfid(mc_elm.idtag))
         line.description = mc_elm.code
         line.name = mc_elm.name
         line.BaseVoltage = find_object_by_attribute(
             object_list=cgmes_model.BaseVoltage_list,
             target_attr_name="nominalVoltage",
             target_value=mc_elm.get_max_bus_nominal_voltage()
-        ) # which Vnom we need?
+        )  # which Vnom we need?
         vnom = line.BaseVoltage.nominalVoltage
 
         if vnom is not None:
             # Calculate Zbase
             zbase = (vnom * vnom) / sbase
             ybase = 1.0 / zbase
 
@@ -459,21 +484,19 @@
 
         cgmes_model.ACLineSegment_list.append(line)
 
 
 def get_cgmes_operational_limits(multicircuit_model: MultiCircuit,
                                  cgmes_model: CgmesCircuit,
                                  logger: DataLogger):
-
     # OperationalLimitSet and OperationalLimitType
 
     pass
 
 
-
 def get_cgmes_current_limits(multicircuit_model: MultiCircuit,
                              cgmes_model: CgmesCircuit,
                              logger: DataLogger):
     pass
 
 
 def get_cgmes_generators(multicircuit_model: MultiCircuit,
@@ -504,40 +527,158 @@
 
         # Synchronous Machine
         cgmes_syn = cgmes.SynchronousMachine(rdfid=form_rdfid(mc_elm.idtag))
         cgmes_syn.description = mc_elm.code
         cgmes_syn.name = mc_elm.name
         # cgmes_syn.aggregate is optional, not exported
         # cgmes_syn.EquipmentContainer: VoltageLevel
-        #TODO implement control_node in MultiCircuit
+        # TODO implement control_node in MultiCircuit
         # has_control: do we have control
         # control_type: voltage or power control, ..
         # is_controlled: enabling flag (already have)
         if mc_elm.is_controlled:
             cgmes_syn.RegulatingControl = create_cgmes_regulating_control(cgmes_syn, cgmes_model)
             cgmes_syn.RegulatingControl.RegulatingCondEq = cgmes_syn
 
         # cgmes_syn.ratedPowerFactor =
         cgmes_syn.ratedS = mc_elm.Snom
-        cgmes_syn.GeneratingUnit = cgmes_gen   # linking them together
+        cgmes_syn.GeneratingUnit = cgmes_gen  # linking them together
         cgmes_gen.RotatingMachine = cgmes_syn  # linking them together
         cgmes_syn.maxQ = mc_elm.Qmax
         cgmes_syn.minQ = mc_elm.Qmin
         # ...
         cgmes_syn.referencePriority = '0'  # ?
 
         cgmes_model.SynchronousMachine_list.append(cgmes_syn)
 
 
-def get_cgmes_power_transformers():
-    pass
+def get_cgmes_power_transformers(multicircuit_model: MultiCircuit,
+                                 cgmes_model: CgmesCircuit,
+                                 logger: DataLogger):
+    for mc_elm in multicircuit_model.transformers2w:
+        cm_transformer = cgmes.PowerTransformer(rdfid=form_rdfid(mc_elm.idtag))
+        cm_transformer.uuid = mc_elm.idtag
+        cm_transformer.description = mc_elm.code
+        cm_transformer.name = mc_elm.name
+        cm_transformer.Terminals = [create_cgmes_terminal(mc_elm.bus_from, cgmes_model, logger),
+                                    create_cgmes_terminal(mc_elm.bus_to, cgmes_model, logger)]
+
+        cm_transformer.PowerTransformerEnd = []
+        pte1 = cgmes.PowerTransformerEnd()
+        pte1.PowerTransformer = cm_transformer
+        R, X, G, B, R0, X0, G0, B0 = (mc_elm.R, mc_elm.X, mc_elm.G, mc_elm.B, mc_elm.R0,
+                                      mc_elm.X0, mc_elm.G0, mc_elm.B0)
+        r, x, g, b, r0, x0, g0, b0 = get_ohm_values_power_transformer(R, X, G, B, R0, X0, G0, B0, mc_elm.Sn, mc_elm.HV)
+        pte1.r = r
+        pte1.x = x
+        pte1.g = g
+        pte1.b = b
+        pte1.r0 = r0
+        pte1.x0 = x0
+        pte1.g0 = g0
+        pte1.b0 = b0
+        pte1.ratedU = mc_elm.HV
+        pte1.ratedS = mc_elm.Sn
+        pte1.endNumber = 1
+
+        pte2 = cgmes.PowerTransformerEnd()
+        pte2.PowerTransformer = cm_transformer
+        pte2.r = 0
+        pte2.x = 0
+        pte2.g = 0
+        pte2.b = 0
+        pte2.r0 = 0
+        pte2.x0 = 0
+        pte2.g0 = 0
+        pte2.b0 = 0
+        pte2.ratedU = mc_elm.LV
+        pte2.ratedS = mc_elm.Sn
+        pte2.endNumber = 2
+
+        cm_transformer.PowerTransformerEnd.append(pte1)
+        cgmes_model.PowerTransformerEnd_list.append(pte1)
+        cm_transformer.PowerTransformerEnd.append(pte2)
+        cgmes_model.PowerTransformerEnd_list.append(pte2)
+
+        cgmes_model.PowerTransformer_list.append(cm_transformer)
+
+    for mc_elm in multicircuit_model.transformers3w:
+        cm_transformer = cgmes.PowerTransformer(rdfid=form_rdfid(mc_elm.idtag))
+        cm_transformer.uuid = mc_elm.idtag
+        cm_transformer.description = mc_elm.code
+        cm_transformer.name = mc_elm.name
+        cm_transformer.Terminals = [create_cgmes_terminal(mc_elm.bus1, cgmes_model, logger),
+                                    create_cgmes_terminal(mc_elm.bus2, cgmes_model, logger),
+                                    create_cgmes_terminal(mc_elm.bus3, cgmes_model, logger)]
+        cm_transformer.PowerTransformerEnd = []
+
+        pte1 = cgmes.PowerTransformerEnd()
+        pte1.PowerTransformer = cm_transformer
+        pte1.ratedU = mc_elm.V1
+        pte1.ratedS = mc_elm.rate12
+        pte1.endNumber = 1
+        R, X, G, B, R0, X0, G0, B0 = (mc_elm.winding1.R, mc_elm.winding1.X, mc_elm.winding1.G, mc_elm.winding1.B, mc_elm.winding1.R0,
+                                      mc_elm.winding1.X0, mc_elm.winding1.G0, mc_elm.winding1.B0)
+        r, x, g, b, r0, x0, g0, b0 = get_ohm_values_power_transformer(R, X, G, B, R0, X0, G0, B0, mc_elm.winding1.rate, mc_elm.winding1.HV)
+        pte1.r = r
+        pte1.x = x
+        pte1.g = g
+        pte1.b = b
+        pte1.r0 = r0
+        pte1.x0 = x0
+        pte1.g0 = g0
+        pte1.b0 = b0
+
+        pte2 = cgmes.PowerTransformerEnd()
+        pte2.PowerTransformer = cm_transformer
+        pte2.ratedU = mc_elm.V2
+        pte2.ratedS = mc_elm.rate23
+        pte2.endNumber = 2
+        R, X, G, B, R0, X0, G0, B0 = (
+        mc_elm.winding2.R, mc_elm.winding2.X, mc_elm.winding2.G, mc_elm.winding2.B, mc_elm.winding2.R0,
+        mc_elm.winding2.X0, mc_elm.winding2.G0, mc_elm.winding2.B0)
+        r, x, g, b, r0, x0, g0, b0 = get_ohm_values_power_transformer(R, X, G, B, R0, X0, G0, B0, mc_elm.winding2.rate,
+                                                                      mc_elm.winding2.HV)
+        pte2.r = r
+        pte2.x = x
+        pte2.g = g
+        pte2.b = b
+        pte2.r0 = r0
+        pte2.x0 = x0
+        pte2.g0 = g0
+        pte2.b0 = b0
+
+        pte3 = cgmes.PowerTransformerEnd()
+        pte3.PowerTransformer = cm_transformer
+        pte3.ratedU = mc_elm.V3
+        pte3.ratedS = mc_elm.rate31
+        pte3.endNumber = 3
+        R, X, G, B, R0, X0, G0, B0 = (
+        mc_elm.winding3.R, mc_elm.winding3.X, mc_elm.winding3.G, mc_elm.winding3.B, mc_elm.winding3.R0,
+        mc_elm.winding3.X0, mc_elm.winding3.G0, mc_elm.winding3.B0)
+        r, x, g, b, r0, x0, g0, b0 = get_ohm_values_power_transformer(R, X, G, B, R0, X0, G0, B0, mc_elm.winding3.rate,
+                                                                      mc_elm.winding3.HV)
+        pte3.r = r
+        pte3.x = x
+        pte3.g = g
+        pte3.b = b
+        pte3.r0 = r0
+        pte3.x0 = x0
+        pte3.g0 = g0
+        pte3.b0 = b0
+
+        cm_transformer.PowerTransformerEnd.append(pte1)
+        cgmes_model.PowerTransformerEnd_list.append(pte1)
+        cm_transformer.PowerTransformerEnd.append(pte2)
+        cgmes_model.PowerTransformerEnd_list.append(pte2)
+        cm_transformer.PowerTransformerEnd.append(pte3)
+        cgmes_model.PowerTransformerEnd_list.append(pte3)
 
+        cgmes_model.PowerTransformer_list.append(cm_transformer)
 
-def get_cgmes_power_transformer_ends():
-    pass
 
 # endregion
 
 
 def gridcal_to_cgmes(gc_model: MultiCircuit, logger: DataLogger) -> CgmesCircuit:
     """
     Converts the input Multi circuit to a new CGMES Circuit.
@@ -562,11 +703,11 @@
 
     get_cgmes_loads(gc_model, cgmes_model, logger)
     get_cgmes_equivalent_injections(gc_model, cgmes_model, logger)
     get_cgmes_generators(gc_model, cgmes_model, logger)
 
     get_cgmes_ac_line_segments(gc_model, cgmes_model, logger)
     # transformers, windings
-
+    get_cgmes_power_transformers(gc_model, cgmes_model, logger)
     # shunts
 
     return cgmes_model
```

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/base.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/base.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_export.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_export.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_utils.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,16 @@
 
 def get_pu_values_power_transformer(power_transformer: PowerTransformer, System_Sbase):
     """
     Get the transformer p.u. values
     :return:
     """
     try:
-        windings = get_windings(power_transformer)
+        # windings = get_windings(power_transformer)
+        windings = list(power_transformer.PowerTransformerEnd)
 
         R, X, G, B = 0, 0, 0, 0
         R0, X0, G0, B0 = 0, 0, 0, 0
         if len(windings) == 2:
             for winding in windings:
                 r, x, g, b, r0, x0, g0, b0 = get_pu_values_power_transformer_end(winding, System_Sbase)
                 R += r
@@ -99,15 +100,16 @@
 
 def get_pu_values_power_transformer3w(power_transformer: PowerTransformer, System_Sbase):
     """
     Get the transformer p.u. values
     :return:
     """
     try:
-        windings = get_windings(power_transformer)
+        # windings = get_windings(power_transformer)
+        windings = list(power_transformer.PowerTransformerEnd)
 
         r12, r23, r31, x12, x23, x31 = 0.0, 0.0, 0.0, 0.0, 0.0, 0.0
 
         if len(windings) == 3:
             r1, x1, g1, b1, r0_1, x0_1, g0_1, b0_1 = get_pu_values_power_transformer_end(windings[0], System_Sbase)
             r2, x2, g2, b2, r0_2, x0_2, g0_2, b0_2 = get_pu_values_power_transformer_end(windings[1], System_Sbase)
             r3, x3, g3, b3, r0_3, x0_3, g0_3, b0_3 = get_pu_values_power_transformer_end(windings[2], System_Sbase)
```

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_data_validator.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_data_validator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_circuit.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_circuit.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
 def find_attribute(referenced_object, obj, property_name, association_inverse_dict):
     for inverse, current in association_inverse_dict.items():
         c_class = str(current).split('.')[0]
         c_prop = str(current).split('.')[-1]
         if isinstance(obj, globals()[c_class]) and c_prop == property_name:
             i_class = str(inverse).split('.')[0]
             i_prop = str(inverse).split('.')[-1]
-            if isinstance(referenced_object, globals()[i_class]) and i_prop in referenced_object.get_all_properties():
+            if isinstance(referenced_object, globals()[i_class]) and i_prop in vars(referenced_object):
                 return i_prop
             else:
                 continue
         else:
             continue
     return None
```

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_switch.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_switch.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_non_linear.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_non_linear.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/connectivity_node.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/connectivity_node.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_equipment_container.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_equipment_container.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/identified_object.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/identified_object.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/control_area.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/control_area.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/location.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/location.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_chopper.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_chopper.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/season_day_type_schedule.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/season_day_type_schedule.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/asynchronous_machine.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/asynchronous_machine.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_injection.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_injection.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_line.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_line.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/caes_plant.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/caes_plant.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/solar_power_plant.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/solar_power_plant.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/curve.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/curve.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/regular_interval_schedule.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/regular_interval_schedule.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/work_location.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/work_location.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/breaker.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/breaker.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_topological_island.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_topological_island.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ratio_tap_changer_table_point.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ratio_tap_changer_table_point.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/surge_arrester.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/surge_arrester.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/battery_unit.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/battery_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/post_line_sensor.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/post_line_sensor.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/shunt_compensator.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/shunt_compensator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/nonlinear_shunt_compensator_point.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/nonlinear_shunt_compensator_point.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_branch.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_branch.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/active_power_limit.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/active_power_limit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/fuse.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/fuse.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/nonlinear_shunt_compensator.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/nonlinear_shunt_compensator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_series_device.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_series_device.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tap_changer_table_point.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tap_changer_table_point.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_system_resource.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_system_resource.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/disconnecting_circuit_breaker.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/disconnecting_circuit_breaker.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_shunt.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_shunt.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/vs_converter.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/vs_converter.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/external_network_injection.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/external_network_injection.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_electronics_connection.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_electronics_connection.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/current_transformer.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/current_transformer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_voltage.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_voltage.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_node.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_node.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_connection.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_connection.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_tap_step.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_tap_step.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/voltage_level.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/voltage_level.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_consumer.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_consumer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/current_limit.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/current_limit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/fault_indicator.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/fault_indicator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ratio_tap_changer.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ratio_tap_changer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/grounding_impedance.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/grounding_impedance.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_ground.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_ground.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/acdc_converter.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/acdc_converter.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/disconnector.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/disconnector.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_transformer_end.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_transformer_end.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_busbar.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_busbar.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/operational_limit.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/operational_limit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/nuclear_generating_unit.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/nuclear_generating_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_scheduling_type.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_scheduling_type.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tap_changer_control.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tap_changer_control.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_transformer.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_transformer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/auxiliary_equipment.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/auxiliary_equipment.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/curve_data.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/curve_data.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/petersen_coil.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/petersen_coil.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/wave_trap.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/wave_trap.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_table.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_table.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ac_line_segment.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ac_line_segment.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_table_point.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_table_point.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_symmetrical.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_symmetrical.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/base_voltage.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/base_voltage.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/transformer_end.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/transformer_end.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/voltage_limit.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/voltage_limit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_network.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_network.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/jumper.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/jumper.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/acdc_terminal.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/acdc_terminal.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_terminal.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_terminal.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_breaker.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_breaker.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/switch.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/switch.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equipment.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equipment.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/topological_node.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/topological_node.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/operational_limit_type.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/operational_limit_type.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/reporting_group.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/reporting_group.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/linear_shunt_compensator.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/linear_shunt_compensator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_source.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_source.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_line_segment.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_line_segment.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conductor.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conductor.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/thermal_generating_unit.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/thermal_generating_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/junction.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/junction.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_equipment.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equivalent_equipment.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sub_geographical_region.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sub_geographical_region.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/cogeneration_plant.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/cogeneration_plant.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_injection.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_injection.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/boundary_point.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/boundary_point.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_response_characteristic.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_response_characteristic.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_converter_unit.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_converter_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/bay.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/bay.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/wind_generating_unit.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/wind_generating_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sub_load_area.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sub_load_area.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_electronics_unit.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_electronics_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/hydro_generating_unit.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/hydro_generating_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conducting_equipment.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conducting_equipment.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/geographical_region.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/geographical_region.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/non_conform_load.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/non_conform_load.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/synchronous_machine.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/synchronous_machine.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/line.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/line.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_group.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_group.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_shunt.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_shunt.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_topological_node.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_topological_node.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_area.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_area.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/control_area_generating_unit.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/control_area_generating_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equipment_container.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/equipment_container.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/topological_island.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/topological_island.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/potential_transformer.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/potential_transformer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_shunt_compensator_sections.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_shunt_compensator_sections.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_tabular.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_tabular.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sensor.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sensor.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/cs_converter.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/cs_converter.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conform_load_group.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conform_load_group.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/wind_power_plant.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/wind_power_plant.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/rotating_machine.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/rotating_machine.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_electronics_wind_unit.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/power_electronics_wind_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_area.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/energy_area.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/reactive_capability_curve.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/reactive_capability_curve.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/hydro_pump.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/hydro_pump.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/protected_switch.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/protected_switch.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_linear.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_linear.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/acdc_converterdc_terminal.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/acdc_converterdc_terminal.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tap_changer.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tap_changer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_switch.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_switch.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/non_conform_load_group.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/non_conform_load_group.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_status.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_status.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_break_switch.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/load_break_switch.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/bus_name_marker.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/bus_name_marker.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/solar_generating_unit.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/solar_generating_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/fossil_fuel.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/fossil_fuel.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/earth_fault_compensator.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/earth_fault_compensator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/operational_limit_set.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/operational_limit_set.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/hydro_power_plant.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/hydro_power_plant.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/generating_unit.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/generating_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/service_location.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/service_location.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/terminal.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/terminal.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_asymmetrical.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/phase_tap_changer_asymmetrical.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/combined_cycle_plant.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/combined_cycle_plant.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/busbar_section.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/busbar_section.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_disconnector.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_disconnector.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/connector.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/connector.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/coordinate_system.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/coordinate_system.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_base_terminal.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_base_terminal.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/static_var_compensator.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/static_var_compensator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/apparent_power_limit.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/apparent_power_limit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conform_load.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/conform_load.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/series_compensator.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/series_compensator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/connectivity_node_container.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/connectivity_node_container.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/substation.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/substation.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/position_point.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/position_point.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/clamp.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/clamp.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tie_flow.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/tie_flow.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/basic_interval_schedule.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/basic_interval_schedule.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/cut.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/cut.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ground_disconnector.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ground_disconnector.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ratio_tap_changer_table.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ratio_tap_changer_table.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_conducting_equipment.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/dc_conducting_equipment.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/vs_capability_curve.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/vs_capability_curve.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/photo_voltaic_unit.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/photo_voltaic_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ground.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/ground.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/regulating_control.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/regulating_control.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_power_flow.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v3_0_0/devices/sv_power_flow.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_switch.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_switch.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_non_linear.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_non_linear.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/connectivity_node.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/connectivity_node.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_equipment_container.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_equipment_container.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/identified_object.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/identified_object.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/control_area.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/control_area.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/location.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/location.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_chopper.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_chopper.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/season_day_type_schedule.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/season_day_type_schedule.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/asynchronous_machine.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/asynchronous_machine.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_injection.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_injection.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_line.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_line.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/curve.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/curve.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/regular_interval_schedule.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/regular_interval_schedule.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/breaker.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/breaker.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_topological_island.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_topological_island.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ratio_tap_changer_table_point.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ratio_tap_changer_table_point.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/shunt_compensator.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/shunt_compensator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/nonlinear_shunt_compensator_point.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/nonlinear_shunt_compensator_point.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_branch.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_branch.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/active_power_limit.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/active_power_limit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/nonlinear_shunt_compensator.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/nonlinear_shunt_compensator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_series_device.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_series_device.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tap_changer_table_point.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tap_changer_table_point.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/power_system_resource.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/power_system_resource.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_shunt.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_shunt.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/vs_converter.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/vs_converter.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/external_network_injection.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/external_network_injection.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_voltage.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_voltage.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_node.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_node.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/__init__.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,7 +15,9 @@
 from GridCalEngine.IO.cim.cgmes.cgmes_v2_4_15.devices.solar_generating_unit import SolarGeneratingUnit
 from GridCalEngine.IO.cim.cgmes.cgmes_v2_4_15.devices.wind_generating_unit import WindGeneratingUnit
 from GridCalEngine.IO.cim.cgmes.cgmes_v2_4_15.devices.nuclear_generating_unit import NuclearGeneratingUnit
 from GridCalEngine.IO.cim.cgmes.cgmes_v2_4_15.devices.synchronous_machine import SynchronousMachine
 from GridCalEngine.IO.cim.cgmes.cgmes_v2_4_15.devices.ac_line_segment import ACLineSegment
 from GridCalEngine.IO.cim.cgmes.cgmes_v2_4_15.devices.regulating_cond_eq import RegulatingCondEq
 from GridCalEngine.IO.cim.cgmes.cgmes_v2_4_15.devices.regulating_control import RegulatingControl
+from GridCalEngine.IO.cim.cgmes.cgmes_v2_4_15.devices.power_transformer import PowerTransformer
+from GridCalEngine.IO.cim.cgmes.cgmes_v2_4_15.devices.power_transformer_end import PowerTransformerEnd
```

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_tap_step.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_tap_step.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/voltage_level.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/voltage_level.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_consumer.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_consumer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/current_limit.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/current_limit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ratio_tap_changer.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ratio_tap_changer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/grounding_impedance.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/grounding_impedance.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_ground.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_ground.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/acdc_converter.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/acdc_converter.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/disconnector.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/disconnector.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/power_transformer_end.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/power_transformer_end.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_busbar.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_busbar.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/operational_limit.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/operational_limit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/nuclear_generating_unit.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/nuclear_generating_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_scheduling_type.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_scheduling_type.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tap_changer_control.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tap_changer_control.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/power_transformer.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/power_transformer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/curve_data.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/curve_data.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/petersen_coil.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/petersen_coil.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_table.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_table.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ac_line_segment.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ac_line_segment.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_table_point.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_table_point.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_symmetrical.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_symmetrical.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/base_voltage.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/base_voltage.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/transformer_end.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/transformer_end.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/voltage_limit.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/voltage_limit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_network.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_network.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/measurement_value.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/measurement_value.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/acdc_terminal.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/acdc_terminal.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_terminal.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_terminal.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_breaker.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_breaker.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/switch.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/switch.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equipment.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equipment.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/quality61850.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/quality61850.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/topological_node.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/topological_node.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/operational_limit_type.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/operational_limit_type.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/reporting_group.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/reporting_group.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/linear_shunt_compensator.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/linear_shunt_compensator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_source.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_source.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_line_segment.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_line_segment.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/limit_set.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/limit_set.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conductor.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conductor.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/thermal_generating_unit.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/thermal_generating_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/full_model.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/full_model.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/junction.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/junction.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_equipment.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equivalent_equipment.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sub_geographical_region.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sub_geographical_region.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_injection.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_injection.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_response_characteristic.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_response_characteristic.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_converter_unit.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_converter_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/bay.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/bay.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/wind_generating_unit.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/wind_generating_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/limit.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/limit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sub_load_area.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sub_load_area.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/hydro_generating_unit.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/hydro_generating_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conducting_equipment.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conducting_equipment.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/geographical_region.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/geographical_region.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/non_conform_load.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/non_conform_load.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/synchronous_machine.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/synchronous_machine.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/line.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/line.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_group.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_group.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_shunt.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_shunt.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_topological_node.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_topological_node.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_area.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_area.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/control_area_generating_unit.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/control_area_generating_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equipment_container.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/equipment_container.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/per_lengthdc_line_parameter.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/per_lengthdc_line_parameter.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/measurement.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/measurement.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/topological_island.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/topological_island.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_shunt_compensator_sections.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_shunt_compensator_sections.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_tabular.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_tabular.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/cs_converter.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/cs_converter.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conform_load_group.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conform_load_group.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/rotating_machine.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/rotating_machine.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_area.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/energy_area.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/reactive_capability_curve.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/reactive_capability_curve.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/hydro_pump.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/hydro_pump.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/protected_switch.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/protected_switch.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_linear.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_linear.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/acdc_converterdc_terminal.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/acdc_converterdc_terminal.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tap_changer.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tap_changer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/non_conform_load_group.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/non_conform_load_group.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_status.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_status.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_break_switch.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/load_break_switch.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/bus_name_marker.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/bus_name_marker.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/solar_generating_unit.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/solar_generating_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/fossil_fuel.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/fossil_fuel.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/earth_fault_compensator.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/earth_fault_compensator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/operational_limit_set.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/operational_limit_set.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/hydro_power_plant.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/hydro_power_plant.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/generating_unit.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/generating_unit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/terminal.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/terminal.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_asymmetrical.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/phase_tap_changer_asymmetrical.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/busbar_section.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/busbar_section.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_disconnector.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_disconnector.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/connector.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/connector.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/coordinate_system.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/coordinate_system.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_base_terminal.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_base_terminal.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/static_var_compensator.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/static_var_compensator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/apparent_power_limit.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/apparent_power_limit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conform_load.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/conform_load.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/series_compensator.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/series_compensator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/connectivity_node_container.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/connectivity_node_container.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/substation.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/substation.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/position_point.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/position_point.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tie_flow.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/tie_flow.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/basic_interval_schedule.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/basic_interval_schedule.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/mutual_coupling.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/mutual_coupling.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ground_disconnector.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ground_disconnector.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ratio_tap_changer_table.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ratio_tap_changer_table.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/regulating_cond_eq.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/regulating_cond_eq.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_conducting_equipment.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/dc_conducting_equipment.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/analog_control.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/analog_control.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/vs_capability_curve.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/vs_capability_curve.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/control.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/control.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ground.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/ground.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/regulating_control.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/regulating_control.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_power_flow.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cgmes/cgmes_v2_4_15/devices/sv_power_flow.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cim16/cim_circuit.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cim16/cim_circuit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cim16/cim_devices.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cim16/cim_devices.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cim16/cim_enums.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cim16/cim_enums.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cim16/cim_parser.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cim16/cim_parser.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/cim16/cim_data_parser.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/cim16/cim_data_parser.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/db/base_db.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/db/base_db.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/db/cgmes_lookup_db.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/db/cgmes_lookup_db.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/db/file_system.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/db/file_system.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/db/psse_lookup_db.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/db/psse_lookup_db.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/IO/cim/db/db_handler.py` & `GridCalEngine-5.1.2/GridCalEngine/IO/cim/db/db_handler.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/types.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,9 +98,18 @@
     TransformerType,
     EmissionGas,
     GeneratorEmission,
     GeneratorFuel,
     GeneratorTechnology,
     BranchGroup,
     LineLocations,
-    LineLocation
+    LineLocation,
+    ModellingAuthority,
+    Fuel,
+    Investment,
+    InvestmentsGroup,
+    Contingency,
+    ContingencyGroup,
+    Technology,
+    UndergroundLineType,
+    SequenceLineType
 ]
```

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/sparse_array.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/sparse_array.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/__init__.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/multi_circuit.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/multi_circuit.py`

 * *Files 1% similar despite different names*

```diff
@@ -312,14 +312,17 @@
 
         # investments group
         self.investments_groups: List[dev.InvestmentsGroup] = list()
 
         # technologies
         self.technologies: List[dev.Technology] = list()
 
+        # Modelling authority
+        self.modelling_authorities: List[dev.ModellingAuthority] = list()
+
         # fuels
         self.fuels: List[dev.Fuel] = list()
 
         # emission gasses
         self.emission_gases: List[dev.EmissionGas] = list()
 
         self.generators_technologies: List[dev.GeneratorTechnology] = list()
@@ -390,14 +393,15 @@
             ],
             "Groups": [
                 dev.ContingencyGroup(),
                 dev.Contingency(),
                 dev.InvestmentsGroup(),
                 dev.Investment(),
                 dev.BranchGroup(),
+                dev.ModellingAuthority()
             ],
             "Tags & Associations": [
                 dev.Technology(),
                 dev.Fuel(),
                 dev.EmissionGas(),
                 dev.GeneratorTechnology(),
                 dev.GeneratorFuel(),
@@ -1751,15 +1755,66 @@
         """
         Add a BranchGroup object
         :param obj: BranchGroup instance
         """
 
         self.branch_groups.remove(obj)
 
-    def get_elements_by_type(self, device_type: DeviceType):
+    # ------------------------------------------------------------------------------------------------------------------
+    # modelling_authority
+    # ------------------------------------------------------------------------------------------------------------------
+
+    def get_modelling_authorities(self) -> List[dev.ModellingAuthority]:
+        """
+        List of modelling_authorities
+        :return: List[dev.ModellingAuthority]
+        """
+        return self.modelling_authorities
+
+    def get_modelling_authorities_number(self) -> int:
+        """
+        Size of the list of modelling_authorities
+        :return: size of modelling_authorities
+        """
+        return len(self.modelling_authorities)
+
+    def get_modelling_authority_at(self, i: int) -> dev.ModellingAuthority:
+        """
+        Get modelling_authority at i
+        :param i: index
+        :return: ModellingAuthority
+        """
+        return self.modelling_authorities[i]
+
+    def get_modelling_authority_names(self) -> StrVec:
+        """
+        Array of modelling_authority names
+        :return: StrVec
+        """
+        return np.array([e.name for e in self.modelling_authorities])
+
+    def add_modelling_authority(self, obj: dev.ModellingAuthority):
+        """
+        Add a ModellingAuthority object
+        :param obj: ModellingAuthority instance
+        """
+
+        if self.time_profile is not None:
+            obj.create_profiles(self.time_profile)
+        self.modelling_authorities.append(obj)
+
+    def delete_modelling_authority(self, obj: dev.ModellingAuthority) -> None:
+        """
+        Add a ModellingAuthority object
+        :param obj: ModellingAuthority instance
+        """
+
+        self.modelling_authorities.remove(obj)
+
+    def get_elements_by_type(self, device_type: DeviceType) -> List[ALL_DEV_TYPES]:
         """
         Get set of elements and their parent nodes
         :param device_type: DeviceTYpe instance
         :return: List of elements, it raises an exception if the elements are unknown
         """
 
         if device_type == DeviceType.LoadDevice:
@@ -1941,14 +1996,17 @@
 
         elif device_type == DeviceType.NoDevice:
             return list()
 
         elif device_type == DeviceType.TimeDevice:
             return self.get_time_array()
 
+        elif device_type == DeviceType.ModellingAuthority:
+            return self.get_modelling_authorities()
+
         else:
             raise Exception('Element type not understood ' + str(device_type))
 
     def set_elements_by_type(self, device_type: DeviceType,
                              devices: List[ALL_DEV_TYPES],
                              logger: Logger = Logger()):
         """
@@ -2132,14 +2190,17 @@
 
         elif device_type == DeviceType.VmMeasurementDevice:
             self.vm_measurements = devices
 
         elif device_type == DeviceType.IfMeasurementDevice:
             self.if_measurements = devices
 
+        elif device_type == DeviceType.ModellingAuthority:
+            self.modelling_authorities = devices
+
         else:
             raise Exception('Element type not understood ' + str(device_type))
 
     def delete_elements_by_type(self, obj: ALL_DEV_TYPES):
         """
         Get set of elements and their parent nodes
         :param obj: device object to delete
@@ -2309,14 +2370,17 @@
 
         elif element_type == DeviceType.VmMeasurementDevice:
             return self.delete_vm_measurement(obj)
 
         elif element_type == DeviceType.IfMeasurementDevice:
             return self.delete_if_measurement(obj)
 
+        elif element_type == DeviceType.ModellingAuthority:
+            return self.delete_modelling_authority(obj)
+
         else:
             raise Exception('Element type not understood ' + str(element_type))
 
     def get_all_elements_dict(self) -> dict[str, ALL_DEV_TYPES]:
         """
         Get a dictionary of all elements
         :return: Dict[idtag] -> object
@@ -2414,66 +2478,30 @@
                 'fluid_paths',
                 'pi_measurements',
                 'qi_measurements',
                 'vm_measurements',
                 'pf_measurements',
                 'qf_measurements',
                 'if_measurements',
+                'modelling_authorities'
                 ]
 
         for pr in ppts:
             setattr(cpy, pr, copy.deepcopy(getattr(self, pr)))
 
         return cpy
 
     def clear(self) -> None:
         """
         Clear the multi-circuit (remove the bus and branch objects)
         """
 
-        for lst in self.get_branch_lists():
-            lst.clear()
-
-        for lst in self.get_injection_devices_lists():
-            lst.clear()
-
-        self.areas = list()
-        self.technologies = list()
-        self.contingencies = list()
-        self.contingency_groups = list()
-        self.investments = list()
-        self.investments_groups = list()
-        self.fuels = list()
-        self.emission_gases = list()
-
-        # Should accept buses
-        self.buses = list()
-        self.voltage_levels = list()
-        self.substations = list()
-
-        # List of overhead line objects
-        self.overhead_line_types = list()
-
-        # list of wire types
-        self.wire_types = list()
-
-        # underground cable lines
-        self.underground_cable_types = list()
-
-        # sequence modelled lines
-        self.sequence_line_types = list()
-
-        # List of transformer types
-        self.transformer_types = list()
-
-        self.time_profile = None
-
-        self.contingencies = list()
-
-        self.branch_groups = list()
+        for key, elm_list in self.objects_with_profiles.items():
+            for elm in elm_list:
+                self.get_elements_by_type(device_type=elm.device_type).clear()
 
     def get_catalogue_dict(self, branches_only=False):
         """
         Returns a dictionary with the catalogue types and the associated list of objects.
 
         Arguments:
```

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/measurement.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/measurement.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/profile.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/profile.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Aggregation/municipality.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Aggregation/municipality.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Aggregation/contingency_group.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Aggregation/contingency_group.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Aggregation/__init__.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Aggregation/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,7 +25,8 @@
 from GridCalEngine.Devices.Aggregation.area import Area
 from GridCalEngine.Devices.Aggregation.zone import Zone
 from GridCalEngine.Devices.Aggregation.country import Country
 from GridCalEngine.Devices.Aggregation.community import Community
 from GridCalEngine.Devices.Aggregation.region import Region
 from GridCalEngine.Devices.Aggregation.municipality import Municipality
 from GridCalEngine.Devices.Aggregation.branch_group import BranchGroup
+from GridCalEngine.Devices.Aggregation.modelling_authority import ModellingAuthority
```

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Aggregation/fuel.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Aggregation/fuel.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Aggregation/contingency.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Aggregation/contingency.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Aggregation/emission_gas.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Aggregation/emission_gas.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Aggregation/country.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Aggregation/country.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Aggregation/region.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Aggregation/region.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Aggregation/area.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Aggregation/area.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Aggregation/technology.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Aggregation/technology.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Aggregation/zone.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Aggregation/zone.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Aggregation/investments_group.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Aggregation/investments_group.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Aggregation/investment.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Aggregation/investment.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Aggregation/community.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Aggregation/community.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Aggregation/branch_group.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Aggregation/branch_group.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Fluid/__init__.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Fluid/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Fluid/fluid_path.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Fluid/fluid_path.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Fluid/fluid_pump.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Fluid/fluid_pump.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Fluid/fluid_node.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Fluid/fluid_node.py`

 * *Files 26% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 
     def __init__(self,
                  name: str = '',
                  idtag: Union[str, None] = None,
                  code: str = '',
                  min_level: float = 0.0,
                  max_level: float = 0.0,
+                 min_soc: float = 0.0,
+                 max_soc: float = 1.0,
                  current_level: float = 0.0,
                  spillage_cost: float = 1000.0,
                  inflow: float = 0.0,
                  bus: Union[None, Bus] = None,
                  build_status: BuildStatus = BuildStatus.Commissioned):
         """
         FluidNode
@@ -54,29 +56,42 @@
                                 name=name,
                                 idtag=idtag,
                                 code=code,
                                 device_type=DeviceType.FluidNodeDevice)
 
         self.min_level = min_level  # hm3
         self.max_level = max_level  # hm3
+        self.max_soc = max_soc  # p.u.
+        self.min_soc = min_soc  # p.u.
         self.initial_level = current_level  # hm3
         self.spillage_cost = spillage_cost  # m3/s
         self.inflow = inflow  # m3/s
         self._bus: Bus = bus
         self.build_status = build_status
 
         self._inflow_prof = Profile(default_value=inflow)  # m3/s
         self._spillage_cost_prof = Profile(default_value=spillage_cost)  # e/(m3/s)
 
+        self._max_soc_prof = Profile(default_value=max_soc)  # p.u.
+        self._min_soc_prof = Profile(default_value=min_soc)  # p.u.
+
         self.register(key='min_level', units='hm3', tpe=float,
                       definition="Minimum amount of fluid at the node/reservoir")
 
         self.register(key='max_level', units='hm3', tpe=float,
                       definition="Maximum amount of fluid at the node/reservoir")
 
+        self.register(key='min_soc', units='p.u.', tpe=float,
+                      definition="Minimum SOC of fluid at the node/reservoir",
+                      profile_name='min_soc_prof')
+
+        self.register(key='max_soc', units='p.u.', tpe=float,
+                      definition="Maximum SOC of fluid at the node/reservoir",
+                      profile_name='max_soc_prof')
+
         self.register(key='initial_level', units='hm3', tpe=float,
                       definition="Initial level of the node/reservoir")
 
         self.register(key='bus', units='', tpe=DeviceType.BusDevice,
                       definition='Electrical bus.', editable=False)
 
         self.register(key='build_status', units='', tpe=BuildStatus,
@@ -120,33 +135,71 @@
         if isinstance(val, Profile):
             self._inflow_prof = val
         elif isinstance(val, np.ndarray):
             self._inflow_prof.set(arr=val)
         else:
             raise Exception(str(type(val)) + 'not supported to be set into a inflow_prof')
 
+    @property
+    def max_soc_prof(self) -> Profile:
+        """
+        Max soc profile
+        :return: Profile
+        """
+        return self._max_soc_prof
+
+    @max_soc_prof.setter
+    def max_soc_prof(self, val: Union[Profile, np.ndarray]):
+        if isinstance(val, Profile):
+            self._max_soc_prof = val
+        elif isinstance(val, np.ndarray):
+            self._max_soc_prof.set(arr=val)
+        else:
+            raise Exception(str(type(val)) + 'not supported to be set into a max soc prof')
+
+    @property
+    def min_soc_prof(self) -> Profile:
+        """
+        Min soc profile
+        :return: Profile
+        """
+        return self._min_soc_prof
+
+    @min_soc_prof.setter
+    def min_soc_prof(self, val: Union[Profile, np.ndarray]):
+        if isinstance(val, Profile):
+            self._min_soc_prof = val
+        elif isinstance(val, np.ndarray):
+            self._min_soc_prof.set(arr=val)
+        else:
+            raise Exception(str(type(val)) + 'not supported to be set into a min soc prof')
+
     def copy(self):
         """
         Make a deep copy of this object
         :return: Copy of this object
         """
 
         # make a new instance (separated object in memory)
         fluid_node = FluidNode()
 
         fluid_node.min_level = self.min_level  # hm3
         fluid_node.max_level = self.max_level  # hm3
+        fluid_node.min_soc = self.min_soc  # p.u.
+        fluid_node.max_soc = self.max_soc  # p.u.
         fluid_node.initial_level = self.initial_level  # hm3
         fluid_node.spillage_cost = self.spillage_cost  # m3/s
         fluid_node.inflow = self.inflow  # m3/s
         fluid_node._bus = self._bus
         fluid_node.build_status = self.build_status
 
         fluid_node.inflow_prof = self.inflow_prof  # m3/s
         fluid_node.spillage_cost_prof = self.spillage_cost_prof  # e/(m3/s)
+        fluid_node.max_soc_prof = self.max_soc_prof  # m3
+        fluid_node.min_soc_prof = self.min_soc_prof  # m3
 
         return fluid_node
 
     @property
     def bus(self) -> Bus:
         """
         Bus getter function
```

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Fluid/fluid_turbine.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Fluid/fluid_turbine.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Fluid/fluid_injection_template.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Fluid/fluid_injection_template.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Fluid/fluid_p2x.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Fluid/fluid_p2x.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Branches/dc_line.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Branches/dc_line.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Branches/underground_line_type.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Branches/underground_line_type.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Branches/__init__.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Branches/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Branches/series_reactance.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Branches/series_reactance.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Branches/wire.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Branches/wire.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Branches/line_locations.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Branches/line_locations.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Branches/sequence_line_type.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Branches/sequence_line_type.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Branches/overhead_line_type.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Branches/overhead_line_type.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Branches/switch.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Branches/switch.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Branches/vsc.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Branches/vsc.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Branches/upfc.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Branches/upfc.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Branches/transformer.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Branches/transformer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Branches/hvdc_line.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Branches/hvdc_line.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Branches/line.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Branches/line.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Branches/tap_changer.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Branches/tap_changer.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Branches/winding.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Branches/winding.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Branches/branch.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Branches/branch.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Branches/transformer_type.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Branches/transformer_type.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Branches/transformer3w.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Branches/transformer3w.py`

 * *Files 4% similar despite different names*

```diff
@@ -167,41 +167,47 @@
         """
         return self._bus1
 
     @bus1.setter
     def bus1(self, obj: Bus):
         self._bus1 = obj
         self.winding1.bus_to = obj
-        self.winding1.set_hv_and_lv(self.winding1.HV, self.winding1.LV)
+
+        if obj is not None:
+            self.winding1.set_hv_and_lv(self.winding1.HV, self.winding1.LV)
 
     @property
     def bus2(self) -> Bus:
         """
         Bus 2
         """
         return self._bus2
 
     @bus2.setter
     def bus2(self, obj: Bus):
         self._bus2 = obj
         self.winding2.bus_to = obj
-        self.winding2.set_hv_and_lv(self.winding2.HV, self.winding2.LV)
+
+        if obj is not None:
+            self.winding2.set_hv_and_lv(self.winding2.HV, self.winding2.LV)
 
     @property
     def bus3(self) -> Bus:
         """
         Bus 3
         """
         return self._bus3
 
     @bus3.setter
     def bus3(self, obj: Bus):
         self._bus3 = obj
         self.winding3.bus_to = obj
-        self.winding3.set_hv_and_lv(self.winding3.HV, self.winding3.LV)
+
+        if obj is not None:
+            self.winding3.set_hv_and_lv(self.winding3.HV, self.winding3.LV)
 
     @property
     def V1(self) -> float:
         """
         Nominal voltage 1 in kV
         """
         return self._V1
```

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Injections/static_generator.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Injections/static_generator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Injections/shunt.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Injections/shunt.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Injections/__init__.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Injections/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Injections/external_grid.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Injections/external_grid.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Injections/current_injection.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Injections/current_injection.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Injections/battery.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Injections/battery.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Injections/generator.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Injections/generator.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Injections/generator_q_curve.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Injections/generator_q_curve.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Injections/controllable_shunt.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Injections/controllable_shunt.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Injections/load.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Injections/load.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Diagrams/graphic_location.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Diagrams/graphic_location.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Diagrams/map_diagram.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Diagrams/map_diagram.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Diagrams/node_breaker_diagram.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Diagrams/node_breaker_diagram.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Diagrams/__init__.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Diagrams/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Diagrams/bus_branch_diagram.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Diagrams/bus_branch_diagram.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Diagrams/map_location.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Diagrams/map_location.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Diagrams/base_diagram.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Diagrams/base_diagram.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Substation/connectivity_node.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Substation/connectivity_node.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Substation/__init__.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Substation/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Substation/voltage_level.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Substation/voltage_level.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Substation/bus.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Substation/bus.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Substation/busbar.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Substation/busbar.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Substation/substation.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Substation/substation.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Parents/injection_parent.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Parents/injection_parent.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Parents/editable_device.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Parents/editable_device.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Parents/generator_parent.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Parents/generator_parent.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Parents/__init__.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Parents/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Parents/controllable_branch_parent.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Parents/controllable_branch_parent.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Parents/load_parent.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Parents/load_parent.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Parents/branch_parent.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Parents/branch_parent.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Parents/shunt_parent.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Parents/shunt_parent.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Associations/generator_emission.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Associations/generator_emission.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Associations/__init__.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Associations/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Associations/generator_technology.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Associations/generator_technology.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Devices/Associations/generator_fuel.py` & `GridCalEngine-5.1.2/GridCalEngine/Devices/Associations/generator_fuel.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/DataStructures/load_data.py` & `GridCalEngine-5.1.2/GridCalEngine/DataStructures/load_data.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/DataStructures/bus_data.py` & `GridCalEngine-5.1.2/GridCalEngine/DataStructures/bus_data.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/DataStructures/branch_data.py` & `GridCalEngine-5.1.2/GridCalEngine/DataStructures/branch_data.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/DataStructures/__init__.py` & `GridCalEngine-5.1.2/GridCalEngine/DataStructures/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/DataStructures/fluid_turbine_data.py` & `GridCalEngine-5.1.2/GridCalEngine/DataStructures/fluid_turbine_data.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/DataStructures/fluid_p2x_data.py` & `GridCalEngine-5.1.2/GridCalEngine/DataStructures/fluid_p2x_data.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/DataStructures/numerical_circuit.py` & `GridCalEngine-5.1.2/GridCalEngine/DataStructures/numerical_circuit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/DataStructures/generator_data.py` & `GridCalEngine-5.1.2/GridCalEngine/DataStructures/generator_data.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/DataStructures/fluid_pump_data.py` & `GridCalEngine-5.1.2/GridCalEngine/DataStructures/fluid_pump_data.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/DataStructures/battery_data.py` & `GridCalEngine-5.1.2/GridCalEngine/DataStructures/battery_data.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/DataStructures/fluid_path_data.py` & `GridCalEngine-5.1.2/GridCalEngine/DataStructures/fluid_path_data.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/DataStructures/hvdc_data.py` & `GridCalEngine-5.1.2/GridCalEngine/DataStructures/hvdc_data.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/DataStructures/shunt_data.py` & `GridCalEngine-5.1.2/GridCalEngine/DataStructures/shunt_data.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/DataStructures/fluid_node_data.py` & `GridCalEngine-5.1.2/GridCalEngine/DataStructures/fluid_node_data.py`

 * *Files 18% similar despite different names*

```diff
@@ -31,16 +31,17 @@
         self.nelm: int = nelm
 
         self.names: StrVec = np.empty(nelm, dtype=object)
         self.idtag: StrVec = np.empty(nelm, dtype=object)
 
         self.min_level = np.zeros(nelm, dtype=float)
         self.max_level = np.zeros(nelm, dtype=float)
+        self.min_soc = np.zeros(nelm, dtype=float)
+        self.max_soc = np.zeros(nelm, dtype=float)
         self.initial_level = np.zeros(nelm, dtype=float)
-        # self.bus_index = np.empty()  # TODO: check if relevant
         self.inflow = np.zeros(nelm, dtype=float)
         self.spillage_cost = np.zeros(nelm, dtype=float)
 
     def size(self) -> int:
         """
         Get size of the structure
         :return:
@@ -57,14 +58,16 @@
         data = FluidNodeData(nelm=self.nelm)
 
         data.names = self.names.copy()
         data.idtag = self.idtag.copy()
 
         data.min_level = self.min_level.copy()
         data.max_level = self.max_level.copy()
+        data.min_soc = self.min_soc.copy()
+        data.max_soc = self.max_soc.copy()
         data.initial_level = self.initial_level.copy()
 
         data.inflow = self.inflow.copy()
         data.spillage_cost = self.spillage_cost.copy()
 
         return data
```

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Compilers/circuit_to_newton_pa.py` & `GridCalEngine-5.1.2/GridCalEngine/Compilers/circuit_to_newton_pa.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Compilers/circuit_to_bentayga.py` & `GridCalEngine-5.1.2/GridCalEngine/Compilers/circuit_to_bentayga.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Compilers/__init__.py` & `GridCalEngine-5.1.2/GridCalEngine/Compilers/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Compilers/circuit_to_data.py` & `GridCalEngine-5.1.2/GridCalEngine/Compilers/circuit_to_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1224,17 +1224,21 @@
         data.min_level[k] = 1e6 * elm.min_level
         data.max_level[k] = 1e6 * elm.max_level
         data.initial_level[k] = 1e6 * elm.initial_level
 
         if time_series:
             data.inflow[k] = elm.inflow_prof[t_idx]
             data.spillage_cost[k] = elm.spillage_cost_prof[t_idx]
+            data.max_soc[k] = elm.max_soc_prof[t_idx]
+            data.min_soc[k] = elm.min_soc_prof[t_idx]
         else:
             data.inflow[k] = elm.inflow
             data.spillage_cost[k] = elm.spillage_cost
+            data.max_soc[k] = elm.max_soc
+            data.min_soc[k] = elm.min_soc
 
     return data, plant_dict
 
 
 def get_fluid_turbine_data(circuit: MultiCircuit,
                            plant_dict: Dict[str, int],
                            gen_dict: Dict[str, int],
```

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Compilers/circuit_to_optimods.py` & `GridCalEngine-5.1.2/GridCalEngine/Compilers/circuit_to_optimods.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Compilers/circuit_to_pgm.py` & `GridCalEngine-5.1.2/GridCalEngine/Compilers/circuit_to_pgm.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/results_template.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/results_template.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/__init__.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/results_table.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/results_table.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/driver_types.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/driver_types.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/driver_template.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/driver_template.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/InvestmentsEvaluation/investments_evaluation_driver.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/InvestmentsEvaluation/investments_evaluation_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/InvestmentsEvaluation/investments_evaluation_results.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/InvestmentsEvaluation/investments_evaluation_results.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/InvestmentsEvaluation/investments_evaluation_options.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/InvestmentsEvaluation/investments_evaluation_options.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/stop_crits.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/stop_crits.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/MVRSM_mo_pareto.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/MVRSM_mo_pareto.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/MVRSM_mo_scaled.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/MVRSM_mo_scaled.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/MVRSM_original.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/InvestmentsEvaluation/NumericalMethods/MVRSM_original.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/Topology/__init__.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/Topology/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/Topology/topology_reduction_driver.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/Topology/topology_reduction_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/Topology/topology_processor_driver.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/Topology/topology_processor_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/Topology/node_groups_driver.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/Topology/node_groups_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/Stochastic/reliability_driver.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/Stochastic/reliability_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/Stochastic/stochastic_power_flow_input.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/Stochastic/stochastic_power_flow_input.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/Stochastic/__init__.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/Stochastic/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/Stochastic/stochastic_power_flow_results.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/Stochastic/stochastic_power_flow_results.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/Stochastic/reliability_iterable.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/Stochastic/reliability_iterable.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/Stochastic/blackout_driver.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/Stochastic/blackout_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/Stochastic/stochastic_power_flow_driver.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/Stochastic/stochastic_power_flow_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/Stochastic/latin_hypercube_sampling.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/Stochastic/latin_hypercube_sampling.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/PowerFlow/power_flow_ts_results.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/PowerFlow/power_flow_ts_results.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/PowerFlow/power_flow_ts_driver.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/PowerFlow/power_flow_ts_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/PowerFlow/power_flow_results.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/PowerFlow/power_flow_results.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/PowerFlow/power_flow_driver.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/PowerFlow/power_flow_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/PowerFlow/__init__.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/PowerFlow/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/PowerFlow/power_flow_ts_input.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/PowerFlow/power_flow_ts_input.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/PowerFlow/grid_analysis.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/PowerFlow/grid_analysis.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/PowerFlow/power_flow_options.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/PowerFlow/power_flow_options.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/PowerFlow/power_flow_worker.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/PowerFlow/power_flow_worker.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/PowerFlow/NumericalMethods/common_functions.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/PowerFlow/NumericalMethods/common_functions.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/PowerFlow/NumericalMethods/__init__.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/PowerFlow/NumericalMethods/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/PowerFlow/NumericalMethods/acdc_jacobian.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/PowerFlow/NumericalMethods/acdc_jacobian.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_acdc.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_acdc.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/PowerFlow/NumericalMethods/iwamoto_newton_raphson.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/PowerFlow/NumericalMethods/iwamoto_newton_raphson.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/PowerFlow/NumericalMethods/levenberg_marquardt_acdc.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/PowerFlow/NumericalMethods/levenberg_marquardt_acdc.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/PowerFlow/NumericalMethods/derivatives.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/PowerFlow/NumericalMethods/derivatives.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/PowerFlow/NumericalMethods/levenberg_marquardt.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/PowerFlow/NumericalMethods/levenberg_marquardt.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/PowerFlow/NumericalMethods/fast_decoupled.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/PowerFlow/NumericalMethods/fast_decoupled.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/PowerFlow/NumericalMethods/helm_power_flow.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/PowerFlow/NumericalMethods/helm_power_flow.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_decoupled.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_decoupled.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/PowerFlow/NumericalMethods/gauss_power_flow.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/PowerFlow/NumericalMethods/gauss_power_flow.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/PowerFlow/NumericalMethods/linearized_power_flow.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/PowerFlow/NumericalMethods/linearized_power_flow.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_ode.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_ode.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/PowerFlow/NumericalMethods/ac_jacobian.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/PowerFlow/NumericalMethods/ac_jacobian.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/PowerFlow/NumericalMethods/discrete_controls.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/PowerFlow/NumericalMethods/discrete_controls.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_current.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/PowerFlow/NumericalMethods/newton_raphson_current.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/InputsAnalysis/inputs_analysis_driver.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/InputsAnalysis/inputs_analysis_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/Dynamics/transient_stability_driver.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/Dynamics/transient_stability_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/Dynamics/dynamic_modules.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/Dynamics/dynamic_modules.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/ContinuationPowerFlow/__init__.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/ContinuationPowerFlow/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_driver.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_input.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_input.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow.py`

 * *Files 2% similar despite different names*

```diff
@@ -293,16 +293,23 @@
     dP_dV, dP_dlam = cpf_p_jac(parametrization, z, V, lam, Vprv, lamprv, pv, pq, pvpq)
 
     # linear operator for computing the tangent predictor
     '''
     J2 = [   J   dF_dlam
            dP_dV dP_dlam ]
     '''
-    J2 = sp.vstack([sp.hstack([J, dF_dlam.reshape(nj, 1)]),
-                    sp.hstack([dP_dV, dP_dlam])], format="csc")
+
+    last_col = np.empty((nj, 1))
+    last_col[:, 0] = dF_dlam
+
+    last_row = np.empty((1, nj + 1))
+    last_row[0, :nj] = dP_dV
+    last_row[0, nj] = dP_dlam
+
+    J2 = sp.vstack([sp.hstack([J, last_col], format="csc"), last_row], format="csc")
 
     Va_prev = np.angle(V)
     Vm_prev = np.abs(V)
 
     # compute normalized tangent predictor
     s = np.zeros(npv + 2 * npq + 1)
 
@@ -420,16 +427,25 @@
         dP_dV, dP_dlam = cpf_p_jac(parametrization, z, V, lam, Vprv, lamprv, pv, pq, pvpq)
 
         # augment J with real/imag - Sxfr and z^T
         '''
         J = [   J   dF_dlam 
               dP_dV dP_dlam ]
         '''
-        J = sp.vstack([sp.hstack([J, dF_dlam.reshape(nj, 1)]),
-                       sp.hstack([dP_dV, dP_dlam])], format="csc")
+        # J = sp.vstack([sp.hstack([J, dF_dlam.reshape(nj, 1)]),
+        #                sp.hstack([dP_dV, dP_dlam])], format="csc")
+
+        last_col = np.empty((nj, 1))
+        last_col[:, 0] = dF_dlam
+
+        last_row = np.empty((1, nj + 1))
+        last_row[0, :nj] = dP_dV
+        last_row[0, nj] = dP_dlam
+
+        J = sp.vstack([sp.hstack([J, last_col], format="csc"), last_row], format="csc")
 
         # compute update step
         dx = linear_solver(J, F)
         dVa[pvpq] = dx[j1:j2]
         dVm[pq] = dx[j2:j3]
         dlam = dx[j3]
 
@@ -732,15 +748,15 @@
             elif stop_at == CpfStopAt.ExtraOverloads:
                 # look for overloads and determine if there are more overloads than in the base situation
                 idx = np.where(np.abs(loading) > 1)[0]
                 if len(idx) > base_overload_number:
                     continuation = False
 
             else:
-                raise Exception('Stop point ' + stop_at.value + ' not recognised.')
+                raise Exception(f'Stop point {stop_at.value} not recognised.')
 
             if adapt_step and continuation:
 
                 # Adapt step size
                 fx = np.r_[np.angle(V[pq]), np.abs(V[pvpq]), lam] - np.r_[np.angle(V0[pq]), np.abs(V0[pvpq]), lam0]
                 cpf_error = np.linalg.norm(fx, np.Inf)
```

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_options.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_options.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_results.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/ContinuationPowerFlow/continuation_power_flow_results.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit_driver.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/ShortCircuitStudies/__init__.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/ShortCircuitStudies/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit_results.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit_results.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit_worker.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/ShortCircuitStudies/short_circuit_worker.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/NTC/ntc_results.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/NTC/ntc_results.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/NTC/ntc_ts_results.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/NTC/ntc_ts_results.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/NTC/ntc_ts_driver.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/NTC/ntc_ts_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/NTC/ntc_opf.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/NTC/ntc_opf.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/NTC/ntc_driver.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/NTC/ntc_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/NTC/ntc_options.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/NTC/ntc_options.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_ts_results.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_ts_results.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_results.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_results.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/ContingencyAnalysis/__init__.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/ContingencyAnalysis/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_driver.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_options.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_options.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/ContingencyAnalysis/contingencies_report.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/ContingencyAnalysis/contingencies_report.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_ts_driver.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/ContingencyAnalysis/contingency_analysis_ts_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/ContingencyAnalysis/contingency_plan.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/ContingencyAnalysis/contingency_plan.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/ContingencyAnalysis/Methods/srap.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/ContingencyAnalysis/Methods/srap.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/ContingencyAnalysis/Methods/optimal_linear_contingency_analysis.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/ContingencyAnalysis/Methods/optimal_linear_contingency_analysis.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/ContingencyAnalysis/Methods/linear_contingency_analysis.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/ContingencyAnalysis/Methods/linear_contingency_analysis.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/ContingencyAnalysis/Methods/nonlinear_contingency_analysis.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/ContingencyAnalysis/Methods/nonlinear_contingency_analysis.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/ContingencyAnalysis/Methods/helm_contingency_analysis.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/ContingencyAnalysis/Methods/helm_contingency_analysis.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/ContingencyAnalysis/Methods/helm_contingencies.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/ContingencyAnalysis/Methods/helm_contingencies.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/Clustering/clustering.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/Clustering/clustering.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/Clustering/__init__.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/Clustering/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/Clustering/clustering_results.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/Clustering/clustering_results.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/Clustering/clustering_options.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/Clustering/clustering_options.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/Clustering/clustering_driver.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/Clustering/clustering_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/StateEstimation/state_stimation_driver.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/StateEstimation/state_stimation_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/StateEstimation/state_estimation.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/StateEstimation/state_estimation.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/OPF/opf_driver.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/OPF/opf_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/OPF/__init__.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/OPF/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/OPF/opf_ts_driver.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/OPF/opf_ts_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/OPF/opf_ts_results.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/OPF/opf_ts_results.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/OPF/opf_results.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/OPF/opf_results.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/OPF/simple_dispatch_ts.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/OPF/simple_dispatch_ts.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/OPF/linear_opf_ts.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/OPF/linear_opf_ts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1314,18 +1314,27 @@
         node_vars.spillage[t, m] = prob.add_var(lb=0.00,
                                                 ub=1e20,
                                                 name=join("NodeSpillage_", [t, m], "_"))
 
         f_obj += node_data.spillage_cost[m] * node_vars.spillage[t, m]
         # f_obj += node_vars.spillage[t, m]
 
-        node_vars.current_level[t, m] = prob.add_var(lb=node_data.min_level[m],
-                                                     ub=node_data.max_level[m],
+        min_abs_level = node_data.max_level[m] * node_data.min_soc[m]
+
+        node_vars.current_level[t, m] = prob.add_var(lb=min_abs_level,
+                                                     ub=node_data.max_level[m] * node_data.max_soc[m],
                                                      name=join("level_", [t, m], "_"))
 
+        if min_abs_level < node_data.min_level[m]:
+            logger.add_error(msg='Node SOC is below the allowed minimum level',
+                             value=min_abs_level,
+                             expected_value=node_data.min_level[m],
+                             device_class="FluidNode",
+                             device_property=f"Min SOC at {t}")
+
     for m in range(path_data.nelm):
         path_vars.flow[t, m] = prob.add_var(lb=path_data.min_flow[m],
                                             ub=path_data.max_flow[m],
                                             name=join("hflow_", [t, m], "_"))
 
     # Constraints
     for m in range(path_data.nelm):
@@ -1393,15 +1402,15 @@
 
         if generator_data.pmax[gen_idx] > 0:
             logger.add_error(msg='P2X generator pmax > 0 is not possible',
                              value=generator_data.pmax[gen_idx])
 
         # f_obj -= p2x_flow
 
-    if t is not None:
+    if time_global_tidx is not None:
         # constraints for the node level
         for m in range(node_data.nelm):
             if t == 0:
                 # Initialize level at the initial one (from snapshot), akin to dt=0
                 if len(time_array) > time_global_tidx + 1:
                     dt = (time_array[time_global_tidx + 1] - time_array[time_global_tidx]).seconds
                 else:
```

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/OPF/opf_options.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/OPF/opf_options.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/OPF/NumericalMethods/ac_opf.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/OPF/NumericalMethods/ac_opf.py`

 * *Files 1% similar despite different names*

```diff
@@ -552,16 +552,16 @@
     f_disp_hvdc = nc.hvdc_data.F[hvdc_disp_idx]
     t_disp_hvdc = nc.hvdc_data.T[hvdc_disp_idx]
     P_hvdc_max = nc.hvdc_data.rate[hvdc_disp_idx]
 
     if use_bound_slacks:
         nsl = 2 * npq + 2 * n_br_mon
         # Slack relaxations for constraints
-        c_s = nc.branch_data.overload_cost[br_mon_idx] + 1e-9
-        c_v = nc.bus_data.cost_v[pq] + 1e-9
+        c_s = 0.0000001 * nc.branch_data.overload_cost[br_mon_idx] + 1e-9
+        c_v = 1000 * nc.bus_data.cost_v[pq] + 1e-9
         sl_sf0 = np.ones(n_br_mon)
         sl_st0 = np.ones(n_br_mon)
         sl_vmax0 = np.ones(npq)
         sl_vmin0 = np.ones(npq)
 
     else:
         nsl = 0
```

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/OPF/NumericalMethods/ac_opf_autodif.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/OPF/NumericalMethods/ac_opf_autodif.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/OPF/NumericalMethods/ac_opf_derivatives.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/OPF/NumericalMethods/ac_opf_derivatives.py`

 * *Files 1% similar despite different names*

```diff
@@ -921,16 +921,20 @@
             Htapml = lil_matrix((ntapm, NV))
             Htaptu = lil_matrix((ntapt, NV))
             Htaptl = lil_matrix((ntapt, NV))
 
             SfX = sp.hstack([Sfva, Sfvm, lil_matrix((M, 2 * Ng + nsl + ndc))])
             StX = sp.hstack([Stva, Stvm, lil_matrix((M, 2 * Ng + nsl + ndc))])
 
-            HSf = 2 * (Sfmat.real @ SfX.real + Sfmat.imag @ SfX.imag)
-            HSt = 2 * (Stmat.real @ StX.real + Stmat.imag @ StX.imag)
+            if use_bound_slacks:
+                HSf = 2 * (Sfmat.real @ SfX.real + Sfmat.imag @ SfX.imag) + Hslsf
+                HSt = 2 * (Stmat.real @ StX.real + Stmat.imag @ StX.imag) + Hslst
+            else:
+                HSf = 2 * (Sfmat.real @ SfX.real + Sfmat.imag @ SfX.imag)
+                HSt = 2 * (Stmat.real @ StX.real + Stmat.imag @ StX.imag)
 
         if ctQ != ReactivePowerControlMode.NoControl:
             # tanmax curves (simplified capability curves of generators)
             Hqmaxp = - 2 * np.power(tanmax, 2) * Pg
             Hqmaxq = 2 * Qg
 
             Hqmax = sp.hstack([lil_matrix((nqct, 2 * N)), diags(Hqmaxp), diags(Hqmaxq),
```

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/ATC/available_transfer_capacity_ts_driver.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/ATC/available_transfer_capacity_ts_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/ATC/__init__.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/ATC/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/ATC/available_transfer_capacity_driver.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/ATC/available_transfer_capacity_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/SigmaAnalysis/sigma_analysis_driver.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/SigmaAnalysis/sigma_analysis_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/LinearFactors/__init__.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/LinearFactors/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/LinearFactors/linear_analysis_driver.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/LinearFactors/linear_analysis_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/LinearFactors/linear_analysis.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/LinearFactors/linear_analysis.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/LinearFactors/linear_analysis_ts_results.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/LinearFactors/linear_analysis_ts_results.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/LinearFactors/linear_analysis_results.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/LinearFactors/linear_analysis_results.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/LinearFactors/linear_analysis_options.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/LinearFactors/linear_analysis_options.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/GridCalEngine/Simulations/LinearFactors/linear_analysis_ts_driver.py` & `GridCalEngine-5.1.2/GridCalEngine/Simulations/LinearFactors/linear_analysis_ts_driver.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/setup.py` & `GridCalEngine-5.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `GridCalEngine-5.1.1/PKG-INFO` & `GridCalEngine-5.1.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GridCalEngine
-Version: 5.1.1
+Version: 5.1.2
 Summary: GridCal is a Power Systems simulation program intended for professional use and research
 Home-page: https://github.com/SanPen/GridCal
 Author: Santiago Peñate Vera et. Al.
 Author-email: santiago@gridcal.org
 License: LGPL
 Keywords: power systems planning
 Classifier:  License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
```

