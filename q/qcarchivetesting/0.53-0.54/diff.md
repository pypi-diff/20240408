# Comparing `tmp/qcarchivetesting-0.53.tar.gz` & `tmp/qcarchivetesting-0.54.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qcarchivetesting-0.53.tar", last modified: Tue Jan  9 21:45:41 2024, max compression
+gzip compressed data, was "qcarchivetesting-0.54.tar", last modified: Mon Apr  8 18:04:27 2024, max compression
```

## Comparing `qcarchivetesting-0.53.tar` & `qcarchivetesting-0.54.tar`

### file list

```diff
@@ -1,173 +1,173 @@
-drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-01-09 21:45:41.903555 qcarchivetesting-0.53/
--rw-r--r--   0 ben       (1000) users      (984)      679 2024-01-09 21:45:41.903555 qcarchivetesting-0.53/PKG-INFO
-drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-01-09 21:45:41.893555 qcarchivetesting-0.53/conda-envs/
--rw-r--r--   0 ben       (1000) users      (984)      366 2023-12-17 03:36:39.000000 qcarchivetesting-0.53/conda-envs/fulltest_qcportal.yaml
--rw-r--r--   0 ben       (1000) users      (984)      699 2023-12-17 03:36:39.000000 qcarchivetesting-0.53/conda-envs/fulltest_server.yaml
--rw-r--r--   0 ben       (1000) users      (984)      874 2023-12-17 03:36:39.000000 qcarchivetesting-0.53/conda-envs/fulltest_snowflake.yaml
--rw-r--r--   0 ben       (1000) users      (984)     1178 2023-12-05 16:08:13.000000 qcarchivetesting-0.53/pyproject.toml
-drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-01-09 21:45:41.896889 qcarchivetesting-0.53/qcarchivetesting/
--rw-r--r--   0 ben       (1000) users      (984)      416 2023-09-20 13:55:23.000000 qcarchivetesting-0.53/qcarchivetesting/__init__.py
-drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-01-09 21:45:41.896889 qcarchivetesting-0.53/qcarchivetesting/config_files/
--rw-r--r--   0 ben       (1000) users      (984)      342 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/config_files/gha_fractal_compute.yaml
--rw-r--r--   0 ben       (1000) users      (984)      517 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/config_files/gha_fractal_oldcompute_dask.yaml
--rw-r--r--   0 ben       (1000) users      (984)      518 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/config_files/gha_fractal_oldcompute_parsl.yaml
--rw-r--r--   0 ben       (1000) users      (984)      465 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/config_files/gha_fractal_oldcompute_pool.yaml
--rw-r--r--   0 ben       (1000) users      (984)      429 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/config_files/gha_fractal_server.yaml
--rw-r--r--   0 ben       (1000) users      (984)      288 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/config_files/qcf_basic.yaml
--rw-r--r--   0 ben       (1000) users      (984)     3752 2023-12-05 16:08:13.000000 qcarchivetesting-0.53/qcarchivetesting/data_generator.py
-drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-01-09 21:45:41.896889 qcarchivetesting-0.53/qcarchivetesting/hash_data/
--rw-r--r--   0 ben       (1000) users      (984)    16240 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/hash_data/dict_hash_test_data.json.xz
--rw-r--r--   0 ben       (1000) users      (984)     1682 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/hash_data/generate_random.py
--rw-r--r--   0 ben       (1000) users      (984)     5617 2023-12-05 16:08:13.000000 qcarchivetesting-0.53/qcarchivetesting/helpers.py
-drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-01-09 21:45:41.896889 qcarchivetesting-0.53/qcarchivetesting/migration_data/
--rw-r--r--   0 ben       (1000) users      (984)    77051 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/migration_data/empty_v0.15.8.sql_dump
--rw-r--r--   0 ben       (1000) users      (984)      541 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/migration_data/qcfractal_config_v0.15.8.yaml
-drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-01-09 21:45:41.896889 qcarchivetesting-0.53/qcarchivetesting/molecule_data/
--rw-r--r--   0 ben       (1000) users      (984)     3468 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/benzene_dimer.json
--rw-r--r--   0 ben       (1000) users      (984)     1684 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/go_C4H4N2OS.json
--rw-r--r--   0 ben       (1000) users      (984)     1851 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/go_C6H5N3.json
--rw-r--r--   0 ben       (1000) users      (984)     1056 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/go_H3NS.json
--rw-r--r--   0 ben       (1000) users      (984)      383 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/hooh.json
-drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-01-09 21:45:41.900222 qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/
--rw-r--r--   0 ben       (1000) users      (984)     1055 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C3H2N_0.json
--rw-r--r--   0 ben       (1000) users      (984)     1055 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C3H2N_1.json
--rw-r--r--   0 ben       (1000) users      (984)     1056 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C3H2N_10.json
--rw-r--r--   0 ben       (1000) users      (984)     1055 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C3H2N_11.json
--rw-r--r--   0 ben       (1000) users      (984)     1053 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C3H2N_12.json
--rw-r--r--   0 ben       (1000) users      (984)     1056 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C3H2N_13.json
--rw-r--r--   0 ben       (1000) users      (984)     1055 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C3H2N_14.json
--rw-r--r--   0 ben       (1000) users      (984)     1052 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C3H2N_15.json
--rw-r--r--   0 ben       (1000) users      (984)     1056 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C3H2N_16.json
--rw-r--r--   0 ben       (1000) users      (984)     1056 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C3H2N_17.json
--rw-r--r--   0 ben       (1000) users      (984)     1055 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C3H2N_18.json
--rw-r--r--   0 ben       (1000) users      (984)     1056 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C3H2N_19.json
--rw-r--r--   0 ben       (1000) users      (984)     1056 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C3H2N_2.json
--rw-r--r--   0 ben       (1000) users      (984)     1055 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C3H2N_20.json
--rw-r--r--   0 ben       (1000) users      (984)     1055 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C3H2N_3.json
--rw-r--r--   0 ben       (1000) users      (984)     1057 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C3H2N_4.json
--rw-r--r--   0 ben       (1000) users      (984)     1055 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C3H2N_5.json
--rw-r--r--   0 ben       (1000) users      (984)     1050 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C3H2N_6.json
--rw-r--r--   0 ben       (1000) users      (984)     1055 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C3H2N_7.json
--rw-r--r--   0 ben       (1000) users      (984)     1057 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C3H2N_8.json
--rw-r--r--   0 ben       (1000) users      (984)     1052 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C3H2N_9.json
--rw-r--r--   0 ben       (1000) users      (984)     1373 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C4H3N2_0.json
--rw-r--r--   0 ben       (1000) users      (984)     1376 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C4H3N2_1.json
--rw-r--r--   0 ben       (1000) users      (984)     1374 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C4H3N2_10.json
--rw-r--r--   0 ben       (1000) users      (984)     1373 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C4H3N2_11.json
--rw-r--r--   0 ben       (1000) users      (984)     1375 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C4H3N2_12.json
--rw-r--r--   0 ben       (1000) users      (984)     1371 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C4H3N2_13.json
--rw-r--r--   0 ben       (1000) users      (984)     1372 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C4H3N2_14.json
--rw-r--r--   0 ben       (1000) users      (984)     1369 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C4H3N2_15.json
--rw-r--r--   0 ben       (1000) users      (984)     1374 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C4H3N2_16.json
--rw-r--r--   0 ben       (1000) users      (984)     1370 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C4H3N2_17.json
--rw-r--r--   0 ben       (1000) users      (984)     1374 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C4H3N2_18.json
--rw-r--r--   0 ben       (1000) users      (984)     1370 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C4H3N2_19.json
--rw-r--r--   0 ben       (1000) users      (984)     1370 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C4H3N2_2.json
--rw-r--r--   0 ben       (1000) users      (984)     1372 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C4H3N2_20.json
--rw-r--r--   0 ben       (1000) users      (984)     1372 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C4H3N2_3.json
--rw-r--r--   0 ben       (1000) users      (984)     1372 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C4H3N2_4.json
--rw-r--r--   0 ben       (1000) users      (984)     1374 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C4H3N2_5.json
--rw-r--r--   0 ben       (1000) users      (984)     1371 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C4H3N2_6.json
--rw-r--r--   0 ben       (1000) users      (984)     1372 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C4H3N2_7.json
--rw-r--r--   0 ben       (1000) users      (984)     1375 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C4H3N2_8.json
--rw-r--r--   0 ben       (1000) users      (984)     1375 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C4H3N2_9.json
--rw-r--r--   0 ben       (1000) users      (984)      708 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_HCN_0.json
--rw-r--r--   0 ben       (1000) users      (984)      711 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_HCN_1.json
--rw-r--r--   0 ben       (1000) users      (984)      710 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_HCN_10.json
--rw-r--r--   0 ben       (1000) users      (984)      712 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_HCN_2.json
--rw-r--r--   0 ben       (1000) users      (984)      710 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_HCN_3.json
--rw-r--r--   0 ben       (1000) users      (984)      711 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_HCN_4.json
--rw-r--r--   0 ben       (1000) users      (984)      710 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_HCN_5.json
--rw-r--r--   0 ben       (1000) users      (984)      711 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_HCN_6.json
--rw-r--r--   0 ben       (1000) users      (984)      710 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_HCN_7.json
--rw-r--r--   0 ben       (1000) users      (984)      709 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_HCN_8.json
--rw-r--r--   0 ben       (1000) users      (984)      710 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_HCN_9.json
--rw-r--r--   0 ben       (1000) users      (984)      529 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/neon_tetramer.json
--rw-r--r--   0 ben       (1000) users      (984)      685 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/peroxide2.json
--rw-r--r--   0 ben       (1000) users      (984)      456 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/rxn_H.json
--rw-r--r--   0 ben       (1000) users      (984)      480 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/rxn_H2.json
--rw-r--r--   0 ben       (1000) users      (984)      555 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/rxn_H2O.json
--rw-r--r--   0 ben       (1000) users      (984)      481 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/rxn_O2.json
--rw-r--r--   0 ben       (1000) users      (984)     5235 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/td_C7H8N2OS_1.json
--rw-r--r--   0 ben       (1000) users      (984)     5236 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/td_C7H8N2OS_2.json
--rw-r--r--   0 ben       (1000) users      (984)     4125 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/td_C9H11NO2_0.json
--rw-r--r--   0 ben       (1000) users      (984)     4124 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/td_C9H11NO2_1.json
--rw-r--r--   0 ben       (1000) users      (984)     4129 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/td_C9H11NO2_2.json
--rw-r--r--   0 ben       (1000) users      (984)     4128 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/td_C9H11NO2_3.json
--rw-r--r--   0 ben       (1000) users      (984)     4128 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/td_C9H11NO2_4.json
--rw-r--r--   0 ben       (1000) users      (984)     4127 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/td_C9H11NO2_5.json
--rw-r--r--   0 ben       (1000) users      (984)     4127 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/td_C9H11NO2_6.json
--rw-r--r--   0 ben       (1000) users      (984)     4128 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/td_C9H11NO2_7.json
--rw-r--r--   0 ben       (1000) users      (984)     4132 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/td_C9H11NO2_8.json
--rw-r--r--   0 ben       (1000) users      (984)     4132 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/td_C9H11NO2_9.json
--rw-r--r--   0 ben       (1000) users      (984)      905 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/water_dimer_minima.json
--rw-r--r--   0 ben       (1000) users      (984)      221 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/water_dimer_minima.psimol
--rw-r--r--   0 ben       (1000) users      (984)      939 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/water_dimer_stretch.json
--rw-r--r--   0 ben       (1000) users      (984)      213 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/water_dimer_stretch.psimol
--rw-r--r--   0 ben       (1000) users      (984)      896 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/water_dimer_stretch2.json
--rw-r--r--   0 ben       (1000) users      (984)      216 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/water_dimer_stretch2.psimol
--rw-r--r--   0 ben       (1000) users      (984)     1281 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/molecule_data/water_stacked.json
-drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-01-09 21:45:41.903555 qcarchivetesting-0.53/qcarchivetesting/procedure_data/
--rw-r--r--   0 ben       (1000) users      (984)      185 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/procedure_data/clean.py
--rw-r--r--   0 ben       (1000) users      (984)      489 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/procedure_data/gen_all.sh
--rw-r--r--   0 ben       (1000) users      (984)     2217 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/procedure_data/generate_gridoptimization.py
--rw-r--r--   0 ben       (1000) users      (984)     2175 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/procedure_data/generate_manybody.py
--rw-r--r--   0 ben       (1000) users      (984)     2291 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/procedure_data/generate_neb.py
--rw-r--r--   0 ben       (1000) users      (984)     2060 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/procedure_data/generate_optimization.py
--rw-r--r--   0 ben       (1000) users      (984)     2300 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/procedure_data/generate_reaction.py
--rw-r--r--   0 ben       (1000) users      (984)     2127 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/procedure_data/generate_singlepoint.py
--rw-r--r--   0 ben       (1000) users      (984)     2225 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/procedure_data/generate_torsiondrive.py
--rw-r--r--   0 ben       (1000) users      (984)   485944 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/procedure_data/go_C4H4N2OS_mopac_pm6.json.xz
--rw-r--r--   0 ben       (1000) users      (984)     5812 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/procedure_data/go_H2O2_psi4_b3lyp.json.xz
--rw-r--r--   0 ben       (1000) users      (984)     5844 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/procedure_data/go_H2O2_psi4_pbe.json.xz
--rw-r--r--   0 ben       (1000) users      (984)    35992 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/procedure_data/go_H3NS_psi4_pbe.json.xz
--rw-r--r--   0 ben       (1000) users      (984)    57048 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/procedure_data/mb_cp_he4_psi4_mp2.json.xz
--rw-r--r--   0 ben       (1000) users      (984)    31472 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/procedure_data/mb_none_he4_psi4_mp2.json.xz
--rw-r--r--   0 ben       (1000) users      (984)   202060 2023-09-20 13:55:23.000000 qcarchivetesting-0.53/qcarchivetesting/procedure_data/neb_HCN_psi4_b3lyp_opt3.json.xz
--rw-r--r--   0 ben       (1000) users      (984)   196968 2023-09-20 13:55:23.000000 qcarchivetesting-0.53/qcarchivetesting/procedure_data/neb_HCN_psi4_pbe.json.xz
--rw-r--r--   0 ben       (1000) users      (984)   240552 2023-09-20 13:55:23.000000 qcarchivetesting-0.53/qcarchivetesting/procedure_data/neb_HCN_psi4_pbe0_opt1.json.xz
--rw-r--r--   0 ben       (1000) users      (984)   213804 2023-09-20 13:55:23.000000 qcarchivetesting-0.53/qcarchivetesting/procedure_data/neb_HCN_psi4_pbe_opt2.json.xz
--rw-r--r--   0 ben       (1000) users      (984)   256760 2023-09-20 13:55:23.000000 qcarchivetesting-0.53/qcarchivetesting/procedure_data/neb_HCN_psi4_pbe_opt_diff.json.xz
--rw-r--r--   0 ben       (1000) users      (984)    27700 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/procedure_data/opt_psi4_benzene.json.xz
--rw-r--r--   0 ben       (1000) users      (984)     2268 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/procedure_data/opt_psi4_fluoroethane_notraj.json.xz
--rw-r--r--   0 ben       (1000) users      (984)    12508 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/procedure_data/opt_psi4_methane_sometraj.json.xz
--rw-r--r--   0 ben       (1000) users      (984)    15628 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/procedure_data/rxn_H2O_psi4_b3lyp_sp.json.xz
--rw-r--r--   0 ben       (1000) users      (984)    95380 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/procedure_data/rxn_H2O_psi4_mp2_opt.json.xz
--rw-r--r--   0 ben       (1000) users      (984)   110060 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/procedure_data/rxn_H2O_psi4_mp2_optsp.json.xz
--rw-r--r--   0 ben       (1000) users      (984)    10220 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/procedure_data/rxn_H2_psi4_b3lyp_sp.json.xz
--rw-r--r--   0 ben       (1000) users      (984)     6800 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/procedure_data/sp_psi4_benzene_energy_1.json.xz
--rw-r--r--   0 ben       (1000) users      (984)     6816 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/procedure_data/sp_psi4_benzene_energy_2.json.xz
--rw-r--r--   0 ben       (1000) users      (984)     6824 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/procedure_data/sp_psi4_benzene_energy_3.json.xz
--rw-r--r--   0 ben       (1000) users      (984)     9612 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/procedure_data/sp_psi4_fluoroethane_wfn.json.xz
--rw-r--r--   0 ben       (1000) users      (984)     6820 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/procedure_data/sp_psi4_h2_b3lyp_nativefiles.json.xz
--rw-r--r--   0 ben       (1000) users      (984)     8632 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/procedure_data/sp_psi4_peroxide_energy_wfn.json.xz
--rw-r--r--   0 ben       (1000) users      (984)     5936 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/procedure_data/sp_psi4_water_energy.json.xz
--rw-r--r--   0 ben       (1000) users      (984)     6380 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/procedure_data/sp_psi4_water_gradient.json.xz
--rw-r--r--   0 ben       (1000) users      (984)    10964 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/procedure_data/sp_psi4_water_hessian.json.xz
--rw-r--r--   0 ben       (1000) users      (984)     1136 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/procedure_data/sp_rdkit_benzene_energy.json.xz
--rw-r--r--   0 ben       (1000) users      (984)      948 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/procedure_data/sp_rdkit_water_energy.json.xz
--rw-r--r--   0 ben       (1000) users      (984)  2388372 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/procedure_data/td_C9H11NO2_mopac_pm6.json.xz
--rw-r--r--   0 ben       (1000) users      (984)    11064 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/procedure_data/td_H2O2_mopac_pm6.json.xz
--rw-r--r--   0 ben       (1000) users      (984)    10720 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/procedure_data/td_H2O2_psi4_pbe.json.xz
--rw-r--r--   0 ben       (1000) users      (984)    10740 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/procedure_data/td_H2O2_psi4_pbe0.json.xz
--rw-r--r--   0 ben       (1000) users      (984)     1238 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/pytest_config.py
--rw-r--r--   0 ben       (1000) users      (984)     3600 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/test_full_gridoptimization.py
--rw-r--r--   0 ben       (1000) users      (984)     2318 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/test_full_manybody.py
--rw-r--r--   0 ben       (1000) users      (984)     1604 2023-11-08 15:48:56.000000 qcarchivetesting-0.53/qcarchivetesting/test_full_neb.py
--rw-r--r--   0 ben       (1000) users      (984)     1845 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/test_full_optimization.py
--rw-r--r--   0 ben       (1000) users      (984)     3367 2023-12-05 16:08:13.000000 qcarchivetesting-0.53/qcarchivetesting/test_full_reaction.py
--rw-r--r--   0 ben       (1000) users      (984)     3006 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/test_full_singlepoint.py
--rw-r--r--   0 ben       (1000) users      (984)     1672 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/test_full_torsiondrive.py
--rw-r--r--   0 ben       (1000) users      (984)     8886 2024-01-09 21:37:21.000000 qcarchivetesting-0.53/qcarchivetesting/testing_classes.py
--rw-r--r--   0 ben       (1000) users      (984)     7064 2023-09-20 13:55:23.000000 qcarchivetesting-0.53/qcarchivetesting/testing_fixtures.py
-drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-01-09 21:45:41.903555 qcarchivetesting-0.53/qcarchivetesting/wavefunction_data/
--rw-r--r--   0 ben       (1000) users      (984)    12508 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/wavefunction_data/psi4_fluoroethane.json
--rw-r--r--   0 ben       (1000) users      (984)    13894 2023-09-11 13:38:01.000000 qcarchivetesting-0.53/qcarchivetesting/wavefunction_data/psi4_peroxide.json
-drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-01-09 21:45:41.903555 qcarchivetesting-0.53/qcarchivetesting.egg-info/
--rw-r--r--   0 ben       (1000) users      (984)      679 2024-01-09 21:45:41.000000 qcarchivetesting-0.53/qcarchivetesting.egg-info/PKG-INFO
--rw-r--r--   0 ben       (1000) users      (984)     8303 2024-01-09 21:45:41.000000 qcarchivetesting-0.53/qcarchivetesting.egg-info/SOURCES.txt
--rw-r--r--   0 ben       (1000) users      (984)        1 2024-01-09 21:45:41.000000 qcarchivetesting-0.53/qcarchivetesting.egg-info/dependency_links.txt
--rw-r--r--   0 ben       (1000) users      (984)      118 2024-01-09 21:45:41.000000 qcarchivetesting-0.53/qcarchivetesting.egg-info/entry_points.txt
--rw-r--r--   0 ben       (1000) users      (984)       26 2024-01-09 21:45:41.000000 qcarchivetesting-0.53/qcarchivetesting.egg-info/requires.txt
--rw-r--r--   0 ben       (1000) users      (984)       17 2024-01-09 21:45:41.000000 qcarchivetesting-0.53/qcarchivetesting.egg-info/top_level.txt
--rw-r--r--   0 ben       (1000) users      (984)       38 2024-01-09 21:45:41.903555 qcarchivetesting-0.53/setup.cfg
+drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-04-08 18:04:27.014097 qcarchivetesting-0.54/
+-rw-r--r--   0 ben       (1000) users      (984)      679 2024-04-08 18:04:27.014097 qcarchivetesting-0.54/PKG-INFO
+drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-04-08 18:04:27.007430 qcarchivetesting-0.54/conda-envs/
+-rw-r--r--   0 ben       (1000) users      (984)      366 2024-03-20 15:53:05.000000 qcarchivetesting-0.54/conda-envs/fulltest_qcportal.yaml
+-rw-r--r--   0 ben       (1000) users      (984)      699 2024-04-07 13:23:41.000000 qcarchivetesting-0.54/conda-envs/fulltest_server.yaml
+-rw-r--r--   0 ben       (1000) users      (984)      874 2024-04-07 13:23:41.000000 qcarchivetesting-0.54/conda-envs/fulltest_snowflake.yaml
+-rw-r--r--   0 ben       (1000) users      (984)     1178 2023-12-05 16:08:13.000000 qcarchivetesting-0.54/pyproject.toml
+drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-04-08 18:04:27.007430 qcarchivetesting-0.54/qcarchivetesting/
+-rw-r--r--   0 ben       (1000) users      (984)      416 2023-09-20 13:55:23.000000 qcarchivetesting-0.54/qcarchivetesting/__init__.py
+drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-04-08 18:04:27.007430 qcarchivetesting-0.54/qcarchivetesting/config_files/
+-rw-r--r--   0 ben       (1000) users      (984)      342 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/config_files/gha_fractal_compute.yaml
+-rw-r--r--   0 ben       (1000) users      (984)      517 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/config_files/gha_fractal_oldcompute_dask.yaml
+-rw-r--r--   0 ben       (1000) users      (984)      518 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/config_files/gha_fractal_oldcompute_parsl.yaml
+-rw-r--r--   0 ben       (1000) users      (984)      465 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/config_files/gha_fractal_oldcompute_pool.yaml
+-rw-r--r--   0 ben       (1000) users      (984)      429 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/config_files/gha_fractal_server.yaml
+-rw-r--r--   0 ben       (1000) users      (984)      288 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/config_files/qcf_basic.yaml
+-rw-r--r--   0 ben       (1000) users      (984)     3752 2024-03-20 15:53:05.000000 qcarchivetesting-0.54/qcarchivetesting/data_generator.py
+drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-04-08 18:04:27.007430 qcarchivetesting-0.54/qcarchivetesting/hash_data/
+-rw-r--r--   0 ben       (1000) users      (984)    16240 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/hash_data/dict_hash_test_data.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)     1682 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/hash_data/generate_random.py
+-rw-r--r--   0 ben       (1000) users      (984)     5617 2024-03-20 15:53:05.000000 qcarchivetesting-0.54/qcarchivetesting/helpers.py
+drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-04-08 18:04:27.007430 qcarchivetesting-0.54/qcarchivetesting/migration_data/
+-rw-r--r--   0 ben       (1000) users      (984)    77051 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/migration_data/empty_v0.15.8.sql_dump
+-rw-r--r--   0 ben       (1000) users      (984)      541 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/migration_data/qcfractal_config_v0.15.8.yaml
+drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-04-08 18:04:27.010764 qcarchivetesting-0.54/qcarchivetesting/molecule_data/
+-rw-r--r--   0 ben       (1000) users      (984)     3468 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/benzene_dimer.json
+-rw-r--r--   0 ben       (1000) users      (984)     1684 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/go_C4H4N2OS.json
+-rw-r--r--   0 ben       (1000) users      (984)     1851 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/go_C6H5N3.json
+-rw-r--r--   0 ben       (1000) users      (984)     1056 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/go_H3NS.json
+-rw-r--r--   0 ben       (1000) users      (984)      383 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/hooh.json
+drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-04-08 18:04:27.010764 qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/
+-rw-r--r--   0 ben       (1000) users      (984)     1055 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C3H2N_0.json
+-rw-r--r--   0 ben       (1000) users      (984)     1055 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C3H2N_1.json
+-rw-r--r--   0 ben       (1000) users      (984)     1056 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C3H2N_10.json
+-rw-r--r--   0 ben       (1000) users      (984)     1055 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C3H2N_11.json
+-rw-r--r--   0 ben       (1000) users      (984)     1053 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C3H2N_12.json
+-rw-r--r--   0 ben       (1000) users      (984)     1056 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C3H2N_13.json
+-rw-r--r--   0 ben       (1000) users      (984)     1055 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C3H2N_14.json
+-rw-r--r--   0 ben       (1000) users      (984)     1052 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C3H2N_15.json
+-rw-r--r--   0 ben       (1000) users      (984)     1056 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C3H2N_16.json
+-rw-r--r--   0 ben       (1000) users      (984)     1056 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C3H2N_17.json
+-rw-r--r--   0 ben       (1000) users      (984)     1055 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C3H2N_18.json
+-rw-r--r--   0 ben       (1000) users      (984)     1056 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C3H2N_19.json
+-rw-r--r--   0 ben       (1000) users      (984)     1056 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C3H2N_2.json
+-rw-r--r--   0 ben       (1000) users      (984)     1055 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C3H2N_20.json
+-rw-r--r--   0 ben       (1000) users      (984)     1055 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C3H2N_3.json
+-rw-r--r--   0 ben       (1000) users      (984)     1057 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C3H2N_4.json
+-rw-r--r--   0 ben       (1000) users      (984)     1055 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C3H2N_5.json
+-rw-r--r--   0 ben       (1000) users      (984)     1050 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C3H2N_6.json
+-rw-r--r--   0 ben       (1000) users      (984)     1055 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C3H2N_7.json
+-rw-r--r--   0 ben       (1000) users      (984)     1057 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C3H2N_8.json
+-rw-r--r--   0 ben       (1000) users      (984)     1052 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C3H2N_9.json
+-rw-r--r--   0 ben       (1000) users      (984)     1373 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C4H3N2_0.json
+-rw-r--r--   0 ben       (1000) users      (984)     1376 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C4H3N2_1.json
+-rw-r--r--   0 ben       (1000) users      (984)     1374 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C4H3N2_10.json
+-rw-r--r--   0 ben       (1000) users      (984)     1373 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C4H3N2_11.json
+-rw-r--r--   0 ben       (1000) users      (984)     1375 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C4H3N2_12.json
+-rw-r--r--   0 ben       (1000) users      (984)     1371 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C4H3N2_13.json
+-rw-r--r--   0 ben       (1000) users      (984)     1372 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C4H3N2_14.json
+-rw-r--r--   0 ben       (1000) users      (984)     1369 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C4H3N2_15.json
+-rw-r--r--   0 ben       (1000) users      (984)     1374 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C4H3N2_16.json
+-rw-r--r--   0 ben       (1000) users      (984)     1370 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C4H3N2_17.json
+-rw-r--r--   0 ben       (1000) users      (984)     1374 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C4H3N2_18.json
+-rw-r--r--   0 ben       (1000) users      (984)     1370 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C4H3N2_19.json
+-rw-r--r--   0 ben       (1000) users      (984)     1370 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C4H3N2_2.json
+-rw-r--r--   0 ben       (1000) users      (984)     1372 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C4H3N2_20.json
+-rw-r--r--   0 ben       (1000) users      (984)     1372 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C4H3N2_3.json
+-rw-r--r--   0 ben       (1000) users      (984)     1372 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C4H3N2_4.json
+-rw-r--r--   0 ben       (1000) users      (984)     1374 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C4H3N2_5.json
+-rw-r--r--   0 ben       (1000) users      (984)     1371 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C4H3N2_6.json
+-rw-r--r--   0 ben       (1000) users      (984)     1372 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C4H3N2_7.json
+-rw-r--r--   0 ben       (1000) users      (984)     1375 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C4H3N2_8.json
+-rw-r--r--   0 ben       (1000) users      (984)     1375 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C4H3N2_9.json
+-rw-r--r--   0 ben       (1000) users      (984)      708 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_HCN_0.json
+-rw-r--r--   0 ben       (1000) users      (984)      711 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_HCN_1.json
+-rw-r--r--   0 ben       (1000) users      (984)      710 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_HCN_10.json
+-rw-r--r--   0 ben       (1000) users      (984)      712 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_HCN_2.json
+-rw-r--r--   0 ben       (1000) users      (984)      710 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_HCN_3.json
+-rw-r--r--   0 ben       (1000) users      (984)      711 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_HCN_4.json
+-rw-r--r--   0 ben       (1000) users      (984)      710 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_HCN_5.json
+-rw-r--r--   0 ben       (1000) users      (984)      711 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_HCN_6.json
+-rw-r--r--   0 ben       (1000) users      (984)      710 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_HCN_7.json
+-rw-r--r--   0 ben       (1000) users      (984)      709 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_HCN_8.json
+-rw-r--r--   0 ben       (1000) users      (984)      710 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_HCN_9.json
+-rw-r--r--   0 ben       (1000) users      (984)      529 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/neon_tetramer.json
+-rw-r--r--   0 ben       (1000) users      (984)      685 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/peroxide2.json
+-rw-r--r--   0 ben       (1000) users      (984)      456 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/rxn_H.json
+-rw-r--r--   0 ben       (1000) users      (984)      480 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/rxn_H2.json
+-rw-r--r--   0 ben       (1000) users      (984)      555 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/rxn_H2O.json
+-rw-r--r--   0 ben       (1000) users      (984)      481 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/rxn_O2.json
+-rw-r--r--   0 ben       (1000) users      (984)     5235 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/td_C7H8N2OS_1.json
+-rw-r--r--   0 ben       (1000) users      (984)     5236 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/td_C7H8N2OS_2.json
+-rw-r--r--   0 ben       (1000) users      (984)     4125 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/td_C9H11NO2_0.json
+-rw-r--r--   0 ben       (1000) users      (984)     4124 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/td_C9H11NO2_1.json
+-rw-r--r--   0 ben       (1000) users      (984)     4129 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/td_C9H11NO2_2.json
+-rw-r--r--   0 ben       (1000) users      (984)     4128 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/td_C9H11NO2_3.json
+-rw-r--r--   0 ben       (1000) users      (984)     4128 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/td_C9H11NO2_4.json
+-rw-r--r--   0 ben       (1000) users      (984)     4127 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/td_C9H11NO2_5.json
+-rw-r--r--   0 ben       (1000) users      (984)     4127 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/td_C9H11NO2_6.json
+-rw-r--r--   0 ben       (1000) users      (984)     4128 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/td_C9H11NO2_7.json
+-rw-r--r--   0 ben       (1000) users      (984)     4132 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/td_C9H11NO2_8.json
+-rw-r--r--   0 ben       (1000) users      (984)     4132 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/td_C9H11NO2_9.json
+-rw-r--r--   0 ben       (1000) users      (984)      905 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/water_dimer_minima.json
+-rw-r--r--   0 ben       (1000) users      (984)      221 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/water_dimer_minima.psimol
+-rw-r--r--   0 ben       (1000) users      (984)      939 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/water_dimer_stretch.json
+-rw-r--r--   0 ben       (1000) users      (984)      213 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/water_dimer_stretch.psimol
+-rw-r--r--   0 ben       (1000) users      (984)      896 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/water_dimer_stretch2.json
+-rw-r--r--   0 ben       (1000) users      (984)      216 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/water_dimer_stretch2.psimol
+-rw-r--r--   0 ben       (1000) users      (984)     1281 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/molecule_data/water_stacked.json
+drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-04-08 18:04:27.014097 qcarchivetesting-0.54/qcarchivetesting/procedure_data/
+-rw-r--r--   0 ben       (1000) users      (984)      185 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/procedure_data/clean.py
+-rw-r--r--   0 ben       (1000) users      (984)      489 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/procedure_data/gen_all.sh
+-rw-r--r--   0 ben       (1000) users      (984)     2217 2024-03-11 20:25:46.000000 qcarchivetesting-0.54/qcarchivetesting/procedure_data/generate_gridoptimization.py
+-rw-r--r--   0 ben       (1000) users      (984)     2175 2024-04-08 18:00:43.000000 qcarchivetesting-0.54/qcarchivetesting/procedure_data/generate_manybody.py
+-rw-r--r--   0 ben       (1000) users      (984)     2291 2024-03-11 20:25:46.000000 qcarchivetesting-0.54/qcarchivetesting/procedure_data/generate_neb.py
+-rw-r--r--   0 ben       (1000) users      (984)     2060 2024-03-11 20:25:46.000000 qcarchivetesting-0.54/qcarchivetesting/procedure_data/generate_optimization.py
+-rw-r--r--   0 ben       (1000) users      (984)     2300 2024-03-11 20:25:46.000000 qcarchivetesting-0.54/qcarchivetesting/procedure_data/generate_reaction.py
+-rw-r--r--   0 ben       (1000) users      (984)     2127 2024-03-11 20:25:46.000000 qcarchivetesting-0.54/qcarchivetesting/procedure_data/generate_singlepoint.py
+-rw-r--r--   0 ben       (1000) users      (984)     2225 2024-03-11 20:25:46.000000 qcarchivetesting-0.54/qcarchivetesting/procedure_data/generate_torsiondrive.py
+-rw-r--r--   0 ben       (1000) users      (984)   485944 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/procedure_data/go_C4H4N2OS_mopac_pm6.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)     5812 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/procedure_data/go_H2O2_psi4_b3lyp.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)     5844 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/procedure_data/go_H2O2_psi4_pbe.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)    35992 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/procedure_data/go_H3NS_psi4_pbe.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)    57048 2024-04-08 18:00:43.000000 qcarchivetesting-0.54/qcarchivetesting/procedure_data/mb_cp_he4_psi4_mp2.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)    31472 2024-04-08 18:00:43.000000 qcarchivetesting-0.54/qcarchivetesting/procedure_data/mb_none_he4_psi4_mp2.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)   323700 2024-04-07 13:23:41.000000 qcarchivetesting-0.54/qcarchivetesting/procedure_data/neb_HCN_psi4_b3lyp_opt3.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)   307128 2024-04-07 13:23:41.000000 qcarchivetesting-0.54/qcarchivetesting/procedure_data/neb_HCN_psi4_pbe.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)   358332 2024-04-07 13:23:41.000000 qcarchivetesting-0.54/qcarchivetesting/procedure_data/neb_HCN_psi4_pbe0_opt1.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)   322480 2024-04-07 13:23:41.000000 qcarchivetesting-0.54/qcarchivetesting/procedure_data/neb_HCN_psi4_pbe_opt2.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)   385408 2024-04-07 13:23:41.000000 qcarchivetesting-0.54/qcarchivetesting/procedure_data/neb_HCN_psi4_pbe_opt_diff.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)    27700 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/procedure_data/opt_psi4_benzene.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)     2268 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/procedure_data/opt_psi4_fluoroethane_notraj.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)    12508 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/procedure_data/opt_psi4_methane_sometraj.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)    15628 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/procedure_data/rxn_H2O_psi4_b3lyp_sp.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)    95380 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/procedure_data/rxn_H2O_psi4_mp2_opt.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)   110060 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/procedure_data/rxn_H2O_psi4_mp2_optsp.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)    10220 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/procedure_data/rxn_H2_psi4_b3lyp_sp.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)     6800 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/procedure_data/sp_psi4_benzene_energy_1.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)     6816 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/procedure_data/sp_psi4_benzene_energy_2.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)     6824 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/procedure_data/sp_psi4_benzene_energy_3.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)     9612 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/procedure_data/sp_psi4_fluoroethane_wfn.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)     6820 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/procedure_data/sp_psi4_h2_b3lyp_nativefiles.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)     8632 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/procedure_data/sp_psi4_peroxide_energy_wfn.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)     5936 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/procedure_data/sp_psi4_water_energy.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)     6380 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/procedure_data/sp_psi4_water_gradient.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)    10964 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/procedure_data/sp_psi4_water_hessian.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)     1136 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/procedure_data/sp_rdkit_benzene_energy.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)      948 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/procedure_data/sp_rdkit_water_energy.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)  2388372 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/procedure_data/td_C9H11NO2_mopac_pm6.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)    11064 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/procedure_data/td_H2O2_mopac_pm6.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)    10720 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/procedure_data/td_H2O2_psi4_pbe.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)    10740 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/procedure_data/td_H2O2_psi4_pbe0.json.xz
+-rw-r--r--   0 ben       (1000) users      (984)     1238 2024-03-11 20:25:46.000000 qcarchivetesting-0.54/qcarchivetesting/pytest_config.py
+-rw-r--r--   0 ben       (1000) users      (984)     3600 2024-03-11 20:25:46.000000 qcarchivetesting-0.54/qcarchivetesting/test_full_gridoptimization.py
+-rw-r--r--   0 ben       (1000) users      (984)     2318 2024-04-08 18:00:43.000000 qcarchivetesting-0.54/qcarchivetesting/test_full_manybody.py
+-rw-r--r--   0 ben       (1000) users      (984)     6542 2024-04-07 13:23:41.000000 qcarchivetesting-0.54/qcarchivetesting/test_full_neb.py
+-rw-r--r--   0 ben       (1000) users      (984)     1845 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/test_full_optimization.py
+-rw-r--r--   0 ben       (1000) users      (984)     3367 2024-03-20 15:53:05.000000 qcarchivetesting-0.54/qcarchivetesting/test_full_reaction.py
+-rw-r--r--   0 ben       (1000) users      (984)     3006 2024-03-11 20:25:46.000000 qcarchivetesting-0.54/qcarchivetesting/test_full_singlepoint.py
+-rw-r--r--   0 ben       (1000) users      (984)     1672 2024-03-11 20:25:46.000000 qcarchivetesting-0.54/qcarchivetesting/test_full_torsiondrive.py
+-rw-r--r--   0 ben       (1000) users      (984)     9265 2024-04-07 13:30:42.000000 qcarchivetesting-0.54/qcarchivetesting/testing_classes.py
+-rw-r--r--   0 ben       (1000) users      (984)     7064 2024-03-11 20:25:46.000000 qcarchivetesting-0.54/qcarchivetesting/testing_fixtures.py
+drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-04-08 18:04:27.014097 qcarchivetesting-0.54/qcarchivetesting/wavefunction_data/
+-rw-r--r--   0 ben       (1000) users      (984)    12508 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/wavefunction_data/psi4_fluoroethane.json
+-rw-r--r--   0 ben       (1000) users      (984)    13894 2023-09-11 13:38:01.000000 qcarchivetesting-0.54/qcarchivetesting/wavefunction_data/psi4_peroxide.json
+drwxr-xr-x   0 ben       (1000) users      (984)        0 2024-04-08 18:04:27.014097 qcarchivetesting-0.54/qcarchivetesting.egg-info/
+-rw-r--r--   0 ben       (1000) users      (984)      679 2024-04-08 18:04:27.000000 qcarchivetesting-0.54/qcarchivetesting.egg-info/PKG-INFO
+-rw-r--r--   0 ben       (1000) users      (984)     8303 2024-04-08 18:04:27.000000 qcarchivetesting-0.54/qcarchivetesting.egg-info/SOURCES.txt
+-rw-r--r--   0 ben       (1000) users      (984)        1 2024-04-08 18:04:27.000000 qcarchivetesting-0.54/qcarchivetesting.egg-info/dependency_links.txt
+-rw-r--r--   0 ben       (1000) users      (984)      118 2024-04-08 18:04:27.000000 qcarchivetesting-0.54/qcarchivetesting.egg-info/entry_points.txt
+-rw-r--r--   0 ben       (1000) users      (984)       26 2024-04-08 18:04:27.000000 qcarchivetesting-0.54/qcarchivetesting.egg-info/requires.txt
+-rw-r--r--   0 ben       (1000) users      (984)       17 2024-04-08 18:04:27.000000 qcarchivetesting-0.54/qcarchivetesting.egg-info/top_level.txt
+-rw-r--r--   0 ben       (1000) users      (984)       38 2024-04-08 18:04:27.017430 qcarchivetesting-0.54/setup.cfg
```

### Comparing `qcarchivetesting-0.53/PKG-INFO` & `qcarchivetesting-0.54/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcarchivetesting
-Version: 0.53
+Version: 0.54
 Summary: A distributed compute and database platform for quantum chemistry.
 Author-email: Benjamin Pritchard <qcarchive@molssi.org>
 Project-URL: Homepage, https://github.com/MolSSI/QCFractal
 Project-URL: Bug Tracker, https://github.com/MolSSI/QCFractal/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `qcarchivetesting-0.53/conda-envs/fulltest_server.yaml` & `qcarchivetesting-0.54/conda-envs/fulltest_server.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -35,9 +35,9 @@
   - psycopg2
   - geoip2
 
   # QCFractal Services
   - torsiondrive
 
   - pip:
