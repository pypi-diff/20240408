# Comparing `tmp/mat3ra-esse-2024.4.8.post3.tar.gz` & `tmp/mat3ra-esse-2024.4.8.post4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mat3ra-esse-2024.4.8.post3.tar", last modified: Mon Apr  8 11:18:05 2024, max compression
+gzip compressed data, was "mat3ra-esse-2024.4.8.post4.tar", last modified: Mon Apr  8 11:31:48 2024, max compression
```

## Comparing `mat3ra-esse-2024.4.8.post3.tar` & `mat3ra-esse-2024.4.8.post4.tar`

### file list

```diff
@@ -1,1397 +1,1397 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.895683 mat3ra-esse-2024.4.8.post3/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-08 11:17:48.000000 mat3ra-esse-2024.4.8.post3/.babelrc
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-08 11:17:48.000000 mat3ra-esse-2024.4.8.post3/.eslintrc.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.679683 mat3ra-esse-2024.4.8.post3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.719683 mat3ra-esse-2024.4.8.post3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     5088 2024-04-08 11:17:48.000000 mat3ra-esse-2024.4.8.post3/.github/workflows/cicd.yml
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-08 11:17:48.000000 mat3ra-esse-2024.4.8.post3/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.719683 mat3ra-esse-2024.4.8.post3/.husky/
--rwxr-xr-x   0 runner    (1001) docker     (127)      792 2024-04-08 11:17:48.000000 mat3ra-esse-2024.4.8.post3/.husky/pre-commit
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-08 11:17:48.000000 mat3ra-esse-2024.4.8.post3/.mocharc.json
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-08 11:17:48.000000 mat3ra-esse-2024.4.8.post3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-08 11:17:48.000000 mat3ra-esse-2024.4.8.post3/.prettierrc
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-08 11:17:48.000000 mat3ra-esse-2024.4.8.post3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     8841 2024-04-08 11:18:05.895683 mat3ra-esse-2024.4.8.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-04-08 11:17:48.000000 mat3ra-esse-2024.4.8.post3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-04-08 11:17:48.000000 mat3ra-esse-2024.4.8.post3/build_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-08 11:17:48.000000 mat3ra-esse-2024.4.8.post3/build_schemas.ts
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-08 11:17:48.000000 mat3ra-esse-2024.4.8.post3/compile_ts.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.719683 mat3ra-esse-2024.4.8.post3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.719683 mat3ra-esse-2024.4.8.post3/example/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.683683 mat3ra-esse-2024.4.8.post3/example/3pse/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.679683 mat3ra-esse-2024.4.8.post3/example/3pse/db/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.683683 mat3ra-esse-2024.4.8.post3/example/3pse/db/nist_jarvis/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.719683 mat3ra-esse-2024.4.8.post3/example/3pse/db/nist_jarvis/2024.3.13/
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/3pse/db/nist_jarvis/2024.3.13/db_entry.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.683683 mat3ra-esse-2024.4.8.post3/example/3pse/file/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.683683 mat3ra-esse-2024.4.8.post3/example/3pse/file/applications/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.683683 mat3ra-esse-2024.4.8.post3/example/3pse/file/applications/espresso/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.723682 mat3ra-esse-2024.4.8.post3/example/3pse/file/applications/espresso/7.2/
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/3pse/file/applications/espresso/7.2/pw.x.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.723682 mat3ra-esse-2024.4.8.post3/example/core/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.723682 mat3ra-esse-2024.4.8.post3/example/core/abstract/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/core/abstract/2d_data.json
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/core/abstract/2d_plot.json
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/core/abstract/3d_grid.json
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/core/abstract/3d_tensor.json
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/core/abstract/3d_vector_basis.json
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/core/abstract/point.json
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/core/abstract/vector.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.723682 mat3ra-esse-2024.4.8.post3/example/core/primitive/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/core/primitive/1d_data_series.json
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/core/primitive/3d_lattice.json
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/core/primitive/array_of_3_booleans.json
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/core/primitive/array_of_3_numbers.json
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/core/primitive/array_of_ids.json
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/core/primitive/axis.json
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/core/primitive/scalar.json
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/core/primitive/string.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.723682 mat3ra-esse-2024.4.8.post3/example/core/reference/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.723682 mat3ra-esse-2024.4.8.post3/example/core/reference/experiment/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/core/reference/experiment/condition.json
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/core/reference/experiment/location.json
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/core/reference/experiment.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.723682 mat3ra-esse-2024.4.8.post3/example/core/reference/literature/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/core/reference/literature/name.json
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/core/reference/literature/pages.json
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/core/reference/literature.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.723682 mat3ra-esse-2024.4.8.post3/example/core/reference/modeling/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/core/reference/modeling/exabyte.json
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/core/reference/modeling.json
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/core/reference.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.723682 mat3ra-esse-2024.4.8.post3/example/core/reusable/
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/core/reusable/atomic_vectors.json
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/core/reusable/band_gap.json
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/core/reusable/energy.json
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/core/reusable/file_metadata.json
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/core/reusable/object_storage_container_data.json
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/element.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.723682 mat3ra-esse-2024.4.8.post3/example/job/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/job/compute.json
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/job.json
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/material.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.727683 mat3ra-esse-2024.4.8.post3/example/method/
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/method/categorized_method.json
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/method/method_parameters.json
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/method.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.683683 mat3ra-esse-2024.4.8.post3/example/methods_directory/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.727683 mat3ra-esse-2024.4.8.post3/example/methods_directory/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/methods_directory/legacy/localorbital.json
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/methods_directory/legacy/pseudopotential.json
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/methods_directory/legacy/regression.json
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/methods_directory/legacy/unknown.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.727683 mat3ra-esse-2024.4.8.post3/example/methods_directory/mathematical/
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/methods_directory/mathematical/cg.json
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/methods_directory/mathematical/regression.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.727683 mat3ra-esse-2024.4.8.post3/example/methods_directory/physical/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.727683 mat3ra-esse-2024.4.8.post3/example/methods_directory/physical/ao/
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/methods_directory/physical/ao/dunning.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.727683 mat3ra-esse-2024.4.8.post3/example/methods_directory/physical/psp/
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/methods_directory/physical/psp/file.json
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/methods_directory/physical/psp.json
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/methods_directory/physical/pw.json
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/methods_directory/physical/smearing.json
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/methods_directory/physical/tetrahedron.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.727683 mat3ra-esse-2024.4.8.post3/example/model/
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/model/categorized_model.json
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/model/model_parameters.json
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/model.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.683683 mat3ra-esse-2024.4.8.post3/example/models_category/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.683683 mat3ra-esse-2024.4.8.post3/example/models_category/pb/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.727683 mat3ra-esse-2024.4.8.post3/example/models_category/pb/qm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.727683 mat3ra-esse-2024.4.8.post3/example/models_category/pb/qm/abin/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/models_category/pb/qm/abin/gw.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.727683 mat3ra-esse-2024.4.8.post3/example/models_category/pb/qm/dft/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/models_category/pb/qm/dft/ksdft.json
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/models_category/pb/qm/semp.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.727683 mat3ra-esse-2024.4.8.post3/example/models_directory/
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/models_directory/gga.json
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/models_directory/gw.json
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/models_directory/hybrid.json
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/models_directory/lda.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.727683 mat3ra-esse-2024.4.8.post3/example/models_directory/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/models_directory/legacy/dft.json
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/models_directory/legacy/ml.json
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/models_directory/legacy/unknown.json
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/models_directory/re.json
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/project.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.727683 mat3ra-esse-2024.4.8.post3/example/properties_directory/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/properties_directory/electronic_configuration.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.731683 mat3ra-esse-2024.4.8.post3/example/properties_directory/elemental/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/properties_directory/elemental/atomic_radius.json
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/properties_directory/elemental/electronegativity.json
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/properties_directory/elemental/ionization_potential.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.731683 mat3ra-esse-2024.4.8.post3/example/properties_directory/non-scalar/
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/properties_directory/non-scalar/band_gaps.json
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/properties_directory/non-scalar/band_structure.json
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/properties_directory/non-scalar/charge_density_profile.json
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/properties_directory/non-scalar/density_of_states.json
--rw-r--r--   0 runner    (1001) docker     (127)     3326 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/properties_directory/non-scalar/dielectric_tensor.json
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/properties_directory/non-scalar/file_content.json
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/properties_directory/non-scalar/hubbard_u.json
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/properties_directory/non-scalar/hubbard_v.json
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/properties_directory/non-scalar/hubbard_v_nn.json
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/properties_directory/non-scalar/phonon_dispersions.json
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/properties_directory/non-scalar/phonon_dos.json
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/properties_directory/non-scalar/potential_profile.json
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/properties_directory/non-scalar/reaction_energy_profile.json
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/properties_directory/non-scalar/stress_tensor.json
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/properties_directory/non-scalar/total_energy_contributions.json
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/properties_directory/non-scalar/vibrational_spectrum.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.735683 mat3ra-esse-2024.4.8.post3/example/properties_directory/scalar/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/properties_directory/scalar/electron_affinity.json
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/properties_directory/scalar/fermi_energy.json
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/properties_directory/scalar/formation_energy.json
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/properties_directory/scalar/ionization_potential.json
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/properties_directory/scalar/pressure.json
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/properties_directory/scalar/reaction_energy_barrier.json
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/properties_directory/scalar/surface_energy.json
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/properties_directory/scalar/total_energy.json
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/properties_directory/scalar/total_force.json
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/properties_directory/scalar/valence_band_offset.json
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/properties_directory/scalar/zero_point_energy.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.735683 mat3ra-esse-2024.4.8.post3/example/properties_directory/structural/
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/properties_directory/structural/atomic_forces.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.735683 mat3ra-esse-2024.4.8.post3/example/properties_directory/structural/basis/
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/properties_directory/structural/basis/atomic_constraints.json
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/properties_directory/structural/basis/atomic_coordinate.json
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/properties_directory/structural/basis/atomic_coordinates.json
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/properties_directory/structural/basis/atomic_element.json
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/properties_directory/structural/basis/bonds.json
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/properties_directory/structural/basis.json
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/properties_directory/structural/density.json
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/properties_directory/structural/elemental_ratio.json
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/properties_directory/structural/inchi.json
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/properties_directory/structural/inchi_key.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.739683 mat3ra-esse-2024.4.8.post3/example/properties_directory/structural/lattice/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/properties_directory/structural/lattice/lattice_bravais.json
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/properties_directory/structural/lattice/lattice_vectors.json
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/properties_directory/structural/lattice.json
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/properties_directory/structural/magnetic_moments.json
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/properties_directory/structural/molecular_pattern.json
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/properties_directory/structural/p-norm.json
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/properties_directory/structural/symmetry.json
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/properties_directory/structural/volume.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.687682 mat3ra-esse-2024.4.8.post3/example/properties_directory/workflow/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.739683 mat3ra-esse-2024.4.8.post3/example/properties_directory/workflow/convergence/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/properties_directory/workflow/convergence/electronic.json
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/properties_directory/workflow/convergence/ionic.json
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/properties_directory/workflow/convergence/kpoint.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.739683 mat3ra-esse-2024.4.8.post3/example/property/
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/property/base.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.739683 mat3ra-esse-2024.4.8.post3/example/software/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/software/application.json
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/software/executable.json
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/software/flavor.json
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/software/template.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.687682 mat3ra-esse-2024.4.8.post3/example/software_directory/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.739683 mat3ra-esse-2024.4.8.post3/example/software_directory/ml/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/software_directory/ml/exabyteml.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.687682 mat3ra-esse-2024.4.8.post3/example/software_directory/ml/unit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.739683 mat3ra-esse-2024.4.8.post3/example/software_directory/ml/unit/execution/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.739683 mat3ra-esse-2024.4.8.post3/example/software_directory/ml/unit/execution/evaluate/
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/software_directory/ml/unit/execution/evaluate/cross-validate.json
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/software_directory/ml/unit/execution/initialize.json
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/software_directory/ml/unit/execution/score.json
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/software_directory/ml/unit/execution/train.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.687682 mat3ra-esse-2024.4.8.post3/example/software_directory/ml/unit/processing/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.739683 mat3ra-esse-2024.4.8.post3/example/software_directory/ml/unit/processing/data_transformation/
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/software_directory/ml/unit/processing/data_transformation/manipulation.json
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/software_directory/ml/unit/processing/data_transformation/scale_and_reduce.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.739683 mat3ra-esse-2024.4.8.post3/example/software_directory/ml/unit/processing/feature_selection/
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/software_directory/ml/unit/processing/feature_selection/filter_based.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.739683 mat3ra-esse-2024.4.8.post3/example/software_directory/modeling/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.739683 mat3ra-esse-2024.4.8.post3/example/software_directory/modeling/espresso/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/software_directory/modeling/espresso/arguments.json
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/software_directory/modeling/espresso.json
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/software_directory/modeling/nwchem.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.739683 mat3ra-esse-2024.4.8.post3/example/software_directory/modeling/unit/
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/software_directory/modeling/unit/execution.json
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/software_directory/modeling/vasp.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.743682 mat3ra-esse-2024.4.8.post3/example/software_directory/scripting/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/software_directory/scripting/jupyter-lab.json
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/software_directory/scripting/python.json
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/software_directory/scripting/shell.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.743682 mat3ra-esse-2024.4.8.post3/example/software_directory/scripting/unit/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/software_directory/scripting/unit/execution.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.743682 mat3ra-esse-2024.4.8.post3/example/system/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/system/_material.json
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/system/_parent_job.json
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/system/_project.json
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/system/consistency_check.json
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/system/creator.json
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/system/entity_reference.json
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/system/file_source.json
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/system/iframe_message.json
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/system/message.json
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/system/owner.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.743682 mat3ra-esse-2024.4.8.post3/example/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/workflow/subworkflow.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.743682 mat3ra-esse-2024.4.8.post3/example/workflow/unit/
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/workflow/unit/assignment.json
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/workflow/unit/condition.json
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/workflow/unit/execution.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.743682 mat3ra-esse-2024.4.8.post3/example/workflow/unit/input/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/workflow/unit/input/_inputItemScope.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.743682 mat3ra-esse-2024.4.8.post3/example/workflow/unit/io/
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/workflow/unit/io/api.json
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/workflow/unit/io/db.json
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/workflow/unit/io/object_storage.json
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/workflow/unit/io.json
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/workflow/unit/map.json
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/workflow/unit/processing.json
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/workflow/unit/reduce.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.743682 mat3ra-esse-2024.4.8.post3/example/workflow/unit/runtime/
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/workflow/unit/runtime/runtime_items.json
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/example/workflow.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.747683 mat3ra-esse-2024.4.8.post3/manifest/
--rw-r--r--   0 runner    (1001) docker     (127)     7807 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/manifest/dft_unit_functionals.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13108 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/manifest/functional_lookup_table.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9760 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/manifest/models.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5545 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/manifest/properties.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/npmignore
--rw-r--r--   0 runner    (1001) docker     (127)   341213 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/package.json
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.747683 mat3ra-esse-2024.4.8.post3/schema/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.687682 mat3ra-esse-2024.4.8.post3/schema/3pse/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.687682 mat3ra-esse-2024.4.8.post3/schema/3pse/db/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.687682 mat3ra-esse-2024.4.8.post3/schema/3pse/db/nist_jarvis/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.747683 mat3ra-esse-2024.4.8.post3/schema/3pse/db/nist_jarvis/2024.3.13/
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/3pse/db/nist_jarvis/2024.3.13/atoms.json
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/3pse/db/nist_jarvis/2024.3.13/db_entry.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.691683 mat3ra-esse-2024.4.8.post3/schema/3pse/file/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.691683 mat3ra-esse-2024.4.8.post3/schema/3pse/file/applications/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.691683 mat3ra-esse-2024.4.8.post3/schema/3pse/file/applications/espresso/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.747683 mat3ra-esse-2024.4.8.post3/schema/3pse/file/applications/espresso/7.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.747683 mat3ra-esse-2024.4.8.post3/schema/3pse/file/applications/espresso/7.2/pw.x/
--rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/3pse/file/applications/espresso/7.2/pw.x/atomic_positions.json
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/3pse/file/applications/espresso/7.2/pw.x/atomic_species.json
--rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/3pse/file/applications/espresso/7.2/pw.x/cell.json
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/3pse/file/applications/espresso/7.2/pw.x/cell_parameters.json
--rw-r--r--   0 runner    (1001) docker     (127)    10526 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/3pse/file/applications/espresso/7.2/pw.x/control.json
--rw-r--r--   0 runner    (1001) docker     (127)     6354 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/3pse/file/applications/espresso/7.2/pw.x/electrons.json
--rw-r--r--   0 runner    (1001) docker     (127)    11220 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/3pse/file/applications/espresso/7.2/pw.x/hubbard.json
--rw-r--r--   0 runner    (1001) docker     (127)     7549 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/3pse/file/applications/espresso/7.2/pw.x/ions.json
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/3pse/file/applications/espresso/7.2/pw.x/k_points.json
--rw-r--r--   0 runner    (1001) docker     (127)    25760 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/3pse/file/applications/espresso/7.2/pw.x/system.json
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/3pse/file/applications/espresso/7.2/pw.x.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.747683 mat3ra-esse-2024.4.8.post3/schema/core/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.751683 mat3ra-esse-2024.4.8.post3/schema/core/abstract/
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/core/abstract/2d_data.json
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/core/abstract/2d_plot.json
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/core/abstract/3d_grid.json
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/core/abstract/3d_tensor.json
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/core/abstract/3d_vector_basis.json
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/core/abstract/point.json
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/core/abstract/vector.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.751683 mat3ra-esse-2024.4.8.post3/schema/core/primitive/
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/core/primitive/1d_data_series.json
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/core/primitive/3d_lattice.json
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/core/primitive/array_of_3_booleans.json
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/core/primitive/array_of_3_numbers.json
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/core/primitive/array_of_ids.json
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/core/primitive/array_of_strings.json
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/core/primitive/axis.json
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/core/primitive/group_info.json
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/core/primitive/integer_one_or_zero.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.751683 mat3ra-esse-2024.4.8.post3/schema/core/primitive/linked_list/
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/core/primitive/linked_list/base_node.json
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/core/primitive/linked_list/named_node.json
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/core/primitive/linked_list/named_node_in_group.json
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/core/primitive/linked_list/node_with_type.json
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/core/primitive/linked_list.json
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/core/primitive/scalar.json
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/core/primitive/slugified_entry.json
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/core/primitive/slugified_entry_or_slug.json
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/core/primitive/string.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.755683 mat3ra-esse-2024.4.8.post3/schema/core/reference/
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/core/reference/exabyte.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.755683 mat3ra-esse-2024.4.8.post3/schema/core/reference/experiment/
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/core/reference/experiment/condition.json
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/core/reference/experiment/location.json
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/core/reference/experiment.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.755683 mat3ra-esse-2024.4.8.post3/schema/core/reference/literature/
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/core/reference/literature/name.json
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/core/reference/literature/pages.json
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/core/reference/literature.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.755683 mat3ra-esse-2024.4.8.post3/schema/core/reference/modeling/
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/core/reference/modeling/exabyte.json
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/core/reference/modeling.json
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/core/reference.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.755683 mat3ra-esse-2024.4.8.post3/schema/core/reusable/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.759683 mat3ra-esse-2024.4.8.post3/schema/core/reusable/atomic_data/
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/core/reusable/atomic_data/per_orbital.json
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/core/reusable/atomic_data/per_orbital_pair.json
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/core/reusable/atomic_data/value_number.json
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/core/reusable/atomic_data/value_string.json
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/core/reusable/atomic_data_per_orbital_numeric.json
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/core/reusable/atomic_data_per_orbital_pair_numeric.json
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/core/reusable/atomic_orbital.json
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/core/reusable/atomic_scalars.json
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/core/reusable/atomic_strings.json
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/core/reusable/atomic_vectors.json
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/core/reusable/band_gap.json
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/core/reusable/categories.json
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/core/reusable/category_path.json
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/core/reusable/dielectric_tensor_component.json
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/core/reusable/energy.json
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/core/reusable/file_metadata.json
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/core/reusable/frequency_function_matrix.json
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/core/reusable/object_storage_container_data.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.759683 mat3ra-esse-2024.4.8.post3/schema/definitions/
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/definitions/units.json
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/element.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.759683 mat3ra-esse-2024.4.8.post3/schema/in_memory_entity/
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/in_memory_entity/base.json
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/in_memory_entity/defaultable.json
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/in_memory_entity/named.json
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/in_memory_entity/named_defaultable.json
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/in_memory_entity/named_defaultable_has_metadata.json
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/in_memory_entity/named_defaultable_runtime_items.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.759683 mat3ra-esse-2024.4.8.post3/schema/job/
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/job/base.json
--rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/job/compute.json
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/job.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.759683 mat3ra-esse-2024.4.8.post3/schema/material/
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/material/conventional.json
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/material.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.759683 mat3ra-esse-2024.4.8.post3/schema/method/
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/method/categorized_method.json
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/method/method_parameters.json
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/method/unit_method.json
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/method.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.695683 mat3ra-esse-2024.4.8.post3/schema/methods_category/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.759683 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.759683 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/diff/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/diff/enum_options.json
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/diff/enum_options.yml
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/diff/fd.json
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/diff.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.763683 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/discr/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/discr/enum_options.json
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/discr/enum_options.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.763683 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/discr/mesh/
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/discr/mesh/enum_options.json
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/discr/mesh/enum_options.yml
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/discr/mesh/hybrid.json
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/discr/mesh/nstruct.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.763683 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/discr/mesh/struct/
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/discr/mesh/struct/cartesian.json
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/discr/mesh/struct/enum_options.json
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/discr/mesh/struct/enum_options.yml
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/discr/mesh/struct.json
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/discr/mesh.json
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/discr.json
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/enum_options.json
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/enum_options.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.763683 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/fapprx/
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/fapprx/basisexp.json
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/fapprx/enum_options.json
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/fapprx/enum_options.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.763683 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/fapprx/ipol/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/fapprx/ipol/enum_options.json
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/fapprx/ipol/enum_options.yml
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/fapprx/ipol/lin.json
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/fapprx/ipol/poly.json
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/fapprx/ipol/spline.json
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/fapprx/ipol.json
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/fapprx.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.767683 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/intgr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.767683 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/intgr/analytic/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/intgr/analytic/enum_options.json
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/intgr/analytic/enum_options.yml
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/intgr/analytic/volume.json
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/intgr/analytic.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.767683 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/intgr/diffeq/
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/intgr/diffeq/enum_options.json
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/intgr/diffeq/enum_options.yml
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/intgr/diffeq/order1.json
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/intgr/diffeq/order2.json
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/intgr/diffeq.json
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/intgr/enum_options.json
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/intgr/enum_options.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.767683 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/intgr/numquad/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/intgr/numquad/enum_options.json
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/intgr/numquad/enum_options.yml
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/intgr/numquad/gauss.json
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/intgr/numquad/newcot.json
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/intgr/numquad.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.767683 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/intgr/transf/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/intgr/transf/enum_options.json
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/intgr/transf/enum_options.yml
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/intgr/transf/fourier.json
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/intgr/transf.json
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/intgr.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.767683 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/linalg/
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/linalg/dcomp.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.767683 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/linalg/diag/
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/linalg/diag/davidson.json
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/linalg/diag/enum_options.json
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/linalg/diag/enum_options.yml
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/linalg/diag.json
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/linalg/enum_options.json
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/linalg/enum_options.yml
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/linalg/lintra.json
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/linalg/matf.json
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/linalg.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.771683 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/opt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.771683 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/opt/diff/
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/opt/diff/bracket.json
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/opt/diff/enum_options.json
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/opt/diff/enum_options.yml
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/opt/diff/local.json
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/opt/diff/order1.json
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/opt/diff/order2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.771683 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/opt/diff/ordern/
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/opt/diff/ordern/cg.json
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/opt/diff/ordern/enum_options.json
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/opt/diff/ordern/enum_options.yml
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/opt/diff/ordern.json
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/opt/diff.json
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/opt/enum_options.json
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/opt/enum_options.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.771683 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/opt/ndiff/
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/opt/ndiff/direct.json
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/opt/ndiff/enum_options.json
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/opt/ndiff/enum_options.yml
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/opt/ndiff/pop.json
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/opt/ndiff/stoch.json
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/opt/ndiff.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.771683 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/opt/root/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/opt/root/bracket.json
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/opt/root/enum_options.json
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/opt/root/enum_options.yml
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/opt/root/iter.json
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/opt/root.json
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/opt.json
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/regression.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.775683 mat3ra-esse-2024.4.8.post3/schema/methods_category/physical/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/physical/enum_options.json
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/physical/enum_options.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.775683 mat3ra-esse-2024.4.8.post3/schema/methods_category/physical/qm/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/physical/qm/enum_options.json
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/physical/qm/enum_options.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.775683 mat3ra-esse-2024.4.8.post3/schema/methods_category/physical/qm/wf/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.775683 mat3ra-esse-2024.4.8.post3/schema/methods_category/physical/qm/wf/ao/
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/physical/qm/wf/ao/dunning.json
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/physical/qm/wf/ao/other.json
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/physical/qm/wf/ao/pople.json
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/physical/qm/wf/ao.json
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/physical/qm/wf/enum_options.json
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/physical/qm/wf/enum_options.yml
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/physical/qm/wf/psp.json
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/physical/qm/wf/pw.json
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/physical/qm/wf/smearing.json
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/physical/qm/wf/tetrahedron.json
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/physical/qm/wf.json
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_category/physical/qm.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.695683 mat3ra-esse-2024.4.8.post3/schema/methods_directory/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.775683 mat3ra-esse-2024.4.8.post3/schema/methods_directory/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_directory/legacy/localorbital.json
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_directory/legacy/pseudopotential.json
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_directory/legacy/regression.json
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_directory/legacy/unknown.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.775683 mat3ra-esse-2024.4.8.post3/schema/methods_directory/mathematical/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_directory/mathematical/cg.json
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_directory/mathematical/davidson.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.779682 mat3ra-esse-2024.4.8.post3/schema/methods_directory/mathematical/regression/
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_directory/mathematical/regression/data.json
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_directory/mathematical/regression/dataset.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.779682 mat3ra-esse-2024.4.8.post3/schema/methods_directory/mathematical/regression/kernel_ridge/
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_directory/mathematical/regression/kernel_ridge/data_per_property.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.779682 mat3ra-esse-2024.4.8.post3/schema/methods_directory/mathematical/regression/linear/
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_directory/mathematical/regression/linear/data_per_property.json
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_directory/mathematical/regression/per_feature_item.json
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_directory/mathematical/regression/precision.json
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_directory/mathematical/regression/precision_per_property.json
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_directory/mathematical/regression.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.779682 mat3ra-esse-2024.4.8.post3/schema/methods_directory/physical/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.779682 mat3ra-esse-2024.4.8.post3/schema/methods_directory/physical/ao/
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_directory/physical/ao/dunning.json
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_directory/physical/ao/enum_options.json
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_directory/physical/ao/enum_options.yml
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_directory/physical/ao/other.json
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_directory/physical/ao/pople.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.779682 mat3ra-esse-2024.4.8.post3/schema/methods_directory/physical/psp/
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_directory/physical/psp/file.json
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_directory/physical/psp/file_data_item.json
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_directory/physical/psp.json
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_directory/physical/pw.json
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_directory/physical/smearing.json
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/methods_directory/physical/tetrahedron.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.779682 mat3ra-esse-2024.4.8.post3/schema/model/
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/model/categorized_model.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.779682 mat3ra-esse-2024.4.8.post3/schema/model/mixins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.783683 mat3ra-esse-2024.4.8.post3/schema/model/mixins/dft/
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/model/mixins/dft/double_hybrid_functional.json
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/model/mixins/dft/enum_options.json
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/model/mixins/dft/enum_options.yml
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/model/mixins/dft/gga_functional.json
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/model/mixins/dft/hybrid_functional.json
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/model/mixins/dft/lda_functional.json
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/model/mixins/dft/mgga_functional.json
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/model/mixins/dispersion_correction.json
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/model/mixins/enum_options.json
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/model/mixins/enum_options.yml
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/model/mixins/hubbard.json
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/model/mixins/spin_orbit_coupling.json
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/model/mixins/spin_polarization.json
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/model/model_parameters.json
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/model/model_without_method.json
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/model.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.783683 mat3ra-esse-2024.4.8.post3/schema/models_category/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/models_category/enum_options.json
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/models_category/enum_options.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.783683 mat3ra-esse-2024.4.8.post3/schema/models_category/pb/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/models_category/pb/enum_options.json
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/models_category/pb/enum_options.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.783683 mat3ra-esse-2024.4.8.post3/schema/models_category/pb/qm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.783683 mat3ra-esse-2024.4.8.post3/schema/models_category/pb/qm/abin/
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/models_category/pb/qm/abin/enum_options.json
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/models_category/pb/qm/abin/enum_options.yml
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/models_category/pb/qm/abin/gw.json
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/models_category/pb/qm/abin.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.783683 mat3ra-esse-2024.4.8.post3/schema/models_category/pb/qm/dft/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/models_category/pb/qm/dft/enum_options.json
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/models_category/pb/qm/dft/enum_options.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.787683 mat3ra-esse-2024.4.8.post3/schema/models_category/pb/qm/dft/ksdft/
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/models_category/pb/qm/dft/ksdft/double_hybrid.json
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/models_category/pb/qm/dft/ksdft/enum_options.json
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/models_category/pb/qm/dft/ksdft/enum_options.yml
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/models_category/pb/qm/dft/ksdft/gga.json
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/models_category/pb/qm/dft/ksdft/hybrid.json
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/models_category/pb/qm/dft/ksdft/lda.json
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/models_category/pb/qm/dft/ksdft/mgga.json
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/models_category/pb/qm/dft/ksdft.json
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/models_category/pb/qm/dft.json
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/models_category/pb/qm/enum_options.json
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/models_category/pb/qm/enum_options.yml
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/models_category/pb/qm/semp.json
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/models_category/pb/qm.json
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/models_category/pb.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.787683 mat3ra-esse-2024.4.8.post3/schema/models_category/st/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.787683 mat3ra-esse-2024.4.8.post3/schema/models_category/st/det/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/models_category/st/det/enum_options.json
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/models_category/st/det/enum_options.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.787683 mat3ra-esse-2024.4.8.post3/schema/models_category/st/det/ml/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/models_category/st/det/ml/enum_options.json
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/models_category/st/det/ml/enum_options.yml
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/models_category/st/det/ml/re.json
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/models_category/st/det/ml.json
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/models_category/st/det.json
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/models_category/st/enum_options.json
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/models_category/st/enum_options.yml
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/models_category/st.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.787683 mat3ra-esse-2024.4.8.post3/schema/models_directory/
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/models_directory/double_hybrid.json
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/models_directory/gga.json
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/models_directory/gw.json
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/models_directory/hybrid.json
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/models_directory/lda.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.787683 mat3ra-esse-2024.4.8.post3/schema/models_directory/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/models_directory/legacy/dft.json
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/models_directory/legacy/ml.json
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/models_directory/legacy/unknown.json
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/models_directory/mgga.json
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/models_directory/re.json
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/project.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.787683 mat3ra-esse-2024.4.8.post3/schema/properties_directory/
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/properties_directory/derived_properties.json
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/properties_directory/electronic_configuration.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.791683 mat3ra-esse-2024.4.8.post3/schema/properties_directory/elemental/
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/properties_directory/elemental/atomic_radius.json
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/properties_directory/elemental/electronegativity.json
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/properties_directory/elemental/ionization_potential.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.791683 mat3ra-esse-2024.4.8.post3/schema/properties_directory/non-scalar/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/properties_directory/non-scalar/average_potential_profile.json
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/properties_directory/non-scalar/band_gaps.json
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/properties_directory/non-scalar/band_structure.json
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/properties_directory/non-scalar/charge_density_profile.json
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/properties_directory/non-scalar/density_of_states.json
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/properties_directory/non-scalar/dielectric_tensor.json
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/properties_directory/non-scalar/file_content.json
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/properties_directory/non-scalar/hubbard_u.json
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/properties_directory/non-scalar/hubbard_v.json
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/properties_directory/non-scalar/hubbard_v_nn.json
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/properties_directory/non-scalar/phonon_dispersions.json
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/properties_directory/non-scalar/phonon_dos.json
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/properties_directory/non-scalar/potential_profile.json
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/properties_directory/non-scalar/reaction_energy_profile.json
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/properties_directory/non-scalar/stress_tensor.json
--rw-r--r--   0 runner    (1001) docker     (127)     6418 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/properties_directory/non-scalar/total_energy_contributions.json
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/properties_directory/non-scalar/vibrational_spectrum.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.795683 mat3ra-esse-2024.4.8.post3/schema/properties_directory/scalar/
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/properties_directory/scalar/electron_affinity.json
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/properties_directory/scalar/fermi_energy.json
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/properties_directory/scalar/formation_energy.json
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/properties_directory/scalar/ionization_potential.json
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/properties_directory/scalar/pressure.json
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/properties_directory/scalar/reaction_energy_barrier.json
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/properties_directory/scalar/surface_energy.json
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/properties_directory/scalar/total_energy.json
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/properties_directory/scalar/total_force.json
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/properties_directory/scalar/valence_band_offset.json
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/properties_directory/scalar/zero_point_energy.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.795683 mat3ra-esse-2024.4.8.post3/schema/properties_directory/structural/
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/properties_directory/structural/atomic_forces.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.795683 mat3ra-esse-2024.4.8.post3/schema/properties_directory/structural/basis/
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/properties_directory/structural/basis/atomic_constraints.json
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/properties_directory/structural/basis/atomic_coordinate.json
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/properties_directory/structural/basis/atomic_coordinates.json
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/properties_directory/structural/basis/atomic_element.json
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/properties_directory/structural/basis/bonds.json
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/properties_directory/structural/basis.json
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/properties_directory/structural/density.json
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/properties_directory/structural/elemental_ratio.json
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/properties_directory/structural/inchi.json
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/properties_directory/structural/inchi_key.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.799683 mat3ra-esse-2024.4.8.post3/schema/properties_directory/structural/lattice/
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/properties_directory/structural/lattice/lattice_bravais.json
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/properties_directory/structural/lattice/lattice_vectors.json
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/properties_directory/structural/lattice/type_enum.json
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/properties_directory/structural/lattice/type_extended_enum.json
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/properties_directory/structural/lattice.json
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/properties_directory/structural/magnetic_moments.json
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/properties_directory/structural/molecular_pattern.json
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/properties_directory/structural/p-norm.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.799683 mat3ra-esse-2024.4.8.post3/schema/properties_directory/structural/patterns/
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/properties_directory/structural/patterns/functional_group.json
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/properties_directory/structural/patterns/ring.json
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/properties_directory/structural/patterns/special_bond.json
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/properties_directory/structural/symmetry.json
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/properties_directory/structural/volume.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.699683 mat3ra-esse-2024.4.8.post3/schema/properties_directory/workflow/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.799683 mat3ra-esse-2024.4.8.post3/schema/properties_directory/workflow/convergence/
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/properties_directory/workflow/convergence/electronic.json
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/properties_directory/workflow/convergence/ionic.json
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/properties_directory/workflow/convergence/kpoint.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.799683 mat3ra-esse-2024.4.8.post3/schema/property/
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/property/base.json
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/property/meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/property/raw.json
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/property/source.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.799683 mat3ra-esse-2024.4.8.post3/schema/software/
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/software/application.json
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/software/executable.json
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/software/flavor.json
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/software/template.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.703683 mat3ra-esse-2024.4.8.post3/schema/software_directory/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.799683 mat3ra-esse-2024.4.8.post3/schema/software_directory/ml/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/software_directory/ml/exabyteml.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.799683 mat3ra-esse-2024.4.8.post3/schema/software_directory/ml/unit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.799683 mat3ra-esse-2024.4.8.post3/schema/software_directory/ml/unit/execution/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.799683 mat3ra-esse-2024.4.8.post3/schema/software_directory/ml/unit/execution/evaluate/
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/software_directory/ml/unit/execution/evaluate/cross-validate.json
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/software_directory/ml/unit/execution/initialize.json
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/software_directory/ml/unit/execution/score.json
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/software_directory/ml/unit/execution/train.json
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/software_directory/ml/unit/execution.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.799683 mat3ra-esse-2024.4.8.post3/schema/software_directory/ml/unit/processing/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.803683 mat3ra-esse-2024.4.8.post3/schema/software_directory/ml/unit/processing/data_transformation/
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/software_directory/ml/unit/processing/data_transformation/manipulation.json
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/software_directory/ml/unit/processing/data_transformation/scale_and_reduce.json
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/software_directory/ml/unit/processing/data_transformation.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.803683 mat3ra-esse-2024.4.8.post3/schema/software_directory/ml/unit/processing/feature_selection/
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/software_directory/ml/unit/processing/feature_selection/filter_based.json
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/software_directory/ml/unit/processing/feature_selection.json
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/software_directory/ml/unit/processing.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.803683 mat3ra-esse-2024.4.8.post3/schema/software_directory/modeling/
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/software_directory/modeling/deepmd.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.803683 mat3ra-esse-2024.4.8.post3/schema/software_directory/modeling/espresso/
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/software_directory/modeling/espresso/arguments.json
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/software_directory/modeling/espresso.json
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/software_directory/modeling/nwchem.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.803683 mat3ra-esse-2024.4.8.post3/schema/software_directory/modeling/unit/
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/software_directory/modeling/unit/execution.json
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/software_directory/modeling/vasp.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.803683 mat3ra-esse-2024.4.8.post3/schema/software_directory/scripting/
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/software_directory/scripting/jupyter-lab.json
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/software_directory/scripting/python.json
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/software_directory/scripting/shell.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.803683 mat3ra-esse-2024.4.8.post3/schema/software_directory/scripting/unit/
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/software_directory/scripting/unit/execution.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.807683 mat3ra-esse-2024.4.8.post3/schema/system/
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/system/_material.json
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/system/_parent_job.json
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/system/_project.json
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/system/bankable.json
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/system/consistency_check.json
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/system/creator.json
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/system/creator_account.json
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/system/database_source.json
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/system/defaultable.json
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/system/description.json
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/system/entity_reference.json
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/system/file_source.json
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/system/history.json
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/system/iframe_message.json
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/system/in_set.json
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/system/is_multi_material.json
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/system/is_outdated.json
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/system/job_extended.json
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/system/message.json
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/system/metadata.json
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/system/name.json
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/system/owner.json
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/system/path.json
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/system/path_entity.json
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/system/schema_version.json
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/system/scope.json
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/system/set.json
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/system/sharing.json
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/system/soft_removable.json
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/system/status.json
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/system/tags.json
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/system/timestampable.json
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/system/use_values.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.807683 mat3ra-esse-2024.4.8.post3/schema/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/workflow/base.json
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/workflow/base_flow.json
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/workflow/scope.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.807683 mat3ra-esse-2024.4.8.post3/schema/workflow/subworkflow/
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/workflow/subworkflow/unit.json
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/workflow/subworkflow.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.811683 mat3ra-esse-2024.4.8.post3/schema/workflow/unit/
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/workflow/unit/assertion.json
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/workflow/unit/assignment.json
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/workflow/unit/base.json
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/workflow/unit/condition.json
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/workflow/unit/execution.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.811683 mat3ra-esse-2024.4.8.post3/schema/workflow/unit/input/
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/workflow/unit/input/_input.json
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/workflow/unit/input/_inputItem.json
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/workflow/unit/input/_inputItemId.json
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/workflow/unit/input/_inputItemScope.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.811683 mat3ra-esse-2024.4.8.post3/schema/workflow/unit/input/_map_input/
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/workflow/unit/input/_map_input/values.json
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/workflow/unit/input/_map_input.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.811683 mat3ra-esse-2024.4.8.post3/schema/workflow/unit/io/
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/workflow/unit/io/api.json
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/workflow/unit/io/db.json
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/workflow/unit/io/object_storage.json
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/workflow/unit/io.json
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/workflow/unit/map.json
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/workflow/unit/processing.json
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/workflow/unit/reduce.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.811683 mat3ra-esse-2024.4.8.post3/schema/workflow/unit/runtime/
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/workflow/unit/runtime/_runtime_item_full_object.json
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/workflow/unit/runtime/_runtime_item_name_object.json
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/workflow/unit/runtime/_runtime_item_string.json
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/workflow/unit/runtime/runtime_item.json
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/workflow/unit/runtime/runtime_items.json
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/workflow/unit/subworkflow.json
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/workflow/unit.json
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/schema/workflow.json
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/set_schema_ids.ts
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 11:18:05.895683 mat3ra-esse-2024.4.8.post3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.811683 mat3ra-esse-2024.4.8.post3/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.703683 mat3ra-esse-2024.4.8.post3/src/js/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.815683 mat3ra-esse-2024.4.8.post3/src/js/esse/
--rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/js/esse/JSONSchemasGenerator.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/js/esse/JSONSchemasInterface.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/js/esse/JSONSchemasInterfaceServer.ts
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/js/esse/schemaUtils.ts
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/js/esse/settings.ts
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/js/esse/types.ts
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/js/esse/utils.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.815683 mat3ra-esse-2024.4.8.post3/src/js/json_include/
--rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/js/json_include/index.ts
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/js/json_include/settings.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.815683 mat3ra-esse-2024.4.8.post3/src/js/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/js/scripts/compileTs.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/js/scripts/createEnumsFromYaml.ts
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/js/scripts/setSchemaIds.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.815683 mat3ra-esse-2024.4.8.post3/src/js/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/js/utils/ajv.ts
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/js/utils/common.ts
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/js/utils/filesystem.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.815683 mat3ra-esse-2024.4.8.post3/src/py/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.815683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.815683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.815683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45982 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/data/examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     6099 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/data/properties.py
--rw-r--r--   0 runner    (1001) docker     (127)  1711304 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/data/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.819683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.819683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.819683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/abstract/
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/abstract/2d_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/abstract/2d_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/abstract/3d_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/abstract/3d_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/abstract/3d_vector_basis.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/abstract/point.py
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/abstract/vector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.823683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/primitive/
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/primitive/1d_data_series.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/primitive/3d_lattice.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/primitive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/primitive/array_of_3_booleans.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/primitive/array_of_3_numbers.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/primitive/array_of_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/primitive/array_of_strings.py
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/primitive/axis.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/primitive/group_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/primitive/integer_one_or_zero.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.823683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/primitive/linked_list/
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/primitive/linked_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/primitive/linked_list/base_node.py
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/primitive/linked_list/named_node.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/primitive/linked_list/named_node_in_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/primitive/linked_list/node_with_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/primitive/scalar.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/primitive/slugified_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/primitive/slugified_entry_or_slug.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/primitive/string.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.823683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/reference/
--rw-r--r--   0 runner    (1001) docker     (127)     6447 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/reference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/reference/exabyte.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.823683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/reference/experiment/
--rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/reference/experiment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/reference/experiment/condition.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/reference/experiment/location.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.823683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/reference/literature/
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/reference/literature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/reference/literature/name.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/reference/literature/pages.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.823683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/reference/modeling/
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/reference/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/reference/modeling/exabyte.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.827683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/reusable/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/reusable/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.827683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/reusable/atomic_data/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/reusable/atomic_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/reusable/atomic_data/per_orbital.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/reusable/atomic_data/per_orbital_pair.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/reusable/atomic_data/value_number.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/reusable/atomic_data/value_string.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/reusable/atomic_data_per_orbital_numeric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/reusable/atomic_data_per_orbital_pair_numeric.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/reusable/atomic_orbital.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/reusable/atomic_scalars.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/reusable/atomic_strings.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/reusable/atomic_vectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/reusable/band_gap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/reusable/categories.py
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/reusable/category_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/reusable/dielectric_tensor_component.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/reusable/energy.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/reusable/file_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/reusable/frequency_function_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/reusable/object_storage_container_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.827683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/definitions/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/definitions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/definitions/units.py
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/element.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.831683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/in_memory_entity/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/in_memory_entity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/in_memory_entity/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/in_memory_entity/defaultable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/in_memory_entity/named.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/in_memory_entity/named_defaultable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/in_memory_entity/named_defaultable_has_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/in_memory_entity/named_defaultable_runtime_items.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.831683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/job/
--rw-r--r--   0 runner    (1001) docker     (127)    82278 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8888 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/job/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/job/compute.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.831683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/material/
--rw-r--r--   0 runner    (1001) docker     (127)    10087 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/material/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/material/conventional.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.831683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/method/
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/method/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/method/categorized_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/method/method_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/method/unit_method.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.707682 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.831683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.831683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/diff/
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/diff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/diff/enum_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/diff/fd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.831683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/discr/
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/discr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/discr/enum_options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.831683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/discr/mesh/
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/discr/mesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/discr/mesh/enum_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/discr/mesh/hybrid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/discr/mesh/nstruct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.835683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/discr/mesh/struct/
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/discr/mesh/struct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/discr/mesh/struct/cartesian.py
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/discr/mesh/struct/enum_options.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/enum_options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.835683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/fapprx/
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/fapprx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/fapprx/basisexp.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/fapprx/enum_options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.835683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/fapprx/ipol/
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/fapprx/ipol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/fapprx/ipol/enum_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/fapprx/ipol/lin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/fapprx/ipol/poly.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/fapprx/ipol/spline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.835683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.835683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/analytic/
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/analytic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/analytic/enum_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/analytic/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.835683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/diffeq/
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/diffeq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/diffeq/enum_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/diffeq/order1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/diffeq/order2.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/enum_options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.835683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/numquad/
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/numquad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/numquad/enum_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/numquad/gauss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/numquad/newcot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.839683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/transf/
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/transf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/transf/enum_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/transf/fourier.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.839683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/linalg/
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/linalg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/linalg/dcomp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.839683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/linalg/diag/
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/linalg/diag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/linalg/diag/davidson.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/linalg/diag/enum_options.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/linalg/enum_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/linalg/lintra.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/linalg/matf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.839683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/opt/
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/opt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.839683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/opt/diff/
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/opt/diff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/opt/diff/bracket.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/opt/diff/enum_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/opt/diff/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/opt/diff/order1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/opt/diff/order2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.839683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/opt/diff/ordern/
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/opt/diff/ordern/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/opt/diff/ordern/cg.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/opt/diff/ordern/enum_options.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/opt/enum_options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.843683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/opt/ndiff/
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/opt/ndiff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/opt/ndiff/direct.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/opt/ndiff/enum_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/opt/ndiff/pop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/opt/ndiff/stoch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.843683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/opt/root/
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/opt/root/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/opt/root/bracket.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/opt/root/enum_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/opt/root/iter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/regression.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.843683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/physical/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/physical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/physical/enum_options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.843683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/physical/qm/
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/physical/qm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/physical/qm/enum_options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.843683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/physical/qm/wf/
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/physical/qm/wf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.843683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/physical/qm/wf/ao/
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/physical/qm/wf/ao/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/physical/qm/wf/ao/dunning.py
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/physical/qm/wf/ao/other.py
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/physical/qm/wf/ao/pople.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/physical/qm/wf/enum_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/physical/qm/wf/psp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/physical/qm/wf/pw.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/physical/qm/wf/smearing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/physical/qm/wf/tetrahedron.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.711683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.843683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/legacy/localorbital.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/legacy/pseudopotential.py
--rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/legacy/regression.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/legacy/unknown.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.847683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/mathematical/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/mathematical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/mathematical/cg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/mathematical/davidson.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.847683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/mathematical/regression/
--rw-r--r--   0 runner    (1001) docker     (127)     4412 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/mathematical/regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/mathematical/regression/data.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/mathematical/regression/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.847683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/mathematical/regression/kernel_ridge/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/mathematical/regression/kernel_ridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/mathematical/regression/kernel_ridge/data_per_property.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.847683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/mathematical/regression/linear/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/mathematical/regression/linear/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/mathematical/regression/linear/data_per_property.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/mathematical/regression/per_feature_item.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/mathematical/regression/precision.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/mathematical/regression/precision_per_property.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.847683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/physical/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/physical/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.847683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/physical/ao/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/physical/ao/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/physical/ao/dunning.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/physical/ao/enum_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/physical/ao/other.py
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/physical/ao/pople.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.847683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/physical/psp/
--rw-r--r--   0 runner    (1001) docker     (127)     4792 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/physical/psp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/physical/psp/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/physical/psp/file_data_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/physical/pw.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/physical/smearing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/physical/tetrahedron.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.851683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/model/
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6271 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/model/categorized_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.851683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/model/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/model/mixins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.851683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/model/mixins/dft/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/model/mixins/dft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/model/mixins/dft/double_hybrid_functional.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/model/mixins/dft/enum_options.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/model/mixins/dft/gga_functional.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/model/mixins/dft/hybrid_functional.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/model/mixins/dft/lda_functional.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/model/mixins/dft/mgga_functional.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/model/mixins/dispersion_correction.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/model/mixins/enum_options.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/model/mixins/hubbard.py
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/model/mixins/spin_orbit_coupling.py
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/model/mixins/spin_polarization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/model/model_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/model/model_without_method.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.851683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_category/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_category/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_category/enum_options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.851683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_category/pb/
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_category/pb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_category/pb/enum_options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.851683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_category/pb/qm/
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_category/pb/qm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.855683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_category/pb/qm/abin/
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_category/pb/qm/abin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_category/pb/qm/abin/enum_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_category/pb/qm/abin/gw.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.855683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_category/pb/qm/dft/
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_category/pb/qm/dft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_category/pb/qm/dft/enum_options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.855683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_category/pb/qm/dft/ksdft/
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_category/pb/qm/dft/ksdft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_category/pb/qm/dft/ksdft/double_hybrid.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_category/pb/qm/dft/ksdft/enum_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_category/pb/qm/dft/ksdft/gga.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_category/pb/qm/dft/ksdft/hybrid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_category/pb/qm/dft/ksdft/lda.py
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_category/pb/qm/dft/ksdft/mgga.py
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_category/pb/qm/enum_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_category/pb/qm/semp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.855683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_category/st/
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_category/st/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.855683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_category/st/det/
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_category/st/det/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_category/st/det/enum_options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.855683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_category/st/det/ml/
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_category/st/det/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_category/st/det/ml/enum_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_category/st/det/ml/re.py
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_category/st/enum_options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.859683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_directory/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_directory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_directory/double_hybrid.py
--rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_directory/gga.py
--rw-r--r--   0 runner    (1001) docker     (127)     7149 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_directory/gw.py
--rw-r--r--   0 runner    (1001) docker     (127)     5675 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_directory/hybrid.py
--rw-r--r--   0 runner    (1001) docker     (127)     5757 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_directory/lda.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.859683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_directory/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_directory/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_directory/legacy/dft.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_directory/legacy/ml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_directory/legacy/unknown.py
--rw-r--r--   0 runner    (1001) docker     (127)     5793 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_directory/mgga.py
--rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_directory/re.py
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/project.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.859683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/derived_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/electronic_configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.859683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/elemental/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/elemental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/elemental/atomic_radius.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/elemental/electronegativity.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/elemental/ionization_potential.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.863683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/non_scalar/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/non_scalar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/non_scalar/average_potential_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/non_scalar/band_gaps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/non_scalar/band_structure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/non_scalar/charge_density_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/non_scalar/density_of_states.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/non_scalar/dielectric_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/non_scalar/file_content.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/non_scalar/hubbard_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/non_scalar/hubbard_v.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/non_scalar/hubbard_v_nn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/non_scalar/phonon_dispersions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/non_scalar/phonon_dos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/non_scalar/potential_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/non_scalar/reaction_energy_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/non_scalar/stress_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/non_scalar/total_energy_contributions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/non_scalar/vibrational_spectrum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.863683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/scalar/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/scalar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/scalar/electron_affinity.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/scalar/fermi_energy.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/scalar/formation_energy.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/scalar/ionization_potential.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/scalar/pressure.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/scalar/reaction_energy_barrier.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/scalar/surface_energy.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/scalar/total_energy.py
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/scalar/total_force.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/scalar/valence_band_offset.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/scalar/zero_point_energy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.867683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/structural/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/structural/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/structural/atomic_forces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.867683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/structural/basis/
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/structural/basis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/structural/basis/atomic_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/structural/basis/atomic_coordinate.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/structural/basis/atomic_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/structural/basis/atomic_element.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/structural/basis/bonds.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/structural/density.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/structural/elemental_ratio.py
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/structural/inchi.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/structural/inchi_key.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.867683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/structural/lattice/
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/structural/lattice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/structural/lattice/lattice_bravais.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/structural/lattice/lattice_vectors.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/structural/lattice/type_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/structural/lattice/type_extended_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/structural/magnetic_moments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/structural/molecular_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/structural/p_norm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.867683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/structural/patterns/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/structural/patterns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/structural/patterns/functional_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/structural/patterns/ring.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/structural/patterns/special_bond.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/structural/symmetry.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/structural/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.711683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/workflow/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.867683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/workflow/convergence/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/workflow/convergence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/workflow/convergence/electronic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/workflow/convergence/ionic.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/workflow/convergence/kpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.867683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/property/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/property/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.867683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/property/base/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.871683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/property/base/The_source_of_a_property/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/property/base/The_source_of_a_property/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/property/base/The_source_of_a_property/field_This_could_be_an_article__a_simulation_on_Exabyte__an_external_simulation__etc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5793 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/property/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.871683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/property/meta/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.871683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/property/meta/The_source_of_a_property/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/property/meta/The_source_of_a_property/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/property/meta/The_source_of_a_property/field_This_could_be_an_article__a_simulation_on_Exabyte__an_external_simulation__etc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5786 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/property/meta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.871683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/property/raw/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.871683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/property/raw/The_source_of_a_property/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/property/raw/The_source_of_a_property/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/property/raw/The_source_of_a_property/field_This_could_be_an_article__a_simulation_on_Exabyte__an_external_simulation__etc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5790 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/property/raw/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.871683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/property/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.871683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/property/source/The_source_of_a_property/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/property/source/The_source_of_a_property/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/property/source/The_source_of_a_property/field_This_could_be_an_article__a_simulation_on_Exabyte__an_external_simulation__etc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/property/source/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.871683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software/application.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software/executable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software/flavor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.715683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.871683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/ml/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/ml/exabyteml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.871683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/ml/unit/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/ml/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.871683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/ml/unit/execution/
--rw-r--r--   0 runner    (1001) docker     (127)    36715 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/ml/unit/execution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.871683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/ml/unit/execution/evaluate/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/ml/unit/execution/evaluate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10067 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/ml/unit/execution/evaluate/cross_validate.py
--rw-r--r--   0 runner    (1001) docker     (127)    10088 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/ml/unit/execution/initialize.py
--rw-r--r--   0 runner    (1001) docker     (127)     9894 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/ml/unit/execution/score.py
--rw-r--r--   0 runner    (1001) docker     (127)    10108 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/ml/unit/execution/train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.875683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/ml/unit/processing/
--rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/ml/unit/processing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.875683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/ml/unit/processing/data_transformation/
--rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/ml/unit/processing/data_transformation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/ml/unit/processing/data_transformation/manipulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/ml/unit/processing/data_transformation/scale_and_reduce.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.875683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/ml/unit/processing/feature_selection/
--rw-r--r--   0 runner    (1001) docker     (127)     4382 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/ml/unit/processing/feature_selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/ml/unit/processing/feature_selection/filter_based.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.875683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/modeling/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/modeling/deepmd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.875683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/modeling/espresso/
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/modeling/espresso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/modeling/espresso/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/modeling/nwchem.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.875683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/modeling/unit/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/modeling/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10439 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/modeling/unit/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/modeling/vasp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.875683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/scripting/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/scripting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/scripting/jupyter_lab.py
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/scripting/python.py
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/scripting/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.875683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/scripting/unit/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/scripting/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10408 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/scripting/unit/execution.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.883683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/system/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/system/_material.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/system/_parent_job.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/system/_project.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/system/bankable.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/system/consistency_check.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/system/creator.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/system/creator_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/system/database_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/system/defaultable.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/system/description.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/system/entity_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/system/file_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/system/history.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/system/iframe_message.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/system/in_set.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/system/is_multi_material.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/system/is_outdated.py
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/system/job_extended.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/system/message.py
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/system/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/system/name.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/system/owner.py
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/system/path.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/system/path_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/system/schema_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/system/scope.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/system/set.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/system/sharing.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/system/soft_removable.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/system/status.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/system/tags.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/system/timestampable.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/system/use_values.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.715683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/third_party/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.715683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/third_party/db/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.715683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/third_party/db/nist_jarvis/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.883683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/third_party/db/nist_jarvis/2024.3.13/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/third_party/db/nist_jarvis/2024.3.13/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/third_party/db/nist_jarvis/2024.3.13/atoms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/third_party/db/nist_jarvis/2024.3.13/db_entry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.715683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/third_party/file/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.715683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/third_party/file/applications/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.715683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/third_party/file/applications/espresso/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.883683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/third_party/file/applications/espresso/7.2/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/third_party/file/applications/espresso/7.2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.883683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/third_party/file/applications/espresso/7.2/pw.x/
--rw-r--r--   0 runner    (1001) docker     (127)    74617 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/third_party/file/applications/espresso/7.2/pw.x/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/third_party/file/applications/espresso/7.2/pw.x/atomic_positions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/third_party/file/applications/espresso/7.2/pw.x/atomic_species.py
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/third_party/file/applications/espresso/7.2/pw.x/cell.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/third_party/file/applications/espresso/7.2/pw.x/cell_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     8786 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/third_party/file/applications/espresso/7.2/pw.x/control.py
--rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/third_party/file/applications/espresso/7.2/pw.x/electrons.py
--rw-r--r--   0 runner    (1001) docker     (127)     4439 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/third_party/file/applications/espresso/7.2/pw.x/hubbard.py
--rw-r--r--   0 runner    (1001) docker     (127)    15280 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/third_party/file/applications/espresso/7.2/pw.x/ions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/third_party/file/applications/espresso/7.2/pw.x/k_points.py
--rw-r--r--   0 runner    (1001) docker     (127)    34350 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/third_party/file/applications/espresso/7.2/pw.x/system.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.883683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)    76517 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5987 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/base_flow.py
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/scope.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.887683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/subworkflow/
--rw-r--r--   0 runner    (1001) docker     (127)    39880 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/subworkflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31216 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/subworkflow/unit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.887683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/unit/
--rw-r--r--   0 runner    (1001) docker     (127)    37479 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/unit/assertion.py
--rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/unit/assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/unit/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/unit/condition.py
--rw-r--r--   0 runner    (1001) docker     (127)     9880 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/unit/execution.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.887683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/unit/input/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/unit/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/unit/input/_input.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/unit/input/_inputItem.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/unit/input/_inputItemId.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/unit/input/_inputItemScope.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.887683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/unit/input/_map_input/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/unit/input/_map_input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/unit/input/_map_input/values.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.887683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/unit/io/
--rw-r--r--   0 runner    (1001) docker     (127)     5869 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/unit/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/unit/io/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/unit/io/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/unit/io/object_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4244 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/unit/map.py
--rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/unit/processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/unit/reduce.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.891683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/unit/runtime/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/unit/runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/unit/runtime/_runtime_item_full_object.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/unit/runtime/_runtime_item_name_object.py
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/unit/runtime/_runtime_item_string.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/unit/runtime/runtime_item.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/unit/runtime/runtime_items.py
--rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/unit/subworkflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.891683 mat3ra-esse-2024.4.8.post3/src/py/mat3ra_esse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8841 2024-04-08 11:18:05.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra_esse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    59789 2024-04-08 11:18:05.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra_esse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 11:18:05.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra_esse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-08 11:18:05.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra_esse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-08 11:18:05.000000 mat3ra-esse-2024.4.8.post3/src/py/mat3ra_esse.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.715683 mat3ra-esse-2024.4.8.post3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.891683 mat3ra-esse-2024.4.8.post3/tests/js/
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/tests/js/JSONSchemasInterface.tests.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.715683 mat3ra-esse-2024.4.8.post3/tests/js/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.891683 mat3ra-esse-2024.4.8.post3/tests/js/fixtures/json/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/tests/js/fixtures/json/1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/tests/js/fixtures/json/2.json
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/tests/js/validate.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.891683 mat3ra-esse-2024.4.8.post3/tests/py/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/tests/py/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:18:05.891683 mat3ra-esse-2024.4.8.post3/tests/py/esse/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/tests/py/esse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/tests/py/esse/test_validate.py
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/tsconfig-transpile.json
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-08 11:17:49.000000 mat3ra-esse-2024.4.8.post3/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.125848 mat3ra-esse-2024.4.8.post4/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/.babelrc
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/.eslintrc.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.881847 mat3ra-esse-2024.4.8.post4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.921847 mat3ra-esse-2024.4.8.post4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     5088 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/.github/workflows/cicd.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.921847 mat3ra-esse-2024.4.8.post4/.husky/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      792 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/.husky/pre-commit
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/.mocharc.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/.prettierrc
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8795 2024-04-08 11:31:48.125848 mat3ra-esse-2024.4.8.post4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/build_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/build_schemas.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/compile_ts.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.921847 mat3ra-esse-2024.4.8.post4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.925847 mat3ra-esse-2024.4.8.post4/example/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.881847 mat3ra-esse-2024.4.8.post4/example/3pse/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.881847 mat3ra-esse-2024.4.8.post4/example/3pse/db/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.881847 mat3ra-esse-2024.4.8.post4/example/3pse/db/nist_jarvis/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.925847 mat3ra-esse-2024.4.8.post4/example/3pse/db/nist_jarvis/2024.3.13/
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/3pse/db/nist_jarvis/2024.3.13/db_entry.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.881847 mat3ra-esse-2024.4.8.post4/example/3pse/file/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.881847 mat3ra-esse-2024.4.8.post4/example/3pse/file/applications/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.881847 mat3ra-esse-2024.4.8.post4/example/3pse/file/applications/espresso/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.925847 mat3ra-esse-2024.4.8.post4/example/3pse/file/applications/espresso/7.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/3pse/file/applications/espresso/7.2/pw.x.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.925847 mat3ra-esse-2024.4.8.post4/example/core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.925847 mat3ra-esse-2024.4.8.post4/example/core/abstract/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/core/abstract/2d_data.json
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/core/abstract/2d_plot.json
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/core/abstract/3d_grid.json
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/core/abstract/3d_tensor.json
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/core/abstract/3d_vector_basis.json
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/core/abstract/point.json
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/core/abstract/vector.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.925847 mat3ra-esse-2024.4.8.post4/example/core/primitive/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/core/primitive/1d_data_series.json
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/core/primitive/3d_lattice.json
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/core/primitive/array_of_3_booleans.json
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/core/primitive/array_of_3_numbers.json
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/core/primitive/array_of_ids.json
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/core/primitive/axis.json
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/core/primitive/scalar.json
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/core/primitive/string.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.929847 mat3ra-esse-2024.4.8.post4/example/core/reference/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.929847 mat3ra-esse-2024.4.8.post4/example/core/reference/experiment/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/core/reference/experiment/condition.json
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/core/reference/experiment/location.json
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/core/reference/experiment.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.929847 mat3ra-esse-2024.4.8.post4/example/core/reference/literature/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/core/reference/literature/name.json
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/core/reference/literature/pages.json
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/core/reference/literature.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.929847 mat3ra-esse-2024.4.8.post4/example/core/reference/modeling/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/core/reference/modeling/exabyte.json
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/core/reference/modeling.json
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/core/reference.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.929847 mat3ra-esse-2024.4.8.post4/example/core/reusable/
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/core/reusable/atomic_vectors.json
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/core/reusable/band_gap.json
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/core/reusable/energy.json
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/core/reusable/file_metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/core/reusable/object_storage_container_data.json
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/element.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.929847 mat3ra-esse-2024.4.8.post4/example/job/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/job/compute.json
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/job.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/material.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.929847 mat3ra-esse-2024.4.8.post4/example/method/
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/method/categorized_method.json
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/method/method_parameters.json
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/method.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.885846 mat3ra-esse-2024.4.8.post4/example/methods_directory/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.929847 mat3ra-esse-2024.4.8.post4/example/methods_directory/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/methods_directory/legacy/localorbital.json
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/methods_directory/legacy/pseudopotential.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/methods_directory/legacy/regression.json
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/methods_directory/legacy/unknown.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.929847 mat3ra-esse-2024.4.8.post4/example/methods_directory/mathematical/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/methods_directory/mathematical/cg.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/methods_directory/mathematical/regression.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.929847 mat3ra-esse-2024.4.8.post4/example/methods_directory/physical/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.933847 mat3ra-esse-2024.4.8.post4/example/methods_directory/physical/ao/
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/methods_directory/physical/ao/dunning.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.933847 mat3ra-esse-2024.4.8.post4/example/methods_directory/physical/psp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/methods_directory/physical/psp/file.json
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/methods_directory/physical/psp.json
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/methods_directory/physical/pw.json
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/methods_directory/physical/smearing.json
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/methods_directory/physical/tetrahedron.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.933847 mat3ra-esse-2024.4.8.post4/example/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/model/categorized_model.json
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/model/model_parameters.json
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/model.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.885846 mat3ra-esse-2024.4.8.post4/example/models_category/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.885846 mat3ra-esse-2024.4.8.post4/example/models_category/pb/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.933847 mat3ra-esse-2024.4.8.post4/example/models_category/pb/qm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.933847 mat3ra-esse-2024.4.8.post4/example/models_category/pb/qm/abin/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/models_category/pb/qm/abin/gw.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.933847 mat3ra-esse-2024.4.8.post4/example/models_category/pb/qm/dft/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/models_category/pb/qm/dft/ksdft.json
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/models_category/pb/qm/semp.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.933847 mat3ra-esse-2024.4.8.post4/example/models_directory/
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/models_directory/gga.json
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/models_directory/gw.json
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/models_directory/hybrid.json
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/models_directory/lda.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.933847 mat3ra-esse-2024.4.8.post4/example/models_directory/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/models_directory/legacy/dft.json
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/models_directory/legacy/ml.json
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/models_directory/legacy/unknown.json
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/models_directory/re.json
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/project.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.933847 mat3ra-esse-2024.4.8.post4/example/properties_directory/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/properties_directory/electronic_configuration.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.933847 mat3ra-esse-2024.4.8.post4/example/properties_directory/elemental/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/properties_directory/elemental/atomic_radius.json
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/properties_directory/elemental/electronegativity.json
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/properties_directory/elemental/ionization_potential.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.937847 mat3ra-esse-2024.4.8.post4/example/properties_directory/non-scalar/
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/properties_directory/non-scalar/band_gaps.json
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/properties_directory/non-scalar/band_structure.json
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/properties_directory/non-scalar/charge_density_profile.json
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/properties_directory/non-scalar/density_of_states.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3326 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/properties_directory/non-scalar/dielectric_tensor.json
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/properties_directory/non-scalar/file_content.json
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/properties_directory/non-scalar/hubbard_u.json
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/properties_directory/non-scalar/hubbard_v.json
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/properties_directory/non-scalar/hubbard_v_nn.json
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/properties_directory/non-scalar/phonon_dispersions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/properties_directory/non-scalar/phonon_dos.json
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/properties_directory/non-scalar/potential_profile.json
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/properties_directory/non-scalar/reaction_energy_profile.json
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/properties_directory/non-scalar/stress_tensor.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/properties_directory/non-scalar/total_energy_contributions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/properties_directory/non-scalar/vibrational_spectrum.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.941847 mat3ra-esse-2024.4.8.post4/example/properties_directory/scalar/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/properties_directory/scalar/electron_affinity.json
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/properties_directory/scalar/fermi_energy.json
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/properties_directory/scalar/formation_energy.json
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/properties_directory/scalar/ionization_potential.json
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/properties_directory/scalar/pressure.json
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/properties_directory/scalar/reaction_energy_barrier.json
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/properties_directory/scalar/surface_energy.json
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/properties_directory/scalar/total_energy.json
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/properties_directory/scalar/total_force.json
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/properties_directory/scalar/valence_band_offset.json
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/properties_directory/scalar/zero_point_energy.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.941847 mat3ra-esse-2024.4.8.post4/example/properties_directory/structural/
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/properties_directory/structural/atomic_forces.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.941847 mat3ra-esse-2024.4.8.post4/example/properties_directory/structural/basis/
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/properties_directory/structural/basis/atomic_constraints.json
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/properties_directory/structural/basis/atomic_coordinate.json
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/properties_directory/structural/basis/atomic_coordinates.json
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/properties_directory/structural/basis/atomic_element.json
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/properties_directory/structural/basis/bonds.json
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/properties_directory/structural/basis.json
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/properties_directory/structural/density.json
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/properties_directory/structural/elemental_ratio.json
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/properties_directory/structural/inchi.json
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/properties_directory/structural/inchi_key.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.941847 mat3ra-esse-2024.4.8.post4/example/properties_directory/structural/lattice/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/properties_directory/structural/lattice/lattice_bravais.json
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/properties_directory/structural/lattice/lattice_vectors.json
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/properties_directory/structural/lattice.json
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/properties_directory/structural/magnetic_moments.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/properties_directory/structural/molecular_pattern.json
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/properties_directory/structural/p-norm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/properties_directory/structural/symmetry.json
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/properties_directory/structural/volume.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.885846 mat3ra-esse-2024.4.8.post4/example/properties_directory/workflow/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.945847 mat3ra-esse-2024.4.8.post4/example/properties_directory/workflow/convergence/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/properties_directory/workflow/convergence/electronic.json
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/properties_directory/workflow/convergence/ionic.json
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/properties_directory/workflow/convergence/kpoint.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.945847 mat3ra-esse-2024.4.8.post4/example/property/
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/property/base.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.945847 mat3ra-esse-2024.4.8.post4/example/software/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/software/application.json
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/software/executable.json
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/software/flavor.json
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/software/template.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.889847 mat3ra-esse-2024.4.8.post4/example/software_directory/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.945847 mat3ra-esse-2024.4.8.post4/example/software_directory/ml/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/software_directory/ml/exabyteml.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.885846 mat3ra-esse-2024.4.8.post4/example/software_directory/ml/unit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.945847 mat3ra-esse-2024.4.8.post4/example/software_directory/ml/unit/execution/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.945847 mat3ra-esse-2024.4.8.post4/example/software_directory/ml/unit/execution/evaluate/
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/software_directory/ml/unit/execution/evaluate/cross-validate.json
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/software_directory/ml/unit/execution/initialize.json
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/software_directory/ml/unit/execution/score.json
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/software_directory/ml/unit/execution/train.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.889847 mat3ra-esse-2024.4.8.post4/example/software_directory/ml/unit/processing/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.945847 mat3ra-esse-2024.4.8.post4/example/software_directory/ml/unit/processing/data_transformation/
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/software_directory/ml/unit/processing/data_transformation/manipulation.json
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/software_directory/ml/unit/processing/data_transformation/scale_and_reduce.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.945847 mat3ra-esse-2024.4.8.post4/example/software_directory/ml/unit/processing/feature_selection/
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/software_directory/ml/unit/processing/feature_selection/filter_based.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.945847 mat3ra-esse-2024.4.8.post4/example/software_directory/modeling/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.945847 mat3ra-esse-2024.4.8.post4/example/software_directory/modeling/espresso/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/software_directory/modeling/espresso/arguments.json
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/software_directory/modeling/espresso.json
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/software_directory/modeling/nwchem.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.945847 mat3ra-esse-2024.4.8.post4/example/software_directory/modeling/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/software_directory/modeling/unit/execution.json
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/software_directory/modeling/vasp.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.949847 mat3ra-esse-2024.4.8.post4/example/software_directory/scripting/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/software_directory/scripting/jupyter-lab.json
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/software_directory/scripting/python.json
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/software_directory/scripting/shell.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.949847 mat3ra-esse-2024.4.8.post4/example/software_directory/scripting/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/software_directory/scripting/unit/execution.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.949847 mat3ra-esse-2024.4.8.post4/example/system/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/system/_material.json
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/system/_parent_job.json
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/system/_project.json
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/system/consistency_check.json
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/system/creator.json
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/system/entity_reference.json
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/system/file_source.json
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/system/iframe_message.json
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/system/message.json
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/system/owner.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.949847 mat3ra-esse-2024.4.8.post4/example/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/workflow/subworkflow.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.949847 mat3ra-esse-2024.4.8.post4/example/workflow/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/workflow/unit/assignment.json
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/workflow/unit/condition.json
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/workflow/unit/execution.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.953847 mat3ra-esse-2024.4.8.post4/example/workflow/unit/input/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/workflow/unit/input/_inputItemScope.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.953847 mat3ra-esse-2024.4.8.post4/example/workflow/unit/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/workflow/unit/io/api.json
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/workflow/unit/io/db.json
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/workflow/unit/io/object_storage.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/workflow/unit/io.json
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/workflow/unit/map.json
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/workflow/unit/processing.json
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/workflow/unit/reduce.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.953847 mat3ra-esse-2024.4.8.post4/example/workflow/unit/runtime/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/workflow/unit/runtime/runtime_items.json
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/example/workflow.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.953847 mat3ra-esse-2024.4.8.post4/manifest/
+-rw-r--r--   0 runner    (1001) docker     (127)     7807 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/manifest/dft_unit_functionals.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13108 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/manifest/functional_lookup_table.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9760 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/manifest/models.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5545 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/manifest/properties.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/npmignore
+-rw-r--r--   0 runner    (1001) docker     (127)   341213 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.953847 mat3ra-esse-2024.4.8.post4/schema/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.889847 mat3ra-esse-2024.4.8.post4/schema/3pse/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.889847 mat3ra-esse-2024.4.8.post4/schema/3pse/db/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.889847 mat3ra-esse-2024.4.8.post4/schema/3pse/db/nist_jarvis/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.953847 mat3ra-esse-2024.4.8.post4/schema/3pse/db/nist_jarvis/2024.3.13/
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/3pse/db/nist_jarvis/2024.3.13/atoms.json
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/3pse/db/nist_jarvis/2024.3.13/db_entry.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.889847 mat3ra-esse-2024.4.8.post4/schema/3pse/file/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.889847 mat3ra-esse-2024.4.8.post4/schema/3pse/file/applications/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.889847 mat3ra-esse-2024.4.8.post4/schema/3pse/file/applications/espresso/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.953847 mat3ra-esse-2024.4.8.post4/schema/3pse/file/applications/espresso/7.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.957847 mat3ra-esse-2024.4.8.post4/schema/3pse/file/applications/espresso/7.2/pw.x/
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/3pse/file/applications/espresso/7.2/pw.x/atomic_positions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/3pse/file/applications/espresso/7.2/pw.x/atomic_species.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/3pse/file/applications/espresso/7.2/pw.x/cell.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/3pse/file/applications/espresso/7.2/pw.x/cell_parameters.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10526 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/3pse/file/applications/espresso/7.2/pw.x/control.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6354 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/3pse/file/applications/espresso/7.2/pw.x/electrons.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11220 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/3pse/file/applications/espresso/7.2/pw.x/hubbard.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7549 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/3pse/file/applications/espresso/7.2/pw.x/ions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/3pse/file/applications/espresso/7.2/pw.x/k_points.json
+-rw-r--r--   0 runner    (1001) docker     (127)    25760 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/3pse/file/applications/espresso/7.2/pw.x/system.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/3pse/file/applications/espresso/7.2/pw.x.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.957847 mat3ra-esse-2024.4.8.post4/schema/core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.957847 mat3ra-esse-2024.4.8.post4/schema/core/abstract/
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/core/abstract/2d_data.json
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/core/abstract/2d_plot.json
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/core/abstract/3d_grid.json
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/core/abstract/3d_tensor.json
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/core/abstract/3d_vector_basis.json
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/core/abstract/point.json
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/core/abstract/vector.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.961847 mat3ra-esse-2024.4.8.post4/schema/core/primitive/
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/core/primitive/1d_data_series.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/core/primitive/3d_lattice.json
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/core/primitive/array_of_3_booleans.json
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/core/primitive/array_of_3_numbers.json
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/core/primitive/array_of_ids.json
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/core/primitive/array_of_strings.json
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/core/primitive/axis.json
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/core/primitive/group_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/core/primitive/integer_one_or_zero.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.961847 mat3ra-esse-2024.4.8.post4/schema/core/primitive/linked_list/
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/core/primitive/linked_list/base_node.json
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/core/primitive/linked_list/named_node.json
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/core/primitive/linked_list/named_node_in_group.json
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/core/primitive/linked_list/node_with_type.json
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/core/primitive/linked_list.json
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/core/primitive/scalar.json
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/core/primitive/slugified_entry.json
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/core/primitive/slugified_entry_or_slug.json
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/core/primitive/string.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.961847 mat3ra-esse-2024.4.8.post4/schema/core/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/core/reference/exabyte.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.961847 mat3ra-esse-2024.4.8.post4/schema/core/reference/experiment/
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/core/reference/experiment/condition.json
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/core/reference/experiment/location.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/core/reference/experiment.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.961847 mat3ra-esse-2024.4.8.post4/schema/core/reference/literature/
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/core/reference/literature/name.json
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/core/reference/literature/pages.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/core/reference/literature.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.961847 mat3ra-esse-2024.4.8.post4/schema/core/reference/modeling/
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/core/reference/modeling/exabyte.json
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/core/reference/modeling.json
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/core/reference.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.965847 mat3ra-esse-2024.4.8.post4/schema/core/reusable/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.965847 mat3ra-esse-2024.4.8.post4/schema/core/reusable/atomic_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/core/reusable/atomic_data/per_orbital.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/core/reusable/atomic_data/per_orbital_pair.json
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/core/reusable/atomic_data/value_number.json
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/core/reusable/atomic_data/value_string.json
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/core/reusable/atomic_data_per_orbital_numeric.json
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/core/reusable/atomic_data_per_orbital_pair_numeric.json
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/core/reusable/atomic_orbital.json
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/core/reusable/atomic_scalars.json
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/core/reusable/atomic_strings.json
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/core/reusable/atomic_vectors.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/core/reusable/band_gap.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/core/reusable/categories.json
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/core/reusable/category_path.json
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/core/reusable/dielectric_tensor_component.json
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/core/reusable/energy.json
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/core/reusable/file_metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/core/reusable/frequency_function_matrix.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/core/reusable/object_storage_container_data.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.965847 mat3ra-esse-2024.4.8.post4/schema/definitions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/definitions/units.json
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/element.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.969847 mat3ra-esse-2024.4.8.post4/schema/in_memory_entity/
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/in_memory_entity/base.json
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/in_memory_entity/defaultable.json
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/in_memory_entity/named.json
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/in_memory_entity/named_defaultable.json
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/in_memory_entity/named_defaultable_has_metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/in_memory_entity/named_defaultable_runtime_items.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.969847 mat3ra-esse-2024.4.8.post4/schema/job/
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/job/base.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/job/compute.json
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/job.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.969847 mat3ra-esse-2024.4.8.post4/schema/material/
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/material/conventional.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/material.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.969847 mat3ra-esse-2024.4.8.post4/schema/method/
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/method/categorized_method.json
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/method/method_parameters.json
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/method/unit_method.json
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/method.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.893847 mat3ra-esse-2024.4.8.post4/schema/methods_category/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.969847 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.969847 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/diff/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/diff/enum_options.json
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/diff/enum_options.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/diff/fd.json
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/diff.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.973847 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/discr/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/discr/enum_options.json
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/discr/enum_options.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.973847 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/discr/mesh/
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/discr/mesh/enum_options.json
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/discr/mesh/enum_options.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/discr/mesh/hybrid.json
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/discr/mesh/nstruct.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.973847 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/discr/mesh/struct/
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/discr/mesh/struct/cartesian.json
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/discr/mesh/struct/enum_options.json
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/discr/mesh/struct/enum_options.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/discr/mesh/struct.json
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/discr/mesh.json
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/discr.json
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/enum_options.json
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/enum_options.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.973847 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/fapprx/
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/fapprx/basisexp.json
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/fapprx/enum_options.json
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/fapprx/enum_options.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.973847 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/fapprx/ipol/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/fapprx/ipol/enum_options.json
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/fapprx/ipol/enum_options.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/fapprx/ipol/lin.json
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/fapprx/ipol/poly.json
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/fapprx/ipol/spline.json
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/fapprx/ipol.json
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/fapprx.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.977847 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/intgr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.977847 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/intgr/analytic/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/intgr/analytic/enum_options.json
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/intgr/analytic/enum_options.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/intgr/analytic/volume.json
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/intgr/analytic.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.977847 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/intgr/diffeq/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/intgr/diffeq/enum_options.json
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/intgr/diffeq/enum_options.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/intgr/diffeq/order1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/intgr/diffeq/order2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/intgr/diffeq.json
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/intgr/enum_options.json
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/intgr/enum_options.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.977847 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/intgr/numquad/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/intgr/numquad/enum_options.json
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/intgr/numquad/enum_options.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/intgr/numquad/gauss.json
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/intgr/numquad/newcot.json
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/intgr/numquad.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.977847 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/intgr/transf/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/intgr/transf/enum_options.json
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/intgr/transf/enum_options.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/intgr/transf/fourier.json
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/intgr/transf.json
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/intgr.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.981847 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/linalg/
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/linalg/dcomp.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.981847 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/linalg/diag/
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/linalg/diag/davidson.json
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/linalg/diag/enum_options.json
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/linalg/diag/enum_options.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/linalg/diag.json
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/linalg/enum_options.json
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/linalg/enum_options.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/linalg/lintra.json
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/linalg/matf.json
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/linalg.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.981847 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/opt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.981847 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/opt/diff/
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/opt/diff/bracket.json
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/opt/diff/enum_options.json
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/opt/diff/enum_options.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/opt/diff/local.json
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/opt/diff/order1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/opt/diff/order2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.981847 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/opt/diff/ordern/
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/opt/diff/ordern/cg.json
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/opt/diff/ordern/enum_options.json
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/opt/diff/ordern/enum_options.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/opt/diff/ordern.json
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/opt/diff.json
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/opt/enum_options.json
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/opt/enum_options.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.985847 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/opt/ndiff/
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/opt/ndiff/direct.json
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/opt/ndiff/enum_options.json
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/opt/ndiff/enum_options.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/opt/ndiff/pop.json
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/opt/ndiff/stoch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/opt/ndiff.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.985847 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/opt/root/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/opt/root/bracket.json
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/opt/root/enum_options.json
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/opt/root/enum_options.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/opt/root/iter.json
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/opt/root.json
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/opt.json
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/regression.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.985847 mat3ra-esse-2024.4.8.post4/schema/methods_category/physical/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/physical/enum_options.json
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/physical/enum_options.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.985847 mat3ra-esse-2024.4.8.post4/schema/methods_category/physical/qm/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/physical/qm/enum_options.json
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/physical/qm/enum_options.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.985847 mat3ra-esse-2024.4.8.post4/schema/methods_category/physical/qm/wf/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.989847 mat3ra-esse-2024.4.8.post4/schema/methods_category/physical/qm/wf/ao/
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/physical/qm/wf/ao/dunning.json
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/physical/qm/wf/ao/other.json
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/physical/qm/wf/ao/pople.json
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/physical/qm/wf/ao.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/physical/qm/wf/enum_options.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/physical/qm/wf/enum_options.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/physical/qm/wf/psp.json
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/physical/qm/wf/pw.json
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/physical/qm/wf/smearing.json
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/physical/qm/wf/tetrahedron.json
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/physical/qm/wf.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_category/physical/qm.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.897847 mat3ra-esse-2024.4.8.post4/schema/methods_directory/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.989847 mat3ra-esse-2024.4.8.post4/schema/methods_directory/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_directory/legacy/localorbital.json
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_directory/legacy/pseudopotential.json
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_directory/legacy/regression.json
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_directory/legacy/unknown.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.989847 mat3ra-esse-2024.4.8.post4/schema/methods_directory/mathematical/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_directory/mathematical/cg.json
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_directory/mathematical/davidson.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.989847 mat3ra-esse-2024.4.8.post4/schema/methods_directory/mathematical/regression/
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_directory/mathematical/regression/data.json
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_directory/mathematical/regression/dataset.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.989847 mat3ra-esse-2024.4.8.post4/schema/methods_directory/mathematical/regression/kernel_ridge/
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_directory/mathematical/regression/kernel_ridge/data_per_property.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.989847 mat3ra-esse-2024.4.8.post4/schema/methods_directory/mathematical/regression/linear/
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_directory/mathematical/regression/linear/data_per_property.json
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_directory/mathematical/regression/per_feature_item.json
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_directory/mathematical/regression/precision.json
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_directory/mathematical/regression/precision_per_property.json
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_directory/mathematical/regression.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.989847 mat3ra-esse-2024.4.8.post4/schema/methods_directory/physical/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.993847 mat3ra-esse-2024.4.8.post4/schema/methods_directory/physical/ao/
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_directory/physical/ao/dunning.json
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_directory/physical/ao/enum_options.json
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_directory/physical/ao/enum_options.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_directory/physical/ao/other.json
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_directory/physical/ao/pople.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.993847 mat3ra-esse-2024.4.8.post4/schema/methods_directory/physical/psp/
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_directory/physical/psp/file.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_directory/physical/psp/file_data_item.json
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_directory/physical/psp.json
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_directory/physical/pw.json
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_directory/physical/smearing.json
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/methods_directory/physical/tetrahedron.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.993847 mat3ra-esse-2024.4.8.post4/schema/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/model/categorized_model.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.993847 mat3ra-esse-2024.4.8.post4/schema/model/mixins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.993847 mat3ra-esse-2024.4.8.post4/schema/model/mixins/dft/
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/model/mixins/dft/double_hybrid_functional.json
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/model/mixins/dft/enum_options.json
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/model/mixins/dft/enum_options.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/model/mixins/dft/gga_functional.json
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/model/mixins/dft/hybrid_functional.json
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/model/mixins/dft/lda_functional.json
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/model/mixins/dft/mgga_functional.json
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/model/mixins/dispersion_correction.json
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/model/mixins/enum_options.json
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/model/mixins/enum_options.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/model/mixins/hubbard.json
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/model/mixins/spin_orbit_coupling.json
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/model/mixins/spin_polarization.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/model/model_parameters.json
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/model/model_without_method.json
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/model.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.997847 mat3ra-esse-2024.4.8.post4/schema/models_category/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/models_category/enum_options.json
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/models_category/enum_options.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.997847 mat3ra-esse-2024.4.8.post4/schema/models_category/pb/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/models_category/pb/enum_options.json
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/models_category/pb/enum_options.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.997847 mat3ra-esse-2024.4.8.post4/schema/models_category/pb/qm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.997847 mat3ra-esse-2024.4.8.post4/schema/models_category/pb/qm/abin/
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/models_category/pb/qm/abin/enum_options.json
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/models_category/pb/qm/abin/enum_options.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/models_category/pb/qm/abin/gw.json
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/models_category/pb/qm/abin.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.997847 mat3ra-esse-2024.4.8.post4/schema/models_category/pb/qm/dft/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/models_category/pb/qm/dft/enum_options.json
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/models_category/pb/qm/dft/enum_options.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.001847 mat3ra-esse-2024.4.8.post4/schema/models_category/pb/qm/dft/ksdft/
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/models_category/pb/qm/dft/ksdft/double_hybrid.json
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/models_category/pb/qm/dft/ksdft/enum_options.json
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/models_category/pb/qm/dft/ksdft/enum_options.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/models_category/pb/qm/dft/ksdft/gga.json
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/models_category/pb/qm/dft/ksdft/hybrid.json
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/models_category/pb/qm/dft/ksdft/lda.json
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/models_category/pb/qm/dft/ksdft/mgga.json
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/models_category/pb/qm/dft/ksdft.json
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/models_category/pb/qm/dft.json
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/models_category/pb/qm/enum_options.json
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/models_category/pb/qm/enum_options.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/models_category/pb/qm/semp.json
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/models_category/pb/qm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/models_category/pb.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.001847 mat3ra-esse-2024.4.8.post4/schema/models_category/st/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.001847 mat3ra-esse-2024.4.8.post4/schema/models_category/st/det/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/models_category/st/det/enum_options.json
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/models_category/st/det/enum_options.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.001847 mat3ra-esse-2024.4.8.post4/schema/models_category/st/det/ml/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/models_category/st/det/ml/enum_options.json
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/models_category/st/det/ml/enum_options.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/models_category/st/det/ml/re.json
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/models_category/st/det/ml.json
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/models_category/st/det.json
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/models_category/st/enum_options.json
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/models_category/st/enum_options.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/models_category/st.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.001847 mat3ra-esse-2024.4.8.post4/schema/models_directory/
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/models_directory/double_hybrid.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/models_directory/gga.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/models_directory/gw.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/models_directory/hybrid.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/models_directory/lda.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.001847 mat3ra-esse-2024.4.8.post4/schema/models_directory/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/models_directory/legacy/dft.json
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/models_directory/legacy/ml.json
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/models_directory/legacy/unknown.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/models_directory/mgga.json
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/models_directory/re.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/project.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.005848 mat3ra-esse-2024.4.8.post4/schema/properties_directory/
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/properties_directory/derived_properties.json
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/properties_directory/electronic_configuration.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.005848 mat3ra-esse-2024.4.8.post4/schema/properties_directory/elemental/
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/properties_directory/elemental/atomic_radius.json
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/properties_directory/elemental/electronegativity.json
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/properties_directory/elemental/ionization_potential.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.005848 mat3ra-esse-2024.4.8.post4/schema/properties_directory/non-scalar/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/properties_directory/non-scalar/average_potential_profile.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/properties_directory/non-scalar/band_gaps.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/properties_directory/non-scalar/band_structure.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/properties_directory/non-scalar/charge_density_profile.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/properties_directory/non-scalar/density_of_states.json
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/properties_directory/non-scalar/dielectric_tensor.json
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/properties_directory/non-scalar/file_content.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/properties_directory/non-scalar/hubbard_u.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/properties_directory/non-scalar/hubbard_v.json
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/properties_directory/non-scalar/hubbard_v_nn.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/properties_directory/non-scalar/phonon_dispersions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/properties_directory/non-scalar/phonon_dos.json
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/properties_directory/non-scalar/potential_profile.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/properties_directory/non-scalar/reaction_energy_profile.json
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/properties_directory/non-scalar/stress_tensor.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6418 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/properties_directory/non-scalar/total_energy_contributions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/properties_directory/non-scalar/vibrational_spectrum.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.009847 mat3ra-esse-2024.4.8.post4/schema/properties_directory/scalar/
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/properties_directory/scalar/electron_affinity.json
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/properties_directory/scalar/fermi_energy.json
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/properties_directory/scalar/formation_energy.json
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/properties_directory/scalar/ionization_potential.json
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/properties_directory/scalar/pressure.json
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/properties_directory/scalar/reaction_energy_barrier.json
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/properties_directory/scalar/surface_energy.json
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/properties_directory/scalar/total_energy.json
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/properties_directory/scalar/total_force.json
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/properties_directory/scalar/valence_band_offset.json
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/properties_directory/scalar/zero_point_energy.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.013847 mat3ra-esse-2024.4.8.post4/schema/properties_directory/structural/
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/properties_directory/structural/atomic_forces.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.013847 mat3ra-esse-2024.4.8.post4/schema/properties_directory/structural/basis/
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/properties_directory/structural/basis/atomic_constraints.json
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/properties_directory/structural/basis/atomic_coordinate.json
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/properties_directory/structural/basis/atomic_coordinates.json
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/properties_directory/structural/basis/atomic_element.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/properties_directory/structural/basis/bonds.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/properties_directory/structural/basis.json
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/properties_directory/structural/density.json
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/properties_directory/structural/elemental_ratio.json
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/properties_directory/structural/inchi.json
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/properties_directory/structural/inchi_key.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.013847 mat3ra-esse-2024.4.8.post4/schema/properties_directory/structural/lattice/
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/properties_directory/structural/lattice/lattice_bravais.json
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/properties_directory/structural/lattice/lattice_vectors.json
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/properties_directory/structural/lattice/type_enum.json
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/properties_directory/structural/lattice/type_extended_enum.json
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/properties_directory/structural/lattice.json
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/properties_directory/structural/magnetic_moments.json
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/properties_directory/structural/molecular_pattern.json
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/properties_directory/structural/p-norm.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.013847 mat3ra-esse-2024.4.8.post4/schema/properties_directory/structural/patterns/
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/properties_directory/structural/patterns/functional_group.json
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/properties_directory/structural/patterns/ring.json
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/properties_directory/structural/patterns/special_bond.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/properties_directory/structural/symmetry.json
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/properties_directory/structural/volume.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.901847 mat3ra-esse-2024.4.8.post4/schema/properties_directory/workflow/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.013847 mat3ra-esse-2024.4.8.post4/schema/properties_directory/workflow/convergence/
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/properties_directory/workflow/convergence/electronic.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/properties_directory/workflow/convergence/ionic.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/properties_directory/workflow/convergence/kpoint.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.013847 mat3ra-esse-2024.4.8.post4/schema/property/
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/property/base.json
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/property/meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/property/raw.json
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/property/source.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.017848 mat3ra-esse-2024.4.8.post4/schema/software/
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/software/application.json
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/software/executable.json
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/software/flavor.json
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/software/template.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.901847 mat3ra-esse-2024.4.8.post4/schema/software_directory/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.017848 mat3ra-esse-2024.4.8.post4/schema/software_directory/ml/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/software_directory/ml/exabyteml.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.017848 mat3ra-esse-2024.4.8.post4/schema/software_directory/ml/unit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.017848 mat3ra-esse-2024.4.8.post4/schema/software_directory/ml/unit/execution/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.017848 mat3ra-esse-2024.4.8.post4/schema/software_directory/ml/unit/execution/evaluate/
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/software_directory/ml/unit/execution/evaluate/cross-validate.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/software_directory/ml/unit/execution/initialize.json
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/software_directory/ml/unit/execution/score.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/software_directory/ml/unit/execution/train.json
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/software_directory/ml/unit/execution.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.017848 mat3ra-esse-2024.4.8.post4/schema/software_directory/ml/unit/processing/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.017848 mat3ra-esse-2024.4.8.post4/schema/software_directory/ml/unit/processing/data_transformation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/software_directory/ml/unit/processing/data_transformation/manipulation.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/software_directory/ml/unit/processing/data_transformation/scale_and_reduce.json
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/software_directory/ml/unit/processing/data_transformation.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.017848 mat3ra-esse-2024.4.8.post4/schema/software_directory/ml/unit/processing/feature_selection/
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/software_directory/ml/unit/processing/feature_selection/filter_based.json
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/software_directory/ml/unit/processing/feature_selection.json
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/software_directory/ml/unit/processing.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.017848 mat3ra-esse-2024.4.8.post4/schema/software_directory/modeling/
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/software_directory/modeling/deepmd.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.017848 mat3ra-esse-2024.4.8.post4/schema/software_directory/modeling/espresso/
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/software_directory/modeling/espresso/arguments.json
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/software_directory/modeling/espresso.json
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/software_directory/modeling/nwchem.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.017848 mat3ra-esse-2024.4.8.post4/schema/software_directory/modeling/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/software_directory/modeling/unit/execution.json
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/software_directory/modeling/vasp.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.021848 mat3ra-esse-2024.4.8.post4/schema/software_directory/scripting/
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/software_directory/scripting/jupyter-lab.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/software_directory/scripting/python.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/software_directory/scripting/shell.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.021848 mat3ra-esse-2024.4.8.post4/schema/software_directory/scripting/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/software_directory/scripting/unit/execution.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.025848 mat3ra-esse-2024.4.8.post4/schema/system/
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/system/_material.json
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/system/_parent_job.json
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/system/_project.json
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/system/bankable.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/system/consistency_check.json
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/system/creator.json
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/system/creator_account.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/system/database_source.json
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/system/defaultable.json
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/system/description.json
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/system/entity_reference.json
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/system/file_source.json
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/system/history.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/system/iframe_message.json
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/system/in_set.json
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/system/is_multi_material.json
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/system/is_outdated.json
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/system/job_extended.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/system/message.json
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/system/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/system/name.json
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/system/owner.json
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/system/path.json
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/system/path_entity.json
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/system/schema_version.json
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/system/scope.json
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/system/set.json
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/system/sharing.json
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/system/soft_removable.json
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/system/status.json
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/system/tags.json
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/system/timestampable.json
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/system/use_values.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.025848 mat3ra-esse-2024.4.8.post4/schema/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/workflow/base.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/workflow/base_flow.json
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/workflow/scope.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.025848 mat3ra-esse-2024.4.8.post4/schema/workflow/subworkflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/workflow/subworkflow/unit.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/workflow/subworkflow.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.029848 mat3ra-esse-2024.4.8.post4/schema/workflow/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/workflow/unit/assertion.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/workflow/unit/assignment.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/workflow/unit/base.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/workflow/unit/condition.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/workflow/unit/execution.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.029848 mat3ra-esse-2024.4.8.post4/schema/workflow/unit/input/
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/workflow/unit/input/_input.json
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/workflow/unit/input/_inputItem.json
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/workflow/unit/input/_inputItemId.json
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/workflow/unit/input/_inputItemScope.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.029848 mat3ra-esse-2024.4.8.post4/schema/workflow/unit/input/_map_input/
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/workflow/unit/input/_map_input/values.json
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/workflow/unit/input/_map_input.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.029848 mat3ra-esse-2024.4.8.post4/schema/workflow/unit/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/workflow/unit/io/api.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/workflow/unit/io/db.json
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/workflow/unit/io/object_storage.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/workflow/unit/io.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/workflow/unit/map.json
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/workflow/unit/processing.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/workflow/unit/reduce.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.029848 mat3ra-esse-2024.4.8.post4/schema/workflow/unit/runtime/
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/workflow/unit/runtime/_runtime_item_full_object.json
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/workflow/unit/runtime/_runtime_item_name_object.json
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/workflow/unit/runtime/_runtime_item_string.json
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/workflow/unit/runtime/runtime_item.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/workflow/unit/runtime/runtime_items.json
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/workflow/unit/subworkflow.json
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/workflow/unit.json
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/schema/workflow.json
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/set_schema_ids.ts
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 11:31:48.125848 mat3ra-esse-2024.4.8.post4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.029848 mat3ra-esse-2024.4.8.post4/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.905847 mat3ra-esse-2024.4.8.post4/src/js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.033848 mat3ra-esse-2024.4.8.post4/src/js/esse/
+-rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/js/esse/JSONSchemasGenerator.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/js/esse/JSONSchemasInterface.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/js/esse/JSONSchemasInterfaceServer.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/js/esse/schemaUtils.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/js/esse/settings.ts
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/js/esse/types.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/js/esse/utils.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.033848 mat3ra-esse-2024.4.8.post4/src/js/json_include/
+-rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/js/json_include/index.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/js/json_include/settings.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.033848 mat3ra-esse-2024.4.8.post4/src/js/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/js/scripts/compileTs.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/js/scripts/createEnumsFromYaml.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/js/scripts/setSchemaIds.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.033848 mat3ra-esse-2024.4.8.post4/src/js/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/js/utils/ajv.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/js/utils/common.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/js/utils/filesystem.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.033848 mat3ra-esse-2024.4.8.post4/src/py/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.033848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.033848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.037848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45982 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/data/examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6099 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/data/properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1711304 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/data/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.037848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.037848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.041848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/abstract/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/abstract/2d_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/abstract/2d_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/abstract/3d_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/abstract/3d_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/abstract/3d_vector_basis.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/abstract/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/abstract/vector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.041848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/primitive/
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/primitive/1d_data_series.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/primitive/3d_lattice.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/primitive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/primitive/array_of_3_booleans.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/primitive/array_of_3_numbers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/primitive/array_of_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/primitive/array_of_strings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/primitive/axis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/primitive/group_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/primitive/integer_one_or_zero.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.045848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/primitive/linked_list/
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/primitive/linked_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/primitive/linked_list/base_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/primitive/linked_list/named_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/primitive/linked_list/named_node_in_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/primitive/linked_list/node_with_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/primitive/scalar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/primitive/slugified_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/primitive/slugified_entry_or_slug.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/primitive/string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.045848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)     6447 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/reference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/reference/exabyte.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.045848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/reference/experiment/
+-rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/reference/experiment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/reference/experiment/condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/reference/experiment/location.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.045848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/reference/literature/
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/reference/literature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/reference/literature/name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/reference/literature/pages.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.045848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/reference/modeling/
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/reference/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/reference/modeling/exabyte.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.049848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/reusable/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/reusable/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.049848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/reusable/atomic_data/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/reusable/atomic_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/reusable/atomic_data/per_orbital.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/reusable/atomic_data/per_orbital_pair.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/reusable/atomic_data/value_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/reusable/atomic_data/value_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/reusable/atomic_data_per_orbital_numeric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/reusable/atomic_data_per_orbital_pair_numeric.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/reusable/atomic_orbital.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/reusable/atomic_scalars.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/reusable/atomic_strings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/reusable/atomic_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/reusable/band_gap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/reusable/categories.py
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/reusable/category_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/reusable/dielectric_tensor_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/reusable/energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/reusable/file_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/reusable/frequency_function_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/reusable/object_storage_container_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.049848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/definitions/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/definitions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/definitions/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/element.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.053848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/in_memory_entity/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/in_memory_entity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/in_memory_entity/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/in_memory_entity/defaultable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/in_memory_entity/named.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/in_memory_entity/named_defaultable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/in_memory_entity/named_defaultable_has_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/in_memory_entity/named_defaultable_runtime_items.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.053848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/job/
+-rw-r--r--   0 runner    (1001) docker     (127)    82278 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8888 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/job/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/job/compute.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.053848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/material/
+-rw-r--r--   0 runner    (1001) docker     (127)    10087 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/material/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/material/conventional.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.053848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/method/
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/method/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/method/categorized_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/method/method_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/method/unit_method.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.909847 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.053848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.053848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/diff/
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/diff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/diff/enum_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/diff/fd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.053848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/discr/
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/discr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/discr/enum_options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.057848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/discr/mesh/
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/discr/mesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/discr/mesh/enum_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/discr/mesh/hybrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/discr/mesh/nstruct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.057848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/discr/mesh/struct/
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/discr/mesh/struct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/discr/mesh/struct/cartesian.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/discr/mesh/struct/enum_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/enum_options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.057848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/fapprx/
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/fapprx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/fapprx/basisexp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/fapprx/enum_options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.057848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/fapprx/ipol/
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/fapprx/ipol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/fapprx/ipol/enum_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/fapprx/ipol/lin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/fapprx/ipol/poly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/fapprx/ipol/spline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.057848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.057848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/analytic/
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/analytic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/analytic/enum_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/analytic/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.057848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/diffeq/
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/diffeq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/diffeq/enum_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/diffeq/order1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/diffeq/order2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/enum_options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.061848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/numquad/
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/numquad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/numquad/enum_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/numquad/gauss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/numquad/newcot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.061848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/transf/
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/transf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/transf/enum_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/transf/fourier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.061848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/linalg/
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/linalg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/linalg/dcomp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.061848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/linalg/diag/
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/linalg/diag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/linalg/diag/davidson.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/linalg/diag/enum_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/linalg/enum_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/linalg/lintra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/linalg/matf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.061848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/opt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/opt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.065848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/opt/diff/
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/opt/diff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/opt/diff/bracket.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/opt/diff/enum_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/opt/diff/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/opt/diff/order1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/opt/diff/order2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.065848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/opt/diff/ordern/
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/opt/diff/ordern/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/opt/diff/ordern/cg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/opt/diff/ordern/enum_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/opt/enum_options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.065848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/opt/ndiff/
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/opt/ndiff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/opt/ndiff/direct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/opt/ndiff/enum_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/opt/ndiff/pop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/opt/ndiff/stoch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.065848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/opt/root/
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/opt/root/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/opt/root/bracket.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/opt/root/enum_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/opt/root/iter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/regression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.065848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/physical/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/physical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/physical/enum_options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.065848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/physical/qm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/physical/qm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/physical/qm/enum_options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.069848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/physical/qm/wf/
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/physical/qm/wf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.069848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/physical/qm/wf/ao/
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/physical/qm/wf/ao/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/physical/qm/wf/ao/dunning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/physical/qm/wf/ao/other.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/physical/qm/wf/ao/pople.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/physical/qm/wf/enum_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/physical/qm/wf/psp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/physical/qm/wf/pw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/physical/qm/wf/smearing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/physical/qm/wf/tetrahedron.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.909847 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.069848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/legacy/localorbital.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/legacy/pseudopotential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/legacy/regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/legacy/unknown.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.069848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/mathematical/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/mathematical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/mathematical/cg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/mathematical/davidson.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.069848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/mathematical/regression/
+-rw-r--r--   0 runner    (1001) docker     (127)     4412 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/mathematical/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/mathematical/regression/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/mathematical/regression/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.073848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/mathematical/regression/kernel_ridge/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/mathematical/regression/kernel_ridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/mathematical/regression/kernel_ridge/data_per_property.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.073848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/mathematical/regression/linear/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/mathematical/regression/linear/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/mathematical/regression/linear/data_per_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/mathematical/regression/per_feature_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/mathematical/regression/precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/mathematical/regression/precision_per_property.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.073848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/physical/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/physical/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.073848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/physical/ao/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/physical/ao/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/physical/ao/dunning.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/physical/ao/enum_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/physical/ao/other.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/physical/ao/pople.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.073848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/physical/psp/
+-rw-r--r--   0 runner    (1001) docker     (127)     4792 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/physical/psp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/physical/psp/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/physical/psp/file_data_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/physical/pw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/physical/smearing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/physical/tetrahedron.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.073848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6271 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/model/categorized_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.077848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/model/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/model/mixins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.077848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/model/mixins/dft/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/model/mixins/dft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/model/mixins/dft/double_hybrid_functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/model/mixins/dft/enum_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/model/mixins/dft/gga_functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/model/mixins/dft/hybrid_functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/model/mixins/dft/lda_functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/model/mixins/dft/mgga_functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/model/mixins/dispersion_correction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/model/mixins/enum_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/model/mixins/hubbard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/model/mixins/spin_orbit_coupling.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/model/mixins/spin_polarization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/model/model_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/model/model_without_method.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.077848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_category/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_category/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_category/enum_options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.077848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_category/pb/
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_category/pb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_category/pb/enum_options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.077848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_category/pb/qm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_category/pb/qm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.077848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_category/pb/qm/abin/
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_category/pb/qm/abin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_category/pb/qm/abin/enum_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_category/pb/qm/abin/gw.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.081848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_category/pb/qm/dft/
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_category/pb/qm/dft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_category/pb/qm/dft/enum_options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.081848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_category/pb/qm/dft/ksdft/
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_category/pb/qm/dft/ksdft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_category/pb/qm/dft/ksdft/double_hybrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_category/pb/qm/dft/ksdft/enum_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_category/pb/qm/dft/ksdft/gga.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_category/pb/qm/dft/ksdft/hybrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_category/pb/qm/dft/ksdft/lda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_category/pb/qm/dft/ksdft/mgga.py
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_category/pb/qm/enum_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_category/pb/qm/semp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.081848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_category/st/
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_category/st/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.081848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_category/st/det/
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_category/st/det/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_category/st/det/enum_options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.081848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_category/st/det/ml/
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_category/st/det/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_category/st/det/ml/enum_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_category/st/det/ml/re.py
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_category/st/enum_options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.085848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_directory/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_directory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_directory/double_hybrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_directory/gga.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7149 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_directory/gw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5675 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_directory/hybrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5757 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_directory/lda.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.085848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_directory/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_directory/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_directory/legacy/dft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_directory/legacy/ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_directory/legacy/unknown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5793 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_directory/mgga.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_directory/re.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.085848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/derived_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/electronic_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.085848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/elemental/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/elemental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/elemental/atomic_radius.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/elemental/electronegativity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/elemental/ionization_potential.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.089848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/non_scalar/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/non_scalar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/non_scalar/average_potential_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/non_scalar/band_gaps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/non_scalar/band_structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/non_scalar/charge_density_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/non_scalar/density_of_states.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/non_scalar/dielectric_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/non_scalar/file_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/non_scalar/hubbard_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/non_scalar/hubbard_v.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/non_scalar/hubbard_v_nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/non_scalar/phonon_dispersions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/non_scalar/phonon_dos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/non_scalar/potential_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/non_scalar/reaction_energy_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/non_scalar/stress_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/non_scalar/total_energy_contributions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/non_scalar/vibrational_spectrum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.093848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/scalar/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/scalar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/scalar/electron_affinity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/scalar/fermi_energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/scalar/formation_energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/scalar/ionization_potential.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/scalar/pressure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/scalar/reaction_energy_barrier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/scalar/surface_energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/scalar/total_energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/scalar/total_force.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/scalar/valence_band_offset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/scalar/zero_point_energy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.093848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/structural/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/structural/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/structural/atomic_forces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.093848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/structural/basis/
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/structural/basis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/structural/basis/atomic_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/structural/basis/atomic_coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/structural/basis/atomic_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/structural/basis/atomic_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/structural/basis/bonds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/structural/density.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/structural/elemental_ratio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/structural/inchi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/structural/inchi_key.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.097848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/structural/lattice/
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/structural/lattice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/structural/lattice/lattice_bravais.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/structural/lattice/lattice_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/structural/lattice/type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/structural/lattice/type_extended_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/structural/magnetic_moments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/structural/molecular_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/structural/p_norm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.097848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/structural/patterns/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/structural/patterns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/structural/patterns/functional_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/structural/patterns/ring.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/structural/patterns/special_bond.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/structural/symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/structural/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.913847 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/workflow/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.097848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/workflow/convergence/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/workflow/convergence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/workflow/convergence/electronic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/workflow/convergence/ionic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/workflow/convergence/kpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.097848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/property/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/property/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.097848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/property/base/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.097848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/property/base/The_source_of_a_property/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/property/base/The_source_of_a_property/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/property/base/The_source_of_a_property/field_This_could_be_an_article__a_simulation_on_Exabyte__an_external_simulation__etc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5793 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/property/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.097848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/property/meta/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.097848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/property/meta/The_source_of_a_property/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/property/meta/The_source_of_a_property/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/property/meta/The_source_of_a_property/field_This_could_be_an_article__a_simulation_on_Exabyte__an_external_simulation__etc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5786 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/property/meta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.097848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/property/raw/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.097848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/property/raw/The_source_of_a_property/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/property/raw/The_source_of_a_property/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/property/raw/The_source_of_a_property/field_This_could_be_an_article__a_simulation_on_Exabyte__an_external_simulation__etc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5790 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/property/raw/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.097848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/property/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.101848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/property/source/The_source_of_a_property/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/property/source/The_source_of_a_property/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/property/source/The_source_of_a_property/field_This_could_be_an_article__a_simulation_on_Exabyte__an_external_simulation__etc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/property/source/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.101848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software/executable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software/flavor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.917847 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.101848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/ml/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/ml/exabyteml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.101848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/ml/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/ml/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.101848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/ml/unit/execution/
+-rw-r--r--   0 runner    (1001) docker     (127)    36715 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/ml/unit/execution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.101848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/ml/unit/execution/evaluate/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/ml/unit/execution/evaluate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10067 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/ml/unit/execution/evaluate/cross_validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10088 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/ml/unit/execution/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9894 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/ml/unit/execution/score.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10108 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/ml/unit/execution/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.101848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/ml/unit/processing/
+-rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/ml/unit/processing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.101848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/ml/unit/processing/data_transformation/
+-rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/ml/unit/processing/data_transformation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/ml/unit/processing/data_transformation/manipulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/ml/unit/processing/data_transformation/scale_and_reduce.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.101848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/ml/unit/processing/feature_selection/
+-rw-r--r--   0 runner    (1001) docker     (127)     4382 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/ml/unit/processing/feature_selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/ml/unit/processing/feature_selection/filter_based.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.105848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/modeling/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/modeling/deepmd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.105848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/modeling/espresso/
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/modeling/espresso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/modeling/espresso/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/modeling/nwchem.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.105848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/modeling/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/modeling/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10439 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/modeling/unit/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/modeling/vasp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.105848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/scripting/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/scripting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/scripting/jupyter_lab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/scripting/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/scripting/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.105848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/scripting/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/scripting/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10408 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/scripting/unit/execution.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.113848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/system/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/system/_material.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/system/_parent_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/system/_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/system/bankable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/system/consistency_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/system/creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/system/creator_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/system/database_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/system/defaultable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/system/description.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/system/entity_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/system/file_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/system/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/system/iframe_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/system/in_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/system/is_multi_material.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/system/is_outdated.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/system/job_extended.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/system/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/system/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/system/name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/system/owner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/system/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/system/path_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/system/schema_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/system/scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/system/set.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/system/sharing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/system/soft_removable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/system/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/system/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/system/timestampable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/system/use_values.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.917847 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/third_party/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.917847 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/third_party/db/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.917847 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/third_party/db/nist_jarvis/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.113848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/third_party/db/nist_jarvis/2024.3.13/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/third_party/db/nist_jarvis/2024.3.13/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/third_party/db/nist_jarvis/2024.3.13/atoms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/third_party/db/nist_jarvis/2024.3.13/db_entry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.917847 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/third_party/file/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.917847 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/third_party/file/applications/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.917847 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/third_party/file/applications/espresso/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.113848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/third_party/file/applications/espresso/7.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/third_party/file/applications/espresso/7.2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.113848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/third_party/file/applications/espresso/7.2/pw.x/
+-rw-r--r--   0 runner    (1001) docker     (127)    74617 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/third_party/file/applications/espresso/7.2/pw.x/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/third_party/file/applications/espresso/7.2/pw.x/atomic_positions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/third_party/file/applications/espresso/7.2/pw.x/atomic_species.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/third_party/file/applications/espresso/7.2/pw.x/cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/third_party/file/applications/espresso/7.2/pw.x/cell_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8786 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/third_party/file/applications/espresso/7.2/pw.x/control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/third_party/file/applications/espresso/7.2/pw.x/electrons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4439 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/third_party/file/applications/espresso/7.2/pw.x/hubbard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15280 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/third_party/file/applications/espresso/7.2/pw.x/ions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/third_party/file/applications/espresso/7.2/pw.x/k_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34350 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/third_party/file/applications/espresso/7.2/pw.x/system.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.117848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)    76517 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5987 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/base_flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/scope.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.117848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/subworkflow/
+-rw-r--r--   0 runner    (1001) docker     (127)    39880 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/subworkflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31216 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/subworkflow/unit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.117848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)    37479 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/unit/assertion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/unit/assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/unit/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/unit/condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9880 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/unit/execution.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.117848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/unit/input/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/unit/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/unit/input/_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/unit/input/_inputItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/unit/input/_inputItemId.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/unit/input/_inputItemScope.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.121848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/unit/input/_map_input/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/unit/input/_map_input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/unit/input/_map_input/values.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.121848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/unit/io/
+-rw-r--r--   0 runner    (1001) docker     (127)     5869 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/unit/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/unit/io/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/unit/io/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/unit/io/object_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4244 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/unit/map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/unit/processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/unit/reduce.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.121848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/unit/runtime/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/unit/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/unit/runtime/_runtime_item_full_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/unit/runtime/_runtime_item_name_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/unit/runtime/_runtime_item_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/unit/runtime/runtime_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/unit/runtime/runtime_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/unit/subworkflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.125848 mat3ra-esse-2024.4.8.post4/src/py/mat3ra_esse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8795 2024-04-08 11:31:47.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra_esse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    59789 2024-04-08 11:31:47.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra_esse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 11:31:47.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra_esse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-08 11:31:47.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra_esse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-08 11:31:47.000000 mat3ra-esse-2024.4.8.post4/src/py/mat3ra_esse.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.917847 mat3ra-esse-2024.4.8.post4/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.121848 mat3ra-esse-2024.4.8.post4/tests/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/tests/js/JSONSchemasInterface.tests.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:47.917847 mat3ra-esse-2024.4.8.post4/tests/js/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.121848 mat3ra-esse-2024.4.8.post4/tests/js/fixtures/json/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/tests/js/fixtures/json/1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/tests/js/fixtures/json/2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/tests/js/validate.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.125848 mat3ra-esse-2024.4.8.post4/tests/py/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/tests/py/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:48.125848 mat3ra-esse-2024.4.8.post4/tests/py/esse/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/tests/py/esse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/tests/py/esse/test_validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/tsconfig-transpile.json
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-08 11:31:29.000000 mat3ra-esse-2024.4.8.post4/tsconfig.json
```

### Comparing `mat3ra-esse-2024.4.8.post3/.github/workflows/cicd.yml` & `mat3ra-esse-2024.4.8.post4/.github/workflows/cicd.yml`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/.gitignore` & `mat3ra-esse-2024.4.8.post4/.gitignore`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/.husky/pre-commit` & `mat3ra-esse-2024.4.8.post4/.husky/pre-commit`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/.pre-commit-config.yaml` & `mat3ra-esse-2024.4.8.post4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/LICENSE.md` & `mat3ra-esse-2024.4.8.post4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/PKG-INFO` & `mat3ra-esse-2024.4.8.post4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mat3ra-esse
-Version: 2024.4.8.post3
+Version: 2024.4.8.post4
 Summary: Excellent Source of Schemas and Examples.
 Author-email: "Exabyte Inc." <info@mat3ra.com>
 License: # LICENSE
         
         Copyright 2019 Exabyte Inc.
         
         Licensed under the Apache License, Version 2.0 (the "License");
@@ -25,16 +25,14 @@
 Classifier: Topic :: Software Development
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: exabyte-json-include>=2023.12.23.post0
 Requires-Dist: jsonschema>=2.6.0
 Requires-Dist: datamodel-code-generator>=0.25.5
-Requires-Dist: pydantic
-Requires-Dist: gradio
 Provides-Extra: tests
 Requires-Dist: coverage[toml]>=5.3; extra == "tests"
 Requires-Dist: parameterized>=0.9.0; extra == "tests"
 Provides-Extra: all
 Requires-Dist: mat3ra-esse[tests]; extra == "all"
 
 [![PyPI version](https://badge.fury.io/py/mat3ra-esse.svg)](https://badge.fury.io/py/mat3ra-esse)
```

