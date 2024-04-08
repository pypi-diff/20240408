# Comparing `tmp/sdk_entrepot_gpf-0.1.24.tar.gz` & `tmp/sdk_entrepot_gpf-0.1.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdk_entrepot_gpf-0.1.24.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sdk_entrepot_gpf-0.1.25.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sdk_entrepot_gpf-0.1.24.tar` & `sdk_entrepot_gpf-0.1.25.tar`

### file list

```diff
@@ -1,264 +1,267 @@
--rw-r--r--   0        0        0      350 2024-03-15 15:49:11.398012 sdk_entrepot_gpf-0.1.24/.github/PULL_REQUEST_TEMPLATE/bug.md
--rw-r--r--   0        0        0      361 2024-03-15 15:49:11.398012 sdk_entrepot_gpf-0.1.24/.github/PULL_REQUEST_TEMPLATE/documentation.md
--rw-r--r--   0        0        0      429 2024-03-15 15:49:11.398012 sdk_entrepot_gpf-0.1.24/.github/PULL_REQUEST_TEMPLATE/enhancement.md
--rw-r--r--   0        0        0      307 2024-03-15 15:49:11.398012 sdk_entrepot_gpf-0.1.24/.github/PULL_REQUEST_TEMPLATE/other.md
--rw-r--r--   0        0        0      370 2024-03-15 15:49:11.398012 sdk_entrepot_gpf-0.1.24/.github/PULL_REQUEST_TEMPLATE/quality.md
--rw-r--r--   0        0        0      383 2024-03-15 15:49:11.398012 sdk_entrepot_gpf-0.1.24/.github/PULL_REQUEST_TEMPLATE/tooling.md
--rw-r--r--   0        0        0      176 2024-03-15 15:49:11.398012 sdk_entrepot_gpf-0.1.24/.github/labeler.yml
--rw-r--r--   0        0        0      506 2024-03-15 15:49:11.398012 sdk_entrepot_gpf-0.1.24/.github/release.yml
--rw-r--r--   0        0        0     1412 2024-03-15 15:49:11.398012 sdk_entrepot_gpf-0.1.24/.github/workflows/ci-dev.yml
--rw-r--r--   0        0        0     1406 2024-03-15 15:49:11.398012 sdk_entrepot_gpf-0.1.24/.github/workflows/ci-prod.yml
--rw-r--r--   0        0        0      856 2024-03-15 15:49:11.398012 sdk_entrepot_gpf-0.1.24/.github/workflows/code-quality.yml
--rw-r--r--   0        0        0     1961 2024-03-15 15:49:11.398012 sdk_entrepot_gpf-0.1.24/.gitignore
--rw-r--r--   0        0        0    23461 2024-03-15 15:49:11.398012 sdk_entrepot_gpf-0.1.24/.pylintrc
--rw-r--r--   0        0        0      200 2024-03-15 15:49:11.398012 sdk_entrepot_gpf-0.1.24/.pypirc
--rw-r--r--   0        0        0     2299 2024-03-15 15:49:11.398012 sdk_entrepot_gpf-0.1.24/.vscode/settings.json
--rw-r--r--   0        0        0     5299 2024-03-15 15:49:11.398012 sdk_entrepot_gpf-0.1.24/CHANGELOG.md
--rw-r--r--   0        0        0    35149 2024-03-15 15:49:11.398012 sdk_entrepot_gpf-0.1.24/LICENSE
--rw-r--r--   0        0        0      134 2024-03-15 15:49:11.398012 sdk_entrepot_gpf-0.1.24/MANIFEST.in
--rw-r--r--   0        0        0      533 2024-03-15 15:49:11.398012 sdk_entrepot_gpf-0.1.24/README.md
--rwxr-xr-x   0        0        0      691 2024-03-15 15:49:11.398012 sdk_entrepot_gpf-0.1.24/check.sh
--rw-r--r--   0        0        0        5 2024-03-15 15:49:11.398012 sdk_entrepot_gpf-0.1.24/docker/.gitignore
--rw-r--r--   0        0        0     1968 2024-03-15 15:49:11.398012 sdk_entrepot_gpf-0.1.24/docker/Dockerfile
--rw-r--r--   0        0        0      808 2024-03-15 15:49:11.398012 sdk_entrepot_gpf-0.1.24/docker/README.md
--rw-r--r--   0        0        0      248 2024-03-15 15:49:11.398012 sdk_entrepot_gpf-0.1.24/docker/config/apache/website.conf
--rw-r--r--   0        0        0      291 2024-03-15 15:49:11.398012 sdk_entrepot_gpf-0.1.24/docker/docker-compose.yml
--rw-r--r--   0        0        0       46 2024-03-15 15:49:11.398012 sdk_entrepot_gpf-0.1.24/docs/.gitignore
--rw-r--r--   0        0        0      394 2024-03-15 15:49:11.398012 sdk_entrepot_gpf-0.1.24/docs/assets/css/custom.css
--rw-r--r--   0        0        0      748 2024-03-15 15:49:11.398012 sdk_entrepot_gpf-0.1.24/docs/assets/css/extra.css
--rw-r--r--   0        0        0    39005 2024-03-15 15:49:11.402012 sdk_entrepot_gpf-0.1.24/docs/assets/css/neoteroi.css
--rw-r--r--   0        0        0     1150 2024-03-15 15:49:11.402012 sdk_entrepot_gpf-0.1.24/docs/assets/images/favicon.ico
--rw-r--r--   0        0        0    12622 2024-03-15 15:49:11.402012 sdk_entrepot_gpf-0.1.24/docs/assets/images/index__utilisation_module.excalidraw
--rw-r--r--   0        0        0   193450 2024-03-15 15:49:11.402012 sdk_entrepot_gpf-0.1.24/docs/assets/images/index__utilisation_module.png
--rw-r--r--   0        0        0    15848 2024-03-15 15:49:11.402012 sdk_entrepot_gpf-0.1.24/docs/assets/images/logo.png
--rw-r--r--   0        0        0     4429 2024-03-15 15:49:11.402012 sdk_entrepot_gpf-0.1.24/docs/comme-executable.md
--rw-r--r--   0        0        0     4960 2024-03-15 15:49:11.402012 sdk_entrepot_gpf-0.1.24/docs/comme-module.md
--rw-r--r--   0        0        0     6776 2024-03-15 15:49:11.402012 sdk_entrepot_gpf-0.1.24/docs/configuration.md
--rw-r--r--   0        0        0    29083 2024-03-15 15:49:11.402012 sdk_entrepot_gpf-0.1.24/docs/configuration_details.md
--rw-r--r--   0        0        0     6052 2024-03-15 15:49:11.402012 sdk_entrepot_gpf-0.1.24/docs/development.md
--rw-r--r--   0        0        0     1327 2024-03-15 15:49:11.402012 sdk_entrepot_gpf-0.1.24/docs/index.md
--rw-r--r--   0        0        0      131 2024-03-15 15:49:11.402012 sdk_entrepot_gpf-0.1.24/docs/reference/auth.md
--rw-r--r--   0        0        0      336 2024-03-15 15:49:11.402012 sdk_entrepot_gpf-0.1.24/docs/reference/io.md
--rw-r--r--   0        0        0      338 2024-03-15 15:49:11.402012 sdk_entrepot_gpf-0.1.24/docs/reference/store.md
--rw-r--r--   0        0        0       68 2024-03-15 15:49:11.402012 sdk_entrepot_gpf-0.1.24/docs/reference/workflow.md
--rw-r--r--   0        0        0      314 2024-03-15 15:49:11.402012 sdk_entrepot_gpf-0.1.24/docs/reference/workflow/action.md
--rw-r--r--   0        0        0      368 2024-03-15 15:49:11.402012 sdk_entrepot_gpf-0.1.24/docs/reference/workflow/resolver.md
--rw-r--r--   0        0        0    11758 2024-03-15 15:49:11.402012 sdk_entrepot_gpf-0.1.24/docs/resolveurs.md
--rw-r--r--   0        0        0     5557 2024-03-15 15:49:11.402012 sdk_entrepot_gpf-0.1.24/docs/tutoriel_1_archive.md
--rw-r--r--   0        0        0     6731 2024-03-15 15:49:11.402012 sdk_entrepot_gpf-0.1.24/docs/tutoriel_2_flux_vecteur.md
--rw-r--r--   0        0        0     5137 2024-03-15 15:49:11.402012 sdk_entrepot_gpf-0.1.24/docs/tutoriel_3_flux_raster.md
--rw-r--r--   0        0        0     4161 2024-03-15 15:49:11.402012 sdk_entrepot_gpf-0.1.24/docs/upload_descriptor.md
--rw-r--r--   0        0        0    22205 2024-03-15 15:49:11.402012 sdk_entrepot_gpf-0.1.24/docs/workflow.md
--rw-r--r--   0        0        0     2201 2024-03-15 15:49:11.402012 sdk_entrepot_gpf-0.1.24/mkdocs.yml
--rw-r--r--   0        0        0      114 2024-03-15 15:49:11.402012 sdk_entrepot_gpf-0.1.24/mypy.ini
--rw-r--r--   0        0        0     1371 2024-03-15 15:49:11.402012 sdk_entrepot_gpf-0.1.24/pyproject.toml
--rw-r--r--   0        0        0      689 2024-03-15 15:49:11.402012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/Errors.py
--rw-r--r--   0        0        0       93 2024-03-15 15:49:11.402012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/__init__.py
--rw-r--r--   0        0        0    48118 2024-03-15 15:49:11.402012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/__main__.py
--rw-r--r--   0        0        0    11475 2024-03-15 15:49:11.402012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/_conf/default.ini
--rw-r--r--   0        0        0     1202 2024-03-15 15:49:11.402012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/_conf/json_schemas/annexe_descriptor_file.json
--rw-r--r--   0        0        0      870 2024-03-15 15:49:11.402012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/_conf/json_schemas/metadata_descriptor_file.json
--rw-r--r--   0        0        0     1226 2024-03-15 15:49:11.402012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/_conf/json_schemas/static_descriptor_file.json
--rw-r--r--   0        0        0     2183 2024-03-15 15:49:11.402012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/_conf/json_schemas/upload_descriptor_file.json
--rw-r--r--   0        0        0     6185 2024-03-15 15:49:11.402012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/_conf/json_schemas/workflow.json
--rw-r--r--   0        0        0      255 2024-03-15 15:49:11.402012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON.md5
--rwxr-xr-x   0        0        0        5 2024-03-15 15:49:11.402012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON/CANTON.cpg
--rw-r--r--   0        0        0     2297 2024-03-15 15:49:11.402012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON/CANTON.dbf
--rwxr-xr-x   0        0        0      655 2024-03-15 15:49:11.402012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON/CANTON.prj
--rw-r--r--   0        0        0   430828 2024-03-15 15:49:11.406012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON/CANTON.shp
--rw-r--r--   0        0        0      588 2024-03-15 15:49:11.406012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON/CANTON.shx
--rw-r--r--   0        0        0     4003 2024-03-15 15:49:11.406012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON_style.sld
--rw-r--r--   0        0        0      529 2024-03-15 15:49:11.406012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/upload_descriptor.json
--rw-r--r--   0        0        0       52 2024-03-15 15:49:11.406012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/_data/datasets/2_dataset_archive/CANTON.md5
--rw-r--r--   0        0        0   991843 2024-03-15 15:49:11.410012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/_data/datasets/2_dataset_archive/CANTON/CANTON.zip
--rw-r--r--   0        0        0      525 2024-03-15 15:49:11.410012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/_data/datasets/2_dataset_archive/upload_descriptor.json
--rw-r--r--   0        0        0     4391 2024-03-15 15:49:11.410012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/_data/datasets/5_dataset_maj_bd_gpf/installation.sld
--rw-r--r--   0        0        0      411 2024-03-15 15:49:11.410012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/_data/datasets/5_dataset_maj_bd_gpf/lot_1/installation-init.sql
--rw-r--r--   0        0        0   368640 2024-03-15 15:49:11.410012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/_data/datasets/5_dataset_maj_bd_gpf/lot_2/installation.gpkg
--rw-r--r--   0        0        0   676357 2024-03-15 15:49:11.414012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/_data/datasets/5_dataset_maj_bd_gpf/lot_3/installation.csv
--rw-r--r--   0        0        0       84 2024-03-15 15:49:11.414012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/_data/datasets/5_dataset_maj_bd_gpf/lot_3/installation.csvt
--rw-r--r--   0        0        0     1731 2024-03-15 15:49:11.414012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/_data/datasets/5_dataset_maj_bd_gpf/upload_descriptor.json
--rw-r--r--   0        0        0     5019 2024-03-15 15:49:11.414012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/_data/workflows/generic_archive.jsonc
--rw-r--r--   0        0        0    15492 2024-03-15 15:49:11.414012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/_data/workflows/generic_joincache.jsonc
--rw-r--r--   0        0        0     9884 2024-03-15 15:49:11.414012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/_data/workflows/generic_maj_bdd.jsonc
--rw-r--r--   0        0        0    11561 2024-03-15 15:49:11.414012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/_data/workflows/generic_moissonnage.jsonc
--rw-r--r--   0        0        0     9209 2024-03-15 15:49:11.414012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/_data/workflows/generic_raster.jsonc
--rw-r--r--   0        0        0    15240 2024-03-15 15:49:11.414012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/_data/workflows/generic_vecteur.jsonc
--rw-r--r--   0        0        0     8059 2024-03-15 15:49:11.414012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/auth/Authentifier.py
--rw-r--r--   0        0        0      274 2024-03-15 15:49:11.414012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/auth/Errors.py
--rw-r--r--   0        0        0     1493 2024-03-15 15:49:11.414012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/auth/Token.py
--rw-r--r--   0        0        0       46 2024-03-15 15:49:11.414012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/auth/__init__.py
--rw-r--r--   0        0        0     2589 2024-03-15 15:49:11.414012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/helper/FileHelper.py
--rw-r--r--   0        0        0     6939 2024-03-15 15:49:11.414012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/helper/JsonHelper.py
--rw-r--r--   0        0        0      916 2024-03-15 15:49:11.414012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/helper/PrintLogHelper.py
--rw-r--r--   0        0        0       59 2024-03-15 15:49:11.414012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/helper/__init__.py
--rw-r--r--   0        0        0    14054 2024-03-15 15:49:11.414012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/io/ApiRequester.py
--rw-r--r--   0        0        0      607 2024-03-15 15:49:11.414012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/io/Color.py
--rw-r--r--   0        0        0     5695 2024-03-15 15:49:11.414012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/io/Config.py
--rw-r--r--   0        0        0     5318 2024-03-15 15:49:11.414012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/io/Dataset.py
--rw-r--r--   0        0        0     4143 2024-03-15 15:49:11.414012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/io/DescriptorFileReader.py
--rw-r--r--   0        0        0     6828 2024-03-15 15:49:11.414012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/io/Errors.py
--rw-r--r--   0        0        0     2772 2024-03-15 15:49:11.414012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/io/JsonConverter.py
--rw-r--r--   0        0        0     4416 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/io/OutputManager.py
--rw-r--r--   0        0        0     4075 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/io/UploadDescriptorFileReader.py
--rw-r--r--   0        0        0       47 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/io/__init__.py
--rw-r--r--   0        0        0      793 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/pattern/SingleInstance.py
--rw-r--r--   0        0        0      637 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/pattern/Singleton.py
--rw-r--r--   0        0        0       33 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/pattern/__init__.py
--rw-r--r--   0        0        0        1 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/py.typed
--rw-r--r--   0        0        0     1209 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/store/AbstractCommonFile.py
--rw-r--r--   0        0        0     2486 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/store/Annexe.py
--rw-r--r--   0        0        0      222 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/store/Check.py
--rw-r--r--   0        0        0     1378 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/store/CheckExecution.py
--rw-r--r--   0        0        0     4214 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/store/Configuration.py
--rw-r--r--   0        0        0     3400 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/store/Datastore.py
--rw-r--r--   0        0        0     3363 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/store/Endpoint.py
--rw-r--r--   0        0        0      183 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/store/Errors.py
--rw-r--r--   0        0        0     2586 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/store/Metadata.py
--rw-r--r--   0        0        0     2140 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/store/Offering.py
--rw-r--r--   0        0        0      332 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/store/Permission.py
--rw-r--r--   0        0        0      231 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/store/Processing.py
--rw-r--r--   0        0        0     2789 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/store/ProcessingExecution.py
--rw-r--r--   0        0        0     1005 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/store/Static.py
--rw-r--r--   0        0        0    14998 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/store/StoreEntity.py
--rw-r--r--   0        0        0     1933 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/store/StoredData.py
--rw-r--r--   0        0        0      235 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/store/Tms.py
--rw-r--r--   0        0        0     7270 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/store/Upload.py
--rw-r--r--   0        0        0     1010 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/store/User.py
--rw-r--r--   0        0        0     1432 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/store/__init__.py
--rw-r--r--   0        0        0     2521 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/store/interface/CommentInterface.py
--rw-r--r--   0        0        0     2025 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/store/interface/CreatedByUploadFileInterface.py
--rw-r--r--   0        0        0     1051 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/store/interface/CsfInterface.py
--rw-r--r--   0        0        0     1102 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/store/interface/DownloadInterface.py
--rw-r--r--   0        0        0      805 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/store/interface/EventInterface.py
--rw-r--r--   0        0        0     1262 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/store/interface/FullEditInterface.py
--rw-r--r--   0        0        0     1116 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/store/interface/PartialEditInterface.py
--rw-r--r--   0        0        0      998 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/store/interface/ReUploadFileInterface.py
--rw-r--r--   0        0        0     2107 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/store/interface/SharingInterface.py
--rw-r--r--   0        0        0     2329 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/store/interface/TagInterface.py
--rw-r--r--   0        0        0       88 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/store/interface/__init__.py
--rw-r--r--   0        0        0      208 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/workflow/Errors.py
--rw-r--r--   0        0        0    20519 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/workflow/Workflow.py
--rw-r--r--   0        0        0       40 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/workflow/__init__.py
--rw-r--r--   0        0        0     5726 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/workflow/action/ActionAbstract.py
--rw-r--r--   0        0        0     7077 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/workflow/action/ConfigurationAction.py
--rw-r--r--   0        0        0     1776 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/workflow/action/CopyConfigurationAction.py
--rw-r--r--   0        0        0     5023 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/workflow/action/DeleteAction.py
--rw-r--r--   0        0        0     3172 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/workflow/action/EditAction.py
--rw-r--r--   0        0        0     6799 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/workflow/action/OfferingAction.py
--rw-r--r--   0        0        0     2153 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/workflow/action/PermissionAction.py
--rw-r--r--   0        0        0    19885 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/workflow/action/ProcessingExecutionAction.py
--rw-r--r--   0        0        0     7452 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/workflow/action/SynchronizeOfferingAction.py
--rw-r--r--   0        0        0    17884 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/workflow/action/UploadAction.py
--rw-r--r--   0        0        0       72 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/workflow/action/__init__.py
--rw-r--r--   0        0        0     1796 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/workflow/resolver/AbstractResolver.py
--rw-r--r--   0        0        0     3389 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/workflow/resolver/DateResolver.py
--rw-r--r--   0        0        0     1700 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/workflow/resolver/DictResolver.py
--rw-r--r--   0        0        0      708 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/workflow/resolver/DumbResolver.py
--rw-r--r--   0        0        0     4533 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/workflow/resolver/Errors.py
--rw-r--r--   0        0        0     5976 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/workflow/resolver/FileResolver.py
--rw-r--r--   0        0        0     3838 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/workflow/resolver/GlobalResolver.py
--rw-r--r--   0        0        0     5760 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/workflow/resolver/StoreEntityResolver.py
--rw-r--r--   0        0        0     1908 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/workflow/resolver/UserResolver.py
--rw-r--r--   0        0        0      110 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/workflow/resolver/__init__.py
--rw-r--r--   0        0        0      960 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/tests/ErrorsTestCase.py
--rw-r--r--   0        0        0     1739 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/tests/GpfTestCase.py
--rw-r--r--   0        0        0     3419 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/tests/MainTestCase.py
--rw-r--r--   0        0        0        0 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/tests/__init__.py
--rw-r--r--   0        0        0      369 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/tests/_conf/test_authentifier.ini
--rw-r--r--   0        0        0      308 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/tests/_conf/test_overload.ini
--rw-r--r--   0        0        0      312 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/tests/_conf/test_requester.ini
--rw-r--r--   0        0        0       40 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/tests/_conf/test_upload.ini
--rw-r--r--   0        0        0       69 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/tests/_conf/test_value_type.ini
--rw-r--r--   0        0        0      460 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/tests/_data/datasets/1_test_dataset_bad_pathes/upload_descriptor.json
--rw-r--r--   0        0        0      305 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/tests/_data/datasets/2_test_dataset_bad_md5/CANTON.md5
--rw-r--r--   0        0        0        5 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.cpg
--rw-r--r--   0        0        0     2318 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.dbf
--rw-r--r--   0        0        0      145 2024-03-15 15:49:11.418012 sdk_entrepot_gpf-0.1.24/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.prj
--rw-r--r--   0        0        0  1279276 2024-03-15 15:49:11.426012 sdk_entrepot_gpf-0.1.24/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.shp
--rw-r--r--   0        0        0      572 2024-03-15 15:49:11.426012 sdk_entrepot_gpf-0.1.24/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.shx
--rw-r--r--   0        0        0        0 2024-03-15 15:49:11.426012 sdk_entrepot_gpf-0.1.24/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/sous_dossier/coucou.txt
--rw-r--r--   0        0        0      567 2024-03-15 15:49:11.426012 sdk_entrepot_gpf-0.1.24/tests/_data/datasets/2_test_dataset_bad_md5/upload_descriptor.json
--rw-r--r--   0        0        0       11 2024-03-15 15:49:11.426012 sdk_entrepot_gpf-0.1.24/tests/_data/datasets/3_test_dataset_sub_dir/.gitignore
--rw-r--r--   0        0        0        5 2024-03-15 15:49:11.426012 sdk_entrepot_gpf-0.1.24/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.cpg
--rw-r--r--   0        0        0     2318 2024-03-15 15:49:11.426012 sdk_entrepot_gpf-0.1.24/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.dbf
--rw-r--r--   0        0        0      145 2024-03-15 15:49:11.426012 sdk_entrepot_gpf-0.1.24/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.prj
--rw-r--r--   0        0        0  1279276 2024-03-15 15:49:11.434012 sdk_entrepot_gpf-0.1.24/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.shp
--rw-r--r--   0        0        0      572 2024-03-15 15:49:11.434012 sdk_entrepot_gpf-0.1.24/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.shx
--rw-r--r--   0        0        0        0 2024-03-15 15:49:11.434012 sdk_entrepot_gpf-0.1.24/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/sous_dossier/coucou.txt
--rw-r--r--   0        0        0      567 2024-03-15 15:49:11.434012 sdk_entrepot_gpf-0.1.24/tests/_data/datasets/3_test_dataset_sub_dir/upload_descriptor.json
--rw-r--r--   0        0        0     2659 2024-03-15 15:49:11.434012 sdk_entrepot_gpf-0.1.24/tests/_data/workflows/bad-workflow.jsonc
--rw-r--r--   0        0        0       53 2024-03-15 15:49:11.434012 sdk_entrepot_gpf-0.1.24/tests/_test/helper/FileHelper/md5.txt
--rw-r--r--   0        0        0       78 2024-03-15 15:49:11.434012 sdk_entrepot_gpf-0.1.24/tests/_test/helper/JsonHelper/json_not_parsable.json
--rw-r--r--   0        0        0       52 2024-03-15 15:49:11.434012 sdk_entrepot_gpf-0.1.24/tests/_test/helper/JsonHelper/json_not_valid.json
--rw-r--r--   0        0        0      108 2024-03-15 15:49:11.434012 sdk_entrepot_gpf-0.1.24/tests/_test/helper/JsonHelper/json_parsable.json
--rw-r--r--   0        0        0      563 2024-03-15 15:49:11.434012 sdk_entrepot_gpf-0.1.24/tests/_test/helper/JsonHelper/schema.json
--rw-r--r--   0        0        0      485 2024-03-15 15:49:11.434012 sdk_entrepot_gpf-0.1.24/tests/_test/helper/JsonHelper/schema_invalid.json
--rw-r--r--   0        0        0       23 2024-03-15 15:49:11.434012 sdk_entrepot_gpf-0.1.24/tests/_test/workflow/resolver/FileResolver/dict.json
--rw-r--r--   0        0        0       21 2024-03-15 15:49:11.434012 sdk_entrepot_gpf-0.1.24/tests/_test/workflow/resolver/FileResolver/list.json
--rw-r--r--   0        0        0        2 2024-03-15 15:49:11.434012 sdk_entrepot_gpf-0.1.24/tests/_test/workflow/resolver/FileResolver/not-valid.json
--rw-r--r--   0        0        0       31 2024-03-15 15:49:11.434012 sdk_entrepot_gpf-0.1.24/tests/_test/workflow/resolver/FileResolver/text.txt
--rw-r--r--   0        0        0     7428 2024-03-15 15:49:11.434012 sdk_entrepot_gpf-0.1.24/tests/auth/AuthentifierTestCase.py
--rw-r--r--   0        0        0     1187 2024-03-15 15:49:11.434012 sdk_entrepot_gpf-0.1.24/tests/auth/TokenTestCase.py
--rw-r--r--   0        0        0        0 2024-03-15 15:49:11.434012 sdk_entrepot_gpf-0.1.24/tests/auth/__init__.py
--rw-r--r--   0        0        0     1060 2024-03-15 15:49:11.434012 sdk_entrepot_gpf-0.1.24/tests/helper/FileHelperTestCase.py
--rw-r--r--   0        0        0     9967 2024-03-15 15:49:11.434012 sdk_entrepot_gpf-0.1.24/tests/helper/JsonHelperTestCase.py
--rw-r--r--   0        0        0        0 2024-03-15 15:49:11.434012 sdk_entrepot_gpf-0.1.24/tests/helper/__init__.py
--rw-r--r--   0        0        0    15778 2024-03-15 15:49:11.434012 sdk_entrepot_gpf-0.1.24/tests/io/ApiRequesterTestCase.py
--rw-r--r--   0        0        0     3599 2024-03-15 15:49:11.434012 sdk_entrepot_gpf-0.1.24/tests/io/ConfigTestCase.py
--rw-r--r--   0        0        0     2225 2024-03-15 15:49:11.434012 sdk_entrepot_gpf-0.1.24/tests/io/DatasetTestCase.py
--rw-r--r--   0        0        0     3197 2024-03-15 15:49:11.434012 sdk_entrepot_gpf-0.1.24/tests/io/ErrorsTestCase.py
--rw-r--r--   0        0        0     1202 2024-03-15 15:49:11.434012 sdk_entrepot_gpf-0.1.24/tests/io/JsonConverterTestCase.py
--rw-r--r--   0        0        0     1774 2024-03-15 15:49:11.434012 sdk_entrepot_gpf-0.1.24/tests/io/UploadDescriptorFileReaderTestCase.py
--rw-r--r--   0        0        0        0 2024-03-15 15:49:11.434012 sdk_entrepot_gpf-0.1.24/tests/io/__init__.py
--rw-r--r--   0        0        0     1122 2024-03-15 15:49:11.434012 sdk_entrepot_gpf-0.1.24/tests/store/AbstractCommonFileTestCase.py
--rw-r--r--   0        0        0     2587 2024-03-15 15:49:11.434012 sdk_entrepot_gpf-0.1.24/tests/store/AnnexeTestCase.py
--rw-r--r--   0        0        0     1964 2024-03-15 15:49:11.434012 sdk_entrepot_gpf-0.1.24/tests/store/CheckExecutionTestCase.py
--rw-r--r--   0        0        0     7172 2024-03-15 15:49:11.434012 sdk_entrepot_gpf-0.1.24/tests/store/ConfigurationTestCase.py
--rw-r--r--   0        0        0     4849 2024-03-15 15:49:11.434012 sdk_entrepot_gpf-0.1.24/tests/store/DatastoreTestCase.py
--rw-r--r--   0        0        0     5595 2024-03-15 15:49:11.434012 sdk_entrepot_gpf-0.1.24/tests/store/EndpointTestCase.py
--rw-r--r--   0        0        0     1152 2024-03-15 15:49:11.434012 sdk_entrepot_gpf-0.1.24/tests/store/ErrorsTestCase.py
--rw-r--r--   0        0        0     2297 2024-03-15 15:49:11.434012 sdk_entrepot_gpf-0.1.24/tests/store/MetadataTestCase.py
--rw-r--r--   0        0        0     2687 2024-03-15 15:49:11.434012 sdk_entrepot_gpf-0.1.24/tests/store/OfferingTestCase.py
--rw-r--r--   0        0        0     4687 2024-03-15 15:49:11.434012 sdk_entrepot_gpf-0.1.24/tests/store/ProcessingExecutionTestCase.py
--rw-r--r--   0        0        0    26065 2024-03-15 15:49:11.434012 sdk_entrepot_gpf-0.1.24/tests/store/StoreEntityTestCase.py
--rw-r--r--   0        0        0     3137 2024-03-15 15:49:11.434012 sdk_entrepot_gpf-0.1.24/tests/store/StoredDataTestCase.py
--rw-r--r--   0        0        0    11003 2024-03-15 15:49:11.434012 sdk_entrepot_gpf-0.1.24/tests/store/UploadTestCase.py
--rw-r--r--   0        0        0        0 2024-03-15 15:49:11.434012 sdk_entrepot_gpf-0.1.24/tests/store/__init__.py
--rw-r--r--   0        0        0     5134 2024-03-15 15:49:11.434012 sdk_entrepot_gpf-0.1.24/tests/store/interface/CommentInterfaceTestCase.py
--rw-r--r--   0        0        0     2790 2024-03-15 15:49:11.434012 sdk_entrepot_gpf-0.1.24/tests/store/interface/CreatedByUploadFileInterfaceTestCase.py
--rw-r--r--   0        0        0     2536 2024-03-15 15:49:11.434012 sdk_entrepot_gpf-0.1.24/tests/store/interface/CsfInterfaceTestCase.py
--rw-r--r--   0        0        0     1767 2024-03-15 15:49:11.434012 sdk_entrepot_gpf-0.1.24/tests/store/interface/DownloadInterfaceTestCase.py
--rw-r--r--   0        0        0     1663 2024-03-15 15:49:11.434012 sdk_entrepot_gpf-0.1.24/tests/store/interface/EventInterfaceTestCase.py
--rw-r--r--   0        0        0     2326 2024-03-15 15:49:11.438012 sdk_entrepot_gpf-0.1.24/tests/store/interface/FullEditInterfaceTestCase.py
--rw-r--r--   0        0        0     2243 2024-03-15 15:49:11.438012 sdk_entrepot_gpf-0.1.24/tests/store/interface/PartialEditInterfaceTestCase.py
--rw-r--r--   0        0        0     1569 2024-03-15 15:49:11.438012 sdk_entrepot_gpf-0.1.24/tests/store/interface/ReUploadFileInterfaceTestCase.py
--rw-r--r--   0        0        0     4039 2024-03-15 15:49:11.438012 sdk_entrepot_gpf-0.1.24/tests/store/interface/SharingInterfaceTestCase.py
--rw-r--r--   0        0        0     3899 2024-03-15 15:49:11.438012 sdk_entrepot_gpf-0.1.24/tests/store/interface/TagInterfaceTestCase.py
--rw-r--r--   0        0        0        0 2024-03-15 15:49:11.438012 sdk_entrepot_gpf-0.1.24/tests/store/interface/__init__.py
--rw-r--r--   0        0        0    28326 2024-03-15 15:49:11.438012 sdk_entrepot_gpf-0.1.24/tests/workflow/WorkflowTestCase.py
--rw-r--r--   0        0        0        0 2024-03-15 15:49:11.438012 sdk_entrepot_gpf-0.1.24/tests/workflow/__init__.py
--rw-r--r--   0        0        0     3595 2024-03-15 15:49:11.438012 sdk_entrepot_gpf-0.1.24/tests/workflow/action/ActionAbstractTestCase.py
--rw-r--r--   0        0        0    10471 2024-03-15 15:49:11.438012 sdk_entrepot_gpf-0.1.24/tests/workflow/action/ConfigurationActionTestCase.py
--rw-r--r--   0        0        0     2502 2024-03-15 15:49:11.438012 sdk_entrepot_gpf-0.1.24/tests/workflow/action/CopyConfigurationActionTestCase.py
--rw-r--r--   0        0        0    11898 2024-03-15 15:49:11.438012 sdk_entrepot_gpf-0.1.24/tests/workflow/action/DeleteActionTestCase.py
--rw-r--r--   0        0        0     5262 2024-03-15 15:49:11.438012 sdk_entrepot_gpf-0.1.24/tests/workflow/action/EditActionTestCase.py
--rw-r--r--   0        0        0    15937 2024-03-15 15:49:11.438012 sdk_entrepot_gpf-0.1.24/tests/workflow/action/OfferingActionTestCase.py
--rw-r--r--   0        0        0     1547 2024-03-15 15:49:11.438012 sdk_entrepot_gpf-0.1.24/tests/workflow/action/PermissionActionTestCase.py
--rw-r--r--   0        0        0    24541 2024-03-15 15:49:11.438012 sdk_entrepot_gpf-0.1.24/tests/workflow/action/ProcessingExecutionActionTestCase.py
--rw-r--r--   0        0        0    10675 2024-03-15 15:49:11.438012 sdk_entrepot_gpf-0.1.24/tests/workflow/action/SynchronizeOfferingActionTestCase.py
--rw-r--r--   0        0        0    26204 2024-03-15 15:49:11.438012 sdk_entrepot_gpf-0.1.24/tests/workflow/action/UploadActionTestCase.py
--rw-r--r--   0        0        0        0 2024-03-15 15:49:11.438012 sdk_entrepot_gpf-0.1.24/tests/workflow/action/__init__.py
--rw-r--r--   0        0        0      772 2024-03-15 15:49:11.438012 sdk_entrepot_gpf-0.1.24/tests/workflow/resolver/AbstractResolverTestCase.py
--rw-r--r--   0        0        0     2401 2024-03-15 15:49:11.438012 sdk_entrepot_gpf-0.1.24/tests/workflow/resolver/DateResolverTestCase.py
--rw-r--r--   0        0        0     1124 2024-03-15 15:49:11.438012 sdk_entrepot_gpf-0.1.24/tests/workflow/resolver/DictResolverTestCase.py
--rw-r--r--   0        0        0     5479 2024-03-15 15:49:11.438012 sdk_entrepot_gpf-0.1.24/tests/workflow/resolver/FileResolverTestCase.py
--rw-r--r--   0        0        0     7364 2024-03-15 15:49:11.438012 sdk_entrepot_gpf-0.1.24/tests/workflow/resolver/GlobalResolverTestCase.py
--rw-r--r--   0        0        0    15246 2024-03-15 15:49:11.438012 sdk_entrepot_gpf-0.1.24/tests/workflow/resolver/StoreEntityResolverTestCase.py
--rw-r--r--   0        0        0     2237 2024-03-15 15:49:11.438012 sdk_entrepot_gpf-0.1.24/tests/workflow/resolver/UserResolverTestCase.py
--rw-r--r--   0        0        0        0 2024-03-15 15:49:11.438012 sdk_entrepot_gpf-0.1.24/tests/workflow/resolver/__init__.py
--rw-r--r--   0        0        0   116760 2024-03-15 15:49:11.438012 sdk_entrepot_gpf-0.1.24/uml/classes.png
--rw-r--r--   0        0        0     9175 2024-03-15 15:49:11.438012 sdk_entrepot_gpf-0.1.24/uml/classes.uxf
--rw-r--r--   0        0        0    43510 2024-03-15 15:49:11.438012 sdk_entrepot_gpf-0.1.24/uml/interfaces.png
--rw-r--r--   0        0        0     7059 2024-03-15 15:49:11.438012 sdk_entrepot_gpf-0.1.24/uml/interfaces.uxf
--rw-r--r--   0        0        0     1773 1970-01-01 00:00:00.000000 sdk_entrepot_gpf-0.1.24/PKG-INFO
+-rw-r--r--   0        0        0      350 2024-04-08 13:52:45.554023 sdk_entrepot_gpf-0.1.25/.github/PULL_REQUEST_TEMPLATE/bug.md
+-rw-r--r--   0        0        0      361 2024-04-08 13:52:45.554023 sdk_entrepot_gpf-0.1.25/.github/PULL_REQUEST_TEMPLATE/documentation.md
+-rw-r--r--   0        0        0      429 2024-04-08 13:52:45.554023 sdk_entrepot_gpf-0.1.25/.github/PULL_REQUEST_TEMPLATE/enhancement.md
+-rw-r--r--   0        0        0      307 2024-04-08 13:52:45.554023 sdk_entrepot_gpf-0.1.25/.github/PULL_REQUEST_TEMPLATE/other.md
+-rw-r--r--   0        0        0      370 2024-04-08 13:52:45.554023 sdk_entrepot_gpf-0.1.25/.github/PULL_REQUEST_TEMPLATE/quality.md
+-rw-r--r--   0        0        0      383 2024-04-08 13:52:45.554023 sdk_entrepot_gpf-0.1.25/.github/PULL_REQUEST_TEMPLATE/tooling.md
+-rw-r--r--   0        0        0      176 2024-04-08 13:52:45.554023 sdk_entrepot_gpf-0.1.25/.github/labeler.yml
+-rw-r--r--   0        0        0      506 2024-04-08 13:52:45.554023 sdk_entrepot_gpf-0.1.25/.github/release.yml
+-rw-r--r--   0        0        0     1412 2024-04-08 13:52:45.554023 sdk_entrepot_gpf-0.1.25/.github/workflows/ci-dev.yml
+-rw-r--r--   0        0        0     1406 2024-04-08 13:52:45.554023 sdk_entrepot_gpf-0.1.25/.github/workflows/ci-prod.yml
+-rw-r--r--   0        0        0      856 2024-04-08 13:52:45.554023 sdk_entrepot_gpf-0.1.25/.github/workflows/code-quality.yml
+-rw-r--r--   0        0        0     1961 2024-04-08 13:52:45.554023 sdk_entrepot_gpf-0.1.25/.gitignore
+-rw-r--r--   0        0        0    23461 2024-04-08 13:52:45.554023 sdk_entrepot_gpf-0.1.25/.pylintrc
+-rw-r--r--   0        0        0      200 2024-04-08 13:52:45.554023 sdk_entrepot_gpf-0.1.25/.pypirc
+-rw-r--r--   0        0        0     2299 2024-04-08 13:52:45.554023 sdk_entrepot_gpf-0.1.25/.vscode/settings.json
+-rw-r--r--   0        0        0     6231 2024-04-08 13:52:45.554023 sdk_entrepot_gpf-0.1.25/CHANGELOG.md
+-rw-r--r--   0        0        0    35149 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/LICENSE
+-rw-r--r--   0        0        0      134 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/MANIFEST.in
+-rw-r--r--   0        0        0      533 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/README.md
+-rwxr-xr-x   0        0        0      691 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/check.sh
+-rw-r--r--   0        0        0        5 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docker/.gitignore
+-rw-r--r--   0        0        0     1968 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docker/Dockerfile
+-rw-r--r--   0        0        0      808 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docker/README.md
+-rw-r--r--   0        0        0      248 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docker/config/apache/website.conf
+-rw-r--r--   0        0        0      291 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docker/docker-compose.yml
+-rw-r--r--   0        0        0       46 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docs/.gitignore
+-rw-r--r--   0        0        0      394 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docs/assets/css/custom.css
+-rw-r--r--   0        0        0      748 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docs/assets/css/extra.css
+-rw-r--r--   0        0        0    39005 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docs/assets/css/neoteroi.css
+-rw-r--r--   0        0        0     1150 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docs/assets/images/favicon.ico
+-rw-r--r--   0        0        0    12622 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docs/assets/images/index__utilisation_module.excalidraw
+-rw-r--r--   0        0        0   193450 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docs/assets/images/index__utilisation_module.png
+-rw-r--r--   0        0        0    15848 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docs/assets/images/logo.png
+-rw-r--r--   0        0        0     4429 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docs/comme-executable.md
+-rw-r--r--   0        0        0     4960 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docs/comme-module.md
+-rw-r--r--   0        0        0     6776 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docs/configuration.md
+-rw-r--r--   0        0        0    29083 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docs/configuration_details.md
+-rw-r--r--   0        0        0     6052 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docs/development.md
+-rw-r--r--   0        0        0     1327 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docs/index.md
+-rw-r--r--   0        0        0      131 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docs/reference/auth.md
+-rw-r--r--   0        0        0      336 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docs/reference/io.md
+-rw-r--r--   0        0        0      338 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docs/reference/store.md
+-rw-r--r--   0        0        0       68 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docs/reference/workflow.md
+-rw-r--r--   0        0        0      314 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docs/reference/workflow/action.md
+-rw-r--r--   0        0        0      368 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docs/reference/workflow/resolver.md
+-rw-r--r--   0        0        0    11758 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docs/resolveurs.md
+-rw-r--r--   0        0        0     5557 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docs/tutoriel_1_archive.md
+-rw-r--r--   0        0        0     6731 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docs/tutoriel_2_flux_vecteur.md
+-rw-r--r--   0        0        0     5137 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docs/tutoriel_3_flux_raster.md
+-rw-r--r--   0        0        0     4161 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docs/upload_descriptor.md
+-rw-r--r--   0        0        0    22205 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/docs/workflow.md
+-rw-r--r--   0        0        0     2201 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/mkdocs.yml
+-rw-r--r--   0        0        0      114 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/mypy.ini
+-rw-r--r--   0        0        0     1371 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/pyproject.toml
+-rw-r--r--   0        0        0      689 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/Errors.py
+-rw-r--r--   0        0        0       93 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/__init__.py
+-rw-r--r--   0        0        0    48450 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/__main__.py
+-rw-r--r--   0        0        0    11475 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_conf/default.ini
+-rw-r--r--   0        0        0     1202 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_conf/json_schemas/annexe_descriptor_file.json
+-rw-r--r--   0        0        0      870 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_conf/json_schemas/metadata_descriptor_file.json
+-rw-r--r--   0        0        0     1226 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_conf/json_schemas/static_descriptor_file.json
+-rw-r--r--   0        0        0     2183 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_conf/json_schemas/upload_descriptor_file.json
+-rw-r--r--   0        0        0     6924 2024-04-08 13:52:45.558023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_conf/json_schemas/workflow.json
+-rw-r--r--   0        0        0      255 2024-04-08 13:52:45.562023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON.md5
+-rwxr-xr-x   0        0        0        5 2024-04-08 13:52:45.562023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON/CANTON.cpg
+-rw-r--r--   0        0        0     2297 2024-04-08 13:52:45.562023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON/CANTON.dbf
+-rwxr-xr-x   0        0        0      655 2024-04-08 13:52:45.562023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON/CANTON.prj
+-rw-r--r--   0        0        0   430828 2024-04-08 13:52:45.562023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON/CANTON.shp
+-rw-r--r--   0        0        0      588 2024-04-08 13:52:45.562023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON/CANTON.shx
+-rw-r--r--   0        0        0     4003 2024-04-08 13:52:45.562023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON_style.sld
+-rw-r--r--   0        0        0      529 2024-04-08 13:52:45.562023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/upload_descriptor.json
+-rw-r--r--   0        0        0       52 2024-04-08 13:52:45.562023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/datasets/2_dataset_archive/CANTON.md5
+-rw-r--r--   0        0        0   991843 2024-04-08 13:52:45.566023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/datasets/2_dataset_archive/CANTON/CANTON.zip
+-rw-r--r--   0        0        0      525 2024-04-08 13:52:45.566023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/datasets/2_dataset_archive/upload_descriptor.json
+-rw-r--r--   0        0        0     4391 2024-04-08 13:52:45.566023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/datasets/5_dataset_maj_bd_gpf/installation.sld
+-rw-r--r--   0        0        0      411 2024-04-08 13:52:45.566023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/datasets/5_dataset_maj_bd_gpf/lot_1/installation-init.sql
+-rw-r--r--   0        0        0   368640 2024-04-08 13:52:45.570023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/datasets/5_dataset_maj_bd_gpf/lot_2/installation.gpkg
+-rw-r--r--   0        0        0   676357 2024-04-08 13:52:45.570023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/datasets/5_dataset_maj_bd_gpf/lot_3/installation.csv
+-rw-r--r--   0        0        0       84 2024-04-08 13:52:45.570023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/datasets/5_dataset_maj_bd_gpf/lot_3/installation.csvt
+-rw-r--r--   0        0        0     1731 2024-04-08 13:52:45.570023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/datasets/5_dataset_maj_bd_gpf/upload_descriptor.json
+-rw-r--r--   0        0        0     5019 2024-04-08 13:52:45.570023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/workflows/generic_archive.jsonc
+-rw-r--r--   0        0        0    15492 2024-04-08 13:52:45.570023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/workflows/generic_joincache.jsonc
+-rw-r--r--   0        0        0     9884 2024-04-08 13:52:45.570023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/workflows/generic_maj_bdd.jsonc
+-rw-r--r--   0        0        0    11561 2024-04-08 13:52:45.570023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/workflows/generic_moissonnage.jsonc
+-rw-r--r--   0        0        0     9209 2024-04-08 13:52:45.570023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/workflows/generic_raster.jsonc
+-rw-r--r--   0        0        0    15240 2024-04-08 13:52:45.570023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/workflows/generic_vecteur.jsonc
+-rw-r--r--   0        0        0     8059 2024-04-08 13:52:45.570023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/auth/Authentifier.py
+-rw-r--r--   0        0        0      274 2024-04-08 13:52:45.570023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/auth/Errors.py
+-rw-r--r--   0        0        0     1493 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/auth/Token.py
+-rw-r--r--   0        0        0       46 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/auth/__init__.py
+-rw-r--r--   0        0        0     2589 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/helper/FileHelper.py
+-rw-r--r--   0        0        0     6939 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/helper/JsonHelper.py
+-rw-r--r--   0        0        0      916 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/helper/PrintLogHelper.py
+-rw-r--r--   0        0        0       59 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/helper/__init__.py
+-rw-r--r--   0        0        0    15811 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/io/ApiRequester.py
+-rw-r--r--   0        0        0      607 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/io/Color.py
+-rw-r--r--   0        0        0     5695 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/io/Config.py
+-rw-r--r--   0        0        0     5318 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/io/Dataset.py
+-rw-r--r--   0        0        0     4143 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/io/DescriptorFileReader.py
+-rw-r--r--   0        0        0     6878 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/io/Errors.py
+-rw-r--r--   0        0        0     2909 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/io/JsonConverter.py
+-rw-r--r--   0        0        0     4416 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/io/OutputManager.py
+-rw-r--r--   0        0        0     4075 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/io/UploadDescriptorFileReader.py
+-rw-r--r--   0        0        0       47 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/io/__init__.py
+-rw-r--r--   0        0        0      793 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/pattern/SingleInstance.py
+-rw-r--r--   0        0        0      637 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/pattern/Singleton.py
+-rw-r--r--   0        0        0       33 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/pattern/__init__.py
+-rw-r--r--   0        0        0        1 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/py.typed
+-rw-r--r--   0        0        0     1209 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/AbstractCommonFile.py
+-rw-r--r--   0        0        0     2486 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/Annexe.py
+-rw-r--r--   0        0        0      222 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/Check.py
+-rw-r--r--   0        0        0      584 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/CheckExecution.py
+-rw-r--r--   0        0        0     4269 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/Configuration.py
+-rw-r--r--   0        0        0     3400 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/Datastore.py
+-rw-r--r--   0        0        0     3363 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/Endpoint.py
+-rw-r--r--   0        0        0      183 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/Errors.py
+-rw-r--r--   0        0        0     2586 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/Metadata.py
+-rw-r--r--   0        0        0     2140 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/Offering.py
+-rw-r--r--   0        0        0      332 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/Permission.py
+-rw-r--r--   0        0        0      231 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/Processing.py
+-rw-r--r--   0        0        0     2026 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/ProcessingExecution.py
+-rw-r--r--   0        0        0     1005 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/Static.py
+-rw-r--r--   0        0        0    14998 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/StoreEntity.py
+-rw-r--r--   0        0        0     1933 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/StoredData.py
+-rw-r--r--   0        0        0      235 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/Tms.py
+-rw-r--r--   0        0        0     7270 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/Upload.py
+-rw-r--r--   0        0        0     1010 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/User.py
+-rw-r--r--   0        0        0     1432 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/__init__.py
+-rw-r--r--   0        0        0     2521 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/interface/CommentInterface.py
+-rw-r--r--   0        0        0     2025 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/interface/CreatedByUploadFileInterface.py
+-rw-r--r--   0        0        0     1051 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/interface/CsfInterface.py
+-rw-r--r--   0        0        0     1102 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/interface/DownloadInterface.py
+-rw-r--r--   0        0        0      805 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/interface/EventInterface.py
+-rw-r--r--   0        0        0     1262 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/interface/FullEditInterface.py
+-rw-r--r--   0        0        0      869 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/interface/LogsInterface.py
+-rw-r--r--   0        0        0     1116 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/interface/PartialEditInterface.py
+-rw-r--r--   0        0        0      998 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/interface/ReUploadFileInterface.py
+-rw-r--r--   0        0        0     2107 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/interface/SharingInterface.py
+-rw-r--r--   0        0        0     2329 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/interface/TagInterface.py
+-rw-r--r--   0        0        0       88 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/interface/__init__.py
+-rw-r--r--   0        0        0      512 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/Errors.py
+-rw-r--r--   0        0        0    20884 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/Workflow.py
+-rw-r--r--   0        0        0       40 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/__init__.py
+-rw-r--r--   0        0        0     5726 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/action/ActionAbstract.py
+-rw-r--r--   0        0        0     7077 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/action/ConfigurationAction.py
+-rw-r--r--   0        0        0     1776 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/action/CopyConfigurationAction.py
+-rw-r--r--   0        0        0     5149 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/action/DeleteAction.py
+-rw-r--r--   0        0        0     3172 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/action/EditAction.py
+-rw-r--r--   0        0        0     2551 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/action/EditUsedDataConfigurationAction.py
+-rw-r--r--   0        0        0     6827 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/action/OfferingAction.py
+-rw-r--r--   0        0        0     2153 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/action/PermissionAction.py
+-rw-r--r--   0        0        0    19885 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/action/ProcessingExecutionAction.py
+-rw-r--r--   0        0        0     7452 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/action/SynchronizeOfferingAction.py
+-rw-r--r--   0        0        0    20644 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/action/UploadAction.py
+-rw-r--r--   0        0        0       72 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/action/__init__.py
+-rw-r--r--   0        0        0     2267 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/resolver/AbstractResolver.py
+-rw-r--r--   0        0        0     3389 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/resolver/DateResolver.py
+-rw-r--r--   0        0        0     1933 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/resolver/DictResolver.py
+-rw-r--r--   0        0        0      708 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/resolver/DumbResolver.py
+-rw-r--r--   0        0        0     4533 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/resolver/Errors.py
+-rw-r--r--   0        0        0     6076 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/resolver/FileResolver.py
+-rw-r--r--   0        0        0     3838 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/resolver/GlobalResolver.py
+-rw-r--r--   0        0        0     5760 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/resolver/StoreEntityResolver.py
+-rw-r--r--   0        0        0     1908 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/resolver/UserResolver.py
+-rw-r--r--   0        0        0      110 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/resolver/__init__.py
+-rw-r--r--   0        0        0      960 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/tests/ErrorsTestCase.py
+-rw-r--r--   0        0        0     1739 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/tests/GpfTestCase.py
+-rw-r--r--   0        0        0     3419 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/tests/MainTestCase.py
+-rw-r--r--   0        0        0        0 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/tests/__init__.py
+-rw-r--r--   0        0        0      369 2024-04-08 13:52:45.574023 sdk_entrepot_gpf-0.1.25/tests/_conf/test_authentifier.ini
+-rw-r--r--   0        0        0      308 2024-04-08 13:52:45.578023 sdk_entrepot_gpf-0.1.25/tests/_conf/test_overload.ini
+-rw-r--r--   0        0        0      594 2024-04-08 13:52:45.578023 sdk_entrepot_gpf-0.1.25/tests/_conf/test_requester.ini
+-rw-r--r--   0        0        0       40 2024-04-08 13:52:45.578023 sdk_entrepot_gpf-0.1.25/tests/_conf/test_upload.ini
+-rw-r--r--   0        0        0       69 2024-04-08 13:52:45.578023 sdk_entrepot_gpf-0.1.25/tests/_conf/test_value_type.ini
+-rw-r--r--   0        0        0      460 2024-04-08 13:52:45.578023 sdk_entrepot_gpf-0.1.25/tests/_data/datasets/1_test_dataset_bad_pathes/upload_descriptor.json
+-rw-r--r--   0        0        0      305 2024-04-08 13:52:45.578023 sdk_entrepot_gpf-0.1.25/tests/_data/datasets/2_test_dataset_bad_md5/CANTON.md5
+-rw-r--r--   0        0        0        5 2024-04-08 13:52:45.578023 sdk_entrepot_gpf-0.1.25/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.cpg
+-rw-r--r--   0        0        0     2318 2024-04-08 13:52:45.578023 sdk_entrepot_gpf-0.1.25/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.dbf
+-rw-r--r--   0        0        0      145 2024-04-08 13:52:45.578023 sdk_entrepot_gpf-0.1.25/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.prj
+-rw-r--r--   0        0        0  1279276 2024-04-08 13:52:45.582023 sdk_entrepot_gpf-0.1.25/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.shp
+-rw-r--r--   0        0        0      572 2024-04-08 13:52:45.582023 sdk_entrepot_gpf-0.1.25/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.shx
+-rw-r--r--   0        0        0        0 2024-04-08 13:52:45.582023 sdk_entrepot_gpf-0.1.25/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/sous_dossier/coucou.txt
+-rw-r--r--   0        0        0      567 2024-04-08 13:52:45.582023 sdk_entrepot_gpf-0.1.25/tests/_data/datasets/2_test_dataset_bad_md5/upload_descriptor.json
+-rw-r--r--   0        0        0       11 2024-04-08 13:52:45.582023 sdk_entrepot_gpf-0.1.25/tests/_data/datasets/3_test_dataset_sub_dir/.gitignore
+-rw-r--r--   0        0        0        5 2024-04-08 13:52:45.582023 sdk_entrepot_gpf-0.1.25/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.cpg
+-rw-r--r--   0        0        0     2318 2024-04-08 13:52:45.582023 sdk_entrepot_gpf-0.1.25/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.dbf
+-rw-r--r--   0        0        0      145 2024-04-08 13:52:45.582023 sdk_entrepot_gpf-0.1.25/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.prj
+-rw-r--r--   0        0        0  1279276 2024-04-08 13:52:45.590023 sdk_entrepot_gpf-0.1.25/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.shp
+-rw-r--r--   0        0        0      572 2024-04-08 13:52:45.590023 sdk_entrepot_gpf-0.1.25/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.shx
+-rw-r--r--   0        0        0        0 2024-04-08 13:52:45.590023 sdk_entrepot_gpf-0.1.25/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/sous_dossier/coucou.txt
+-rw-r--r--   0        0        0      567 2024-04-08 13:52:45.590023 sdk_entrepot_gpf-0.1.25/tests/_data/datasets/3_test_dataset_sub_dir/upload_descriptor.json
+-rw-r--r--   0        0        0     2659 2024-04-08 13:52:45.590023 sdk_entrepot_gpf-0.1.25/tests/_data/workflows/bad-workflow.jsonc
+-rw-r--r--   0        0        0       53 2024-04-08 13:52:45.590023 sdk_entrepot_gpf-0.1.25/tests/_test/helper/FileHelper/md5.txt
+-rw-r--r--   0        0        0       78 2024-04-08 13:52:45.590023 sdk_entrepot_gpf-0.1.25/tests/_test/helper/JsonHelper/json_not_parsable.json
+-rw-r--r--   0        0        0       52 2024-04-08 13:52:45.590023 sdk_entrepot_gpf-0.1.25/tests/_test/helper/JsonHelper/json_not_valid.json
+-rw-r--r--   0        0        0      108 2024-04-08 13:52:45.590023 sdk_entrepot_gpf-0.1.25/tests/_test/helper/JsonHelper/json_parsable.json
+-rw-r--r--   0        0        0      563 2024-04-08 13:52:45.590023 sdk_entrepot_gpf-0.1.25/tests/_test/helper/JsonHelper/schema.json
+-rw-r--r--   0        0        0      485 2024-04-08 13:52:45.590023 sdk_entrepot_gpf-0.1.25/tests/_test/helper/JsonHelper/schema_invalid.json
+-rw-r--r--   0        0        0       23 2024-04-08 13:52:45.590023 sdk_entrepot_gpf-0.1.25/tests/_test/workflow/resolver/FileResolver/dict.json
+-rw-r--r--   0        0        0       21 2024-04-08 13:52:45.590023 sdk_entrepot_gpf-0.1.25/tests/_test/workflow/resolver/FileResolver/list.json
+-rw-r--r--   0        0        0        2 2024-04-08 13:52:45.590023 sdk_entrepot_gpf-0.1.25/tests/_test/workflow/resolver/FileResolver/not-valid.json
+-rw-r--r--   0        0        0       31 2024-04-08 13:52:45.590023 sdk_entrepot_gpf-0.1.25/tests/_test/workflow/resolver/FileResolver/text.txt
+-rw-r--r--   0        0        0     7428 2024-04-08 13:52:45.590023 sdk_entrepot_gpf-0.1.25/tests/auth/AuthentifierTestCase.py
+-rw-r--r--   0        0        0     1187 2024-04-08 13:52:45.590023 sdk_entrepot_gpf-0.1.25/tests/auth/TokenTestCase.py
+-rw-r--r--   0        0        0        0 2024-04-08 13:52:45.590023 sdk_entrepot_gpf-0.1.25/tests/auth/__init__.py
+-rw-r--r--   0        0        0     1060 2024-04-08 13:52:45.590023 sdk_entrepot_gpf-0.1.25/tests/helper/FileHelperTestCase.py
+-rw-r--r--   0        0        0     9967 2024-04-08 13:52:45.590023 sdk_entrepot_gpf-0.1.25/tests/helper/JsonHelperTestCase.py
+-rw-r--r--   0        0        0        0 2024-04-08 13:52:45.590023 sdk_entrepot_gpf-0.1.25/tests/helper/__init__.py
+-rw-r--r--   0        0        0    23354 2024-04-08 13:52:45.590023 sdk_entrepot_gpf-0.1.25/tests/io/ApiRequesterTestCase.py
+-rw-r--r--   0        0        0     3599 2024-04-08 13:52:45.590023 sdk_entrepot_gpf-0.1.25/tests/io/ConfigTestCase.py
+-rw-r--r--   0        0        0     2225 2024-04-08 13:52:45.590023 sdk_entrepot_gpf-0.1.25/tests/io/DatasetTestCase.py
+-rw-r--r--   0        0        0     3197 2024-04-08 13:52:45.590023 sdk_entrepot_gpf-0.1.25/tests/io/ErrorsTestCase.py
+-rw-r--r--   0        0        0     1202 2024-04-08 13:52:45.590023 sdk_entrepot_gpf-0.1.25/tests/io/JsonConverterTestCase.py
+-rw-r--r--   0        0        0     1774 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/io/UploadDescriptorFileReaderTestCase.py
+-rw-r--r--   0        0        0        0 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/io/__init__.py
+-rw-r--r--   0        0        0     1122 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/store/AbstractCommonFileTestCase.py
+-rw-r--r--   0        0        0     2587 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/store/AnnexeTestCase.py
+-rw-r--r--   0        0        0     2025 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/store/CheckExecutionTestCase.py
+-rw-r--r--   0        0        0     7221 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/store/ConfigurationTestCase.py
+-rw-r--r--   0        0        0     4849 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/store/DatastoreTestCase.py
+-rw-r--r--   0        0        0     5595 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/store/EndpointTestCase.py
+-rw-r--r--   0        0        0     1152 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/store/ErrorsTestCase.py
+-rw-r--r--   0        0        0     2297 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/store/MetadataTestCase.py
+-rw-r--r--   0        0        0     2687 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/store/OfferingTestCase.py
+-rw-r--r--   0        0        0     4691 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/store/ProcessingExecutionTestCase.py
+-rw-r--r--   0        0        0    26065 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/store/StoreEntityTestCase.py
+-rw-r--r--   0        0        0     3137 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/store/StoredDataTestCase.py
+-rw-r--r--   0        0        0    11003 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/store/UploadTestCase.py
+-rw-r--r--   0        0        0        0 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/store/__init__.py
+-rw-r--r--   0        0        0     5134 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/store/interface/CommentInterfaceTestCase.py
+-rw-r--r--   0        0        0     2790 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/store/interface/CreatedByUploadFileInterfaceTestCase.py
+-rw-r--r--   0        0        0     2536 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/store/interface/CsfInterfaceTestCase.py
+-rw-r--r--   0        0        0     1767 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/store/interface/DownloadInterfaceTestCase.py
+-rw-r--r--   0        0        0     1663 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/store/interface/EventInterfaceTestCase.py
+-rw-r--r--   0        0        0     2326 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/store/interface/FullEditInterfaceTestCase.py
+-rw-r--r--   0        0        0     2243 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/store/interface/PartialEditInterfaceTestCase.py
+-rw-r--r--   0        0        0     1569 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/store/interface/ReUploadFileInterfaceTestCase.py
+-rw-r--r--   0        0        0     4039 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/store/interface/SharingInterfaceTestCase.py
+-rw-r--r--   0        0        0     3899 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/store/interface/TagInterfaceTestCase.py
+-rw-r--r--   0        0        0        0 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/store/interface/__init__.py
+-rw-r--r--   0        0        0    28836 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/workflow/WorkflowTestCase.py
+-rw-r--r--   0        0        0        0 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/workflow/__init__.py
+-rw-r--r--   0        0        0     3595 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/workflow/action/ActionAbstractTestCase.py
+-rw-r--r--   0        0        0    10471 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/workflow/action/ConfigurationActionTestCase.py
+-rw-r--r--   0        0        0     2502 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/workflow/action/CopyConfigurationActionTestCase.py
+-rw-r--r--   0        0        0    12123 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/workflow/action/DeleteActionTestCase.py
+-rw-r--r--   0        0        0     5262 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/workflow/action/EditActionTestCase.py
+-rw-r--r--   0        0        0     2392 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/workflow/action/EditUsedDataConfigurationActionTestCase.py
+-rw-r--r--   0        0        0    16051 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/workflow/action/OfferingActionTestCase.py
+-rw-r--r--   0        0        0     1547 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/workflow/action/PermissionActionTestCase.py
+-rw-r--r--   0        0        0    24541 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/workflow/action/ProcessingExecutionActionTestCase.py
+-rw-r--r--   0        0        0    10675 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/workflow/action/SynchronizeOfferingActionTestCase.py
+-rw-r--r--   0        0        0    26204 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/workflow/action/UploadActionTestCase.py
+-rw-r--r--   0        0        0        0 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/workflow/action/__init__.py
+-rw-r--r--   0        0        0     2133 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/workflow/resolver/AbstractResolverTestCase.py
+-rw-r--r--   0        0        0     2401 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/workflow/resolver/DateResolverTestCase.py
+-rw-r--r--   0        0        0     1124 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/workflow/resolver/DictResolverTestCase.py
+-rw-r--r--   0        0        0     5479 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/workflow/resolver/FileResolverTestCase.py
+-rw-r--r--   0        0        0     7361 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/workflow/resolver/GlobalResolverTestCase.py
+-rw-r--r--   0        0        0    15246 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/workflow/resolver/StoreEntityResolverTestCase.py
+-rw-r--r--   0        0        0     2237 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/workflow/resolver/UserResolverTestCase.py
+-rw-r--r--   0        0        0        0 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/tests/workflow/resolver/__init__.py
+-rw-r--r--   0        0        0   116760 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/uml/classes.png
+-rw-r--r--   0        0        0     9175 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/uml/classes.uxf
+-rw-r--r--   0        0        0    43510 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/uml/interfaces.png
+-rw-r--r--   0        0        0     7059 2024-04-08 13:52:45.594023 sdk_entrepot_gpf-0.1.25/uml/interfaces.uxf
+-rw-r--r--   0        0        0     1773 1970-01-01 00:00:00.000000 sdk_entrepot_gpf-0.1.25/PKG-INFO
```