-      - "geometric @ git+https://github.com/hjnpark/geomeTRIC"
+      - "geometric @ git+https://github.com/leeping/geomeTRIC"
       - scipy # for geometric
```

### Comparing `qcarchivetesting-0.53/conda-envs/fulltest_snowflake.yaml` & `qcarchivetesting-0.54/conda-envs/fulltest_snowflake.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -47,9 +47,9 @@
   - psi4>=1.7
   - rdkit
 
   # Testing packages
   - pytest
 
   - pip:
-      - "geometric @ git+https://github.com/hjnpark/geomeTRIC"
+      - "geometric @ git+https://github.com/leeping/geomeTRIC"
       - scipy # for geometric
```

### Comparing `qcarchivetesting-0.53/pyproject.toml` & `qcarchivetesting-0.54/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/config_files/gha_fractal_oldcompute_dask.yaml` & `qcarchivetesting-0.54/qcarchivetesting/config_files/gha_fractal_oldcompute_dask.yaml`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/config_files/gha_fractal_oldcompute_parsl.yaml` & `qcarchivetesting-0.54/qcarchivetesting/config_files/gha_fractal_oldcompute_parsl.yaml`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/data_generator.py` & `qcarchivetesting-0.54/qcarchivetesting/data_generator.py`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/hash_data/dict_hash_test_data.json.xz` & `qcarchivetesting-0.54/qcarchivetesting/hash_data/dict_hash_test_data.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/hash_data/generate_random.py` & `qcarchivetesting-0.54/qcarchivetesting/hash_data/generate_random.py`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/helpers.py` & `qcarchivetesting-0.54/qcarchivetesting/helpers.py`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/migration_data/empty_v0.15.8.sql_dump` & `qcarchivetesting-0.54/qcarchivetesting/migration_data/empty_v0.15.8.sql_dump`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/migration_data/qcfractal_config_v0.15.8.yaml` & `qcarchivetesting-0.54/qcarchivetesting/migration_data/qcfractal_config_v0.15.8.yaml`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/benzene_dimer.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/benzene_dimer.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/go_C4H4N2OS.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/go_C4H4N2OS.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/go_C6H5N3.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/go_C6H5N3.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/go_H3NS.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/go_H3NS.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C3H2N_0.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C3H2N_0.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C3H2N_1.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C3H2N_1.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C3H2N_10.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C3H2N_10.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C3H2N_11.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C3H2N_11.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C3H2N_12.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C3H2N_12.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C3H2N_13.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C3H2N_13.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C3H2N_14.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C3H2N_14.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C3H2N_15.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C3H2N_15.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C3H2N_16.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C3H2N_16.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C3H2N_17.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C3H2N_17.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C3H2N_18.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C3H2N_18.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C3H2N_19.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C3H2N_19.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C3H2N_2.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C3H2N_2.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C3H2N_20.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C3H2N_20.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C3H2N_3.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C3H2N_3.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C3H2N_4.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C3H2N_4.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C3H2N_5.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C3H2N_5.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C3H2N_6.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C3H2N_6.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C3H2N_7.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C3H2N_7.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C3H2N_8.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C3H2N_8.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C3H2N_9.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C3H2N_9.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C4H3N2_0.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C4H3N2_0.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C4H3N2_1.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C4H3N2_1.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C4H3N2_10.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C4H3N2_10.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C4H3N2_11.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C4H3N2_11.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C4H3N2_12.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C4H3N2_12.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C4H3N2_13.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C4H3N2_13.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C4H3N2_14.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C4H3N2_14.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C4H3N2_15.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C4H3N2_15.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C4H3N2_16.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C4H3N2_16.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C4H3N2_17.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C4H3N2_17.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C4H3N2_18.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C4H3N2_18.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C4H3N2_19.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C4H3N2_19.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C4H3N2_2.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C4H3N2_2.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C4H3N2_20.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C4H3N2_20.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C4H3N2_3.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C4H3N2_3.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C4H3N2_4.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C4H3N2_4.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C4H3N2_5.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C4H3N2_5.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C4H3N2_6.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C4H3N2_6.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C4H3N2_7.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C4H3N2_7.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C4H3N2_8.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C4H3N2_8.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_C4H3N2_9.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_C4H3N2_9.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_HCN_0.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_HCN_0.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_HCN_1.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_HCN_1.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_HCN_10.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_HCN_10.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_HCN_2.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_HCN_2.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_HCN_3.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_HCN_3.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_HCN_4.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_HCN_4.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_HCN_5.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_HCN_5.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_HCN_6.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_HCN_6.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_HCN_7.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_HCN_7.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_HCN_8.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_HCN_8.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/neb/neb_HCN_9.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/neb/neb_HCN_9.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/neon_tetramer.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/neon_tetramer.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/peroxide2.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/peroxide2.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/rxn_H2O.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/rxn_H2O.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/td_C7H8N2OS_1.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/td_C7H8N2OS_1.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/td_C7H8N2OS_2.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/td_C7H8N2OS_2.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/td_C9H11NO2_0.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/td_C9H11NO2_0.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/td_C9H11NO2_1.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/td_C9H11NO2_1.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/td_C9H11NO2_2.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/td_C9H11NO2_2.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/td_C9H11NO2_3.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/td_C9H11NO2_3.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/td_C9H11NO2_4.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/td_C9H11NO2_4.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/td_C9H11NO2_5.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/td_C9H11NO2_5.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/td_C9H11NO2_6.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/td_C9H11NO2_6.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/td_C9H11NO2_7.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/td_C9H11NO2_7.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/td_C9H11NO2_8.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/td_C9H11NO2_8.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/td_C9H11NO2_9.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/td_C9H11NO2_9.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/water_dimer_minima.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/water_dimer_minima.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/water_dimer_stretch.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/water_dimer_stretch.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/water_dimer_stretch2.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/water_dimer_stretch2.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/molecule_data/water_stacked.json` & `qcarchivetesting-0.54/qcarchivetesting/molecule_data/water_stacked.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/procedure_data/generate_gridoptimization.py` & `qcarchivetesting-0.54/qcarchivetesting/procedure_data/generate_gridoptimization.py`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/procedure_data/generate_manybody.py` & `qcarchivetesting-0.54/qcarchivetesting/procedure_data/generate_manybody.py`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/procedure_data/generate_neb.py` & `qcarchivetesting-0.54/qcarchivetesting/procedure_data/generate_neb.py`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/procedure_data/generate_optimization.py` & `qcarchivetesting-0.54/qcarchivetesting/procedure_data/generate_optimization.py`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/procedure_data/generate_reaction.py` & `qcarchivetesting-0.54/qcarchivetesting/procedure_data/generate_reaction.py`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/procedure_data/generate_singlepoint.py` & `qcarchivetesting-0.54/qcarchivetesting/procedure_data/generate_singlepoint.py`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/procedure_data/generate_torsiondrive.py` & `qcarchivetesting-0.54/qcarchivetesting/procedure_data/generate_torsiondrive.py`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/procedure_data/go_C4H4N2OS_mopac_pm6.json.xz` & `qcarchivetesting-0.54/qcarchivetesting/procedure_data/go_C4H4N2OS_mopac_pm6.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/procedure_data/go_H2O2_psi4_b3lyp.json.xz` & `qcarchivetesting-0.54/qcarchivetesting/procedure_data/go_H2O2_psi4_b3lyp.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/procedure_data/go_H2O2_psi4_pbe.json.xz` & `qcarchivetesting-0.54/qcarchivetesting/procedure_data/go_H2O2_psi4_pbe.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/procedure_data/go_H3NS_psi4_pbe.json.xz` & `qcarchivetesting-0.54/qcarchivetesting/procedure_data/go_H3NS_psi4_pbe.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/procedure_data/mb_cp_he4_psi4_mp2.json.xz` & `qcarchivetesting-0.54/qcarchivetesting/procedure_data/mb_cp_he4_psi4_mp2.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/procedure_data/mb_none_he4_psi4_mp2.json.xz` & `qcarchivetesting-0.54/qcarchivetesting/procedure_data/mb_none_he4_psi4_mp2.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/procedure_data/opt_psi4_benzene.json.xz` & `qcarchivetesting-0.54/qcarchivetesting/procedure_data/opt_psi4_benzene.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/procedure_data/opt_psi4_fluoroethane_notraj.json.xz` & `qcarchivetesting-0.54/qcarchivetesting/procedure_data/opt_psi4_fluoroethane_notraj.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/procedure_data/opt_psi4_methane_sometraj.json.xz` & `qcarchivetesting-0.54/qcarchivetesting/procedure_data/opt_psi4_methane_sometraj.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/procedure_data/rxn_H2O_psi4_b3lyp_sp.json.xz` & `qcarchivetesting-0.54/qcarchivetesting/procedure_data/rxn_H2O_psi4_b3lyp_sp.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/procedure_data/rxn_H2O_psi4_mp2_opt.json.xz` & `qcarchivetesting-0.54/qcarchivetesting/procedure_data/rxn_H2O_psi4_mp2_opt.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/procedure_data/rxn_H2O_psi4_mp2_optsp.json.xz` & `qcarchivetesting-0.54/qcarchivetesting/procedure_data/rxn_H2O_psi4_mp2_optsp.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/procedure_data/rxn_H2_psi4_b3lyp_sp.json.xz` & `qcarchivetesting-0.54/qcarchivetesting/procedure_data/rxn_H2_psi4_b3lyp_sp.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/procedure_data/sp_psi4_benzene_energy_1.json.xz` & `qcarchivetesting-0.54/qcarchivetesting/procedure_data/sp_psi4_benzene_energy_1.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/procedure_data/sp_psi4_benzene_energy_2.json.xz` & `qcarchivetesting-0.54/qcarchivetesting/procedure_data/sp_psi4_benzene_energy_2.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/procedure_data/sp_psi4_benzene_energy_3.json.xz` & `qcarchivetesting-0.54/qcarchivetesting/procedure_data/sp_psi4_benzene_energy_3.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/procedure_data/sp_psi4_fluoroethane_wfn.json.xz` & `qcarchivetesting-0.54/qcarchivetesting/procedure_data/sp_psi4_fluoroethane_wfn.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/procedure_data/sp_psi4_h2_b3lyp_nativefiles.json.xz` & `qcarchivetesting-0.54/qcarchivetesting/procedure_data/sp_psi4_h2_b3lyp_nativefiles.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/procedure_data/sp_psi4_peroxide_energy_wfn.json.xz` & `qcarchivetesting-0.54/qcarchivetesting/procedure_data/sp_psi4_peroxide_energy_wfn.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/procedure_data/sp_psi4_water_energy.json.xz` & `qcarchivetesting-0.54/qcarchivetesting/procedure_data/sp_psi4_water_energy.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/procedure_data/sp_psi4_water_gradient.json.xz` & `qcarchivetesting-0.54/qcarchivetesting/procedure_data/sp_psi4_water_gradient.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/procedure_data/sp_psi4_water_hessian.json.xz` & `qcarchivetesting-0.54/qcarchivetesting/procedure_data/sp_psi4_water_hessian.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/procedure_data/sp_rdkit_benzene_energy.json.xz` & `qcarchivetesting-0.54/qcarchivetesting/procedure_data/sp_rdkit_benzene_energy.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/procedure_data/sp_rdkit_water_energy.json.xz` & `qcarchivetesting-0.54/qcarchivetesting/procedure_data/sp_rdkit_water_energy.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/procedure_data/td_C9H11NO2_mopac_pm6.json.xz` & `qcarchivetesting-0.54/qcarchivetesting/procedure_data/td_C9H11NO2_mopac_pm6.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/procedure_data/td_H2O2_mopac_pm6.json.xz` & `qcarchivetesting-0.54/qcarchivetesting/procedure_data/td_H2O2_mopac_pm6.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/procedure_data/td_H2O2_psi4_pbe.json.xz` & `qcarchivetesting-0.54/qcarchivetesting/procedure_data/td_H2O2_psi4_pbe.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/procedure_data/td_H2O2_psi4_pbe0.json.xz` & `qcarchivetesting-0.54/qcarchivetesting/procedure_data/td_H2O2_psi4_pbe0.json.xz`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/pytest_config.py` & `qcarchivetesting-0.54/qcarchivetesting/pytest_config.py`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/test_full_gridoptimization.py` & `qcarchivetesting-0.54/qcarchivetesting/test_full_gridoptimization.py`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/test_full_manybody.py` & `qcarchivetesting-0.54/qcarchivetesting/test_full_manybody.py`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/test_full_neb.py` & `qcarchivetesting-0.54/qcarchivetesting/test_full_optimization.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,59 +1,61 @@
 from __future__ import annotations
 
 import time
 from typing import TYPE_CHECKING
 