### Comparing `mat3ra-esse-2024.4.8.post3/README.md` & `mat3ra-esse-2024.4.8.post4/README.md`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/build_schemas.py` & `mat3ra-esse-2024.4.8.post4/build_schemas.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/build_schemas.ts` & `mat3ra-esse-2024.4.8.post4/build_schemas.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/example/3pse/db/nist_jarvis/2024.3.13/db_entry.json` & `mat3ra-esse-2024.4.8.post4/example/3pse/db/nist_jarvis/2024.3.13/db_entry.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/example/3pse/file/applications/espresso/7.2/pw.x.json` & `mat3ra-esse-2024.4.8.post4/example/3pse/file/applications/espresso/7.2/pw.x.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/example/job/compute.json` & `mat3ra-esse-2024.4.8.post4/example/job/compute.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/example/job.json` & `mat3ra-esse-2024.4.8.post4/example/job.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/example/material.json` & `mat3ra-esse-2024.4.8.post4/example/material.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/example/method/categorized_method.json` & `mat3ra-esse-2024.4.8.post4/example/method/categorized_method.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/example/methods_directory/legacy/regression.json` & `mat3ra-esse-2024.4.8.post4/example/methods_directory/legacy/regression.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/example/methods_directory/mathematical/regression.json` & `mat3ra-esse-2024.4.8.post4/example/methods_directory/mathematical/regression.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/example/methods_directory/physical/psp/file.json` & `mat3ra-esse-2024.4.8.post4/example/methods_directory/physical/psp/file.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/example/model/categorized_model.json` & `mat3ra-esse-2024.4.8.post4/example/model/categorized_model.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/example/properties_directory/non-scalar/band_structure.json` & `mat3ra-esse-2024.4.8.post4/example/properties_directory/non-scalar/band_structure.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/example/properties_directory/non-scalar/density_of_states.json` & `mat3ra-esse-2024.4.8.post4/example/properties_directory/non-scalar/density_of_states.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/example/properties_directory/non-scalar/dielectric_tensor.json` & `mat3ra-esse-2024.4.8.post4/example/properties_directory/non-scalar/dielectric_tensor.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/example/properties_directory/non-scalar/hubbard_v_nn.json` & `mat3ra-esse-2024.4.8.post4/example/properties_directory/non-scalar/hubbard_v_nn.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/example/properties_directory/non-scalar/phonon_dispersions.json` & `mat3ra-esse-2024.4.8.post4/example/properties_directory/non-scalar/phonon_dispersions.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/example/properties_directory/non-scalar/phonon_dos.json` & `mat3ra-esse-2024.4.8.post4/example/properties_directory/non-scalar/phonon_dos.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/example/properties_directory/non-scalar/potential_profile.json` & `mat3ra-esse-2024.4.8.post4/example/properties_directory/non-scalar/potential_profile.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/example/properties_directory/non-scalar/reaction_energy_profile.json` & `mat3ra-esse-2024.4.8.post4/example/properties_directory/non-scalar/reaction_energy_profile.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/example/properties_directory/non-scalar/total_energy_contributions.json` & `mat3ra-esse-2024.4.8.post4/example/properties_directory/non-scalar/total_energy_contributions.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/example/properties_directory/structural/molecular_pattern.json` & `mat3ra-esse-2024.4.8.post4/example/properties_directory/structural/molecular_pattern.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/example/software_directory/ml/unit/execution/train.json` & `mat3ra-esse-2024.4.8.post4/example/software_directory/ml/unit/execution/train.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/example/software_directory/ml/unit/processing/data_transformation/scale_and_reduce.json` & `mat3ra-esse-2024.4.8.post4/example/software_directory/ml/unit/processing/data_transformation/scale_and_reduce.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/example/system/file_source.json` & `mat3ra-esse-2024.4.8.post4/example/system/file_source.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/example/workflow/unit/execution.json` & `mat3ra-esse-2024.4.8.post4/example/workflow/unit/execution.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/example/workflow/unit/io/api.json` & `mat3ra-esse-2024.4.8.post4/example/workflow/unit/io/api.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/example/workflow/unit/io.json` & `mat3ra-esse-2024.4.8.post4/example/workflow/unit/io.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/example/workflow.json` & `mat3ra-esse-2024.4.8.post4/example/workflow.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/manifest/dft_unit_functionals.yaml` & `mat3ra-esse-2024.4.8.post4/manifest/dft_unit_functionals.yaml`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/manifest/functional_lookup_table.yaml` & `mat3ra-esse-2024.4.8.post4/manifest/functional_lookup_table.yaml`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/manifest/models.yaml` & `mat3ra-esse-2024.4.8.post4/manifest/models.yaml`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/manifest/properties.yaml` & `mat3ra-esse-2024.4.8.post4/manifest/properties.yaml`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/package-lock.json` & `mat3ra-esse-2024.4.8.post4/package-lock.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/package.json` & `mat3ra-esse-2024.4.8.post4/package.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/pyproject.toml` & `mat3ra-esse-2024.4.8.post4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,14 @@
     "Development Status :: 3 - Alpha",
     "Topic :: Software Development",
 ]
 dependencies = [
     "exabyte-json-include>=2023.12.23.post0",
     "jsonschema>=2.6.0",
     "datamodel-code-generator>=0.25.5",
-    "pydantic",
-    "gradio",
     # "python-slugify==2.0.1",
     # PyYAML install could be problematic, see https://github.com/yaml/pyyaml/issues/601
     # To avoid "AttributeError: cython_sources", consider "cython<3.0.0", the below might be needed:
     #"PyYAML==5.4.1",
     # "Unidecode==1.1.1",
     # "toml==0.10.2",
     # "importlib-resources==5.2.2",
```

### Comparing `mat3ra-esse-2024.4.8.post3/schema/3pse/db/nist_jarvis/2024.3.13/atoms.json` & `mat3ra-esse-2024.4.8.post4/schema/3pse/db/nist_jarvis/2024.3.13/atoms.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/3pse/db/nist_jarvis/2024.3.13/db_entry.json` & `mat3ra-esse-2024.4.8.post4/schema/3pse/db/nist_jarvis/2024.3.13/db_entry.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/3pse/file/applications/espresso/7.2/pw.x/atomic_positions.json` & `mat3ra-esse-2024.4.8.post4/schema/3pse/file/applications/espresso/7.2/pw.x/atomic_positions.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/3pse/file/applications/espresso/7.2/pw.x/atomic_species.json` & `mat3ra-esse-2024.4.8.post4/schema/3pse/file/applications/espresso/7.2/pw.x/atomic_species.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/3pse/file/applications/espresso/7.2/pw.x/cell.json` & `mat3ra-esse-2024.4.8.post4/schema/3pse/file/applications/espresso/7.2/pw.x/cell.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/3pse/file/applications/espresso/7.2/pw.x/cell_parameters.json` & `mat3ra-esse-2024.4.8.post4/schema/3pse/file/applications/espresso/7.2/pw.x/cell_parameters.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/3pse/file/applications/espresso/7.2/pw.x/control.json` & `mat3ra-esse-2024.4.8.post4/schema/3pse/file/applications/espresso/7.2/pw.x/control.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/3pse/file/applications/espresso/7.2/pw.x/electrons.json` & `mat3ra-esse-2024.4.8.post4/schema/3pse/file/applications/espresso/7.2/pw.x/electrons.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/3pse/file/applications/espresso/7.2/pw.x/hubbard.json` & `mat3ra-esse-2024.4.8.post4/schema/3pse/file/applications/espresso/7.2/pw.x/hubbard.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/3pse/file/applications/espresso/7.2/pw.x/ions.json` & `mat3ra-esse-2024.4.8.post4/schema/3pse/file/applications/espresso/7.2/pw.x/ions.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/3pse/file/applications/espresso/7.2/pw.x/k_points.json` & `mat3ra-esse-2024.4.8.post4/schema/3pse/file/applications/espresso/7.2/pw.x/k_points.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/3pse/file/applications/espresso/7.2/pw.x/system.json` & `mat3ra-esse-2024.4.8.post4/schema/3pse/file/applications/espresso/7.2/pw.x/system.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/3pse/file/applications/espresso/7.2/pw.x.json` & `mat3ra-esse-2024.4.8.post4/schema/3pse/file/applications/espresso/7.2/pw.x.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/core/abstract/2d_plot.json` & `mat3ra-esse-2024.4.8.post4/schema/core/abstract/2d_plot.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/core/abstract/3d_vector_basis.json` & `mat3ra-esse-2024.4.8.post4/schema/core/abstract/3d_vector_basis.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/core/primitive/3d_lattice.json` & `mat3ra-esse-2024.4.8.post4/schema/core/primitive/3d_lattice.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/core/primitive/linked_list/base_node.json` & `mat3ra-esse-2024.4.8.post4/schema/core/primitive/linked_list/base_node.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/core/primitive/linked_list.json` & `mat3ra-esse-2024.4.8.post4/schema/core/primitive/linked_list.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/core/primitive/slugified_entry.json` & `mat3ra-esse-2024.4.8.post4/schema/core/primitive/slugified_entry.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/core/reference/exabyte.json` & `mat3ra-esse-2024.4.8.post4/schema/core/reference/exabyte.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/core/reference/experiment/condition.json` & `mat3ra-esse-2024.4.8.post4/schema/core/reference/experiment/condition.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/core/reference/experiment.json` & `mat3ra-esse-2024.4.8.post4/schema/core/reference/experiment.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/core/reference/literature.json` & `mat3ra-esse-2024.4.8.post4/schema/core/reference/literature.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/core/reference/modeling/exabyte.json` & `mat3ra-esse-2024.4.8.post4/schema/core/reference/modeling/exabyte.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/core/reusable/atomic_data/per_orbital.json` & `mat3ra-esse-2024.4.8.post4/schema/core/reusable/atomic_data/per_orbital.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/core/reusable/atomic_data/per_orbital_pair.json` & `mat3ra-esse-2024.4.8.post4/schema/core/reusable/atomic_data/per_orbital_pair.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/core/reusable/atomic_orbital.json` & `mat3ra-esse-2024.4.8.post4/schema/core/reusable/atomic_orbital.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/core/reusable/band_gap.json` & `mat3ra-esse-2024.4.8.post4/schema/core/reusable/band_gap.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/core/reusable/categories.json` & `mat3ra-esse-2024.4.8.post4/schema/core/reusable/categories.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/core/reusable/dielectric_tensor_component.json` & `mat3ra-esse-2024.4.8.post4/schema/core/reusable/dielectric_tensor_component.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/core/reusable/energy.json` & `mat3ra-esse-2024.4.8.post4/schema/core/reusable/energy.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/core/reusable/file_metadata.json` & `mat3ra-esse-2024.4.8.post4/schema/core/reusable/file_metadata.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/core/reusable/frequency_function_matrix.json` & `mat3ra-esse-2024.4.8.post4/schema/core/reusable/frequency_function_matrix.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/core/reusable/object_storage_container_data.json` & `mat3ra-esse-2024.4.8.post4/schema/core/reusable/object_storage_container_data.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/definitions/units.json` & `mat3ra-esse-2024.4.8.post4/schema/definitions/units.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/element.json` & `mat3ra-esse-2024.4.8.post4/schema/element.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/in_memory_entity/base.json` & `mat3ra-esse-2024.4.8.post4/schema/in_memory_entity/base.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/job/base.json` & `mat3ra-esse-2024.4.8.post4/schema/job/base.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/job/compute.json` & `mat3ra-esse-2024.4.8.post4/schema/job/compute.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/material.json` & `mat3ra-esse-2024.4.8.post4/schema/material.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/method/categorized_method.json` & `mat3ra-esse-2024.4.8.post4/schema/method/categorized_method.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/method/method_parameters.json` & `mat3ra-esse-2024.4.8.post4/schema/method/method_parameters.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/method/unit_method.json` & `mat3ra-esse-2024.4.8.post4/schema/method/unit_method.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/method.json` & `mat3ra-esse-2024.4.8.post4/schema/method.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/enum_options.json` & `mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/enum_options.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/methods_category/mathematical/linalg/enum_options.yml` & `mat3ra-esse-2024.4.8.post4/schema/methods_category/mathematical/linalg/enum_options.yml`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/methods_category/physical/qm/wf/enum_options.json` & `mat3ra-esse-2024.4.8.post4/schema/methods_category/physical/qm/wf/enum_options.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/methods_category/physical/qm/wf/enum_options.yml` & `mat3ra-esse-2024.4.8.post4/schema/methods_category/physical/qm/wf/enum_options.yml`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/methods_category/physical/qm/wf/smearing.json` & `mat3ra-esse-2024.4.8.post4/schema/methods_category/physical/qm/wf/smearing.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/methods_directory/legacy/pseudopotential.json` & `mat3ra-esse-2024.4.8.post4/schema/methods_directory/legacy/pseudopotential.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/methods_directory/legacy/regression.json` & `mat3ra-esse-2024.4.8.post4/schema/methods_directory/legacy/regression.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/methods_directory/mathematical/cg.json` & `mat3ra-esse-2024.4.8.post4/schema/methods_directory/mathematical/cg.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/methods_directory/mathematical/davidson.json` & `mat3ra-esse-2024.4.8.post4/schema/methods_directory/mathematical/davidson.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/methods_directory/mathematical/regression/data.json` & `mat3ra-esse-2024.4.8.post4/schema/methods_directory/mathematical/regression/data.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/methods_directory/mathematical/regression/dataset.json` & `mat3ra-esse-2024.4.8.post4/schema/methods_directory/mathematical/regression/dataset.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/methods_directory/mathematical/regression/kernel_ridge/data_per_property.json` & `mat3ra-esse-2024.4.8.post4/schema/methods_directory/mathematical/regression/kernel_ridge/data_per_property.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/methods_directory/mathematical/regression/linear/data_per_property.json` & `mat3ra-esse-2024.4.8.post4/schema/methods_directory/mathematical/regression/linear/data_per_property.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/methods_directory/mathematical/regression/per_feature_item.json` & `mat3ra-esse-2024.4.8.post4/schema/methods_directory/mathematical/regression/per_feature_item.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/methods_directory/mathematical/regression/precision_per_property.json` & `mat3ra-esse-2024.4.8.post4/schema/methods_directory/mathematical/regression/precision_per_property.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/methods_directory/mathematical/regression.json` & `mat3ra-esse-2024.4.8.post4/schema/methods_directory/mathematical/regression.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/methods_directory/physical/ao/dunning.json` & `mat3ra-esse-2024.4.8.post4/schema/methods_directory/physical/ao/dunning.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/methods_directory/physical/ao/enum_options.json` & `mat3ra-esse-2024.4.8.post4/schema/methods_directory/physical/ao/enum_options.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/methods_directory/physical/ao/other.json` & `mat3ra-esse-2024.4.8.post4/schema/methods_directory/physical/ao/other.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/methods_directory/physical/ao/pople.json` & `mat3ra-esse-2024.4.8.post4/schema/methods_directory/physical/ao/pople.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/methods_directory/physical/psp/file.json` & `mat3ra-esse-2024.4.8.post4/schema/methods_directory/physical/psp/file.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/methods_directory/physical/psp/file_data_item.json` & `mat3ra-esse-2024.4.8.post4/schema/methods_directory/physical/psp/file_data_item.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/methods_directory/physical/psp.json` & `mat3ra-esse-2024.4.8.post4/schema/methods_directory/physical/psp.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/methods_directory/physical/pw.json` & `mat3ra-esse-2024.4.8.post4/schema/methods_directory/physical/pw.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/methods_directory/physical/smearing.json` & `mat3ra-esse-2024.4.8.post4/schema/methods_directory/physical/smearing.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/model/model_parameters.json` & `mat3ra-esse-2024.4.8.post4/schema/model/model_parameters.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/model/model_without_method.json` & `mat3ra-esse-2024.4.8.post4/schema/model/model_without_method.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/model.json` & `mat3ra-esse-2024.4.8.post4/schema/model.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/models_directory/double_hybrid.json` & `mat3ra-esse-2024.4.8.post4/schema/models_directory/double_hybrid.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/models_directory/gga.json` & `mat3ra-esse-2024.4.8.post4/schema/models_directory/gga.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/models_directory/gw.json` & `mat3ra-esse-2024.4.8.post4/schema/models_directory/gw.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/models_directory/hybrid.json` & `mat3ra-esse-2024.4.8.post4/schema/models_directory/hybrid.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/models_directory/lda.json` & `mat3ra-esse-2024.4.8.post4/schema/models_directory/lda.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/models_directory/legacy/dft.json` & `mat3ra-esse-2024.4.8.post4/schema/models_directory/legacy/dft.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/models_directory/mgga.json` & `mat3ra-esse-2024.4.8.post4/schema/models_directory/mgga.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/models_directory/re.json` & `mat3ra-esse-2024.4.8.post4/schema/models_directory/re.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/project.json` & `mat3ra-esse-2024.4.8.post4/schema/project.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/properties_directory/derived_properties.json` & `mat3ra-esse-2024.4.8.post4/schema/properties_directory/derived_properties.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/properties_directory/elemental/atomic_radius.json` & `mat3ra-esse-2024.4.8.post4/schema/properties_directory/elemental/atomic_radius.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/properties_directory/elemental/ionization_potential.json` & `mat3ra-esse-2024.4.8.post4/schema/properties_directory/elemental/ionization_potential.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/properties_directory/non-scalar/average_potential_profile.json` & `mat3ra-esse-2024.4.8.post4/schema/properties_directory/non-scalar/average_potential_profile.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/properties_directory/non-scalar/band_gaps.json` & `mat3ra-esse-2024.4.8.post4/schema/properties_directory/non-scalar/band_gaps.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/properties_directory/non-scalar/band_structure.json` & `mat3ra-esse-2024.4.8.post4/schema/properties_directory/non-scalar/band_structure.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/properties_directory/non-scalar/charge_density_profile.json` & `mat3ra-esse-2024.4.8.post4/schema/properties_directory/non-scalar/charge_density_profile.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/properties_directory/non-scalar/density_of_states.json` & `mat3ra-esse-2024.4.8.post4/schema/properties_directory/non-scalar/density_of_states.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/properties_directory/non-scalar/dielectric_tensor.json` & `mat3ra-esse-2024.4.8.post4/schema/properties_directory/non-scalar/dielectric_tensor.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/properties_directory/non-scalar/file_content.json` & `mat3ra-esse-2024.4.8.post4/schema/properties_directory/non-scalar/file_content.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/properties_directory/non-scalar/hubbard_u.json` & `mat3ra-esse-2024.4.8.post4/schema/properties_directory/non-scalar/hubbard_u.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/properties_directory/non-scalar/hubbard_v.json` & `mat3ra-esse-2024.4.8.post4/schema/properties_directory/non-scalar/hubbard_v.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/properties_directory/non-scalar/phonon_dispersions.json` & `mat3ra-esse-2024.4.8.post4/schema/properties_directory/non-scalar/phonon_dispersions.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/properties_directory/non-scalar/phonon_dos.json` & `mat3ra-esse-2024.4.8.post4/schema/properties_directory/non-scalar/phonon_dos.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/properties_directory/non-scalar/potential_profile.json` & `mat3ra-esse-2024.4.8.post4/schema/properties_directory/non-scalar/potential_profile.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/properties_directory/non-scalar/reaction_energy_profile.json` & `mat3ra-esse-2024.4.8.post4/schema/properties_directory/non-scalar/reaction_energy_profile.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/properties_directory/non-scalar/total_energy_contributions.json` & `mat3ra-esse-2024.4.8.post4/schema/properties_directory/non-scalar/total_energy_contributions.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/properties_directory/non-scalar/vibrational_spectrum.json` & `mat3ra-esse-2024.4.8.post4/schema/properties_directory/non-scalar/vibrational_spectrum.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/properties_directory/scalar/pressure.json` & `mat3ra-esse-2024.4.8.post4/schema/properties_directory/scalar/pressure.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/properties_directory/structural/atomic_forces.json` & `mat3ra-esse-2024.4.8.post4/schema/properties_directory/structural/atomic_forces.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/properties_directory/structural/basis/atomic_coordinates.json` & `mat3ra-esse-2024.4.8.post4/schema/properties_directory/structural/basis/atomic_coordinates.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/properties_directory/structural/basis/atomic_element.json` & `mat3ra-esse-2024.4.8.post4/schema/properties_directory/structural/basis/atomic_element.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/properties_directory/structural/basis/bonds.json` & `mat3ra-esse-2024.4.8.post4/schema/properties_directory/structural/basis/bonds.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/properties_directory/structural/basis.json` & `mat3ra-esse-2024.4.8.post4/schema/properties_directory/structural/basis.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/properties_directory/structural/elemental_ratio.json` & `mat3ra-esse-2024.4.8.post4/schema/properties_directory/structural/elemental_ratio.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/properties_directory/structural/lattice/lattice_bravais.json` & `mat3ra-esse-2024.4.8.post4/schema/properties_directory/structural/lattice/lattice_bravais.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/properties_directory/structural/lattice/lattice_vectors.json` & `mat3ra-esse-2024.4.8.post4/schema/properties_directory/structural/lattice/lattice_vectors.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/properties_directory/structural/lattice/type_extended_enum.json` & `mat3ra-esse-2024.4.8.post4/schema/properties_directory/structural/lattice/type_extended_enum.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/properties_directory/structural/lattice.json` & `mat3ra-esse-2024.4.8.post4/schema/properties_directory/structural/lattice.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/properties_directory/structural/magnetic_moments.json` & `mat3ra-esse-2024.4.8.post4/schema/properties_directory/structural/magnetic_moments.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/properties_directory/structural/p-norm.json` & `mat3ra-esse-2024.4.8.post4/schema/properties_directory/structural/p-norm.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/properties_directory/structural/patterns/functional_group.json` & `mat3ra-esse-2024.4.8.post4/schema/properties_directory/structural/patterns/functional_group.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/properties_directory/structural/patterns/ring.json` & `mat3ra-esse-2024.4.8.post4/schema/properties_directory/structural/patterns/ring.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/properties_directory/structural/patterns/special_bond.json` & `mat3ra-esse-2024.4.8.post4/schema/properties_directory/structural/patterns/special_bond.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/properties_directory/structural/symmetry.json` & `mat3ra-esse-2024.4.8.post4/schema/properties_directory/structural/symmetry.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/properties_directory/workflow/convergence/electronic.json` & `mat3ra-esse-2024.4.8.post4/schema/properties_directory/workflow/convergence/electronic.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/properties_directory/workflow/convergence/ionic.json` & `mat3ra-esse-2024.4.8.post4/schema/properties_directory/workflow/convergence/ionic.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/properties_directory/workflow/convergence/kpoint.json` & `mat3ra-esse-2024.4.8.post4/schema/properties_directory/workflow/convergence/kpoint.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/property/base.json` & `mat3ra-esse-2024.4.8.post4/schema/property/base.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/property/raw.json` & `mat3ra-esse-2024.4.8.post4/schema/property/raw.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/property/source.json` & `mat3ra-esse-2024.4.8.post4/schema/property/source.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/software/application.json` & `mat3ra-esse-2024.4.8.post4/schema/software/application.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/software/executable.json` & `mat3ra-esse-2024.4.8.post4/schema/software/executable.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/software/flavor.json` & `mat3ra-esse-2024.4.8.post4/schema/software/flavor.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/software/template.json` & `mat3ra-esse-2024.4.8.post4/schema/software/template.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/software_directory/ml/exabyteml.json` & `mat3ra-esse-2024.4.8.post4/schema/software_directory/ml/exabyteml.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/software_directory/ml/unit/execution/evaluate/cross-validate.json` & `mat3ra-esse-2024.4.8.post4/schema/software_directory/ml/unit/execution/evaluate/cross-validate.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/software_directory/ml/unit/execution/initialize.json` & `mat3ra-esse-2024.4.8.post4/schema/software_directory/ml/unit/execution/initialize.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/software_directory/ml/unit/execution/train.json` & `mat3ra-esse-2024.4.8.post4/schema/software_directory/ml/unit/execution/train.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/software_directory/ml/unit/processing/data_transformation/manipulation.json` & `mat3ra-esse-2024.4.8.post4/schema/software_directory/ml/unit/processing/data_transformation/manipulation.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/software_directory/ml/unit/processing/data_transformation/scale_and_reduce.json` & `mat3ra-esse-2024.4.8.post4/schema/software_directory/ml/unit/processing/data_transformation/scale_and_reduce.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/software_directory/ml/unit/processing/feature_selection/filter_based.json` & `mat3ra-esse-2024.4.8.post4/schema/software_directory/ml/unit/processing/feature_selection/filter_based.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/software_directory/modeling/deepmd.json` & `mat3ra-esse-2024.4.8.post4/schema/software_directory/modeling/deepmd.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/software_directory/modeling/espresso/arguments.json` & `mat3ra-esse-2024.4.8.post4/schema/software_directory/modeling/espresso/arguments.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/software_directory/modeling/espresso.json` & `mat3ra-esse-2024.4.8.post4/schema/software_directory/modeling/espresso.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/software_directory/modeling/nwchem.json` & `mat3ra-esse-2024.4.8.post4/schema/software_directory/modeling/nwchem.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/software_directory/modeling/vasp.json` & `mat3ra-esse-2024.4.8.post4/schema/software_directory/modeling/vasp.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/software_directory/scripting/jupyter-lab.json` & `mat3ra-esse-2024.4.8.post4/schema/software_directory/scripting/jupyter-lab.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/software_directory/scripting/python.json` & `mat3ra-esse-2024.4.8.post4/schema/software_directory/scripting/python.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/software_directory/scripting/shell.json` & `mat3ra-esse-2024.4.8.post4/schema/software_directory/scripting/shell.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/system/consistency_check.json` & `mat3ra-esse-2024.4.8.post4/schema/system/consistency_check.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/system/database_source.json` & `mat3ra-esse-2024.4.8.post4/schema/system/database_source.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/system/file_source.json` & `mat3ra-esse-2024.4.8.post4/schema/system/file_source.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/system/history.json` & `mat3ra-esse-2024.4.8.post4/schema/system/history.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/system/iframe_message.json` & `mat3ra-esse-2024.4.8.post4/schema/system/iframe_message.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/system/in_set.json` & `mat3ra-esse-2024.4.8.post4/schema/system/in_set.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/system/job_extended.json` & `mat3ra-esse-2024.4.8.post4/schema/system/job_extended.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/system/message.json` & `mat3ra-esse-2024.4.8.post4/schema/system/message.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/system/status.json` & `mat3ra-esse-2024.4.8.post4/schema/system/status.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/system/timestampable.json` & `mat3ra-esse-2024.4.8.post4/schema/system/timestampable.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/workflow/base.json` & `mat3ra-esse-2024.4.8.post4/schema/workflow/base.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/workflow/base_flow.json` & `mat3ra-esse-2024.4.8.post4/schema/workflow/base_flow.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/workflow/subworkflow/unit.json` & `mat3ra-esse-2024.4.8.post4/schema/workflow/subworkflow/unit.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/workflow/subworkflow.json` & `mat3ra-esse-2024.4.8.post4/schema/workflow/subworkflow.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/workflow/unit/assertion.json` & `mat3ra-esse-2024.4.8.post4/schema/workflow/unit/assertion.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/workflow/unit/assignment.json` & `mat3ra-esse-2024.4.8.post4/schema/workflow/unit/assignment.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/workflow/unit/base.json` & `mat3ra-esse-2024.4.8.post4/schema/workflow/unit/base.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/workflow/unit/condition.json` & `mat3ra-esse-2024.4.8.post4/schema/workflow/unit/condition.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/workflow/unit/execution.json` & `mat3ra-esse-2024.4.8.post4/schema/workflow/unit/execution.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/workflow/unit/input/_input.json` & `mat3ra-esse-2024.4.8.post4/schema/workflow/unit/input/_input.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/workflow/unit/input/_inputItem.json` & `mat3ra-esse-2024.4.8.post4/schema/workflow/unit/input/_inputItem.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/workflow/unit/input/_inputItemId.json` & `mat3ra-esse-2024.4.8.post4/schema/workflow/unit/input/_inputItemId.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/workflow/unit/input/_inputItemScope.json` & `mat3ra-esse-2024.4.8.post4/schema/workflow/unit/input/_inputItemScope.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/workflow/unit/input/_map_input.json` & `mat3ra-esse-2024.4.8.post4/schema/workflow/unit/input/_map_input.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/workflow/unit/io/api.json` & `mat3ra-esse-2024.4.8.post4/schema/workflow/unit/io/api.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/workflow/unit/io/db.json` & `mat3ra-esse-2024.4.8.post4/schema/workflow/unit/io/db.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/workflow/unit/io/object_storage.json` & `mat3ra-esse-2024.4.8.post4/schema/workflow/unit/io/object_storage.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/workflow/unit/io.json` & `mat3ra-esse-2024.4.8.post4/schema/workflow/unit/io.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/workflow/unit/map.json` & `mat3ra-esse-2024.4.8.post4/schema/workflow/unit/map.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/workflow/unit/processing.json` & `mat3ra-esse-2024.4.8.post4/schema/workflow/unit/processing.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/workflow/unit/reduce.json` & `mat3ra-esse-2024.4.8.post4/schema/workflow/unit/reduce.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/workflow/unit/runtime/runtime_items.json` & `mat3ra-esse-2024.4.8.post4/schema/workflow/unit/runtime/runtime_items.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/workflow/unit.json` & `mat3ra-esse-2024.4.8.post4/schema/workflow/unit.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/schema/workflow.json` & `mat3ra-esse-2024.4.8.post4/schema/workflow.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/js/esse/JSONSchemasGenerator.ts` & `mat3ra-esse-2024.4.8.post4/src/js/esse/JSONSchemasGenerator.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/js/esse/JSONSchemasInterface.ts` & `mat3ra-esse-2024.4.8.post4/src/js/esse/JSONSchemasInterface.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/js/esse/JSONSchemasInterfaceServer.ts` & `mat3ra-esse-2024.4.8.post4/src/js/esse/JSONSchemasInterfaceServer.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/js/esse/schemaUtils.ts` & `mat3ra-esse-2024.4.8.post4/src/js/esse/schemaUtils.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/js/esse/utils.ts` & `mat3ra-esse-2024.4.8.post4/src/js/esse/utils.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/js/json_include/index.ts` & `mat3ra-esse-2024.4.8.post4/src/js/json_include/index.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/js/scripts/compileTs.ts` & `mat3ra-esse-2024.4.8.post4/src/js/scripts/compileTs.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/js/scripts/createEnumsFromYaml.ts` & `mat3ra-esse-2024.4.8.post4/src/js/scripts/createEnumsFromYaml.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/js/scripts/setSchemaIds.ts` & `mat3ra-esse-2024.4.8.post4/src/js/scripts/setSchemaIds.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/js/utils/ajv.ts` & `mat3ra-esse-2024.4.8.post4/src/js/utils/ajv.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/js/utils/common.ts` & `mat3ra-esse-2024.4.8.post4/src/js/utils/common.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/js/utils/filesystem.ts` & `mat3ra-esse-2024.4.8.post4/src/js/utils/filesystem.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/__init__.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/__init__.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/data/examples.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/data/examples.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/data/properties.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/data/properties.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/data/schemas.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/data/schemas.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/abstract/2d_plot.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/abstract/2d_plot.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/abstract/3d_tensor.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/abstract/3d_tensor.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/abstract/3d_vector_basis.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/abstract/3d_vector_basis.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/primitive/3d_lattice.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/primitive/3d_lattice.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/primitive/linked_list/__init__.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/primitive/linked_list/__init__.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/primitive/linked_list/base_node.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/primitive/linked_list/base_node.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/primitive/linked_list/named_node.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/primitive/linked_list/named_node.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/primitive/linked_list/named_node_in_group.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/primitive/linked_list/named_node_in_group.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/primitive/linked_list/node_with_type.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/primitive/linked_list/node_with_type.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/primitive/slugified_entry_or_slug.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/primitive/slugified_entry_or_slug.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/reference/__init__.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/reference/__init__.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/reference/experiment/__init__.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/reference/experiment/__init__.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/reference/experiment/condition.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/reference/experiment/condition.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/reference/literature/__init__.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/reference/literature/__init__.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/reference/modeling/__init__.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/reference/modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/reference/modeling/exabyte.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/reference/modeling/exabyte.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/reusable/atomic_data/per_orbital.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/reusable/atomic_data/per_orbital.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/reusable/atomic_data/per_orbital_pair.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/reusable/atomic_data/per_orbital_pair.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/reusable/atomic_data_per_orbital_numeric.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/reusable/atomic_data_per_orbital_numeric.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/reusable/atomic_data_per_orbital_pair_numeric.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/reusable/atomic_data_per_orbital_pair_numeric.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/reusable/atomic_orbital.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/reusable/atomic_orbital.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/reusable/atomic_scalars.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/reusable/atomic_scalars.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/reusable/atomic_strings.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/reusable/atomic_strings.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/reusable/atomic_vectors.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/reusable/atomic_vectors.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/reusable/band_gap.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/reusable/band_gap.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/reusable/categories.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/reusable/categories.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/reusable/dielectric_tensor_component.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/reusable/dielectric_tensor_component.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/reusable/energy.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/reusable/energy.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/reusable/file_metadata.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/reusable/file_metadata.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/core/reusable/object_storage_container_data.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/core/reusable/object_storage_container_data.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/element.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/element.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/in_memory_entity/base.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/in_memory_entity/base.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/in_memory_entity/defaultable.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/in_memory_entity/defaultable.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/in_memory_entity/named.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/in_memory_entity/named.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/in_memory_entity/named_defaultable.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/in_memory_entity/named_defaultable.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/in_memory_entity/named_defaultable_has_metadata.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/in_memory_entity/named_defaultable_has_metadata.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/in_memory_entity/named_defaultable_runtime_items.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/in_memory_entity/named_defaultable_runtime_items.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/job/__init__.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/job/__init__.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/job/base.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/job/base.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/job/compute.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/job/compute.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/material/__init__.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/material/__init__.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/method/__init__.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/method/__init__.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/method/categorized_method.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/method/categorized_method.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/method/method_parameters.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/method/method_parameters.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/method/unit_method.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/method/unit_method.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/diff/__init__.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/diff/__init__.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/diff/fd.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/diff/fd.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/discr/__init__.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/discr/__init__.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/discr/mesh/__init__.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/discr/mesh/__init__.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/discr/mesh/hybrid.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/discr/mesh/hybrid.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/discr/mesh/nstruct.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/discr/mesh/nstruct.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/discr/mesh/struct/__init__.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/discr/mesh/struct/__init__.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/discr/mesh/struct/cartesian.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/discr/mesh/struct/cartesian.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/fapprx/__init__.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/fapprx/__init__.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/fapprx/basisexp.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/fapprx/basisexp.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/fapprx/ipol/__init__.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/fapprx/ipol/__init__.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/fapprx/ipol/lin.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/fapprx/ipol/lin.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/fapprx/ipol/poly.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/fapprx/ipol/poly.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/fapprx/ipol/spline.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/fapprx/ipol/spline.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/__init__.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/__init__.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/analytic/__init__.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/analytic/__init__.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/analytic/volume.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/analytic/volume.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/diffeq/__init__.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/diffeq/__init__.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/diffeq/order1.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/diffeq/order1.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/diffeq/order2.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/diffeq/order2.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/numquad/__init__.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/numquad/__init__.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/numquad/gauss.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/numquad/gauss.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/numquad/newcot.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/numquad/newcot.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/transf/__init__.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/transf/__init__.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/transf/fourier.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/intgr/transf/fourier.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/linalg/__init__.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/linalg/dcomp.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/linalg/dcomp.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/linalg/diag/__init__.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/linalg/diag/__init__.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/linalg/diag/davidson.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/linalg/diag/davidson.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/linalg/lintra.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/linalg/lintra.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/linalg/matf.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/linalg/matf.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/opt/__init__.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/opt/__init__.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/opt/diff/__init__.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/opt/diff/__init__.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/opt/diff/bracket.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/opt/diff/bracket.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/opt/diff/local.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/opt/diff/local.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/opt/diff/order1.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/opt/diff/order1.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/opt/diff/order2.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/opt/diff/order2.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/opt/diff/ordern/__init__.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/opt/diff/ordern/__init__.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/opt/diff/ordern/cg.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/opt/diff/ordern/cg.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/opt/ndiff/__init__.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/opt/ndiff/__init__.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/opt/ndiff/direct.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/opt/ndiff/direct.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/opt/ndiff/pop.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/opt/ndiff/pop.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/opt/ndiff/stoch.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/opt/ndiff/stoch.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/opt/root/__init__.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/opt/root/__init__.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/opt/root/bracket.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/opt/root/bracket.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/opt/root/iter.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/opt/root/iter.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/mathematical/regression.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/mathematical/regression.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/physical/qm/__init__.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/physical/qm/__init__.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/physical/qm/wf/__init__.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/physical/qm/wf/__init__.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/physical/qm/wf/ao/__init__.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/physical/qm/wf/ao/__init__.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/physical/qm/wf/ao/dunning.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/physical/qm/wf/ao/dunning.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/physical/qm/wf/ao/other.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/physical/qm/wf/ao/other.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/physical/qm/wf/ao/pople.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/physical/qm/wf/ao/pople.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/physical/qm/wf/psp.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/physical/qm/wf/psp.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/physical/qm/wf/pw.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/physical/qm/wf/pw.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/physical/qm/wf/smearing.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/physical/qm/wf/smearing.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_category/physical/qm/wf/tetrahedron.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_category/physical/qm/wf/tetrahedron.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/legacy/localorbital.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/legacy/localorbital.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/legacy/pseudopotential.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/legacy/pseudopotential.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/legacy/regression.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/legacy/regression.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/legacy/unknown.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/legacy/unknown.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/mathematical/cg.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/mathematical/cg.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/mathematical/davidson.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/mathematical/davidson.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/mathematical/regression/__init__.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/mathematical/regression/__init__.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/mathematical/regression/data.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/mathematical/regression/data.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/mathematical/regression/kernel_ridge/data_per_property.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/mathematical/regression/kernel_ridge/data_per_property.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/mathematical/regression/linear/data_per_property.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/mathematical/regression/linear/data_per_property.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/mathematical/regression/per_feature_item.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/mathematical/regression/per_feature_item.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/mathematical/regression/precision.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/mathematical/regression/precision.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/mathematical/regression/precision_per_property.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/mathematical/regression/precision_per_property.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/physical/ao/dunning.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/physical/ao/dunning.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/physical/ao/other.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/physical/ao/other.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/physical/ao/pople.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/physical/ao/pople.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/physical/psp/__init__.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/physical/psp/__init__.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/physical/psp/file.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/physical/psp/file.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/physical/psp/file_data_item.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/physical/psp/file_data_item.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/physical/pw.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/physical/pw.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/physical/smearing.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/physical/smearing.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/methods_directory/physical/tetrahedron.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/methods_directory/physical/tetrahedron.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/model/__init__.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/model/__init__.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/model/categorized_model.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/model/categorized_model.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/model/model_parameters.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/model/model_parameters.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/model/model_without_method.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/model/model_without_method.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_category/pb/__init__.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_category/pb/__init__.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_category/pb/qm/__init__.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_category/pb/qm/__init__.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_category/pb/qm/abin/__init__.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_category/pb/qm/abin/__init__.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_category/pb/qm/abin/gw.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_category/pb/qm/abin/gw.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_category/pb/qm/dft/__init__.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_category/pb/qm/dft/__init__.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_category/pb/qm/dft/ksdft/__init__.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_category/pb/qm/dft/ksdft/__init__.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_category/pb/qm/dft/ksdft/double_hybrid.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_category/pb/qm/dft/ksdft/double_hybrid.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_category/pb/qm/dft/ksdft/gga.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_category/pb/qm/dft/ksdft/gga.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_category/pb/qm/dft/ksdft/hybrid.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_category/pb/qm/dft/ksdft/hybrid.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_category/pb/qm/dft/ksdft/lda.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_category/pb/qm/dft/ksdft/lda.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_category/pb/qm/dft/ksdft/mgga.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_category/pb/qm/dft/ksdft/mgga.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_category/pb/qm/semp.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_category/pb/qm/semp.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_category/st/__init__.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_category/st/__init__.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_category/st/det/__init__.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_category/st/det/__init__.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_category/st/det/ml/__init__.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_category/st/det/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_category/st/det/ml/re.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_category/st/det/ml/re.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_directory/double_hybrid.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_directory/double_hybrid.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_directory/gga.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_directory/gga.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_directory/gw.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_directory/gw.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_directory/hybrid.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_directory/hybrid.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_directory/lda.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_directory/lda.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_directory/legacy/dft.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_directory/legacy/dft.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_directory/legacy/ml.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_directory/legacy/ml.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_directory/legacy/unknown.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_directory/legacy/unknown.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_directory/mgga.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_directory/mgga.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/models_directory/re.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/models_directory/re.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/project.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/project.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/derived_properties.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/derived_properties.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/elemental/atomic_radius.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/elemental/atomic_radius.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/elemental/ionization_potential.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/elemental/ionization_potential.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/non_scalar/average_potential_profile.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/non_scalar/average_potential_profile.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/non_scalar/band_gaps.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/non_scalar/band_gaps.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/non_scalar/band_structure.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/non_scalar/band_structure.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/non_scalar/charge_density_profile.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/non_scalar/charge_density_profile.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/non_scalar/density_of_states.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/non_scalar/density_of_states.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/non_scalar/dielectric_tensor.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/non_scalar/dielectric_tensor.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/non_scalar/file_content.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/non_scalar/file_content.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/non_scalar/hubbard_u.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/non_scalar/hubbard_u.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/non_scalar/hubbard_v.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/non_scalar/hubbard_v.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/non_scalar/hubbard_v_nn.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/non_scalar/hubbard_v_nn.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/non_scalar/phonon_dispersions.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/non_scalar/phonon_dispersions.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/non_scalar/phonon_dos.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/non_scalar/phonon_dos.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/non_scalar/potential_profile.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/non_scalar/potential_profile.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/non_scalar/reaction_energy_profile.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/non_scalar/reaction_energy_profile.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/non_scalar/stress_tensor.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/non_scalar/stress_tensor.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/non_scalar/total_energy_contributions.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/non_scalar/total_energy_contributions.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/non_scalar/vibrational_spectrum.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/non_scalar/vibrational_spectrum.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/scalar/electron_affinity.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/scalar/electron_affinity.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/scalar/fermi_energy.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/scalar/fermi_energy.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/scalar/formation_energy.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/scalar/formation_energy.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/scalar/ionization_potential.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/scalar/ionization_potential.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/scalar/reaction_energy_barrier.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/scalar/reaction_energy_barrier.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/scalar/surface_energy.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/scalar/surface_energy.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/scalar/total_energy.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/scalar/total_energy.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/scalar/total_force.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/scalar/total_force.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/scalar/valence_band_offset.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/scalar/valence_band_offset.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/scalar/zero_point_energy.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/scalar/zero_point_energy.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/structural/atomic_forces.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/structural/atomic_forces.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/structural/basis/__init__.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/structural/basis/__init__.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/structural/basis/atomic_constraints.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/structural/basis/atomic_constraints.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/structural/basis/atomic_coordinates.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/structural/basis/atomic_coordinates.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/structural/basis/bonds.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/structural/basis/bonds.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/structural/lattice/__init__.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/structural/lattice/__init__.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/structural/lattice/lattice_bravais.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/structural/lattice/lattice_bravais.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/structural/lattice/lattice_vectors.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/structural/lattice/lattice_vectors.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/structural/lattice/type_extended_enum.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/structural/lattice/type_extended_enum.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/structural/magnetic_moments.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/structural/magnetic_moments.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/structural/molecular_pattern.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/structural/molecular_pattern.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/structural/patterns/functional_group.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/structural/patterns/functional_group.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/structural/patterns/ring.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/structural/patterns/ring.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/structural/patterns/special_bond.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/structural/patterns/special_bond.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/structural/symmetry.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/structural/symmetry.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/workflow/convergence/electronic.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/workflow/convergence/electronic.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/workflow/convergence/ionic.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/workflow/convergence/ionic.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/properties_directory/workflow/convergence/kpoint.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/properties_directory/workflow/convergence/kpoint.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/property/base/The_source_of_a_property/field_This_could_be_an_article__a_simulation_on_Exabyte__an_external_simulation__etc.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/property/base/The_source_of_a_property/field_This_could_be_an_article__a_simulation_on_Exabyte__an_external_simulation__etc.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/property/base/__init__.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/property/base/__init__.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/property/meta/The_source_of_a_property/field_This_could_be_an_article__a_simulation_on_Exabyte__an_external_simulation__etc.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/property/meta/The_source_of_a_property/field_This_could_be_an_article__a_simulation_on_Exabyte__an_external_simulation__etc.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/property/meta/__init__.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/property/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/property/raw/The_source_of_a_property/field_This_could_be_an_article__a_simulation_on_Exabyte__an_external_simulation__etc.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/property/raw/The_source_of_a_property/field_This_could_be_an_article__a_simulation_on_Exabyte__an_external_simulation__etc.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/property/raw/__init__.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/property/raw/__init__.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/property/source/The_source_of_a_property/field_This_could_be_an_article__a_simulation_on_Exabyte__an_external_simulation__etc.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/property/source/The_source_of_a_property/field_This_could_be_an_article__a_simulation_on_Exabyte__an_external_simulation__etc.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/property/source/__init__.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/property/source/__init__.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software/application.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software/application.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software/executable.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software/executable.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software/flavor.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software/flavor.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software/template.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software/template.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/ml/exabyteml.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/ml/exabyteml.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/ml/unit/execution/__init__.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/ml/unit/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/ml/unit/execution/evaluate/cross_validate.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/ml/unit/execution/evaluate/cross_validate.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/ml/unit/execution/initialize.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/ml/unit/execution/initialize.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/ml/unit/execution/score.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/ml/unit/execution/score.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/ml/unit/execution/train.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/ml/unit/execution/train.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/ml/unit/processing/__init__.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/ml/unit/processing/__init__.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/ml/unit/processing/data_transformation/__init__.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/ml/unit/processing/data_transformation/__init__.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/ml/unit/processing/data_transformation/manipulation.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/ml/unit/processing/data_transformation/manipulation.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/ml/unit/processing/data_transformation/scale_and_reduce.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/ml/unit/processing/data_transformation/scale_and_reduce.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/ml/unit/processing/feature_selection/__init__.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/ml/unit/processing/feature_selection/__init__.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/ml/unit/processing/feature_selection/filter_based.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/ml/unit/processing/feature_selection/filter_based.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/modeling/deepmd.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/modeling/deepmd.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/modeling/espresso/__init__.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/modeling/espresso/__init__.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/modeling/espresso/arguments.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/modeling/espresso/arguments.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/modeling/nwchem.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/modeling/nwchem.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/modeling/unit/execution.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/modeling/unit/execution.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/modeling/vasp.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/modeling/vasp.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/scripting/jupyter_lab.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/scripting/jupyter_lab.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/scripting/python.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/scripting/python.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/scripting/shell.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/scripting/shell.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/software_directory/scripting/unit/execution.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/software_directory/scripting/unit/execution.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/system/_material.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/system/_material.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/system/_parent_job.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/system/_parent_job.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/system/_project.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/system/_project.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/system/consistency_check.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/system/consistency_check.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/system/creator.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/system/creator.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/system/creator_account.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/system/creator_account.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/system/database_source.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/system/database_source.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/system/iframe_message.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/system/iframe_message.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/system/in_set.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/system/in_set.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/system/job_extended.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/system/job_extended.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/system/message.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/system/message.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/system/owner.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/system/owner.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/third_party/db/nist_jarvis/2024.3.13/atoms.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/third_party/db/nist_jarvis/2024.3.13/atoms.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/third_party/db/nist_jarvis/2024.3.13/db_entry.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/third_party/db/nist_jarvis/2024.3.13/db_entry.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/third_party/file/applications/espresso/7.2/pw.x/__init__.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/third_party/file/applications/espresso/7.2/pw.x/__init__.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/third_party/file/applications/espresso/7.2/pw.x/atomic_positions.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/third_party/file/applications/espresso/7.2/pw.x/atomic_positions.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/third_party/file/applications/espresso/7.2/pw.x/atomic_species.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/third_party/file/applications/espresso/7.2/pw.x/atomic_species.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/third_party/file/applications/espresso/7.2/pw.x/cell.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/third_party/file/applications/espresso/7.2/pw.x/cell.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/third_party/file/applications/espresso/7.2/pw.x/cell_parameters.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/third_party/file/applications/espresso/7.2/pw.x/cell_parameters.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/third_party/file/applications/espresso/7.2/pw.x/control.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/third_party/file/applications/espresso/7.2/pw.x/control.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/third_party/file/applications/espresso/7.2/pw.x/electrons.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/third_party/file/applications/espresso/7.2/pw.x/electrons.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/third_party/file/applications/espresso/7.2/pw.x/hubbard.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/third_party/file/applications/espresso/7.2/pw.x/hubbard.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/third_party/file/applications/espresso/7.2/pw.x/ions.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/third_party/file/applications/espresso/7.2/pw.x/ions.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/third_party/file/applications/espresso/7.2/pw.x/k_points.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/third_party/file/applications/espresso/7.2/pw.x/k_points.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/third_party/file/applications/espresso/7.2/pw.x/system.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/third_party/file/applications/espresso/7.2/pw.x/system.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/__init__.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/base.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/base.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/base_flow.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/base_flow.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/subworkflow/__init__.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/subworkflow/__init__.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/subworkflow/unit.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/subworkflow/unit.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/unit/__init__.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/unit/assertion.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/unit/assertion.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/unit/assignment.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/unit/assignment.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/unit/base.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/unit/base.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/unit/condition.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/unit/condition.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/unit/execution.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/unit/execution.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/unit/input/_input.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/unit/input/_input.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/unit/input/_inputItemId.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/unit/input/_inputItemId.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/unit/io/__init__.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/unit/io/__init__.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/unit/io/api.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/unit/io/api.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/unit/io/db.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/unit/io/db.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/unit/io/object_storage.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/unit/io/object_storage.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/unit/map.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/unit/map.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/unit/processing.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/unit/processing.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/unit/reduce.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/unit/reduce.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/unit/runtime/runtime_items.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/unit/runtime/runtime_items.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/models/workflow/unit/subworkflow.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/models/workflow/unit/subworkflow.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra/esse/utils.py` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra/esse/utils.py`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra_esse.egg-info/PKG-INFO` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra_esse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mat3ra-esse
-Version: 2024.4.8.post3
+Version: 2024.4.8.post4
 Summary: Excellent Source of Schemas and Examples.
 Author-email: "Exabyte Inc." <info@mat3ra.com>
 License: # LICENSE
         
         Copyright 2019 Exabyte Inc.
         
         Licensed under the Apache License, Version 2.0 (the "License");
@@ -25,16 +25,14 @@
 Classifier: Topic :: Software Development
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: exabyte-json-include>=2023.12.23.post0
 Requires-Dist: jsonschema>=2.6.0
 Requires-Dist: datamodel-code-generator>=0.25.5
-Requires-Dist: pydantic
-Requires-Dist: gradio
 Provides-Extra: tests
 Requires-Dist: coverage[toml]>=5.3; extra == "tests"
 Requires-Dist: parameterized>=0.9.0; extra == "tests"
 Provides-Extra: all
 Requires-Dist: mat3ra-esse[tests]; extra == "all"
 
 [![PyPI version](https://badge.fury.io/py/mat3ra-esse.svg)](https://badge.fury.io/py/mat3ra-esse)
```

### Comparing `mat3ra-esse-2024.4.8.post3/src/py/mat3ra_esse.egg-info/SOURCES.txt` & `mat3ra-esse-2024.4.8.post4/src/py/mat3ra_esse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/tests/js/JSONSchemasInterface.tests.ts` & `mat3ra-esse-2024.4.8.post4/tests/js/JSONSchemasInterface.tests.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/tests/js/fixtures/json/2.json` & `mat3ra-esse-2024.4.8.post4/tests/js/fixtures/json/2.json`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/tests/js/validate.ts` & `mat3ra-esse-2024.4.8.post4/tests/js/validate.ts`

 * *Files identical despite different names*

### Comparing `mat3ra-esse-2024.4.8.post3/tests/py/esse/test_validate.py` & `mat3ra-esse-2024.4.8.post4/tests/py/esse/test_validate.py`

 * *Files identical despite different names*