### Comparing `sdk_entrepot_gpf-0.1.24/.github/workflows/ci-dev.yml` & `sdk_entrepot_gpf-0.1.25/.github/workflows/ci-dev.yml`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/.github/workflows/ci-prod.yml` & `sdk_entrepot_gpf-0.1.25/.github/workflows/ci-prod.yml`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/.github/workflows/code-quality.yml` & `sdk_entrepot_gpf-0.1.25/.github/workflows/code-quality.yml`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/.gitignore` & `sdk_entrepot_gpf-0.1.25/.gitignore`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/.pylintrc` & `sdk_entrepot_gpf-0.1.25/.pylintrc`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/.vscode/settings.json` & `sdk_entrepot_gpf-0.1.25/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/CHANGELOG.md` & `sdk_entrepot_gpf-0.1.25/CHANGELOG.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,31 @@
 # CHANGE LOG
 
 ## v0.1.25
 
 ### [Added]
 
+* workflow : ajout de EditUsedDataConfigurationAction #105
+* DeleteAction: meilleur gestion cas sans élément à supprimé #115
+* UploadAction: les conflits de livraisons et timeout lors de la livraison ne bloquent pas la suite du traitement #119, #121
+* ApiRequester: ajout de timeout #121
+
 ### [Changed]
 