-from qcportal.neb import NEBKeywords
-from qcportal.optimization import OptimizationSpecification
+from qcelemental.models import Molecule
+
 from qcportal.record_models import RecordStatusEnum
-from qcarchivetesting import load_molecule_data
-from qcportal.singlepoint import QCSpecification
 
 if TYPE_CHECKING:
     from qcportal import PortalClient
 
 
-def test_neb_full_1(fulltest_client: PortalClient):
-    chain = [load_molecule_data("neb/neb_HCN_%i" % i) for i in range(11)]
-    neb_keywords = NEBKeywords(
-        images=11,
-        spring_constant=1,
-        optimize_endpoints=True,
-        maximum_force=0.02,
-        average_force=0.02,
-        optimize_ts=True,
-        epsilon=1e-6,
-        hessian_reset=True,
-        spring_type=0,
+def test_optimization_full_1(fulltest_client: PortalClient):
+    mol = Molecule(symbols=["H", "H"], geometry=[[0.0, 0.0, 0.0], [0.0, 0.0, 1.0]])
+    meta, ids = fulltest_client.add_optimizations(
+        initial_molecules=[mol],
+        program="geometric",
+        qc_specification={
+            "program": "psi4",
+            "method": "b3lyp",
+            "basis": "6-31g**",
+            "keywords": {"maxiter": 100},
+        },
+        keywords={"maxiter": 30},
     )
 
-    sp_spec = QCSpecification(
-        program="psi4",
-        driver="gradient",
-        method="hf",
-        basis="6-31g",
-        keywords={},
-    )
+    for i in range(120):
+        time.sleep(1)
+        rec = fulltest_client.get_optimizations(ids[0])
+        if rec.status not in [RecordStatusEnum.running, RecordStatusEnum.waiting]:
+            break
+    else:
+        raise RuntimeError("Did not finish calculation in time")
+
+    assert rec.status == RecordStatusEnum.complete
 
-    opt_spec = OptimizationSpecification(
-        program="geometric",
-        qc_specification=sp_spec,
-    )
 
-    meta, ids = fulltest_client.add_nebs(
-        initial_chains=[chain],
+def test_optimization_full_error_1(fulltest_client: PortalClient):
+    mol = Molecule(symbols=["H", "H"], geometry=[[0.0, 0.0, 0.0], [0.0, 0.0, 1.0]])
+    meta, ids = fulltest_client.add_optimizations(
+        initial_molecules=[mol],
         program="geometric",
-        singlepoint_specification=sp_spec,
-        optimization_specification=opt_spec,
-        keywords=neb_keywords,
+        qc_specification={
+            "program": "psi4",
+            "method": "b3lyp",
+            "basis": "6-31g**",
+            "keywords": {"maxiter": 1},
+        },
+        keywords={"maxiter": 30},
     )
 
-    for i in range(600):
-        time.sleep(15)
-        rec = fulltest_client.get_nebs(ids[0])
+    for i in range(120):
+        time.sleep(1)
+        rec = fulltest_client.get_optimizations(ids[0])
         if rec.status not in [RecordStatusEnum.running, RecordStatusEnum.waiting]:
             break
     else:
         raise RuntimeError("Did not finish calculation in time")
 
-    assert rec.status == RecordStatusEnum.complete
+    assert rec.status == RecordStatusEnum.error
```

### Comparing `qcarchivetesting-0.53/qcarchivetesting/test_full_optimization.py` & `qcarchivetesting-0.54/qcarchivetesting/test_full_torsiondrive.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,61 +1,57 @@
 from __future__ import annotations
 
 import time
 from typing import TYPE_CHECKING
 
-from qcelemental.models import Molecule
-
+from qcportal.molecules import Molecule
 from qcportal.record_models import RecordStatusEnum
 
 if TYPE_CHECKING:
     from qcportal import PortalClient
 
 
-def test_optimization_full_1(fulltest_client: PortalClient):
-    mol = Molecule(symbols=["H", "H"], geometry=[[0.0, 0.0, 0.0], [0.0, 0.0, 1.0]])
-    meta, ids = fulltest_client.add_optimizations(
-        initial_molecules=[mol],
-        program="geometric",
-        qc_specification={
-            "program": "psi4",
-            "method": "b3lyp",
-            "basis": "6-31g**",
-            "keywords": {"maxiter": 100},
-        },
-        keywords={"maxiter": 30},
+def test_torsiondrive_full_1(fulltest_client: PortalClient):
+    molecule = Molecule(
+        symbols=["H", "O", "O", "H"],
+        connectivity=[[0, 1, 1], [1, 2, 1], [2, 3, 1]],
+        geometry=[
+            1.848671612718783,
+            1.4723466699847623,
+            0.6446435664312682,
+            1.3127881568370925,
+            -0.1304193792618355,
+            -0.2118922703584585,
+            -1.3127927010942337,
+            0.1334187339129038,
+            -0.21189641512867613,
+            -1.8386801669381663,
+            -1.482348324549995,
+            0.6446369709610646,
+        ],
     )
 
-    for i in range(120):
-        time.sleep(1)
-        rec = fulltest_client.get_optimizations(ids[0])
-        if rec.status not in [RecordStatusEnum.running, RecordStatusEnum.waiting]:
-            break
-    else:
-        raise RuntimeError("Did not finish calculation in time")
-
-    assert rec.status == RecordStatusEnum.complete
+    td_keywords = {"dihedrals": [[0, 1, 2, 3]], "grid_spacing": [90]}
 
-
-def test_optimization_full_error_1(fulltest_client: PortalClient):
-    mol = Molecule(symbols=["H", "H"], geometry=[[0.0, 0.0, 0.0], [0.0, 0.0, 1.0]])
-    meta, ids = fulltest_client.add_optimizations(
-        initial_molecules=[mol],
-        program="geometric",
-        qc_specification={
-            "program": "psi4",
-            "method": "b3lyp",
-            "basis": "6-31g**",
-            "keywords": {"maxiter": 1},
-        },
-        keywords={"maxiter": 30},
+    opt_spec = {
+        "keywords": {},
+        "program": "geometric",
+        "protocols": {"trajectory": "none"},
+        "qc_specification": {"basis": "sto-3g", "keywords": {}, "method": "pbe", "program": "psi4"},
+    }
+
+    meta, ids = fulltest_client.add_torsiondrives(
+        initial_molecules=[[molecule]],
+        program="torsiondrive",
+        optimization_specification=opt_spec,
+        keywords=td_keywords,
     )
 
-    for i in range(120):
+    for i in range(240):
         time.sleep(1)
-        rec = fulltest_client.get_optimizations(ids[0])
+        rec = fulltest_client.get_torsiondrives(ids[0])
         if rec.status not in [RecordStatusEnum.running, RecordStatusEnum.waiting]:
             break
     else:
         raise RuntimeError("Did not finish calculation in time")
 
-    assert rec.status == RecordStatusEnum.error
+    assert rec.status == RecordStatusEnum.complete
```

### Comparing `qcarchivetesting-0.53/qcarchivetesting/test_full_reaction.py` & `qcarchivetesting-0.54/qcarchivetesting/test_full_reaction.py`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/test_full_singlepoint.py` & `qcarchivetesting-0.54/qcarchivetesting/test_full_singlepoint.py`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/testing_classes.py` & `qcarchivetesting-0.54/qcarchivetesting/testing_classes.py`

 * *Files 7% similar despite different names*

```diff
@@ -244,36 +244,40 @@
 
     def stop_job_runner(self) -> None:
         """
         Stops the job_runner thread
         """
         self._stop_job_runner()
 
-    def client(self, username=None, password=None) -> PortalClient:
+    def client(self, username=None, password=None, cache_dir=None, shared_memory_cache=False) -> PortalClient:
         """
         Obtain a client connected to this snowflake
 
         Parameters
         ----------
         username
             The username to connect as
         password
             The password to use
+        cache_dir
+            Directory to store cache files in
+        shared_memory_cache
+            Whether to use a shared memory cache
+
+        Note: We generally don't want a shared memory cache for tests, so the default is False here
+        rather than True as in the main codebase
 
         Returns
         -------
         :
             A PortalClient that is connected to this snowflake
         """
 
-        client = PortalClient(
-            self.get_uri(),
-            username=username,
-            password=password,
-        )
+        client = PortalClient(self.get_uri(), username=username, password=password, cache_dir=cache_dir,
+                              shared_memory_cache=shared_memory_cache)
         client.encoding = self.encoding
         return client
 
     def manager_client(self, name_data: ManagerName, username=None, password=None) -> ManagerClient:
         """
         Obtain a manager client connected to this snowflake
```

### Comparing `qcarchivetesting-0.53/qcarchivetesting/testing_fixtures.py` & `qcarchivetesting-0.54/qcarchivetesting/testing_fixtures.py`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/wavefunction_data/psi4_fluoroethane.json` & `qcarchivetesting-0.54/qcarchivetesting/wavefunction_data/psi4_fluoroethane.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting/wavefunction_data/psi4_peroxide.json` & `qcarchivetesting-0.54/qcarchivetesting/wavefunction_data/psi4_peroxide.json`

 * *Files identical despite different names*

### Comparing `qcarchivetesting-0.53/qcarchivetesting.egg-info/PKG-INFO` & `qcarchivetesting-0.54/qcarchivetesting.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcarchivetesting
-Version: 0.53
+Version: 0.54
 Summary: A distributed compute and database platform for quantum chemistry.
 Author-email: Benjamin Pritchard <qcarchive@molssi.org>
 Project-URL: Homepage, https://github.com/MolSSI/QCFractal
 Project-URL: Bug Tracker, https://github.com/MolSSI/QCFractal/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `qcarchivetesting-0.53/qcarchivetesting.egg-info/SOURCES.txt` & `qcarchivetesting-0.54/qcarchivetesting.egg-info/SOURCES.txt`

 * *Files identical despite different names*