+* ajout d'une `LogsInterface` pour gérer les logs (mutualisation de `api_logs`).
+* utilisation systématique de la fonction `JsonHelper.loads` (au lieu de `json.loads`) pour afficher un message d'erreur et le JSON posant problème en cas de besoin (sauf si raison particulière, à expliquer).
+* UploadAction: mise en commun fonctions__push_data_files et __push_md5_files
+
 ### [Fixed]
 
+* correction de la résolution de la valeur d'itération dans les workflows.
+* OfferingAction: utilisation du bon datastore #116
+* DeleteAction: debug mauvaise utilisation des filtres #114
+* Configuration: création/récupération des offres avec le bon datastore
+
 ## v0.1.24
 
 ### [Added]
 
 * StoreEntityResolver: possibilité de récupérer une liste d'entités ou d’informations sur une entité #85
 * ajout classe Permission : gère les permissions sur les offres #93
 * ajout classe PermissionAction : gère les permissions sur les offres depuis le workflow #94
```

### Comparing `sdk_entrepot_gpf-0.1.24/LICENSE` & `sdk_entrepot_gpf-0.1.25/LICENSE`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/README.md` & `sdk_entrepot_gpf-0.1.25/README.md`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/check.sh` & `sdk_entrepot_gpf-0.1.25/check.sh`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/docker/Dockerfile` & `sdk_entrepot_gpf-0.1.25/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/docker/README.md` & `sdk_entrepot_gpf-0.1.25/docker/README.md`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/docs/assets/css/extra.css` & `sdk_entrepot_gpf-0.1.25/docs/assets/css/extra.css`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/docs/assets/css/neoteroi.css` & `sdk_entrepot_gpf-0.1.25/docs/assets/css/neoteroi.css`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/docs/assets/images/favicon.ico` & `sdk_entrepot_gpf-0.1.25/docs/assets/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/docs/assets/images/index__utilisation_module.excalidraw` & `sdk_entrepot_gpf-0.1.25/docs/assets/images/index__utilisation_module.excalidraw`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/docs/assets/images/index__utilisation_module.png` & `sdk_entrepot_gpf-0.1.25/docs/assets/images/index__utilisation_module.png`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/docs/assets/images/logo.png` & `sdk_entrepot_gpf-0.1.25/docs/assets/images/logo.png`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/docs/comme-executable.md` & `sdk_entrepot_gpf-0.1.25/docs/comme-executable.md`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/docs/comme-module.md` & `sdk_entrepot_gpf-0.1.25/docs/comme-module.md`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/docs/configuration.md` & `sdk_entrepot_gpf-0.1.25/docs/configuration.md`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/docs/configuration_details.md` & `sdk_entrepot_gpf-0.1.25/docs/configuration_details.md`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/docs/development.md` & `sdk_entrepot_gpf-0.1.25/docs/development.md`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/docs/index.md` & `sdk_entrepot_gpf-0.1.25/docs/index.md`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/docs/resolveurs.md` & `sdk_entrepot_gpf-0.1.25/docs/resolveurs.md`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/docs/tutoriel_1_archive.md` & `sdk_entrepot_gpf-0.1.25/docs/tutoriel_1_archive.md`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/docs/tutoriel_2_flux_vecteur.md` & `sdk_entrepot_gpf-0.1.25/docs/tutoriel_2_flux_vecteur.md`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/docs/tutoriel_3_flux_raster.md` & `sdk_entrepot_gpf-0.1.25/docs/tutoriel_3_flux_raster.md`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/docs/upload_descriptor.md` & `sdk_entrepot_gpf-0.1.25/docs/upload_descriptor.md`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/docs/workflow.md` & `sdk_entrepot_gpf-0.1.25/docs/workflow.md`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/mkdocs.yml` & `sdk_entrepot_gpf-0.1.25/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/pyproject.toml` & `sdk_entrepot_gpf-0.1.25/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/Errors.py` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/Errors.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/__main__.py` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 
 import configparser
 import io
 import sys
 import argparse
 import traceback
 from pathlib import Path
-from typing import Any, Callable, Dict, List, Optional, Sequence, Union
 import shutil
+from typing import Any, Callable, Dict, List, Optional, Sequence, Union
+import requests
+
 
 import sdk_entrepot_gpf
 from sdk_entrepot_gpf.Errors import GpfSdkError
 from sdk_entrepot_gpf.auth.Authentifier import Authentifier
 from sdk_entrepot_gpf.helper.JsonHelper import JsonHelper
 from sdk_entrepot_gpf.helper.PrintLogHelper import PrintLogHelper
 from sdk_entrepot_gpf.io.Color import Color
@@ -876,12 +878,18 @@
         Config().om.critical(f"L'élément demandé n'existe pas ({e_error.message}). Contactez le support si vous n'êtes pas à l'origine de la demande. URL : {e_error.method} {e_error.url}.")
     except ConflictError as e_error:
         # gestion "globale" des ConflictError (ConfigurationAction et OfferingAction
         # possèdent chacune leur propre gestion)
         Config().om.debug(traceback.format_exc())
         Config().om.critical("La requête envoyée à l'Entrepôt génère un conflit. N'avez-vous pas déjà effectué l'action que vous essayez de faire ?")
         Config().om.error(e_error.message)
+    except requests.Timeout as e_error:
+        # gestion "globale" des timeout
+        Config().om.debug(traceback.format_exc())
+        Config().om.critical(f"Requête trop longe, timeout. URL : {str(e_error.request.method)+' ' +str(e_error.request.url) if e_error.request else ''}.")
+
     except Exception as e_exception:
+        print(e_exception)
         Config().om.critical("Erreur non spécifiée :")
         Config().om.error(traceback.format_exc())
         Config().om.critical("Erreur non spécifiée.")
     sys.exit(1)
```

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/_conf/default.ini` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_conf/default.ini`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/_conf/json_schemas/annexe_descriptor_file.json` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_conf/json_schemas/annexe_descriptor_file.json`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/_conf/json_schemas/metadata_descriptor_file.json` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_conf/json_schemas/metadata_descriptor_file.json`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/_conf/json_schemas/static_descriptor_file.json` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_conf/json_schemas/static_descriptor_file.json`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/_conf/json_schemas/upload_descriptor_file.json` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_conf/json_schemas/upload_descriptor_file.json`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/_conf/json_schemas/workflow.json` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_conf/json_schemas/workflow.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999999957129596%*

 * *Differences: {"'properties'": "{'workflow': {'properties': {'steps': {'additionalProperties': {'properties': "*

 * *                 "{'actions': {'items': {'properties': {'type': {'enum': {insert: [(4, "*

 * *                 "'used_data-configuration')]}}, 'delete_used_data': OrderedDict([('type', "*

 * *                 "'array'), ('items', OrderedDict([('type', 'object')]))]), 'append_used_data': "*

 * *                 "OrderedDict([('type', 'array'), ('items', OrderedDict([('type', "*

 * *                 "'object')]))])}}}}}}}}}"}*

```diff
@@ -22,14 +22,20 @@
                     "additionalProperties": {
                         "additionalProperties": false,
                         "properties": {
                             "actions": {
                                 "items": {
                                     "additionalProperties": false,
                                     "properties": {
+                                        "append_used_data": {
+                                            "items": {
+                                                "type": "object"
+                                            },
+                                            "type": "array"
+                                        },
                                         "body_parameters": {
                                             "type": "object"
                                         },
                                         "cascade": {
                                             "type": "boolean"
                                         },
                                         "comments": {
@@ -40,14 +46,20 @@
                                         },
                                         "confirm": {
                                             "type": "boolean"
                                         },
                                         "datastore": {
                                             "type": "string"
                                         },
+                                        "delete_used_data": {
+                                            "items": {
+                                                "type": "object"
+                                            },
+                                            "type": "array"
+                                        },
                                         "entity_id": {
                                             "type": "string"
                                         },
                                         "entity_type": {
                                             "type": "string"
                                         },
                                         "filter_infos": {
@@ -72,14 +84,15 @@
                                         },
                                         "type": {
                                             "enum": [
                                                 "delete-entity",
                                                 "processing-execution",
                                                 "configuration",
                                                 "copy-configuration",
+                                                "used_data-configuration",
                                                 "offering",
                                                 "synchronize-offering",
                                                 "edit-entity",
                                                 "permission"
                                             ],
                                             "type": "string"
                                         },
```

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON/CANTON.dbf` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON/CANTON.dbf`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON/CANTON.prj` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON/CANTON.prj`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON/CANTON.shp` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON/CANTON.shp`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON/CANTON.shx` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON/CANTON.shx`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON_style.sld` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON_style.sld`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/upload_descriptor.json` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/upload_descriptor.json`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/_data/datasets/2_dataset_archive/CANTON/CANTON.zip` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/datasets/2_dataset_archive/CANTON/CANTON.zip`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/_data/datasets/2_dataset_archive/upload_descriptor.json` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/datasets/2_dataset_archive/upload_descriptor.json`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/_data/datasets/5_dataset_maj_bd_gpf/installation.sld` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/datasets/5_dataset_maj_bd_gpf/installation.sld`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/_data/datasets/5_dataset_maj_bd_gpf/lot_2/installation.gpkg` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/datasets/5_dataset_maj_bd_gpf/lot_2/installation.gpkg`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/_data/datasets/5_dataset_maj_bd_gpf/lot_3/installation.csv` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/datasets/5_dataset_maj_bd_gpf/lot_3/installation.csv`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/_data/datasets/5_dataset_maj_bd_gpf/upload_descriptor.json` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/datasets/5_dataset_maj_bd_gpf/upload_descriptor.json`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/_data/workflows/generic_archive.jsonc` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/workflows/generic_archive.jsonc`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/_data/workflows/generic_joincache.jsonc` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/workflows/generic_joincache.jsonc`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/_data/workflows/generic_maj_bdd.jsonc` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/workflows/generic_maj_bdd.jsonc`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/_data/workflows/generic_moissonnage.jsonc` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/workflows/generic_moissonnage.jsonc`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/_data/workflows/generic_raster.jsonc` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/workflows/generic_raster.jsonc`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/_data/workflows/generic_vecteur.jsonc` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/_data/workflows/generic_vecteur.jsonc`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/auth/Authentifier.py` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/auth/Authentifier.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/auth/Token.py` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/auth/Token.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/helper/FileHelper.py` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/helper/FileHelper.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/helper/JsonHelper.py` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/helper/JsonHelper.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/helper/PrintLogHelper.py` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/helper/PrintLogHelper.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/io/ApiRequester.py` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/io/ApiRequester.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from __future__ import unicode_literals
-from io import BufferedReader
-import json
-from pathlib import Path
+
 import re
 import time
 import traceback
+from io import BufferedReader
+from pathlib import Path
 from typing import Any, Dict, Optional, Tuple, List, Union
 import requests
 from requests_toolbelt import MultipartEncoder
 
 from sdk_entrepot_gpf.Errors import GpfSdkError
 from sdk_entrepot_gpf.auth.Authentifier import Authentifier
+from sdk_entrepot_gpf.helper.JsonHelper import JsonHelper
 from sdk_entrepot_gpf.pattern.Singleton import Singleton
 from sdk_entrepot_gpf.io.JsonConverter import JsonConverter
 from sdk_entrepot_gpf.io.Errors import ApiError, ConflictError, RouteNotFoundError, InternalServerError, NotFoundError, NotAuthorizedError, BadRequestError, StatusCodeError
 from sdk_entrepot_gpf.io.Config import Config
 
 
 class ApiRequester(metaclass=Singleton):
@@ -43,38 +44,45 @@
         self,
         route_name: str,
         route_params: Optional[Dict[str, Any]] = None,
         method: str = "GET",
         params: Optional[Dict[str, Any]] = None,
         data: Optional[Union[Dict[str, Any], List[Any]]] = None,
         files: Optional[Dict[str, Tuple[str, BufferedReader]]] = None,
+        timeout: Optional[int] = -1000,
     ) -> requests.Response:
         """Exécute une requête à l'API à partir du nom d'une route. La requête est retentée plusieurs fois s'il y a un problème.
 
         Args:
             route_name (str): Route à utiliser
             route_params (Optional[Dict[str, Any]], optional): Paramètres obligatoires pour compléter la route.
             params (Optional[Dict[str, Any]], optional): Paramètres optionnels de l'URL.
             method (str, optional): méthode de la requête.
             data (Optional[Dict[str, Any]], optional): Données de la requête.
             files (Optional[Dict[str, Tuple[Any]]], optional): Liste des fichiers à envoyer {"file":('fichier.ext', File)}.
+            timeout (Optional[int], optional): timeout en seconde ou None pour désactivé le timeout.
 
         Raises:
             RouteNotFoundError: levée si la route demandée n'est pas définie dans les paramètres
             InternalServerError: levée si erreur interne de l'API
             NotFoundError: levée si l'entité demandée n'est pas trouvée par l'API
             NotAuthorizedError: levée si l'action effectuée demande d'autres autorisations
             BadRequestError: levée si la requête envoyée n'est pas correcte
             StatusCodeError: levée si un "status code" non prévu est récupéré
 
         Returns:
             réponse vérifiée
         """
         Config().om.debug(f"route_request({route_name}, {method}, {route_params}, {params})")
 
+        # gestion timeout
+        if timeout and timeout < 0:
+            s_timeout = Config().get("routing", f"{route_name}_timeout", "-1000")
+            timeout = None if not s_timeout or s_timeout == "null" else int(s_timeout)
+
         # La valeur par défaut est transformée en un dict valide
         if route_params is None:
             route_params = {}
 
         # Si la clef 'datastore' n'est pas définie ou vide, on le récupère dans la config
         if not route_params.get("datastore", None):
             route_params["datastore"] = Config().get("store_api", "datastore", fallback=None)
@@ -93,65 +101,69 @@
         # On formate l'URL
         s_url = s_route.format(**route_params)
 
         # récupération du header additionnel
         s_header = Config().get("routing", route_name + "_header", fallback=None)
         d_header = {}
         if s_header is not None:
-            d_header = json.loads(s_header)
+            d_header = JsonHelper.loads(s_header, f"config.routing.{route_name}_header")
 
         # Exécution de la requête en boucle jusqu'au succès (ou erreur au bout d'un certains temps)
-        return self.url_request(s_url, method, params, data, files, d_header)
+        return self.url_request(s_url, method, params, data, files, d_header, timeout)
 
     def url_request(
         self,
         url: str,
         method: str = "GET",
         params: Optional[Dict[str, Any]] = None,
         data: Optional[Union[Dict[str, Any], List[Any]]] = None,
         files: Optional[Dict[str, Tuple[str, BufferedReader]]] = None,
         header: Dict[str, str] = {},
+        timeout: Optional[int] = -1000,
     ) -> requests.Response:
         """Effectue une requête à l'API à partir d'une url. La requête est retentée plusieurs fois s'il y a un problème.
 
         Args:
             url (str): url absolue de la requête
             method (str, optional): méthode de la requête
             params (Optional[Dict[str, Any]], optional): paramètres de la requête (ajouté à l'url)
             data (Optional[Union[Dict[str, Any], List[Any]]], optional): contenue de la requête (ajouté au corp)
             files (Optional[Dict[str, Tuple[Any]]], optional): fichiers à envoyer
             header (Dict[str, str], optional): Header additionnel pour la requête
+            timeout (Optional[int], optional): timeout en seconde ou None pour désactivé le timeout.
 
         Returns:
             réponse si succès
         """
         Config().om.debug(f"url_request({url}, {method}, {params}, {data})")
 
+        # gestion timeout
+        if timeout and timeout < 0:
+            s_timeout = Config().get("store_api", "timeout")
+            timeout = None if not s_timeout or s_timeout == "null" else int(s_timeout)
+
         i_nb_attempts = 0
         while True:
             i_nb_attempts += 1
             try:
                 # On fait la requête
-                return self.__url_request(url, method, params=params, data=data, files=files, header=header)
-            except NotFoundError as e_error:
-                # S'il on a un 404, on ne retente pas, on ne fait rien. On propage l'erreur.
-                raise e_error
+                return self.__url_request(url, method, params=params, data=data, files=files, header=header, timeout=timeout)
 
             except (requests.HTTPError, requests.URLRequired) as e_error:
                 # S'il y a une erreur d'URL, on ne retente pas, on indique de contacter le support
                 s_message = "L'URL indiquée en configuration est invalide ou inexistante. Contactez le support."
                 raise GpfSdkError(s_message) from e_error
 
             except BadRequestError as e_error:
                 # S'il y a une erreur de requête incorrecte, on ne retente pas, on indique de contacter le support
                 s_message = f"La requête formulée par le programme est incorrecte ({e_error.message}). Contactez le support."
                 raise GpfSdkError(s_message) from e_error
 
-            except ConflictError as e_error:
-                # S'il y a un conflit, on ne retente pas, on ne fait rien. On propage l'erreur.
+            except (ConflictError, NotFoundError, requests.Timeout) as e_error:
+                # S'il y a un conflit, un 404 ou un timeout, on ne retente pas, on ne fait rien. On propage l'erreur.
                 raise e_error
 
             except (ApiError, requests.RequestException) as e_error:
                 # Pour les autres erreurs, on retente selon les paramètres indiqués.
                 # On récupère la classe de l'erreur histoire que ce soit plus parlant...
                 s_title = e_error.__class__.__name__
                 Config().om.warning(f"L'exécution d'une requête a échoué (tentative {i_nb_attempts}/{self.__nb_attempts})... ({s_title})")
@@ -169,48 +181,50 @@
         self,
         url: str,
         method: str = "GET",
         params: Optional[Dict[str, Any]] = None,
         data: Optional[Union[Dict[str, Any], List[Any]]] = None,
         files: Optional[Dict[str, Tuple[str, BufferedReader]]] = None,
         header: Dict[str, str] = {},
+        timeout: Optional[int] = None,
     ) -> requests.Response:
         """Effectue une requête à l'API à partir d'une url. Ne retente pas plusieurs fois si problème.
 
         Args:
             url (str): url absolue de la requête
             method (str, optional): méthode de la requête.
             params (Optional[Dict[str, Any]], optional): paramètres.
             data (Optional[Union[Dict[str, Any], List[Any]]], optional): données.
             files (Optional[Dict[str, Tuple[Any]]], optional): fichiers.
             header (Dict[str, str], optional): Header additionnel pour la requête.
+            timeout (Optional[int], optional): timeout en seconde ou None pour désactivé le timeout.
 
         Returns:
             réponse si succès
         """
-        Config().om.debug(f"__url_request({url}, {method}, {params}, {data})")
+        Config().om.debug(f"__url_request({url}, {method}, {params}, {data}, {timeout})")
 
         # Définition du header
         d_headers = Authentifier().get_http_header(json_content_type=files is None)
         d_headers.update(header)
 
         # Création du MultipartEncoder (cf. https://github.com/requests/toolbelt#multipartform-data-encoder)
         d_requests: Dict[str, Any] = {
             "url": url,
             "method": method,
             "headers": d_headers,
             "proxies": self.__proxy,
             "params": params,
+            "timeout": timeout,
         }
         if files:
             d_fields = {**files}
             o_me = MultipartEncoder(fields=d_fields)
             d_headers["content-type"] = o_me.content_type
             # Execution de la requête
-            # TODO : contournement pour les uploads, supprimer `"verify": False` une fois le problème résolu + suppression proxy
             d_requests.update({"data": o_me})
         else:
             d_requests.update({"params": params, "json": data})
 
         # exécution de la requête
         r = requests.request(**d_requests)
 
@@ -244,14 +258,15 @@
         route_name: str,
         file_path: Path,
         file_key: str,
         route_params: Optional[Dict[str, Any]] = None,
         method: str = "POST",
         params: Optional[Dict[str, Any]] = None,
         data: Optional[Union[Dict[str, Any], List[Any]]] = None,
+        timeout: Optional[int] = -1000,
     ) -> requests.Response:
         """Exécute une requête à l'API à partir du nom d'une route. La requête est retentée plusieurs fois s'il y a un problème.
 
         Args:
             route_name (str): Route à utiliser
             file_path (Path): Chemin du fichier à uploader
             file_key (str): nom de la clef dans le dictionnaire
@@ -259,21 +274,38 @@
             params (Optional[Dict[str, Any]], optional): Paramètres optionnels de l'URL.
             method (str, optional): méthode de la requête.
             data (Optional[Dict[str, Any]], optional): Données de la requête.
 
         Returns:
             réponse vérifiée
         """
+
+        # gestion timeout
+        if timeout and timeout < 0:
+            s_timeout = Config().get("routing", f"{route_name}_timeout", "-1000")
+            if not s_timeout or s_timeout.lower() == "null" or s_timeout.lower() == "none":
+                # timeout directe ou None (pas de timeout)
+                timeout = None
+            elif re.search(r"^ *-? *\d+ *$", s_timeout):
+                timeout = int(s_timeout)
+            else:
+                # timeout selon la taille du fichier
+                d_timeout_dict: Dict[str, Optional[int]] = dict(JsonHelper.loads(s_timeout, "du dictionnaire des timeout pour {route_name}"))
+                # on rajoute une valeur par défaut
+                d_timeout_dict["-1000"] = -1000
+                i_index_timeout = max(int(i) for i in d_timeout_dict if int(i) <= file_path.stat().st_size)
+                timeout = d_timeout_dict[str(i_index_timeout)]
+
         # Ouverture du fichier et remplissage du tuple de fichier
         with file_path.open("rb") as o_file_binary:
             o_tuple_file = (file_path.name, o_file_binary)
             o_dict_files = {file_key: o_tuple_file}
 
             # Requête
-            return self.route_request(route_name, route_params=route_params, method=method, params=params, data=data, files=o_dict_files)
+            return self.route_request(route_name, route_params=route_params, method=method, params=params, data=data, files=o_dict_files, timeout=timeout)
 
     @staticmethod
     def range_next_page(content_range: Optional[str], length: int) -> bool:
         """Fonction analysant le `Content-Range` d'une réponse pour indiquer s'il
         faut faire d'autres requêtes ou si tout est déjà récupéré.
 
         Args:
```

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/io/Color.py` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/io/Color.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/io/Config.py` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/io/Config.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/io/Dataset.py` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/io/Dataset.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/io/DescriptorFileReader.py` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/io/DescriptorFileReader.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/io/Errors.py` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/io/Errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
             response (str): données reçues
         """
         super().__init__(url, method, params, data)
         self.response_str = response
         self.response_data = None
         # On tente de parser la réponse
         try:
-            self.response_data = json.loads(self.response_str)
+            self.response_data = json.loads(self.response_str)  # json.loads ok car on veut récupérer l'erreur
         except json.JSONDecodeError:
             # Le parsing a échoué, pas grave
             pass
 
     def __str__(self) -> str:
         return self.__repr__()
```

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/io/JsonConverter.py` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/io/JsonConverter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 from __future__ import unicode_literals
 
 import datetime
 import json as JSON
-from typing import Any, Dict, Optional
+from typing import Any, Optional
 
 from sdk_entrepot_gpf.pattern.Singleton import Singleton
 from sdk_entrepot_gpf.io.Config import Config
 
 
 class JsonConverter(metaclass=Singleton):
     """Classe de conversion des objects python en json. Le but est de convertir
-    les objets qui ne sont pas nativement gérés par Python comme les dates."""
+    les objets qui ne sont pas nativement gérés par Python comme les dates mais
+    aussi de permettre de corriger les erreurs en loguant ce qui pose problème."""
 
     def __init__(self) -> None:
         """initialisation : liste des routes et adresse site"""
         # Stockage en attributs de classe des patterns
         self.__datetime_pattern = Config().get_str("json_converter", "datetime_pattern")
         self.__date_pattern = Config().get_str("json_converter", "date_pattern")
         self.__time_pattern = Config().get_str("json_converter", "time_pattern")
 
-    def dumps(self, data: Dict[Any, Any]) -> str:
+    def dumps(self, data: Any) -> str:
         """Cette fonction permet de convertir les classes python en string JSON.
         Pour le moment, sont traitées les dates, times, et datetimes.
         On utilise un "converter" spécialisé.
 
         Args:
             data (Any): données à envoyer à l'api avec des classes python
 
         Returns:
             str: JSON avec gestion des classes Python
         """
         if data is None:
-            return None
+            return "null"
         s_json = JSON.dumps(data, default=self.__converter)
         return s_json
 
     def convert(self, data: Any) -> Any:
         """Passe en string les objets non gérés nativement en JSON par Python.
         Ex : {"date": date(2020, 1, 1)} => {"date": "2020-01-01"}
 
@@ -44,15 +45,15 @@
 
         Returns:
             Any: données à envoyer à l'api sans classe python
         """
         if data is None:
             return None
         s_json = self.dumps(data)
-        return JSON.loads(s_json)
+        return JSON.loads(s_json)  # json.loads ok car pas d'erreur possible ici (dumps juste avant)
 
     def __converter(self, obj: object) -> Optional[str]:
         """Converter spécialisé pour passer des classes python au json.
 
         Args:
             obj (object): objet à convertir
```

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/io/OutputManager.py` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/io/OutputManager.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/io/UploadDescriptorFileReader.py` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/io/UploadDescriptorFileReader.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/pattern/SingleInstance.py` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/pattern/SingleInstance.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/pattern/Singleton.py` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/pattern/Singleton.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/store/AbstractCommonFile.py` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/AbstractCommonFile.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/store/Annexe.py` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/Annexe.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/store/Configuration.py` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/Configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,26 +31,26 @@
         # Requête "get"
         o_response = ApiRequester().route_request(
             s_route,
             method=ApiRequester.GET,
             route_params={"datastore": self.datastore, self._entity_name: self.id},
         )
         # Instanciation de chaque élément renvoyé dans la liste
-        l_offerings: List[Offering] = [Offering(i) for i in o_response.json()]
+        l_offerings: List[Offering] = [Offering(i, datastore=self.datastore) for i in o_response.json()]
 
         return l_offerings
 
     def api_add_offering(self, data_offering: Dict[str, Any]) -> Offering:
         """Ajoute une Offering à cette Configuration.
         Args:
             data_offering (Dict[str, Any]): données pour la création de l'Offering
         Returns:
             Offering: représentation Python de l'Offering créée
         """
-        return Offering.api_create(data_offering, route_params={self._entity_name: self.id})
+        return Offering.api_create(data_offering, route_params={self._entity_name: self.id, "datastore": self.datastore})
 
     def get_liste_deletable_cascade(self) -> List[StoreEntity]:
         """liste les entités à supprimé lors d'une suppression en cascade de la Configuration en supprimant en cascade les offres liées (et uniquement les offres, pas les données stockées).
 
         Returns:
             List[StoreEntity]: liste des entités qui seront supprimé
         """
```

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/store/Datastore.py` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/Datastore.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/store/Endpoint.py` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/Endpoint.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/store/Metadata.py` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/Metadata.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/store/Offering.py` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/Offering.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/store/Static.py` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/Static.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/store/StoreEntity.py` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/StoreEntity.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/store/StoredData.py` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/StoredData.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/store/Upload.py` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/Upload.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/store/User.py` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/User.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/store/__init__.py` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/__init__.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/store/interface/CommentInterface.py` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/interface/CommentInterface.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/store/interface/CreatedByUploadFileInterface.py` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/interface/CreatedByUploadFileInterface.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/store/interface/CsfInterface.py` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/interface/CsfInterface.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/store/interface/DownloadInterface.py` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/interface/DownloadInterface.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/store/interface/EventInterface.py` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/interface/EventInterface.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/store/interface/FullEditInterface.py` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/interface/FullEditInterface.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/store/interface/PartialEditInterface.py` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/interface/PartialEditInterface.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/store/interface/ReUploadFileInterface.py` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/interface/ReUploadFileInterface.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/store/interface/SharingInterface.py` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/interface/SharingInterface.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/store/interface/TagInterface.py` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/store/interface/TagInterface.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/workflow/Workflow.py` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/Workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from sdk_entrepot_gpf.store.StoreEntity import StoreEntity
 from sdk_entrepot_gpf.workflow.Errors import WorkflowError
 from sdk_entrepot_gpf.io.Config import Config
 from sdk_entrepot_gpf.workflow.action.ActionAbstract import ActionAbstract
 from sdk_entrepot_gpf.workflow.action.CopyConfigurationAction import CopyConfigurationAction
 from sdk_entrepot_gpf.workflow.action.DeleteAction import DeleteAction
 from sdk_entrepot_gpf.workflow.action.EditAction import EditAction
+from sdk_entrepot_gpf.workflow.action.EditUsedDataConfigurationAction import EditUsedDataConfigurationAction
 from sdk_entrepot_gpf.workflow.action.PermissionAction import PermissionAction
 from sdk_entrepot_gpf.workflow.action.ProcessingExecutionAction import ProcessingExecutionAction
 from sdk_entrepot_gpf.workflow.action.ConfigurationAction import ConfigurationAction
 from sdk_entrepot_gpf.workflow.action.OfferingAction import OfferingAction
 from sdk_entrepot_gpf.workflow.action.SynchronizeOfferingAction import SynchronizeOfferingAction
 from sdk_entrepot_gpf.workflow.resolver.DictResolver import DictResolver
 from sdk_entrepot_gpf.workflow.resolver.GlobalResolver import GlobalResolver
@@ -166,27 +167,27 @@
         # Gestion des itérations
         if "iter_vals" in d_step and "iter_key" in d_step:
             # on itère sur les clefs
             l_actions = []
             s_actions = str(json.dumps(d_step["actions"], ensure_ascii=False))
 
             # on lance la résolution sur iter_vals
-            d_step["iter_vals"] = json.loads(GlobalResolver().resolve(json.dumps(d_step["iter_vals"]), datastore=datastore))
+            d_step["iter_vals"] = JsonHelper.loads(GlobalResolver().resolve(json.dumps(d_step["iter_vals"]), datastore=datastore), "iter_vals résolu")
             Config().om.debug(f"iter_vals : {d_step['iter_vals']}")
             if isinstance(d_step["iter_vals"][0], (str, float, int)):
-                # si la liste est une liste de string, un int ou flat : on remplace directement
-                for s_val in d_step["iter_vals"]:
-                    l_actions += json.loads(s_actions.replace("{" + d_step["iter_key"] + "}", s_val))
+                # si la liste est une liste de string, un int ou float : on remplace directement
+                for o_val in d_step["iter_vals"]:
+                    l_actions += JsonHelper.loads(s_actions.replace("{" + d_step["iter_key"] + "}", o_val), "iter_val str/float/int")
             else:
                 # on a une liste de sous dict ou apparenté on utilise un résolveur
-                for i, s_val in enumerate(d_step["iter_vals"]):
-                    l_actions += json.loads(s_actions.replace(d_step["iter_key"], f"iter_resolve_{i}"))
-                    GlobalResolver().add_resolver(DictResolver(f"iter_resolve_{i}", s_val))
-
+                for i, o_val in enumerate(d_step["iter_vals"]):
+                    l_actions += JsonHelper.loads(s_actions.replace(d_step["iter_key"], f"iter_resolve_{i}"), f"iter_vals list({i})")
+                    GlobalResolver().add_resolver(DictResolver(f"iter_resolve_{i}", o_val))
             d_step["actions"] = l_actions
+
         elif "iter_vals" in d_step or "iter_key" in d_step:
             # on a une seule des deux clef
             s_error_message = f"Une seule des clefs iter_vals ou iter_key est trouvée: il faut mettre les deux valeurs ou aucune. Étape {step_name} workflow {self.__name}"
             Config().om.error(s_error_message)
             raise WorkflowError(s_error_message)
 
         # on récupère les commentaires commun au workflow et à l'étape
@@ -269,14 +270,16 @@
             return DeleteAction(workflow_context, definition_dict, parent_action)
         if definition_dict["type"] == "processing-execution":
             return ProcessingExecutionAction(workflow_context, definition_dict, parent_action, behavior=behavior)
         if definition_dict["type"] == "configuration":
             return ConfigurationAction(workflow_context, definition_dict, parent_action, behavior=behavior)
         if definition_dict["type"] == "copy-configuration":
             return CopyConfigurationAction(workflow_context, definition_dict, parent_action, behavior=behavior)
+        if definition_dict["type"] == "used_data-configuration":
+            return EditUsedDataConfigurationAction(workflow_context, definition_dict, parent_action)
         if definition_dict["type"] == "offering":
             return OfferingAction(workflow_context, definition_dict, parent_action, behavior=behavior)
         if definition_dict["type"] == "synchronize-offering":
             return SynchronizeOfferingAction(workflow_context, definition_dict, parent_action)
         if definition_dict["type"] == "edit-entity":
             return EditAction(workflow_context, definition_dict, parent_action)
         if definition_dict["type"] == "permission":
```

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/workflow/action/ActionAbstract.py` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/action/ActionAbstract.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/workflow/action/ConfigurationAction.py` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/action/ConfigurationAction.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/workflow/action/CopyConfigurationAction.py` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/action/CopyConfigurationAction.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/workflow/action/DeleteAction.py` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/action/DeleteAction.py`

 * *Files 5% similar despite different names*

```diff
@@ -71,28 +71,31 @@
             ## si id => on recherche directement
             try:
                 l_entities.append(store.TYPE__ENTITY[self.definition_dict["entity_type"]].api_get(self.definition_dict["entity_id"], datastore=datastore))
             except NotFoundError:
                 pass
         elif "filter_infos" in self.definition_dict or "filter_tags" in self.definition_dict:
             ## par liste des éléments
-            l_entities = store.TYPE__ENTITY[self.definition_dict["entity_type"]].api_list(self.definition_dict.get("filter_infos"), self.definition_dict.get("filter_infos"), datastore=datastore)
+            l_entities = store.TYPE__ENTITY[self.definition_dict["entity_type"]].api_list(self.definition_dict.get("filter_infos"), self.definition_dict.get("filter_tags"), datastore=datastore)
         else:
             raise StepActionError('Il faut au moins une des clefs suivantes : "entity_id", "filter_infos", "filter_tags" pour cette action.')
 
-        if len(l_entities) == 0 and not self.definition_dict.get("not_found_ok"):
-            raise StepActionError("Aucune entité trouvée pour la suppression")
-        if len(l_entities) > 1:
-            if self.definition_dict.get("if_multi") == "error":
-                # On sort en erreur
-                raise StepActionError(f"Plusieurs entités trouvées pour la suppression : {l_entities}")
-            if self.definition_dict.get("if_multi") == "first":
-                # on ne supprime que le 1er élément trouvé
-                l_entities = [l_entities[0]]
-            # on les supprimera tous
+        if len(l_entities) == 0:
+            if not self.definition_dict.get("not_found_ok"):
+                raise StepActionError("Aucune entité trouvée pour la suppression")
+            # sinon OK
+            Config().om.info("Aucune entité à supprimé.", green_colored=True)
+            return
+        if len(l_entities) > 1 and self.definition_dict.get("if_multi") == "error":
+            # On sort en erreur
+            raise StepActionError(f"Plusieurs entités trouvées pour la suppression : {l_entities}")
+        if len(l_entities) > 1 and self.definition_dict.get("if_multi") == "first":
+            # on ne supprime que le 1er élément trouvé
+            l_entities = [l_entities[0]]
+        # on les supprimera tous
 
         # récupération des entités en cascades si demandé
         if self.definition_dict.get("cascade", False):
             Config().om.info("Suppression en cascade, recherche des entités à supprimer ...")
             l_entities_cascade = []
             for o_entity in l_entities:
                 l_entities_cascade += o_entity.get_liste_deletable_cascade()
```

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/workflow/action/EditAction.py` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/action/EditAction.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/workflow/action/OfferingAction.py` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/action/OfferingAction.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
                 return
             else:
                 raise GpfSdkError(
                     f"Le comportement {self.__behavior} n'est pas reconnu ({self.BEHAVIOR_STOP}|{self.BEHAVIOR_DELETE}|{self.BEHAVIOR_CONTINUE}), l'exécution de traitement n'est pas possible."
                 )
         # Création en gérant une erreur de type ConflictError (si la Configuration existe déjà selon les critères de l'API)
         try:
-            self.__offering = Offering.api_create(self.definition_dict["body_parameters"], route_params=self.definition_dict["url_parameters"])
+            self.__offering = Offering.api_create(self.definition_dict["body_parameters"], route_params={"datastore": datastore, **self.definition_dict["url_parameters"]})
         except ConflictError as e:
             raise StepActionError(f"Impossible de créer l'offre il y a un conflict : \n{e.message}") from e
 
     def find_configuration(self, datastore: Optional[str] = None) -> Optional[Configuration]:
         """Fonction permettant de récupérer la Configuration associée à l'Offering qui doit être crée par cette Action.
 
         C'est à dire la Configuration indiquée dans `url_parameters` du `definition_dict` de cette Action.
```

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/workflow/action/PermissionAction.py` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/action/PermissionAction.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/workflow/action/ProcessingExecutionAction.py` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/action/ProcessingExecutionAction.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/workflow/action/SynchronizeOfferingAction.py` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/action/SynchronizeOfferingAction.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/workflow/action/UploadAction.py` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/action/UploadAction.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,20 @@
+from pathlib import Path
 import time
-from typing import Any, Callable, Dict, List, Optional
+from typing import Any, Callable, Dict, List, Optional, Tuple
+import requests
 
 
 from sdk_entrepot_gpf.Errors import GpfSdkError
+from sdk_entrepot_gpf.io.Errors import ConflictError
 from sdk_entrepot_gpf.store.CheckExecution import CheckExecution
 from sdk_entrepot_gpf.store.Upload import Upload
 from sdk_entrepot_gpf.io.Dataset import Dataset
 from sdk_entrepot_gpf.io.Config import Config
+from sdk_entrepot_gpf.workflow.Errors import UploadFileError
 from sdk_entrepot_gpf.workflow.action.ActionAbstract import ActionAbstract
 
 
 class UploadAction:
     """Classe permettant d'accompagner la création d'une livraison.
 
     Attributes:
@@ -125,67 +129,118 @@
             Config().om.info(f"Livraison {self.__upload['name']} : les {len(self.__dataset.comments)} commentaires ont été ajoutés avec succès.")
 
     def __push_data_files(self) -> None:
         """Téléverse les fichiers de données (listés dans le dataset)."""
         if self.__upload is not None:
             # Liste les fichiers déjà téléversés sur l'entrepôt et récupère leur taille
             Config().om.info(f"Livraison {self.__upload['name']} : récupération de l'arborescence des données déjà téléversées...")
-            l_arborescence = self.__upload.api_tree()
-            d_destination_taille = UploadAction.parse_tree(l_arborescence)
+            i_file_upload = self.__push_files(
+                list(self.__dataset.data_files.items()),
+                self.__upload.api_push_data_file,
+                self.__upload.api_delete_data_file,
+            )
 
-            for p_file_path, s_api_path in self.__dataset.data_files.items():
-                # Regarde si le fichier du dataset est déjà dans la liste des fichiers téléversés sur l'entrepôt
-                # NB: sur l'entrepôt, tous les fichiers "data" sont dans le dossier parent "data" TODO vérifier que c'est toujours le cas !
-                s_data_api_path = f"{s_api_path}/{p_file_path.name}"
-                Config().om.info(f"Livraison {self.__upload['name']} : livraison de {s_data_api_path}...")
-                if s_data_api_path in d_destination_taille:
-                    # le fichier est déjà livré, on check sa taille :
-                    if d_destination_taille[s_data_api_path] == p_file_path.stat().st_size:
-                        # le fichier a été complètement téléversé. On passe au fichier suivant.
-                        Config().om.info(f"Livraison {self.__upload['name']} : livraison de {s_data_api_path}: déjà livré")
-                        continue
-
-                    # le fichier n'a pas été téléversé en totalité.
-                    # Si le mode "Append" n'est pas disponible sur le serveur, il faut supprimer le fichier à moitié téléversé.
-                    # Sinon il faudra reprendre le téléversement (!)
-                    self.__upload.api_delete_data_file(s_data_api_path)
-
-                # sinon, on doit livrer le fichier
-                self.__upload.api_push_data_file(p_file_path, s_api_path)
-                Config().om.info(f"Livraison {self.__upload['name']} : livraison de {s_data_api_path}: terminé")
-            Config().om.info(f"Livraison {self.__upload}: les {len(self.__dataset.data_files)} fichiers de données ont été ajoutés avec succès.")
+            Config().om.info(f"Livraison {self.__upload}: les {len(self.__dataset.data_files)} fichiers de données ont été ajoutés avec succès. ({i_file_upload} livrer lors de ce traitement)")
 
     def __push_md5_files(self) -> None:
         """Téléverse les fichiers de clefs (listés dans le dataset)."""
         if self.__upload is not None:
-            # Liste les fichiers md5 téléversés sur l'entrepôt et récupère leur taille
-            l_arborescence = self.__upload.api_tree()
-            d_destination_taille = UploadAction.parse_tree(l_arborescence)
-
-            for p_file_path in self.__dataset.md5_files:
-                # Regarde si le fichier du dataset est déjà dans la liste des fichiers téléversés sur l'entrepôt
-                # NB: sur l'entrepot, tous les fichiers md5 sont à la racine
-                s_api_path = p_file_path.name
-                Config().om.info(f"Livraison {self.__upload['name']} : livraison de {s_api_path}...")
-                if s_api_path in d_destination_taille:
-                    # le fichier est déjà livré, on check sa taille :
-                    if d_destination_taille[s_api_path] == p_file_path.stat().st_size:
-                        # le fichier a été complètement téléversé. On passe au fichier suivant.
-                        Config().om.info(f"Livraison {self.__upload['name']} : livraison de {s_api_path}: déjà livré")
-                        continue
-
-                    # le fichier n'a pas été téléversé en totalité.
-                    # Si le mode "Append" n'est pas disponible sur le serveur, il faut supprimer le fichier à moitié téléversé.
-                    # Sinon il faudra reprendre le téléversement (!)
-                    self.__upload.api_delete_data_file(s_api_path)
-
-                # sinon, on doit livrer le fichier
-                self.__upload.api_push_md5_file(p_file_path)
-                Config().om.info(f"Livraison {self.__upload['name']} : livraison de {s_api_path}: terminé")
-            Config().om.info(f"Livraison {self.__upload}: les {len(self.__dataset.md5_files)} fichiers md5 ont été ajoutés avec succès.")
+            i_file_upload = self.__push_files(
+                [(p_file, "") for p_file in self.__dataset.md5_files],
+                self.__normalise_api_push_md5_file,
+                self.__upload.api_delete_md5_file,
+            )
+            Config().om.info(f"Livraison {self.__upload}: les {len(self.__dataset.md5_files)} fichiers md5 ont été ajoutés avec succès. ({i_file_upload} livrer lors de ce traitement)")
+
+    def __normalise_api_push_md5_file(self, path: Path, nom: str) -> None:
+        """fonction cachant api_push_md5_file pour avoir une fonction ayant les même entrées que api_push_data_file, utilisé comme paramétre de __push_files
+
+        Args:
+            path (Path): chemin le la chef MD5
+            nom (str): non du ficher md5
+        """
+        if self.__upload is None:
+            raise GpfSdkError(f"Aucune livraison de définie - impossible de livrer {nom}")
+        self.__upload.api_push_md5_file(path)
+
+    def __push_files(self, l_files: List[Tuple[Path, str]], f_api_push: Callable[[Path, str], None], f_api_delete: Callable[[str], None]) -> int:
+        """pousse un ficher de données ou un ficher md5 sur le store. Gére la reprise de Livraison et les conflicts lors de la livraison.
+
+        Args:
+            l_files (List[Tuple[Path, str]]): liste de tuple Path du ficher à livre, nom du ficher sous la gpf
+            f_api_push (Callable[[Path, str], None]): fonction pour livrer les données
+            f_api_delete (Callable[[str], None]): fonction pour supprimé les données si livrer partiellement.
+
+        Returns:
+            int: nombre de ficher réellement téléverser durant l'action
+        """
+        if self.__upload is None:
+            raise GpfSdkError("Aucune livraison de définie")
+        # Liste les fichiers téléversés sur l'entrepôt et récupère leur taille
+        l_arborescence = self.__upload.api_tree()
+        d_destination_taille = UploadAction.parse_tree(l_arborescence)
+        l_conflict = []
+        i_file_upload = 0
+        for p_file_path, s_api_path in l_files:
+            # Regarde si le fichier du dataset est déjà dans la liste des fichiers téléversés sur l'entrepôt
+            # NB: sur l'entrepot, tous les fichiers md5 sont à la racine
+            s_data_api_path = f"{s_api_path}/{p_file_path.name}" if s_api_path else p_file_path.name
+            Config().om.info(f"Livraison {self.__upload['name']} : livraison de {s_data_api_path}...")
+            if s_data_api_path in d_destination_taille:
+                # le fichier est déjà livré, on check sa taille :
+                if d_destination_taille[s_data_api_path] == p_file_path.stat().st_size:
+                    # le fichier a été complètement téléversé. On passe au fichier suivant.
+                    Config().om.info(f"Livraison {self.__upload['name']} : livraison de {s_data_api_path}: déjà livré")
+                    continue
+
+                # le fichier n'a pas été téléversé en totalité.
+                # Si le mode "Append" n'est pas disponible sur le serveur, il faut supprimer le fichier à moitié téléversé.
+                # Sinon il faudra reprendre le téléversement (!)
+                f_api_delete(s_data_api_path)
+
+            try:
+                # livraison du fichier
+                f_api_push(p_file_path, s_api_path)
+                i_file_upload += 1
+                Config().om.info(f"Livraison {self.__upload['name']} : livraison de {s_data_api_path}: terminé")
+            except requests.Timeout:
+                Config().om.warning(f"Livraison {self.__upload['name']} : livraison de {s_data_api_path}: timeout.")
+                l_conflict.append((p_file_path, s_data_api_path))
+            except ConflictError:
+                Config().om.warning(f"Livraison {self.__upload['name']} : livraison de {s_data_api_path}: conflict.")
+                l_conflict.append((p_file_path, s_data_api_path))
+        if l_conflict:
+            Config().om.info(f"Livraison {self.__upload}: {len(l_conflict)} fichiers en conflict, vérification de leur livraisons...")
+            l_error = self._check_file_uploaded(l_conflict)
+            if l_error:
+                raise UploadFileError(f"Livraison {self.__upload['name']} : Problème de livraison pour {len(l_error)} fichiers. Il faut relancer la livraison.", l_error)
+        return i_file_upload
+
+    def _check_file_uploaded(self, l_files: List[Tuple[Path, str]]) -> List[Tuple[Path, str]]:
+        if self.__upload is None:
+            raise GpfSdkError("Aucune livraison de définie")
+        # on recharge la l'arborescence
+        l_arborescence = self.__upload.api_tree()
+        d_destination_taille = UploadAction.parse_tree(l_arborescence)
+        l_error: List[Tuple[Path, str]] = []
+        # vérifications
+        for p_file_path, s_api_path in l_files:
+            s_data_api_path = f"{s_api_path}/{p_file_path.name}" if s_api_path else p_file_path.name
+            if s_data_api_path in d_destination_taille:
+                # le fichier est déjà livré, on check sa taille :
+                if d_destination_taille[s_data_api_path] == p_file_path.stat().st_size:
+                    # le fichier a été complètement téléversé. On passe au fichier suivant.
+                    Config().om.info(f"Livraison {self.__upload['name']} : livraison de {s_data_api_path}: déjà livré")
+                else:
+                    Config().om.error(f"Livraison {self.__upload['name']} : livraison de {s_data_api_path}: à re-livré, problème de taille")
+                    l_error.append((p_file_path, s_api_path))
+            else:
+                Config().om.error(f"Livraison {self.__upload['name']} : livraison de {s_data_api_path}: Non trouvé dans la liste des fichiers livrer")
+                l_error.append((p_file_path, s_api_path))
+        return l_error
 
     def __close(self) -> None:
         """Ferme la livraison."""
         if self.__upload is not None:
             Config().om.info(f"Livraison {self.__upload['name']} : fermeture de la livraison...")
             self.__upload.api_close()
             Config().om.info(f"Livraison {self.__upload['name']} : livraison fermée avec succès. La livraison va maintenant être vérifiée par la Géoplateforme.")
```

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/workflow/resolver/AbstractResolver.py` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/resolver/AbstractResolver.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,14 @@
-from abc import ABC, abstractmethod
 import re
+import json
+from abc import ABC, abstractmethod
 from typing import Any, Dict
 
+from sdk_entrepot_gpf.io.Config import Config
+
 
 class AbstractResolver(ABC):
     """Classe abstraite permettant de résoudre le paramétrage des fichiers d'action.
 
     Vous pouvez créer vos propres classe de résolution en les héritant de
     celle-ci et en les ajoutant au GlobalResolver.
 
@@ -30,28 +33,33 @@
         """
 
     @property
     def name(self) -> str:
         return self.__name
 
     @staticmethod
-    def get(key_value: Dict[str, Any], js_key: str) -> Any:
-        """fonction permettant de récupérer une valeur dans un dictionnaire complexe avec une récupération de style JS
+    def get(key_value: Dict[str, Any], js_key: str) -> str:
+        """fonction permettant de récupérer une valeur dans un dictionnaire complexe avec une récupération de style JS.
+        La valeur est convertie en str (json) si elle n'est pas de type str.
 
         Args:
             key_value (Dict[str, Any]): dictionnaire dont on veut récupérer l'info
             string (str): pattern type JS pour récupérer la valeur du dictionnaire
 
         Returns:
-            Any: valeur demandée
+            str: valeur demandée
         """
         o_val = key_value
         l_keys = js_key.split(".")
         # On itère selon les morceaux
         for s_key in l_keys:
-            # traitement du cas des array (cle[0], cle[1], cle[-1], ...)
-            o_match = re.search(r"(.*)\[(-?\d*)\]$", s_key)
-            if o_match:
-                o_val = o_val[o_match.group(1)][int(o_match.group(2))]
-            else:
-                o_val = o_val[s_key]
-        return o_val
+            try:
+                # traitement du cas des array (cle[0], cle[1], cle[-1], ...)
+                o_match = re.search(r"(.*)\[(-?\d*)\]$", s_key)
+                if o_match:
+                    o_val = o_val[o_match.group(1)][int(o_match.group(2))]
+                else:
+                    o_val = o_val[s_key]
+            except KeyError as e_error:
+                Config().om.error(f"Impossible de résoudre la clef '{js_key}' : sous-clef '{s_key}' non trouvée, clefs possibles à ce niveau : {', '.join(o_val.keys())}")
+                raise e_error
+        return o_val if isinstance(o_val, str) else json.dumps(o_val)
```

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/workflow/resolver/DateResolver.py` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/resolver/DateResolver.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/workflow/resolver/DumbResolver.py` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/resolver/DumbResolver.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/workflow/resolver/Errors.py` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/resolver/Errors.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/workflow/resolver/FileResolver.py` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/resolver/FileResolver.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,15 @@
 
         Returns:
             liste contenue dans le fichier
         """
         s_data = self.__resolve_str(string_to_solve, s_path)
         # on vérifie que cela est bien une liste
         try:
-            l_to_solve = json.loads(s_data)
+            l_to_solve = json.loads(s_data)  # json.loads ok car on veut récupérer l'erreur
         except json.decoder.JSONDecodeError as e_not_list:
             raise ResolveFileInvalidError(self.name, string_to_solve) from e_not_list
 
         if not isinstance(l_to_solve, list):
             raise ResolveFileInvalidError(self.name, string_to_solve)
 
         return s_data
@@ -121,15 +121,15 @@
 
         Returns:
             dictionnaire contenu dans le fichier
         """
         s_data = self.__resolve_str(string_to_solve, s_path)
         # on vérifie que cela est bien un dictionnaire
         try:
-            d_to_solve = json.loads(s_data)
+            d_to_solve = json.loads(s_data)  # json.loads ok car on veut récupérer l'erreur
         except json.decoder.JSONDecodeError as e_not_list:
             raise ResolveFileInvalidError(self.name, string_to_solve) from e_not_list
 
         if not isinstance(d_to_solve, dict):
             # le programme émet une erreur
             raise ResolveFileInvalidError(self.name, string_to_solve)
         return s_data
```

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/workflow/resolver/GlobalResolver.py` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/resolver/GlobalResolver.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/workflow/resolver/StoreEntityResolver.py` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/resolver/StoreEntityResolver.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/sdk_entrepot_gpf/workflow/resolver/UserResolver.py` & `sdk_entrepot_gpf-0.1.25/sdk_entrepot_gpf/workflow/resolver/UserResolver.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/tests/ErrorsTestCase.py` & `sdk_entrepot_gpf-0.1.25/tests/ErrorsTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/tests/GpfTestCase.py` & `sdk_entrepot_gpf-0.1.25/tests/GpfTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/tests/MainTestCase.py` & `sdk_entrepot_gpf-0.1.25/tests/MainTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.dbf` & `sdk_entrepot_gpf-0.1.25/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.dbf`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.shp` & `sdk_entrepot_gpf-0.1.25/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.shp`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.shx` & `sdk_entrepot_gpf-0.1.25/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.shx`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/tests/_data/datasets/2_test_dataset_bad_md5/upload_descriptor.json` & `sdk_entrepot_gpf-0.1.25/tests/_data/datasets/2_test_dataset_bad_md5/upload_descriptor.json`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.dbf` & `sdk_entrepot_gpf-0.1.25/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.dbf`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.shp` & `sdk_entrepot_gpf-0.1.25/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.shp`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.shx` & `sdk_entrepot_gpf-0.1.25/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.shx`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/tests/_data/datasets/3_test_dataset_sub_dir/upload_descriptor.json` & `sdk_entrepot_gpf-0.1.25/tests/_data/datasets/3_test_dataset_sub_dir/upload_descriptor.json`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/tests/_data/workflows/bad-workflow.jsonc` & `sdk_entrepot_gpf-0.1.25/tests/_data/workflows/bad-workflow.jsonc`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/tests/_test/helper/JsonHelper/schema.json` & `sdk_entrepot_gpf-0.1.25/tests/_test/helper/JsonHelper/schema.json`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/tests/auth/AuthentifierTestCase.py` & `sdk_entrepot_gpf-0.1.25/tests/auth/AuthentifierTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/tests/auth/TokenTestCase.py` & `sdk_entrepot_gpf-0.1.25/tests/auth/TokenTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/tests/helper/FileHelperTestCase.py` & `sdk_entrepot_gpf-0.1.25/tests/helper/FileHelperTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/tests/helper/JsonHelperTestCase.py` & `sdk_entrepot_gpf-0.1.25/tests/helper/JsonHelperTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/tests/io/ApiRequesterTestCase.py` & `sdk_entrepot_gpf-0.1.25/tests/io/ApiRequesterTestCase.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from http import HTTPStatus
 from io import BufferedReader
 import json
 from pathlib import Path
 from typing import Dict, Tuple
-from unittest.mock import patch, mock_open
+from unittest.mock import MagicMock, patch, mock_open
 import requests
 import requests_mock
 
 from sdk_entrepot_gpf.io.Config import Config
 from sdk_entrepot_gpf.Errors import GpfSdkError
 from sdk_entrepot_gpf.auth.Authentifier import Authentifier
 from sdk_entrepot_gpf.io.ApiRequester import ApiRequester
@@ -73,15 +73,53 @@
                 ApiRequester.POST,
                 params=self.param,
                 data=self.data,
                 files=self.files,
             )
             # Vérification sur o_mock_request
             s_url = "https://api.test.io/api/v1/datastores/TEST_DATASTORE/create/42"
-            o_mock_request.assert_called_once_with(s_url, ApiRequester.POST, self.param, self.data, self.files, {})
+            o_mock_request.assert_called_once_with(s_url, ApiRequester.POST, self.param, self.data, self.files, {}, -1000)
+            # Vérification sur la réponse renvoyée par la fonction : ça doit être celle renvoyée par url_request
+            self.assertEqual(o_fct_response, o_api_response)
+
+    def test_route_request_timeout(self) -> None:
+        """Test de route_request quand la route existe pour le timeout."""
+        # Instanciation d'une fausse réponse HTTP
+        o_api_response = GpfTestCase.get_response()
+        # timeout dans la requête
+        with patch.object(ApiRequester(), "url_request", return_value=o_api_response) as o_mock_request:
+            # On effectue une requête
+            o_fct_response = ApiRequester().route_request(
+                "test_timeout",
+                {"id": 42},
+                ApiRequester.POST,
+                params=self.param,
+                data=self.data,
+                files=self.files,
+                timeout=40,
+            )
+            # Vérification sur o_mock_request
+            s_url = "https://api.test.io/api/v1/datastores/TEST_DATASTORE/timeout/42"
+            o_mock_request.assert_called_once_with(s_url, ApiRequester.POST, self.param, self.data, self.files, {}, 40)
+            # Vérification sur la réponse renvoyée par la fonction : ça doit être celle renvoyée par url_request
+            self.assertEqual(o_fct_response, o_api_response)
+        # timeout pour la route
+        with patch.object(ApiRequester(), "url_request", return_value=o_api_response) as o_mock_request:
+            # On effectue une requête
+            o_fct_response = ApiRequester().route_request(
+                "test_timeout",
+                {"id": 42},
+                ApiRequester.POST,
+                params=self.param,
+                data=self.data,
+                files=self.files,
+            )
+            # Vérification sur o_mock_request
+            s_url = "https://api.test.io/api/v1/datastores/TEST_DATASTORE/timeout/42"
+            o_mock_request.assert_called_once_with(s_url, ApiRequester.POST, self.param, self.data, self.files, {}, 50)
             # Vérification sur la réponse renvoyée par la fonction : ça doit être celle renvoyée par url_request
             self.assertEqual(o_fct_response, o_api_response)
 
     def test_route_request_ok_datastore_params(self) -> None:
         """Test de route_request quand la route existe en surchargeant le datastore."""
         # Instanciation d'une fausse réponse HTTP
         o_api_response = GpfTestCase.get_response()
@@ -94,15 +132,15 @@
                 ApiRequester.POST,
                 params=self.param,
                 data=self.data,
                 files=self.files,
             )
             # Vérification sur o_mock_request
             s_url = "https://api.test.io/api/v1/datastores/OTHER_DATASTORE/create/42"
-            o_mock_request.assert_called_once_with(s_url, ApiRequester.POST, self.param, self.data, self.files, {})
+            o_mock_request.assert_called_once_with(s_url, ApiRequester.POST, self.param, self.data, self.files, {}, -1000)
             # Vérification sur la réponse renvoyée par la fonction : ça doit être celle renvoyée par url_request
             self.assertEqual(o_fct_response, o_api_response)
 
     def test_route_request_ko(self) -> None:
         """Test de route_request quand la route n'existe pas."""
         # On veut vérifier que l'exception RouteNotFoundError est levée avec le bon nom de route non trouvée
         with self.assertRaises(RouteNotFoundError) as o_arc:
@@ -128,14 +166,16 @@
             # Requête 1 : vérification de l'url
             self.assertEqual(o_history[0].url, self.url + self.encoded_param, "check url")
             # Requête 1 : vérification du type
             self.assertEqual(o_history[0].method.lower(), "get", "method == get")
             # Requête 1 : vérification du corps de requête
             s_text = json.dumps(self.data)
             self.assertEqual(o_history[0].text, s_text, "check text")
+            # Requête 1 : timeout valeur par défaut
+            self.assertEqual(o_history[0].timeout, 600)
 
     def test_url_request_post(self) -> None:
         """Test de url_request dans le cadre d'une requête post."""
         # On mock...
         with requests_mock.Mocker() as o_mock:
             # Une requête réussie
             o_mock.post(self.url, json=self.response)
@@ -150,14 +190,61 @@
             # Requête 1 : vérification de l'url
             self.assertEqual(o_history[0].url, self.url + self.encoded_param, "check url")
             # Requête 1 : vérification du type
             self.assertEqual(o_history[0].method.lower(), "post", "method == post")
             # Requête 1 : vérification du corps de requête
             s_text = json.dumps(self.data)
             self.assertEqual(o_history[0].text, s_text, "check text")
+            # Requête 1 : timeout valeur par défaut
+            self.assertEqual(o_history[0].timeout, 600, "timeout")
+
+    def test_url_request_timeout_param(self) -> None:
+        """Test de url_request pour les timeout."""
+        # Timeout None
+        with requests_mock.Mocker() as o_mock:
+            # Une requête réussie
+            o_mock.post(self.url, json=self.response)
+            # On effectue une requête
+            o_response = ApiRequester().url_request(self.url, ApiRequester.POST, params=self.param, data=self.data, timeout=None)
+            # Vérification sur la réponse
+            self.assertDictEqual(o_response.json(), self.response)
+            # On a dû faire une requête
+            self.assertEqual(o_mock.call_count, 1, "o_mock.call_count == 1")
+            # Vérifications sur l'historique (enfin ici y'a une requête...)
+            o_history = o_mock.request_history
+            # Requête 1 : vérification de l'url
+            self.assertEqual(o_history[0].url, self.url + self.encoded_param, "check url")
+            # Requête 1 : vérification du type
+            self.assertEqual(o_history[0].method.lower(), "post", "method == post")
+            # Requête 1 : vérification du corps de requête
+            s_text = json.dumps(self.data)
+            self.assertEqual(o_history[0].text, s_text, "check text")
+            # Requête 1 : timeout
+            self.assertEqual(o_history[0].timeout, None)
+        # Timeout 10s
+        with requests_mock.Mocker() as o_mock:
+            # Une requête réussie
+            o_mock.post(self.url, json=self.response)
+            # On effectue une requête
+            o_response = ApiRequester().url_request(self.url, ApiRequester.POST, params=self.param, data=self.data, timeout=10)
+            # Vérification sur la réponse
+            self.assertDictEqual(o_response.json(), self.response)
+            # On a dû faire une requête
+            self.assertEqual(o_mock.call_count, 1, "o_mock.call_count == 1")
+            # Vérifications sur l'historique (enfin ici y'a une requête...)
+            o_history = o_mock.request_history
+            # Requête 1 : vérification de l'url
+            self.assertEqual(o_history[0].url, self.url + self.encoded_param, "check url")
+            # Requête 1 : vérification du type
+            self.assertEqual(o_history[0].method.lower(), "post", "method == post")
+            # Requête 1 : vérification du corps de requête
+            s_text = json.dumps(self.data)
+            self.assertEqual(o_history[0].text, s_text, "check text")
+            # Requête 1 : timeout
+            self.assertEqual(o_history[0].timeout, 10)
 
     def test_url_request_internal_server_error(self) -> None:
         """Test de url_request dans le cadre de 3 erreurs internes de suite."""
         # On mock...
         with requests_mock.Mocker() as o_mock:
             # Une requête non réussie
             o_mock.post(
@@ -288,21 +375,58 @@
         # Content-Range non parsable : on doit s'arrêter
         self.assertFalse(ApiRequester.range_next_page("non_parsable", 0))
 
     def test_route_upload_file(self) -> None:
         """test de route_upload_file"""
         p_file = Path("rep/file")
         s_path_api = "key"
-        s_route_name = "route_mane"
+        s_route_name = "route_name"
         d_route_params = None
         s_method = "POST"
         d_params = None
         d_data = None
 
         o_open = mock_open()
         o_tuple_file = (p_file.name, o_open.return_value)
         o_dict_files = {s_path_api: o_tuple_file}
+        o_mock_stat = MagicMock()
+        o_mock_stat.st_size = 10
+        # pas de timeout
+        with patch.object(Path, "open", return_value=o_open.return_value) as o_mock_open:
+            with patch.object(Path, "stat", return_value=o_mock_stat):
+                with patch.object(ApiRequester, "route_request", return_value=None) as o_mock_request:
+                    ApiRequester().route_upload_file(s_route_name, p_file, s_path_api, d_route_params, s_method, d_params, d_data)
+                    o_mock_open.assert_called_once_with("rb")
+                    o_mock_request.assert_called_once_with(s_route_name, route_params=d_route_params, method=s_method, params=d_params, data=d_data, files=o_dict_files, timeout=-1000)
+        o_mock_stat.reset_mock()
+
+        # timeout None
+        for s_route_name in ["test_upload_none_1", "test_upload_none_2", "test_upload_none_3"]:
+            with patch.object(Path, "open", return_value=o_open.return_value) as o_mock_open:
+                with patch.object(Path, "stat", return_value=o_mock_stat):
+                    with patch.object(ApiRequester, "route_request", return_value=None) as o_mock_request:
+                        ApiRequester().route_upload_file(s_route_name, p_file, s_path_api, d_route_params, s_method, d_params, d_data)
+                        o_mock_open.assert_called_once_with("rb")
+                        o_mock_request.assert_called_once_with(s_route_name, route_params=d_route_params, method=s_method, params=d_params, data=d_data, files=o_dict_files, timeout=None)
+            o_mock_stat.reset_mock()
+
+        # timeout fixe
+        s_route_name = "test_upload_fixe"
         with patch.object(Path, "open", return_value=o_open.return_value) as o_mock_open:
-            with patch.object(ApiRequester, "route_request", return_value=None) as o_mock_request:
-                ApiRequester().route_upload_file(s_route_name, p_file, s_path_api, d_route_params, s_method, d_params, d_data)
-                o_mock_open.assert_called_once_with("rb")
-                o_mock_request.assert_called_once_with(s_route_name, route_params=d_route_params, method=s_method, params=d_params, data=d_data, files=o_dict_files)
+            with patch.object(Path, "stat", return_value=o_mock_stat):
+                with patch.object(ApiRequester, "route_request", return_value=None) as o_mock_request:
+                    ApiRequester().route_upload_file(s_route_name, p_file, s_path_api, d_route_params, s_method, d_params, d_data)
+                    o_mock_open.assert_called_once_with("rb")
+                    o_mock_request.assert_called_once_with(s_route_name, route_params=d_route_params, method=s_method, params=d_params, data=d_data, files=o_dict_files, timeout=60)
+        o_mock_stat.reset_mock()
+
+        # timeout selon taille du fichier
+        s_route_name = "test_upload_variable"
+        for i_taille_ficher, i_timeout in [(1, -1000), (15, 15), (16, 15), (35, 30), (65, None), (70, 70), (700000, 70)]:
+            o_mock_stat.st_size = i_taille_ficher
+            with patch.object(Path, "open", return_value=o_open.return_value) as o_mock_open:
+                with patch.object(Path, "stat", return_value=o_mock_stat):
+                    with patch.object(ApiRequester, "route_request", return_value=None) as o_mock_request:
+                        ApiRequester().route_upload_file(s_route_name, p_file, s_path_api, d_route_params, s_method, d_params, d_data)
+                        o_mock_open.assert_called_once_with("rb")
+                        o_mock_request.assert_called_once_with(s_route_name, route_params=d_route_params, method=s_method, params=d_params, data=d_data, files=o_dict_files, timeout=i_timeout)
+            o_mock_stat.reset_mock()
```

### Comparing `sdk_entrepot_gpf-0.1.24/tests/io/ConfigTestCase.py` & `sdk_entrepot_gpf-0.1.25/tests/io/ConfigTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/tests/io/DatasetTestCase.py` & `sdk_entrepot_gpf-0.1.25/tests/io/DatasetTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/tests/io/ErrorsTestCase.py` & `sdk_entrepot_gpf-0.1.25/tests/io/ErrorsTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/tests/io/JsonConverterTestCase.py` & `sdk_entrepot_gpf-0.1.25/tests/io/JsonConverterTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/tests/io/UploadDescriptorFileReaderTestCase.py` & `sdk_entrepot_gpf-0.1.25/tests/io/UploadDescriptorFileReaderTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/tests/store/AbstractCommonFileTestCase.py` & `sdk_entrepot_gpf-0.1.25/tests/store/AbstractCommonFileTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/tests/store/AnnexeTestCase.py` & `sdk_entrepot_gpf-0.1.25/tests/store/AnnexeTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/tests/store/CheckExecutionTestCase.py` & `sdk_entrepot_gpf-0.1.25/tests/store/CheckExecutionTestCase.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Any, Dict, List
 from unittest.mock import patch
 
 from sdk_entrepot_gpf.io.ApiRequester import ApiRequester
 from sdk_entrepot_gpf.store.CheckExecution import CheckExecution
 from tests.GpfTestCase import GpfTestCase
 
 
@@ -10,23 +11,23 @@
 
     cmd : python3 -m unittest -b tests.store.CheckExecutionTestCase
     """
 
     def test_api_logs(self) -> None:
         "Vérifie le bon fonctionnement de api_logs."
         s_data = "2022/05/18 14:29:25       INFO §USER§ Envoi du signal de début de l'exécution à l'API.\n2022/05/18 14:29:25       INFO §USER§ Signal transmis avec succès."
-        l_rep = [
-            {"datastore": "datastore_id", "data": s_data, "rep": s_data},
+        l_rep: List[Dict[str, Any]] = [
+            {"datastore": "datastore_id", "data": s_data.split("\n"), "rep": s_data},
             {"datastore": "datastore_id", "data": "", "rep": ""},
-            {"datastore": "datastore_id", "data": "[]", "rep": ""},
-            {"datastore": "datastore_id", "data": '["log1", "log2", " log \\"complexe\\""]', "rep": 'log1\nlog2\n log "complexe"'},
+            {"datastore": "datastore_id", "data": [], "rep": ""},
+            {"datastore": "datastore_id", "data": ["log1", "log2", ' log "complexe"'], "rep": 'log1\nlog2\n log "complexe"'},
         ]
 
         for d_rep in l_rep:
-            o_response = GpfTestCase.get_response(text=d_rep["data"])
+            o_response = GpfTestCase.get_response(json=d_rep["data"])
             # On mock la fonction route_request, on veut vérifier qu'elle est appelée avec les bons params
             with patch.object(ApiRequester, "route_request", return_value=o_response) as o_mock_request:
                 # on appelle la fonction à tester : api_logs
                 o_check_execution = CheckExecution({"_id": "id_entité"}, datastore=d_rep["datastore"])
                 s_data_recupere = o_check_execution.api_logs()
                 # on vérifie que route_request est appelé correctement
                 o_mock_request.assert_called_once_with(
```

### Comparing `sdk_entrepot_gpf-0.1.24/tests/store/ConfigurationTestCase.py` & `sdk_entrepot_gpf-0.1.25/tests/store/ConfigurationTestCase.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,21 +49,21 @@
         """
 
         d_data_offering = {"_id": "11111111"}
 
         # On mock la fonction api_create, on veut vérifier qu'elle est appelée avec les bons param
         with patch.object(StoreEntity, "api_create", return_value=Offering(d_data_offering)) as o_mock_create:
             # Instanciation d'une Configuration
-            o_configuration = Configuration({"_id": "2222222"})
+            o_configuration = Configuration({"_id": "2222222"}, datastore="datastore")
             # Ajout d'une Offre
             o_offering = o_configuration.api_add_offering(d_data_offering)
             # on vérifie que api_create est appelé correctement
             o_mock_create.assert_called_once_with(
                 d_data_offering,
-                route_params={"configuration": "2222222"},
+                route_params={"configuration": "2222222", "datastore": "datastore"},
             )
             # on vérifie que l'entité renvoyée est cohérente
             self.assertIsInstance(o_offering, Offering)
             self.assertEqual(o_offering.id, "11111111")
             self.assertDictEqual(o_offering.get_store_properties(), d_data_offering)
 
     def test_delete_cascade(self) -> None:
```

### Comparing `sdk_entrepot_gpf-0.1.24/tests/store/DatastoreTestCase.py` & `sdk_entrepot_gpf-0.1.25/tests/store/DatastoreTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/tests/store/EndpointTestCase.py` & `sdk_entrepot_gpf-0.1.25/tests/store/EndpointTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/tests/store/ErrorsTestCase.py` & `sdk_entrepot_gpf-0.1.25/tests/store/ErrorsTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/tests/store/MetadataTestCase.py` & `sdk_entrepot_gpf-0.1.25/tests/store/MetadataTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/tests/store/OfferingTestCase.py` & `sdk_entrepot_gpf-0.1.25/tests/store/OfferingTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/tests/store/ProcessingExecutionTestCase.py` & `sdk_entrepot_gpf-0.1.25/tests/store/ProcessingExecutionTestCase.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,23 +13,23 @@
     cmd : python3 -m unittest -b tests.store.ProcessingExecutionTestCase
     """
 
     def test_api_logs(self) -> None:
         """Vérifie le bon fonctionnement de api_logs."""
         s_data = "2022/05/18 14:29:25       INFO §USER§ Envoi du signal de début de l'exécution à l'API.\n2022/05/18 14:29:25       INFO §USER§ Signal transmis avec succès."
         l_rep: List[Dict[str, Any]] = [
-            {"data": s_data, "rep": s_data, "datastore": None},
+            {"data": s_data.split("\n"), "rep": s_data, "datastore": None},
             {"data": "", "rep": "", "datastore": "datastore"},
-            {"data": "[]", "rep": "", "datastore": None},
-            {"data": '["log1", "log2", " log \\"complexe\\""]', "rep": 'log1\nlog2\n log "complexe"', "datastore": "datastore"},
+            {"data": [], "rep": "", "datastore": None},
+            {"data": ["log1", "log2", ' log "complexe"'], "rep": 'log1\nlog2\n log "complexe"', "datastore": "datastore"},
         ]
 
         for d_rep in l_rep:
             # Instanciation d'une fausse réponse HTTP
-            o_response = GpfTestCase.get_response(text=d_rep["data"])
+            o_response = GpfTestCase.get_response(json=d_rep["data"])
             # On mock la fonction route_request, on veut vérifier qu'elle est appelée avec les bons params
             with patch.object(ApiRequester, "route_request", return_value=o_response) as o_mock_request:
                 # on appelle la fonction à tester : api_logs
                 o_processing_execution = ProcessingExecution({"_id": "id_entité"}, d_rep["datastore"])
                 s_data_recupere = o_processing_execution.api_logs()
 
                 # on vérifie que route_request est appelé correctement
```

### Comparing `sdk_entrepot_gpf-0.1.24/tests/store/StoreEntityTestCase.py` & `sdk_entrepot_gpf-0.1.25/tests/store/StoreEntityTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/tests/store/StoredDataTestCase.py` & `sdk_entrepot_gpf-0.1.25/tests/store/StoredDataTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/tests/store/UploadTestCase.py` & `sdk_entrepot_gpf-0.1.25/tests/store/UploadTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/tests/store/interface/CommentInterfaceTestCase.py` & `sdk_entrepot_gpf-0.1.25/tests/store/interface/CommentInterfaceTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/tests/store/interface/CreatedByUploadFileInterfaceTestCase.py` & `sdk_entrepot_gpf-0.1.25/tests/store/interface/CreatedByUploadFileInterfaceTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/tests/store/interface/CsfInterfaceTestCase.py` & `sdk_entrepot_gpf-0.1.25/tests/store/interface/CsfInterfaceTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/tests/store/interface/DownloadInterfaceTestCase.py` & `sdk_entrepot_gpf-0.1.25/tests/store/interface/DownloadInterfaceTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/tests/store/interface/EventInterfaceTestCase.py` & `sdk_entrepot_gpf-0.1.25/tests/store/interface/EventInterfaceTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/tests/store/interface/FullEditInterfaceTestCase.py` & `sdk_entrepot_gpf-0.1.25/tests/store/interface/FullEditInterfaceTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/tests/store/interface/PartialEditInterfaceTestCase.py` & `sdk_entrepot_gpf-0.1.25/tests/store/interface/PartialEditInterfaceTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/tests/store/interface/ReUploadFileInterfaceTestCase.py` & `sdk_entrepot_gpf-0.1.25/tests/store/interface/ReUploadFileInterfaceTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/tests/store/interface/SharingInterfaceTestCase.py` & `sdk_entrepot_gpf-0.1.25/tests/store/interface/SharingInterfaceTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/tests/store/interface/TagInterfaceTestCase.py` & `sdk_entrepot_gpf-0.1.25/tests/store/interface/TagInterfaceTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/tests/workflow/WorkflowTestCase.py` & `sdk_entrepot_gpf-0.1.25/tests/workflow/WorkflowTestCase.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from sdk_entrepot_gpf.workflow.Errors import WorkflowError
 from sdk_entrepot_gpf.workflow.Workflow import Workflow
 from sdk_entrepot_gpf.workflow.action.ActionAbstract import ActionAbstract
 from sdk_entrepot_gpf.workflow.action.ConfigurationAction import ConfigurationAction
 from sdk_entrepot_gpf.workflow.action.CopyConfigurationAction import CopyConfigurationAction
 from sdk_entrepot_gpf.workflow.action.DeleteAction import DeleteAction
 from sdk_entrepot_gpf.workflow.action.EditAction import EditAction
+from sdk_entrepot_gpf.workflow.action.EditUsedDataConfigurationAction import EditUsedDataConfigurationAction
 from sdk_entrepot_gpf.workflow.action.OfferingAction import OfferingAction
 from sdk_entrepot_gpf.workflow.action.PermissionAction import PermissionAction
 from sdk_entrepot_gpf.workflow.action.ProcessingExecutionAction import ProcessingExecutionAction
 from sdk_entrepot_gpf.workflow.action.SynchronizeOfferingAction import SynchronizeOfferingAction
 from sdk_entrepot_gpf.workflow.resolver.GlobalResolver import GlobalResolver
 
 from tests.GpfTestCase import GpfTestCase
@@ -86,19 +87,19 @@
         if "iter_vals" in d_etape and "iter_key" in d_etape:
             # on itère sur les clefs
             s_actions = str(json.dumps(l_actions, ensure_ascii=False))
             l_actions = []
             if isinstance(d_etape["iter_vals"][0], (str, float, int)):
                 # si la liste est une liste de string, un int ou flat : on remplace directement
                 for s_val in d_etape["iter_vals"]:
-                    l_actions += json.loads(s_actions.replace("{" + d_etape["iter_key"] + "}", s_val))
+                    l_actions += json.loads(s_actions.replace("{" + d_etape["iter_key"] + "}", s_val))  # json.loads ok car on est dans des tests
             else:
                 # on a une liste de sous dict ou apparenté on utilise un résolveur
                 for i, s_val in enumerate(d_etape["iter_vals"]):
-                    l_actions += json.loads(s_actions.replace(d_etape["iter_key"], f"iter_resolve_{i}"))
+                    l_actions += json.loads(s_actions.replace(d_etape["iter_key"], f"iter_resolve_{i}"))  # json.loads ok car on est dans des tests
         return l_actions
 
     def run_run_step(
         self,
         d_args_run_step: Dict[str, Any],
         d_workflow: Dict[str, Any],
         l_run_args: List[Any],
@@ -369,14 +370,15 @@
         # fmt: off
         with patch.object(DeleteAction, "__init__", wraps=new_init) as d_mock["DeleteAction"], \
         patch.object(ProcessingExecutionAction, "__init__", wraps=new_init) as d_mock["ProcessingExecutionAction"], \
         patch.object(ConfigurationAction, "__init__", wraps=new_init) as d_mock["ConfigurationAction"], \
         patch.object(OfferingAction, "__init__", wraps=new_init) as d_mock["OfferingAction"], \
         patch.object(SynchronizeOfferingAction, "__init__", wraps=new_init) as d_mock["SynchronizeOfferingAction"], \
         patch.object(CopyConfigurationAction, "__init__", wraps=new_init) as d_mock["CopyConfigurationAction"], \
+        patch.object(EditUsedDataConfigurationAction, "__init__", wraps=new_init) as d_mock["EditUsedDataConfigurationAction"], \
         patch.object(EditAction, "__init__", wraps=new_init) as d_mock["EditAction"]:
             # fmt: on
             # exécution
             o_action_generated = Workflow.generate(name, dico_def, parent, behavior=behavior)
             # tests
             self.assertIsInstance(o_action_generated, expected_type)
             for s_class_name, o_mock in d_mock.items():
@@ -410,14 +412,16 @@
         self.run_generation(SynchronizeOfferingAction, "name", {"type": "synchronize-offering"}, o_mock_parent, with_beavior=False)
         # test type copie-configuration
         self.run_generation(CopyConfigurationAction, "name", {"type": "copy-configuration"}, o_mock_parent, with_beavior=True)
         # test type edit-entity
         self.run_generation(EditAction, "name", {"type": "edit-entity"}, o_mock_parent, with_beavior=False)
         # test type permission
         self.run_generation(PermissionAction, "name", {"type": "permission"}, o_mock_parent, with_beavior=False)
+        # test type used_data-configuration
+        self.run_generation(EditUsedDataConfigurationAction, "name", {"type": "used_data-configuration"}, o_mock_parent, with_beavior=False)
 
     def test_open_workflow(self) -> None:
         """Test de la fonction open_workflow."""
         p_workflows = Config().data_dir_path / "workflows"
         # On teste le workflow generic_archive.jsonc
         o_workflow_1 = Workflow.open_workflow(p_workflows / "generic_archive.jsonc")
         self.assertEqual(o_workflow_1.name, "generic_archive.jsonc")
```

### Comparing `sdk_entrepot_gpf-0.1.24/tests/workflow/action/ActionAbstractTestCase.py` & `sdk_entrepot_gpf-0.1.25/tests/workflow/action/ActionAbstractTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/tests/workflow/action/ConfigurationActionTestCase.py` & `sdk_entrepot_gpf-0.1.25/tests/workflow/action/ConfigurationActionTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/tests/workflow/action/CopyConfigurationActionTestCase.py` & `sdk_entrepot_gpf-0.1.25/tests/workflow/action/CopyConfigurationActionTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/tests/workflow/action/DeleteActionTestCase.py` & `sdk_entrepot_gpf-0.1.25/tests/workflow/action/DeleteActionTestCase.py`

 * *Files 11% similar despite different names*

```diff
@@ -48,53 +48,53 @@
             o_action_delete.run()
         self.assertEqual('Il faut au moins une des clefs suivantes : "entity_id", "filter_infos", "filter_tags" pour cette action.', o_err.exception.message)
 
         s_entity_id = "entity_id"
         for c_classe in [Upload, StoredData, Configuration, Offering]:
             print(c_classe.entity_name())
             # rien trouvé avec les filtres
-            d_action = {"type": "delete-entity", "entity_type": c_classe.entity_name(), "filter_infos": {}}
+            d_action = {"type": "delete-entity", "entity_type": c_classe.entity_name(), "filter_infos": {"nom": "name"}, "filter_tags": {"tag1": "val1"}}
             o_action_delete = DeleteAction("contexte", d_action)
             with patch.object(c_classe, "api_list", return_value=[]) as o_mock_api_list:
                 with self.assertRaises(StepActionError) as o_err:
                     o_action_delete.run(s_datastore)
             self.assertEqual("Aucune entité trouvée pour la suppression", o_err.exception.message)
-            o_mock_api_list.assert_called_once_with(d_action.get("filter_infos"), d_action.get("filter_infos"), datastore=s_datastore)
+            o_mock_api_list.assert_called_once_with(d_action.get("filter_infos"), d_action.get("filter_tags"), datastore=s_datastore)
 
             # rien trouvé avec "entity_id"
             d_action = {"type": "delete-entity", "entity_type": c_classe.entity_name(), "entity_id": s_entity_id}
             o_action_delete = DeleteAction("contexte", d_action)
             with patch.object(c_classe, "api_get", side_effect=NotFoundError("", "", None, None, "")) as o_mock_api_list:
                 with self.assertRaises(StepActionError) as o_err:
                     o_action_delete.run(s_datastore)
             self.assertEqual("Aucune entité trouvée pour la suppression", o_err.exception.message)
             o_mock_api_list.assert_called_once_with(s_entity_id, datastore=s_datastore)
 
-        d_action = {"type": "delete-entity", "entity_type": "offering", "filter_infos": {}, "if_multi": "error"}
+        d_action = {"type": "delete-entity", "entity_type": "offering", "filter_infos": {"nom": "name"}, "filter_tags": {"tag1": "val1"}, "if_multi": "error"}
         o_action_delete = DeleteAction("contexte", d_action)
         l_entities = [MagicMock(), MagicMock(), MagicMock()]
         with patch.object(Offering, "api_list", return_value=l_entities) as o_mock_api_list:
             with self.assertRaises(StepActionError) as o_err:
                 o_action_delete.run(s_datastore)
         self.assertEqual(f"Plusieurs entités trouvées pour la suppression : {l_entities}", o_err.exception.message)
-        o_mock_api_list.assert_called_once_with(d_action.get("filter_infos"), d_action.get("filter_infos"), datastore=s_datastore)
+        o_mock_api_list.assert_called_once_with(d_action.get("filter_infos"), d_action.get("filter_tags"), datastore=s_datastore)
 
     def test_run_ok(self) -> None:  # pylint: disable=too-many-locals,too-many-statements
         """test pour la fonction run() sortie sans erreur"""
         s_datastore = "datastore"
         s_entity_id = "entity_id"
         for c_classe in [Upload, StoredData, Configuration, Offering]:
             # Aucune entité mais c'est OK
-            d_action = {"type": "delete-entity", "entity_type": c_classe.entity_name(), "filter_infos": {}, "if_multi": "error", "not_found_ok": True}
+            d_action = {"type": "delete-entity", "entity_type": c_classe.entity_name(), "filter_infos": {"nom": "name"}, "filter_tags": {"tag1": "val1"}, "if_multi": "error", "not_found_ok": True}
             o_action_delete = DeleteAction("contexte", d_action)
             with patch.object(c_classe, "api_list", return_value=[]) as o_mock_api_list:
                 with patch.object(StoreEntity, "delete_liste_entities", return_value=[]) as o_mock_delete:
                     o_action_delete.run(s_datastore)
-            o_mock_api_list.assert_called_once_with(d_action.get("filter_infos"), d_action.get("filter_infos"), datastore=s_datastore)
-            o_mock_delete.assert_called_once_with([], DeleteAction.question_before_delete)
+            o_mock_api_list.assert_called_once_with(d_action.get("filter_infos"), d_action.get("filter_tags"), datastore=s_datastore)
+            o_mock_delete.assert_not_called()
 
             # suppression avec entity_id
             o_entity = MagicMock()
             d_action = {"type": "delete-entity", "entity_type": c_classe.entity_name(), "entity_id": s_entity_id}
             o_action_delete = DeleteAction("contexte", d_action)
             with patch.object(c_classe, "api_get", return_value=o_entity) as o_mock_api_list:
                 with patch.object(StoreEntity, "delete_liste_entities", return_value=[]) as o_mock_delete:
@@ -115,50 +115,50 @@
             o_mock_api_list.assert_called_once_with(s_entity_id, datastore=s_datastore)
             o_mock_delete.assert_called_once_with(l_cascade, DeleteAction.question_before_delete)
             o_entity.get_liste_deletable_cascade.assert_called_once_with()
 
             # suppression avec les filtres
             o_entity_1 = MagicMock()
             o_entity_2 = MagicMock()
-            d_action = {"type": "delete-entity", "entity_type": c_classe.entity_name(), "filter_infos": {}}
+            d_action = {"type": "delete-entity", "entity_type": c_classe.entity_name(), "filter_infos": {"nom": "name"}, "filter_tags": {"tag1": "val1"}}
             o_action_delete = DeleteAction("contexte", d_action)
             with patch.object(c_classe, "api_list", return_value=[o_entity_1, o_entity_2]) as o_mock_api_list:
                 with patch.object(StoreEntity, "delete_liste_entities", return_value=[]) as o_mock_delete:
                     o_action_delete.run(s_datastore)
             o_mock_delete.assert_called_once_with([o_entity_1, o_entity_2], DeleteAction.question_before_delete)
-            o_mock_api_list.assert_called_once_with(d_action.get("filter_infos"), d_action.get("filter_infos"), datastore=s_datastore)
+            o_mock_api_list.assert_called_once_with(d_action.get("filter_infos"), d_action.get("filter_tags"), datastore=s_datastore)
             o_entity_1.get_liste_deletable_cascade.assert_not_called()
             o_entity_2.get_liste_deletable_cascade.assert_not_called()
 
             # suppression avec les filtres cascade
             o_entity_1 = MagicMock()
             l_cascade = [MagicMock(), MagicMock()]
             o_entity_1.get_liste_deletable_cascade.return_value = l_cascade
             o_entity_2 = MagicMock()
             o_entity_2.get_liste_deletable_cascade.return_value = l_cascade
-            d_action = {"type": "delete-entity", "entity_type": c_classe.entity_name(), "filter_infos": {}, "cascade": True}
+            d_action = {"type": "delete-entity", "entity_type": c_classe.entity_name(), "filter_infos": {"nom": "name"}, "filter_tags": {"tag1": "val1"}, "cascade": True}
             o_action_delete = DeleteAction("contexte", d_action)
             with patch.object(c_classe, "api_list", return_value=[o_entity_1, o_entity_2]) as o_mock_api_list:
                 with patch.object(StoreEntity, "delete_liste_entities", return_value=[]) as o_mock_delete:
                     o_action_delete.run(s_datastore)
             o_mock_delete.assert_called_once_with(l_cascade * 2, DeleteAction.question_before_delete)
-            o_mock_api_list.assert_called_once_with(d_action.get("filter_infos"), d_action.get("filter_infos"), datastore=s_datastore)
+            o_mock_api_list.assert_called_once_with(d_action.get("filter_infos"), d_action.get("filter_tags"), datastore=s_datastore)
             o_entity_1.get_liste_deletable_cascade.assert_called_once_with()
             o_entity_2.get_liste_deletable_cascade.assert_called_once_with()
 
             # suppression avec les filtres avec "if_multi": "first"
             o_entity_1 = MagicMock()
             o_entity_2 = MagicMock()
-            d_action = {"type": "delete-entity", "entity_type": c_classe.entity_name(), "filter_infos": {}, "if_multi": "first"}
+            d_action = {"type": "delete-entity", "entity_type": c_classe.entity_name(), "filter_infos": {"nom": "name"}, "filter_tags": {"tag1": "val1"}, "if_multi": "first"}
             o_action_delete = DeleteAction("contexte", d_action)
             with patch.object(c_classe, "api_list", return_value=[o_entity_1, o_entity_2]) as o_mock_api_list:
                 with patch.object(StoreEntity, "delete_liste_entities", return_value=[]) as o_mock_delete:
                     o_action_delete.run(s_datastore)
             o_mock_delete.assert_called_once_with([o_entity_1], DeleteAction.question_before_delete)
-            o_mock_api_list.assert_called_once_with(d_action.get("filter_infos"), d_action.get("filter_infos"), datastore=s_datastore)
+            o_mock_api_list.assert_called_once_with(d_action.get("filter_infos"), d_action.get("filter_tags"), datastore=s_datastore)
             o_entity_1.get_liste_deletable_cascade.assert_not_called()
             o_entity_2.get_liste_deletable_cascade.assert_not_called()
 
             # suppression avec entity_id
             o_entity = MagicMock()
             d_action = {"type": "delete-entity", "entity_type": c_classe.entity_name(), "entity_id": s_entity_id, "confirm": False}
             o_action_delete = DeleteAction("contexte", d_action)
```

### Comparing `sdk_entrepot_gpf-0.1.24/tests/workflow/action/EditActionTestCase.py` & `sdk_entrepot_gpf-0.1.25/tests/workflow/action/EditActionTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/tests/workflow/action/OfferingActionTestCase.py` & `sdk_entrepot_gpf-0.1.25/tests/workflow/action/OfferingActionTestCase.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import time
 from unittest.mock import patch, MagicMock
-from typing import Any, Optional
+from typing import Any, Dict, Optional
 from sdk_entrepot_gpf.Errors import GpfSdkError
 from sdk_entrepot_gpf.io.Errors import ConflictError
 
 from sdk_entrepot_gpf.store.Offering import Offering
 from sdk_entrepot_gpf.store.Configuration import Configuration
 from sdk_entrepot_gpf.workflow.Errors import StepActionError
 from sdk_entrepot_gpf.workflow.action.OfferingAction import OfferingAction
@@ -15,15 +15,15 @@
 class OfferingActionTestCase(GpfTestCase):
     """Tests OfferingAction class.
 
     cmd : python3 -m unittest -b tests.workflow.action.OfferingActionTestCase
     """
 
     # creation du dictionnaire qui reprend les paramètres du workflow pour créer une offre
-    d_action = {"type": "offering", "body_parameters": {"endpoint": "id_endpoint"}, "url_parameters": {"configuration": "id_configuration"}}
+    d_action: Dict[str, Any] = {"type": "offering", "body_parameters": {"endpoint": "id_endpoint"}, "url_parameters": {"configuration": "id_configuration"}}
 
     def __get_offering_action(self, behavior: Optional[str] = None) -> OfferingAction:
         # Instanciation de OfferingAction
         o_offering_action = OfferingAction("contexte", self.d_action, behavior=behavior)
         # Retour
         return o_offering_action
 
@@ -36,21 +36,21 @@
         o_mock_offering = MagicMock()
         o_mock_offering.__getitem__.return_value = Offering.STATUS_PUBLISHED
 
         # On mock find_offering et api_create
         with patch.object(o_offering_action, "find_offering", return_value=None) as o_mock_offering_action_list_offering:
             with patch.object(Offering, "api_create", return_value=o_mock_offering) as o_mock_offering_api_create:
                 # on lance l'exécution de run
-                o_offering_action.run()
+                o_offering_action.run(datastore="datastore")
 
                 # test de l'appel à OfferingAction.find_offering
                 o_mock_offering_action_list_offering.assert_called_once()
 
                 # test de l'appel à Offering.api_create
-                o_mock_offering_api_create.assert_called_once_with(self.d_action["body_parameters"], route_params=self.d_action["url_parameters"])
+                o_mock_offering_api_create.assert_called_once_with(self.d_action["body_parameters"], route_params={"datastore": "datastore", **self.d_action["url_parameters"]})
 
                 # api update appelé 2 fois
                 self.assertEqual(2, o_mock_offering.api_update.call_count)
 
     def test_run_not_existing_not_create(self) -> None:
         """test de run quand l'offre à créer n'existe pas et que l'offering n'est pas créer."""
         # problème lors de la création de l'offre
@@ -104,19 +104,19 @@
 
         # On mock find_offering et api_create
         with patch.object(o_offering_action, "find_offering", return_value=None) as o_mock_offering_action_list_offering:
             with patch.object(Offering, "api_create", return_value=o_mock_offering) as o_mock_offering_api_create:
                 with patch.object(time, "sleep", return_value=None) as o_mock_time:
                     # on lance l'exécution de run
                     with self.assertRaises(StepActionError) as o_err:
-                        o_offering_action.run()
+                        o_offering_action.run("datastore")
                     self.assertEqual(o_err.exception.message, "Création d'une offre : terminé en erreur.")
 
                     o_mock_offering_action_list_offering.assert_called_once()
-                    o_mock_offering_api_create.assert_called_once_with(self.d_action["body_parameters"], route_params=self.d_action["url_parameters"])
+                    o_mock_offering_api_create.assert_called_once_with(self.d_action["body_parameters"], route_params={"datastore": "datastore", **self.d_action["url_parameters"]})
                     self.assertEqual(o_mock_offering.api_update.call_count, 4)
                     o_mock_time.assert_any_call(1)
 
     # On mock find_offering et api_create
     def test_run_existing_behavior_continue(self) -> None:
         """test de run quand l'offre à créer existe behavior continue"""
```

### Comparing `sdk_entrepot_gpf-0.1.24/tests/workflow/action/PermissionActionTestCase.py` & `sdk_entrepot_gpf-0.1.25/tests/workflow/action/PermissionActionTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/tests/workflow/action/ProcessingExecutionActionTestCase.py` & `sdk_entrepot_gpf-0.1.25/tests/workflow/action/ProcessingExecutionActionTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/tests/workflow/action/SynchronizeOfferingActionTestCase.py` & `sdk_entrepot_gpf-0.1.25/tests/workflow/action/SynchronizeOfferingActionTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/tests/workflow/action/UploadActionTestCase.py` & `sdk_entrepot_gpf-0.1.25/tests/workflow/action/UploadActionTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/tests/workflow/resolver/DateResolverTestCase.py` & `sdk_entrepot_gpf-0.1.25/tests/workflow/resolver/DateResolverTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/tests/workflow/resolver/DictResolverTestCase.py` & `sdk_entrepot_gpf-0.1.25/tests/workflow/resolver/DictResolverTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/tests/workflow/resolver/FileResolverTestCase.py` & `sdk_entrepot_gpf-0.1.25/tests/workflow/resolver/FileResolverTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/tests/workflow/resolver/GlobalResolverTestCase.py` & `sdk_entrepot_gpf-0.1.25/tests/workflow/resolver/GlobalResolverTestCase.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,20 +12,20 @@
 
     cmd : python3 -m unittest -b tests.workflow.resolver.GlobalResolverTestCase
     """
 
     localization = {
         "Jacques_country": "France",
         "Jacques_city": "Paris",
-        "Jacques_street": "Champs-Elysée",
+        "Jacques_street": "Champs-Elysee",
         "John_country": "England",
         "John_city": "London",
         "John_street": "rue_Londres",
         "city": ["Paris", "London"],
-        "store": {"Paris": "Champs-Elysée", "London": "rue_Londres"},
+        "store": {"Paris": "Champs-Elysee", "London": "rue_Londres"},
     }
     profession = {
         "chef": "Jacques",
         "sailor": "John",
     }
 
     @classmethod
@@ -119,17 +119,17 @@
         self.assertEqual(GlobalResolver().resolve("{profession.sailor}"), "John")
         self.assertEqual(GlobalResolver().resolve("{localization.Jacques_country}_{profession.sailor}"), "France_John")
         # Comme liste (pour insérer une string)
         self.assertEqual(GlobalResolver().resolve('["_localization_","Jacques_country"]'), "France")
         # Comme dict (pour insérer une string)
         self.assertEqual(GlobalResolver().resolve('{"_localization_":"Jacques_country"}'), "France")
         # Comme liste (pour insérer une liste)
-        self.assertEqual(GlobalResolver().resolve('["_localization_","city"]'), "['Paris', 'London']")
+        self.assertEqual(GlobalResolver().resolve('["_localization_","city"]'), '["Paris", "London"]')
         # Comme dict (pour insérer un dict)
-        self.assertEqual(GlobalResolver().resolve('{"_localization_":"store"}'), "{'Paris': 'Champs-Elysée', 'London': 'rue_Londres'}")
+        self.assertEqual(GlobalResolver().resolve('{"_localization_":"store"}'), '{"Paris": "Champs-Elysee", "London": "rue_Londres"}')
         # Cas avancés : deux résolutions l'une dans l'autre
         # Comme string
         self.assertEqual(GlobalResolver().resolve("{localization.{profession.sailor}_country}"), "England")
         self.assertEqual(GlobalResolver().resolve("{localization.{profession.chef}_city}"), "Paris")
         # Comme liste (pour insérer une string)
         self.assertEqual(GlobalResolver().resolve('["_localization_","{profession.sailor}_country"]'), "England")
         # Comme dict (pour insérer une string)
```

### Comparing `sdk_entrepot_gpf-0.1.24/tests/workflow/resolver/StoreEntityResolverTestCase.py` & `sdk_entrepot_gpf-0.1.25/tests/workflow/resolver/StoreEntityResolverTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/tests/workflow/resolver/UserResolverTestCase.py` & `sdk_entrepot_gpf-0.1.25/tests/workflow/resolver/UserResolverTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/uml/classes.png` & `sdk_entrepot_gpf-0.1.25/uml/classes.png`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/uml/classes.uxf` & `sdk_entrepot_gpf-0.1.25/uml/classes.uxf`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/uml/interfaces.png` & `sdk_entrepot_gpf-0.1.25/uml/interfaces.png`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/uml/interfaces.uxf` & `sdk_entrepot_gpf-0.1.25/uml/interfaces.uxf`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.24/PKG-INFO` & `sdk_entrepot_gpf-0.1.25/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdk_entrepot_gpf
-Version: 0.1.24
+Version: 0.1.25
 Summary: SDK Python pour simplifier l'utilisation de l'API Entrepôt de la Géoplateforme.
 Author-email: Valentin Sasyan <valentin.sasyan@ign.fr>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

