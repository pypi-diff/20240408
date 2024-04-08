# Comparing `tmp/sempyro-1.0.0.tar.gz` & `tmp/sempyro-1.1.0.tar.gz`

## Comparing `sempyro-1.0.0.tar` & `sempyro-1.1.0.tar`

### file list

```diff
@@ -1,275 +1,279 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sempyro-1.0.0/doc_notebook.ipynb
--rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 sempyro-1.0.0/junk.py
--rw-r--r--   0        0        0   176359 2020-02-02 00:00:00.000000 sempyro-1.0.0/poetry.lock
--rw-r--r--   0        0        0    55138 2020-02-02 00:00:00.000000 sempyro-1.0.0/wizard.png
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 sempyro-1.0.0/.idea/.gitignore
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 sempyro-1.0.0/.idea/.name
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 sempyro-1.0.0/.idea/HRIPydanticModels.iml
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 sempyro-1.0.0/.idea/misc.xml
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 sempyro-1.0.0/.idea/modules.xml
--rw-r--r--   0        0        0    15698 2020-02-02 00:00:00.000000 sempyro-1.0.0/.idea/workspace.xml
--rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 sempyro-1.0.0/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 sempyro-1.0.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     4717 2020-02-02 00:00:00.000000 sempyro-1.0.0/__tests__/test_cvard.py
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 sempyro-1.0.0/__tests__/test_dcat_models.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 sempyro-1.0.0/__tests__/test_hri_models.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 sempyro-1.0.0/__tests__/test_policy.py
--rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 sempyro-1.0.0/__tests__/test_prov.py
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 sempyro-1.0.0/__tests__/test_rdf_model.py
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 sempyro-1.0.0/__tests__/test_spatial.py
--rw-r--r--   0        0        0    13697 2020-02-02 00:00:00.000000 sempyro-1.0.0/__tests__/test_time_models.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 sempyro-1.0.0/__tests__/test_data/agent.ttl
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/__tests__/test_data/agent.ttl.license
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 sempyro-1.0.0/__tests__/test_data/date_time_description.json
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/__tests__/test_data/date_time_description.json.license
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 sempyro-1.0.0/__tests__/test_data/date_time_description.ttl
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/__tests__/test_data/date_time_description.ttl.license
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 sempyro-1.0.0/__tests__/test_data/example_26.ttl
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/__tests__/test_data/example_26.ttl.license
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 sempyro-1.0.0/__tests__/test_data/general_date_time_descr_example.ttl
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/__tests__/test_data/general_date_time_descr_example.ttl.license
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 sempyro-1.0.0/__tests__/test_data/general_date_time_description.json
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/__tests__/test_data/general_date_time_description.json.license
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 sempyro-1.0.0/__tests__/test_data/period_of_time_ex23.ttl
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/__tests__/test_data/period_of_time_ex23.ttl.license
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 sempyro-1.0.0/__tests__/test_data/period_of_time_ex24.ttl
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/__tests__/test_data/period_of_time_ex24.ttl.license
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 sempyro-1.0.0/__tests__/test_data/spatial_ex29.ttl
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/__tests__/test_data/spatial_ex29.ttl.license
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 sempyro-1.0.0/__tests__/test_data/time_position_nominal.json
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/__tests__/test_data/time_position_nominal.json.license
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 sempyro-1.0.0/__tests__/test_data/time_position_numeric.json
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/__tests__/test_data/time_position_numeric.json.license
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 sempyro-1.0.0/__tests__/test_data/vCard.ttl
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/__tests__/test_data/vCard.ttl.license
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 sempyro-1.0.0/__tests__/test_data/vCard_as_a_node.ttl
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/__tests__/test_data/vCard_as_a_node.ttl.license
--rw-r--r--   0        0        0     7698 2020-02-02 00:00:00.000000 sempyro-1.0.0/beacon/beacon_model.json
--rw-r--r--   0        0        0     5716 2020-02-02 00:00:00.000000 sempyro-1.0.0/beacon/beacon_model.yaml
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 sempyro-1.0.0/beacon/commonDefinitions.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 sempyro-1.0.0/beacon/example.json
--rw-r--r--   0        0        0     3291 2020-02-02 00:00:00.000000 sempyro-1.0.0/beacon/ind_schema.json
--rw-r--r--   0        0        0     6347 2020-02-02 00:00:00.000000 sempyro-1.0.0/beacon/individual.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 sempyro-1.0.0/beacon/validate_ex.py
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 sempyro-1.0.0/beacon/src/common.py
--rw-r--r--   0        0        0     9660 2020-02-02 00:00:00.000000 sempyro-1.0.0/docs/Defining_extendind_a_model.md
--rw-r--r--   0        0        0     9562 2020-02-02 00:00:00.000000 sempyro-1.0.0/docs/Intro.md
--rw-r--r--   0        0        0    27211 2020-02-02 00:00:00.000000 sempyro-1.0.0/docs/Models.md
--rw-r--r--   0        0        0    31491 2020-02-02 00:00:00.000000 sempyro-1.0.0/docs/Usage_example_time_models.ipynb
--rw-r--r--   0        0        0    23455 2020-02-02 00:00:00.000000 sempyro-1.0.0/docs/Usage_example_with_test_data.ipynb
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 sempyro-1.0.0/docs/example_data.csv
--rw-r--r--   0        0        0    10258 2020-02-02 00:00:00.000000 sempyro-1.0.0/docs/example_data.xlsx
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 sempyro-1.0.0/docs/junk.py
--rw-r--r--   0        0        0    81752 2020-02-02 00:00:00.000000 sempyro-1.0.0/docs/imgs/minimal_catalog.png
--rw-r--r--   0        0        0    44187 2020-02-02 00:00:00.000000 sempyro-1.0.0/docs/imgs/minimal_dataset.png
--rw-r--r--   0        0        0    55138 2020-02-02 00:00:00.000000 sempyro-1.0.0/docs/imgs/wizard.png
--rw-r--r--   0        0        0    70614 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/dcat/DCATCatalog.json
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/dcat/DCATCatalog.json.license
--rw-r--r--   0        0        0    57487 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/dcat/DCATCatalog.yaml
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/dcat/DCATCatalog.yaml.license
--rw-r--r--   0        0        0    68391 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/dcat/DCATDataset.json
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/dcat/DCATDataset.json.license
--rw-r--r--   0        0        0    55751 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/dcat/DCATDataset.yaml
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/dcat/DCATDataset.yaml.license
--rw-r--r--   0        0        0   113037 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/dcat/DCATDistribution.json
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/dcat/DCATDistribution.json.license
--rw-r--r--   0        0        0    89992 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/dcat/DCATDistribution.yaml
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/dcat/DCATDistribution.yaml.license
--rw-r--r--   0        0        0    25826 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/dcat/DCATResource.json
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/dcat/DCATResource.json.license
--rw-r--r--   0        0        0    19675 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/dcat/DCATResource.yaml
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/dcat/DCATResource.yaml.license
--rw-r--r--   0        0        0   101159 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/dcat/DataService.json
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/dcat/DataService.json.license
--rw-r--r--   0        0        0    80737 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/dcat/DataService.yaml
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/dcat/DataService.yaml.license
--rw-r--r--   0        0        0    68548 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/dcat/DatasetSeries.json
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/dcat/DatasetSeries.json.license
--rw-r--r--   0        0        0    55903 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/dcat/DatasetSeries.yaml
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/dcat/DatasetSeries.yaml.license
--rw-r--r--   0        0        0  1226834 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/dcat/dcat_catalog.png
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/dcat/dcat_catalog.png.license
--rw-r--r--   0        0        0  2315800 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/dcat/dcat_data_service.png
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/dcat/dcat_data_service.png.license
--rw-r--r--   0        0        0  1191013 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/dcat/dcat_dataset.png
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/dcat/dcat_dataset.png.license
--rw-r--r--   0        0        0  1190890 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/dcat/dcat_dataset_series.png
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/dcat/dcat_dataset_series.png.license
--rw-r--r--   0        0        0  3117157 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/dcat/dcat_distribution.png
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/dcat/dcat_distribution.png.license
--rw-r--r--   0        0        0   557640 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/dcat/dcat_resource.png
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/dcat/dcat_resource.png.license
--rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/foaf/Agent.json
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/foaf/Agent.json.license
--rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/foaf/Agent.yaml
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/foaf/Agent.yaml.license
--rw-r--r--   0        0        0     5111 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/foaf/Project.json
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/foaf/Project.json.license
--rw-r--r--   0        0        0     3871 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/foaf/Project.yaml
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/foaf/Project.yaml.license
--rw-r--r--   0        0        0     5722 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/geo/Geometry.json
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/geo/Geometry.json.license
--rw-r--r--   0        0        0     4781 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/geo/Geometry.yaml
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/geo/Geometry.yaml.license
--rw-r--r--   0        0        0     7694 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/geo/Location.json
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/geo/Location.json.license
--rw-r--r--   0        0        0     6301 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/geo/Location.yaml
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/geo/Location.yaml.license
--rw-r--r--   0        0        0     4770 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/hri_dcat/HRICatalog.json
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/hri_dcat/HRICatalog.json.license
--rw-r--r--   0        0        0     3640 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/hri_dcat/HRICatalog.yaml
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/hri_dcat/HRICatalog.yaml.license
--rw-r--r--   0        0        0    37279 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/hri_dcat/HRIDataService.json
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/hri_dcat/HRIDataService.json.license
--rw-r--r--   0        0        0    28153 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/hri_dcat/HRIDataService.yaml
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/hri_dcat/HRIDataService.yaml.license
--rw-r--r--   0        0        0     9186 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/hri_dcat/HRIDataset.json
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/hri_dcat/HRIDataset.json.license
--rw-r--r--   0        0        0     6791 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/hri_dcat/HRIDataset.yaml
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/hri_dcat/HRIDataset.yaml.license
--rw-r--r--   0        0        0    40730 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/hri_dcat/HRIDistribution.json
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/hri_dcat/HRIDistribution.json.license
--rw-r--r--   0        0        0    30887 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/hri_dcat/HRIDistribution.yaml
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/hri_dcat/HRIDistribution.yaml.license
--rw-r--r--   0        0        0    59340 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/hri_dcat/hri_catalog.png
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/hri_dcat/hri_catalog.png.license
--rw-r--r--   0        0        0   795313 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/hri_dcat/hri_dataservice.png
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/hri_dcat/hri_dataservice.png.license
--rw-r--r--   0        0        0   143108 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/hri_dcat/hri_dataset.png
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/hri_dcat/hri_dataset.png.license
--rw-r--r--   0        0        0  1027125 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/hri_dcat/hri_distribution.png
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/hri_dcat/hri_distribution.png.license
--rw-r--r--   0        0        0     6116 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/odrl/ODRLPolicy.json
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/odrl/ODRLPolicy.json.license
--rw-r--r--   0        0        0     4530 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/odrl/ODRLPolicy.yaml
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/odrl/ODRLPolicy.yaml.license
--rw-r--r--   0        0        0    19767 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/prov/Activity.json
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/prov/Activity.json.license
--rw-r--r--   0        0        0    17686 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/prov/Activity.yaml
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/prov/Activity.yaml.license
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/prov/Association.json
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/prov/Association.json.license
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/prov/Association.yaml
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/prov/Association.yaml.license
--rw-r--r--   0        0        0     3575 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/prov/End.json
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/prov/End.json.license
--rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/prov/End.yaml
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/prov/End.yaml.license
--rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/prov/EntityInfluence.json
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/prov/EntityInfluence.json.license
--rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/prov/EntityInfluence.yaml
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/prov/EntityInfluence.yaml.license
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/prov/InstantaneousEvent.json
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/prov/InstantaneousEvent.json.license
--rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/prov/InstantaneousEvent.yaml
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/prov/InstantaneousEvent.yaml.license
--rw-r--r--   0        0        0     3585 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/prov/Start.json
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/prov/Start.json.license
--rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/prov/Start.yaml
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/prov/Start.yaml.license
--rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/spdx/Checksum.json
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/spdx/Checksum.json.license
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/spdx/Checksum.yaml
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/spdx/Checksum.yaml.license
--rw-r--r--   0        0        0     6396 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/time/DateTimeDescription.json
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/time/DateTimeDescription.json.license
--rw-r--r--   0        0        0     5308 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/time/DateTimeDescription.yaml
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/time/DateTimeDescription.yaml.license
--rw-r--r--   0        0        0     4557 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/time/GeneralDateTimeDescription.json
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/time/GeneralDateTimeDescription.json.license
--rw-r--r--   0        0        0     3730 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/time/GeneralDateTimeDescription.yaml
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/time/GeneralDateTimeDescription.yaml.license
--rw-r--r--   0        0        0    13063 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/time/PeriodOfTime.json
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/time/PeriodOfTime.json.license
--rw-r--r--   0        0        0    10707 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/time/PeriodOfTime.yaml
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/time/PeriodOfTime.yaml.license
--rw-r--r--   0        0        0     9574 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/time/TimeInstant.json
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/time/TimeInstant.json.license
--rw-r--r--   0        0        0     7911 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/time/TimeInstant.yaml
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/time/TimeInstant.yaml.license
--rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/time/TimePosition.json
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/time/TimePosition.json.license
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/time/TimePosition.yaml
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/time/TimePosition.yaml.license
--rw-r--r--   0        0        0   108255 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/time/period_of_time.png
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/time/period_of_time.png.license
--rw-r--r--   0        0        0    65271 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/time/time_instant.png
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/time/time_instant.png.license
--rw-r--r--   0        0        0     3279 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/vcard/VCard.json
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/vcard/VCard.json.license
--rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/vcard/VCard.yaml
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.0.0/models/vcard/VCard.yaml.license
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 sempyro-1.0.0/sempyro/__init__.py
--rw-r--r--   0        0        0    12638 2020-02-02 00:00:00.000000 sempyro-1.0.0/sempyro/rdf_model.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 sempyro-1.0.0/sempyro/dcat/__init__.py
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 sempyro-1.0.0/sempyro/dcat/data_service.py
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 sempyro-1.0.0/sempyro/dcat/dataset_series.py
--rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 sempyro-1.0.0/sempyro/dcat/dcat_catalog.py
--rw-r--r--   0        0        0     4093 2020-02-02 00:00:00.000000 sempyro-1.0.0/sempyro/dcat/dcat_dataset.py
--rw-r--r--   0        0        0     7367 2020-02-02 00:00:00.000000 sempyro-1.0.0/sempyro/dcat/dcat_distribution.py
--rw-r--r--   0        0        0    11171 2020-02-02 00:00:00.000000 sempyro-1.0.0/sempyro/dcat/dcat_resource.py
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 sempyro-1.0.0/sempyro/foaf/__init__.py
--rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 sempyro-1.0.0/sempyro/foaf/agent.py
--rw-r--r--   0        0        0     2913 2020-02-02 00:00:00.000000 sempyro-1.0.0/sempyro/foaf/project.py
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 sempyro-1.0.0/sempyro/geo/__init__.py
--rw-r--r--   0        0        0     6099 2020-02-02 00:00:00.000000 sempyro-1.0.0/sempyro/geo/spatial.py
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 sempyro-1.0.0/sempyro/hri_dcat/__init__.py
--rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 sempyro-1.0.0/sempyro/hri_dcat/hri_catalog.py
--rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 sempyro-1.0.0/sempyro/hri_dcat/hri_data_service.py
--rw-r--r--   0        0        0     5331 2020-02-02 00:00:00.000000 sempyro-1.0.0/sempyro/hri_dcat/hri_dataset.py
--rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 sempyro-1.0.0/sempyro/hri_dcat/hri_distribution.py
--rw-r--r--   0        0        0     3767 2020-02-02 00:00:00.000000 sempyro-1.0.0/sempyro/namespaces/ADMS.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 sempyro-1.0.0/sempyro/namespaces/DCATv3.py
--rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 sempyro-1.0.0/sempyro/namespaces/FREQ.py
--rw-r--r--   0        0        0     8591 2020-02-02 00:00:00.000000 sempyro-1.0.0/sempyro/namespaces/GEOSPARQL.py
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 sempyro-1.0.0/sempyro/namespaces/GREG.py
--rw-r--r--   0        0        0     4298 2020-02-02 00:00:00.000000 sempyro-1.0.0/sempyro/namespaces/LOCN.py
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 sempyro-1.0.0/sempyro/namespaces/__init__.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 sempyro-1.0.0/sempyro/odrl/__init__.py
--rw-r--r--   0        0        0     4440 2020-02-02 00:00:00.000000 sempyro-1.0.0/sempyro/odrl/policy.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 sempyro-1.0.0/sempyro/prov/__init__.py
--rw-r--r--   0        0        0    16867 2020-02-02 00:00:00.000000 sempyro-1.0.0/sempyro/prov/prov_classes.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 sempyro-1.0.0/sempyro/spdx/__init__.py
--rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 sempyro-1.0.0/sempyro/spdx/spdx_classes.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 sempyro-1.0.0/sempyro/time/__init__.py
--rw-r--r--   0        0        0    20718 2020-02-02 00:00:00.000000 sempyro-1.0.0/sempyro/time/dcat_time_models.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 sempyro-1.0.0/sempyro/utils/__init__.py
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 sempyro-1.0.0/sempyro/utils/constants.py
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 sempyro-1.0.0/sempyro/utils/validator_functions.py
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 sempyro-1.0.0/sempyro/vcard/__init__.py
--rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 sempyro-1.0.0/sempyro/vcard/vcard.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 sempyro-1.0.0/venv2/.gitignore
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 sempyro-1.0.0/venv2/pyvenv.cfg
--rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 sempyro-1.0.0/venv2/bin/activate
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 sempyro-1.0.0/venv2/bin/activate.csh
--rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 sempyro-1.0.0/venv2/bin/activate.fish
--rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 sempyro-1.0.0/venv2/bin/activate.nu
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 sempyro-1.0.0/venv2/bin/activate.ps1
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 sempyro-1.0.0/venv2/bin/activate_this.py
--rwxr-xr-x   0        0        0      300 2020-02-02 00:00:00.000000 sempyro-1.0.0/venv2/bin/coverage
--rwxr-xr-x   0        0        0      300 2020-02-02 00:00:00.000000 sempyro-1.0.0/venv2/bin/coverage-3.9
--rwxr-xr-x   0        0        0      300 2020-02-02 00:00:00.000000 sempyro-1.0.0/venv2/bin/coverage3
--rwxr-xr-x   0        0        0      304 2020-02-02 00:00:00.000000 sempyro-1.0.0/venv2/bin/csv2rdf
--rwxr-xr-x   0        0        0      308 2020-02-02 00:00:00.000000 sempyro-1.0.0/venv2/bin/email_validator
--rwxr-xr-x   0        0        0      306 2020-02-02 00:00:00.000000 sempyro-1.0.0/venv2/bin/pip
--rwxr-xr-x   0        0        0      306 2020-02-02 00:00:00.000000 sempyro-1.0.0/venv2/bin/pip-3.9
--rwxr-xr-x   0        0        0      306 2020-02-02 00:00:00.000000 sempyro-1.0.0/venv2/bin/pip3
--rwxr-xr-x   0        0        0      306 2020-02-02 00:00:00.000000 sempyro-1.0.0/venv2/bin/pip3.9
--rwxr-xr-x   0        0        0      306 2020-02-02 00:00:00.000000 sempyro-1.0.0/venv2/bin/py.test
--rwxr-xr-x   0        0        0      306 2020-02-02 00:00:00.000000 sempyro-1.0.0/venv2/bin/pytest
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 sempyro-1.0.0/venv2/bin/python -> /Library/Developer/CommandLineTools/Library/Frameworks/Python3.framework/Versions/3.9/Resources/Python.app/Contents/MacOS/Python
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 sempyro-1.0.0/venv2/bin/python3 -> python
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 sempyro-1.0.0/venv2/bin/python3.9 -> python
--rwxr-xr-x   0        0        0      304 2020-02-02 00:00:00.000000 sempyro-1.0.0/venv2/bin/rdf2dot
--rwxr-xr-x   0        0        0      313 2020-02-02 00:00:00.000000 sempyro-1.0.0/venv2/bin/rdfgraphisomorphism
--rwxr-xr-x   0        0        0      304 2020-02-02 00:00:00.000000 sempyro-1.0.0/venv2/bin/rdfpipe
--rwxr-xr-x   0        0        0      305 2020-02-02 00:00:00.000000 sempyro-1.0.0/venv2/bin/rdfs2dot
--rwxr-xr-x   0        0        0      293 2020-02-02 00:00:00.000000 sempyro-1.0.0/venv2/bin/wheel
--rwxr-xr-x   0        0        0      293 2020-02-02 00:00:00.000000 sempyro-1.0.0/venv2/bin/wheel-3.9
--rwxr-xr-x   0        0        0      293 2020-02-02 00:00:00.000000 sempyro-1.0.0/venv2/bin/wheel3
--rwxr-xr-x   0        0        0      293 2020-02-02 00:00:00.000000 sempyro-1.0.0/venv2/bin/wheel3.9
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 sempyro-1.0.0/.gitignore
--rw-r--r--   0        0        0    10279 2020-02-02 00:00:00.000000 sempyro-1.0.0/LICENSE
--rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 sempyro-1.0.0/README.md
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 sempyro-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 sempyro-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 sempyro-1.1.0/junk.py
+-rw-r--r--   0        0        0   176359 2020-02-02 00:00:00.000000 sempyro-1.1.0/poetry.lock
+-rw-r--r--   0        0        0    55138 2020-02-02 00:00:00.000000 sempyro-1.1.0/wizard.png
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 sempyro-1.1.0/.idea/.gitignore
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 sempyro-1.1.0/.idea/.name
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 sempyro-1.1.0/.idea/HRIPydanticModels.iml
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 sempyro-1.1.0/.idea/misc.xml
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 sempyro-1.1.0/.idea/modules.xml
+-rw-r--r--   0        0        0    15698 2020-02-02 00:00:00.000000 sempyro-1.1.0/.idea/workspace.xml
+-rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 sempyro-1.1.0/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 sempyro-1.1.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     4717 2020-02-02 00:00:00.000000 sempyro-1.1.0/__tests__/test_cvard.py
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 sempyro-1.1.0/__tests__/test_dcat_models.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 sempyro-1.1.0/__tests__/test_hri_models.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 sempyro-1.1.0/__tests__/test_policy.py
+-rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 sempyro-1.1.0/__tests__/test_prov.py
+-rw-r--r--   0        0        0     3241 2020-02-02 00:00:00.000000 sempyro-1.1.0/__tests__/test_rdf_model.py
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 sempyro-1.1.0/__tests__/test_spatial.py
+-rw-r--r--   0        0        0    13697 2020-02-02 00:00:00.000000 sempyro-1.1.0/__tests__/test_time_models.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 sempyro-1.1.0/__tests__/test_data/agent.ttl
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/__tests__/test_data/agent.ttl.license
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 sempyro-1.1.0/__tests__/test_data/date_time_description.json
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/__tests__/test_data/date_time_description.json.license
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 sempyro-1.1.0/__tests__/test_data/date_time_description.ttl
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/__tests__/test_data/date_time_description.ttl.license
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 sempyro-1.1.0/__tests__/test_data/example_26.ttl
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/__tests__/test_data/example_26.ttl.license
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 sempyro-1.1.0/__tests__/test_data/general_date_time_descr_example.ttl
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/__tests__/test_data/general_date_time_descr_example.ttl.license
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 sempyro-1.1.0/__tests__/test_data/general_date_time_description.json
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/__tests__/test_data/general_date_time_description.json.license
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 sempyro-1.1.0/__tests__/test_data/period_of_time_ex23.ttl
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/__tests__/test_data/period_of_time_ex23.ttl.license
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 sempyro-1.1.0/__tests__/test_data/period_of_time_ex24.ttl
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/__tests__/test_data/period_of_time_ex24.ttl.license
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 sempyro-1.1.0/__tests__/test_data/spatial_ex29.ttl
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/__tests__/test_data/spatial_ex29.ttl.license
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 sempyro-1.1.0/__tests__/test_data/time_position_nominal.json
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/__tests__/test_data/time_position_nominal.json.license
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 sempyro-1.1.0/__tests__/test_data/time_position_numeric.json
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/__tests__/test_data/time_position_numeric.json.license
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 sempyro-1.1.0/__tests__/test_data/vCard.ttl
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/__tests__/test_data/vCard.ttl.license
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 sempyro-1.1.0/__tests__/test_data/vCard_as_a_node.ttl
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/__tests__/test_data/vCard_as_a_node.ttl.license
+-rw-r--r--   0        0        0     7698 2020-02-02 00:00:00.000000 sempyro-1.1.0/beacon/beacon_model.json
+-rw-r--r--   0        0        0     5716 2020-02-02 00:00:00.000000 sempyro-1.1.0/beacon/beacon_model.yaml
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 sempyro-1.1.0/beacon/commonDefinitions.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 sempyro-1.1.0/beacon/example.json
+-rw-r--r--   0        0        0     3291 2020-02-02 00:00:00.000000 sempyro-1.1.0/beacon/ind_schema.json
+-rw-r--r--   0        0        0     6347 2020-02-02 00:00:00.000000 sempyro-1.1.0/beacon/individual.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 sempyro-1.1.0/beacon/validate_ex.py
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 sempyro-1.1.0/beacon/src/common.py
+-rw-r--r--   0        0        0     9660 2020-02-02 00:00:00.000000 sempyro-1.1.0/docs/Defining_extendind_a_model.md
+-rw-r--r--   0        0        0     9562 2020-02-02 00:00:00.000000 sempyro-1.1.0/docs/Intro.md
+-rw-r--r--   0        0        0    27211 2020-02-02 00:00:00.000000 sempyro-1.1.0/docs/Models.md
+-rw-r--r--   0        0        0    31491 2020-02-02 00:00:00.000000 sempyro-1.1.0/docs/Usage_example_time_models.ipynb
+-rw-r--r--   0        0        0    23455 2020-02-02 00:00:00.000000 sempyro-1.1.0/docs/Usage_example_with_test_data.ipynb
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 sempyro-1.1.0/docs/example_data.csv
+-rw-r--r--   0        0        0    10258 2020-02-02 00:00:00.000000 sempyro-1.1.0/docs/example_data.xlsx
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 sempyro-1.1.0/docs/example_data2.csv
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 sempyro-1.1.0/docs/example_rdf.ttl
+-rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 sempyro-1.1.0/docs/example_rdf_2.ttl
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 sempyro-1.1.0/docs/junk.py
+-rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 sempyro-1.1.0/docs/simple_example.py
+-rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 sempyro-1.1.0/docs/simple_example2.py
+-rw-r--r--   0        0        0    81752 2020-02-02 00:00:00.000000 sempyro-1.1.0/docs/imgs/minimal_catalog.png
+-rw-r--r--   0        0        0    44187 2020-02-02 00:00:00.000000 sempyro-1.1.0/docs/imgs/minimal_dataset.png
+-rw-r--r--   0        0        0    55138 2020-02-02 00:00:00.000000 sempyro-1.1.0/docs/imgs/wizard.png
+-rw-r--r--   0        0        0    70614 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/dcat/DCATCatalog.json
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/dcat/DCATCatalog.json.license
+-rw-r--r--   0        0        0    57487 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/dcat/DCATCatalog.yaml
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/dcat/DCATCatalog.yaml.license
+-rw-r--r--   0        0        0    68391 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/dcat/DCATDataset.json
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/dcat/DCATDataset.json.license
+-rw-r--r--   0        0        0    55751 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/dcat/DCATDataset.yaml
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/dcat/DCATDataset.yaml.license
+-rw-r--r--   0        0        0   113037 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/dcat/DCATDistribution.json
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/dcat/DCATDistribution.json.license
+-rw-r--r--   0        0        0    89992 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/dcat/DCATDistribution.yaml
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/dcat/DCATDistribution.yaml.license
+-rw-r--r--   0        0        0    25826 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/dcat/DCATResource.json
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/dcat/DCATResource.json.license
+-rw-r--r--   0        0        0    19675 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/dcat/DCATResource.yaml
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/dcat/DCATResource.yaml.license
+-rw-r--r--   0        0        0   101159 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/dcat/DataService.json
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/dcat/DataService.json.license
+-rw-r--r--   0        0        0    80737 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/dcat/DataService.yaml
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/dcat/DataService.yaml.license
+-rw-r--r--   0        0        0    68548 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/dcat/DatasetSeries.json
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/dcat/DatasetSeries.json.license
+-rw-r--r--   0        0        0    55903 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/dcat/DatasetSeries.yaml
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/dcat/DatasetSeries.yaml.license
+-rw-r--r--   0        0        0  1226834 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/dcat/dcat_catalog.png
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/dcat/dcat_catalog.png.license
+-rw-r--r--   0        0        0  2315800 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/dcat/dcat_data_service.png
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/dcat/dcat_data_service.png.license
+-rw-r--r--   0        0        0  1191013 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/dcat/dcat_dataset.png
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/dcat/dcat_dataset.png.license
+-rw-r--r--   0        0        0  1190890 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/dcat/dcat_dataset_series.png
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/dcat/dcat_dataset_series.png.license
+-rw-r--r--   0        0        0  3117157 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/dcat/dcat_distribution.png
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/dcat/dcat_distribution.png.license
+-rw-r--r--   0        0        0   557640 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/dcat/dcat_resource.png
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/dcat/dcat_resource.png.license
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/foaf/Agent.json
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/foaf/Agent.json.license
+-rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/foaf/Agent.yaml
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/foaf/Agent.yaml.license
+-rw-r--r--   0        0        0     5111 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/foaf/Project.json
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/foaf/Project.json.license
+-rw-r--r--   0        0        0     3871 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/foaf/Project.yaml
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/foaf/Project.yaml.license
+-rw-r--r--   0        0        0     5722 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/geo/Geometry.json
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/geo/Geometry.json.license
+-rw-r--r--   0        0        0     4781 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/geo/Geometry.yaml
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/geo/Geometry.yaml.license
+-rw-r--r--   0        0        0     7694 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/geo/Location.json
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/geo/Location.json.license
+-rw-r--r--   0        0        0     6301 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/geo/Location.yaml
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/geo/Location.yaml.license
+-rw-r--r--   0        0        0     4770 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/hri_dcat/HRICatalog.json
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/hri_dcat/HRICatalog.json.license
+-rw-r--r--   0        0        0     3640 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/hri_dcat/HRICatalog.yaml
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/hri_dcat/HRICatalog.yaml.license
+-rw-r--r--   0        0        0    37279 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/hri_dcat/HRIDataService.json
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/hri_dcat/HRIDataService.json.license
+-rw-r--r--   0        0        0    28153 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/hri_dcat/HRIDataService.yaml
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/hri_dcat/HRIDataService.yaml.license
+-rw-r--r--   0        0        0     9186 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/hri_dcat/HRIDataset.json
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/hri_dcat/HRIDataset.json.license
+-rw-r--r--   0        0        0     6791 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/hri_dcat/HRIDataset.yaml
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/hri_dcat/HRIDataset.yaml.license
+-rw-r--r--   0        0        0    40730 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/hri_dcat/HRIDistribution.json
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/hri_dcat/HRIDistribution.json.license
+-rw-r--r--   0        0        0    30887 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/hri_dcat/HRIDistribution.yaml
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/hri_dcat/HRIDistribution.yaml.license
+-rw-r--r--   0        0        0    59340 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/hri_dcat/hri_catalog.png
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/hri_dcat/hri_catalog.png.license
+-rw-r--r--   0        0        0   795313 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/hri_dcat/hri_dataservice.png
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/hri_dcat/hri_dataservice.png.license
+-rw-r--r--   0        0        0   143108 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/hri_dcat/hri_dataset.png
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/hri_dcat/hri_dataset.png.license
+-rw-r--r--   0        0        0  1027125 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/hri_dcat/hri_distribution.png
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/hri_dcat/hri_distribution.png.license
+-rw-r--r--   0        0        0     6116 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/odrl/ODRLPolicy.json
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/odrl/ODRLPolicy.json.license
+-rw-r--r--   0        0        0     4530 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/odrl/ODRLPolicy.yaml
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/odrl/ODRLPolicy.yaml.license
+-rw-r--r--   0        0        0    19767 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/prov/Activity.json
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/prov/Activity.json.license
+-rw-r--r--   0        0        0    17686 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/prov/Activity.yaml
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/prov/Activity.yaml.license
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/prov/Association.json
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/prov/Association.json.license
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/prov/Association.yaml
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/prov/Association.yaml.license
+-rw-r--r--   0        0        0     3575 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/prov/End.json
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/prov/End.json.license
+-rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/prov/End.yaml
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/prov/End.yaml.license
+-rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/prov/EntityInfluence.json
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/prov/EntityInfluence.json.license
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/prov/EntityInfluence.yaml
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/prov/EntityInfluence.yaml.license
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/prov/InstantaneousEvent.json
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/prov/InstantaneousEvent.json.license
+-rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/prov/InstantaneousEvent.yaml
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/prov/InstantaneousEvent.yaml.license
+-rw-r--r--   0        0        0     3585 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/prov/Start.json
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/prov/Start.json.license
+-rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/prov/Start.yaml
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/prov/Start.yaml.license
+-rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/spdx/Checksum.json
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/spdx/Checksum.json.license
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/spdx/Checksum.yaml
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/spdx/Checksum.yaml.license
+-rw-r--r--   0        0        0     6396 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/time/DateTimeDescription.json
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/time/DateTimeDescription.json.license
+-rw-r--r--   0        0        0     5308 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/time/DateTimeDescription.yaml
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/time/DateTimeDescription.yaml.license
+-rw-r--r--   0        0        0     4557 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/time/GeneralDateTimeDescription.json
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/time/GeneralDateTimeDescription.json.license
+-rw-r--r--   0        0        0     3730 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/time/GeneralDateTimeDescription.yaml
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/time/GeneralDateTimeDescription.yaml.license
+-rw-r--r--   0        0        0    13063 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/time/PeriodOfTime.json
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/time/PeriodOfTime.json.license
+-rw-r--r--   0        0        0    10707 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/time/PeriodOfTime.yaml
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/time/PeriodOfTime.yaml.license
+-rw-r--r--   0        0        0     9574 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/time/TimeInstant.json
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/time/TimeInstant.json.license
+-rw-r--r--   0        0        0     7911 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/time/TimeInstant.yaml
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/time/TimeInstant.yaml.license
+-rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/time/TimePosition.json
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/time/TimePosition.json.license
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/time/TimePosition.yaml
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/time/TimePosition.yaml.license
+-rw-r--r--   0        0        0   108255 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/time/period_of_time.png
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/time/period_of_time.png.license
+-rw-r--r--   0        0        0    65271 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/time/time_instant.png
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/time/time_instant.png.license
+-rw-r--r--   0        0        0     3279 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/vcard/VCard.json
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/vcard/VCard.json.license
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/vcard/VCard.yaml
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 sempyro-1.1.0/models/vcard/VCard.yaml.license
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 sempyro-1.1.0/sempyro/__init__.py
+-rw-r--r--   0        0        0    12709 2020-02-02 00:00:00.000000 sempyro-1.1.0/sempyro/rdf_model.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 sempyro-1.1.0/sempyro/dcat/__init__.py
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 sempyro-1.1.0/sempyro/dcat/data_service.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 sempyro-1.1.0/sempyro/dcat/dataset_series.py
+-rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 sempyro-1.1.0/sempyro/dcat/dcat_catalog.py
+-rw-r--r--   0        0        0     4093 2020-02-02 00:00:00.000000 sempyro-1.1.0/sempyro/dcat/dcat_dataset.py
+-rw-r--r--   0        0        0     7367 2020-02-02 00:00:00.000000 sempyro-1.1.0/sempyro/dcat/dcat_distribution.py
+-rw-r--r--   0        0        0    11171 2020-02-02 00:00:00.000000 sempyro-1.1.0/sempyro/dcat/dcat_resource.py
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 sempyro-1.1.0/sempyro/foaf/__init__.py
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 sempyro-1.1.0/sempyro/foaf/agent.py
+-rw-r--r--   0        0        0     2913 2020-02-02 00:00:00.000000 sempyro-1.1.0/sempyro/foaf/project.py
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 sempyro-1.1.0/sempyro/geo/__init__.py
+-rw-r--r--   0        0        0     6099 2020-02-02 00:00:00.000000 sempyro-1.1.0/sempyro/geo/spatial.py
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 sempyro-1.1.0/sempyro/hri_dcat/__init__.py
+-rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 sempyro-1.1.0/sempyro/hri_dcat/hri_catalog.py
+-rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 sempyro-1.1.0/sempyro/hri_dcat/hri_data_service.py
+-rw-r--r--   0        0        0     5331 2020-02-02 00:00:00.000000 sempyro-1.1.0/sempyro/hri_dcat/hri_dataset.py
+-rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 sempyro-1.1.0/sempyro/hri_dcat/hri_distribution.py
+-rw-r--r--   0        0        0     3767 2020-02-02 00:00:00.000000 sempyro-1.1.0/sempyro/namespaces/ADMS.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 sempyro-1.1.0/sempyro/namespaces/DCATv3.py
+-rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 sempyro-1.1.0/sempyro/namespaces/FREQ.py
+-rw-r--r--   0        0        0     8591 2020-02-02 00:00:00.000000 sempyro-1.1.0/sempyro/namespaces/GEOSPARQL.py
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 sempyro-1.1.0/sempyro/namespaces/GREG.py
+-rw-r--r--   0        0        0     4298 2020-02-02 00:00:00.000000 sempyro-1.1.0/sempyro/namespaces/LOCN.py
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 sempyro-1.1.0/sempyro/namespaces/__init__.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 sempyro-1.1.0/sempyro/odrl/__init__.py
+-rw-r--r--   0        0        0     4440 2020-02-02 00:00:00.000000 sempyro-1.1.0/sempyro/odrl/policy.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 sempyro-1.1.0/sempyro/prov/__init__.py
+-rw-r--r--   0        0        0    16867 2020-02-02 00:00:00.000000 sempyro-1.1.0/sempyro/prov/prov_classes.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 sempyro-1.1.0/sempyro/spdx/__init__.py
+-rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 sempyro-1.1.0/sempyro/spdx/spdx_classes.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 sempyro-1.1.0/sempyro/time/__init__.py
+-rw-r--r--   0        0        0    20718 2020-02-02 00:00:00.000000 sempyro-1.1.0/sempyro/time/dcat_time_models.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 sempyro-1.1.0/sempyro/utils/__init__.py
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 sempyro-1.1.0/sempyro/utils/constants.py
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 sempyro-1.1.0/sempyro/utils/validator_functions.py
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 sempyro-1.1.0/sempyro/vcard/__init__.py
+-rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 sempyro-1.1.0/sempyro/vcard/vcard.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 sempyro-1.1.0/venv2/.gitignore
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 sempyro-1.1.0/venv2/pyvenv.cfg
+-rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 sempyro-1.1.0/venv2/bin/activate
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 sempyro-1.1.0/venv2/bin/activate.csh
+-rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 sempyro-1.1.0/venv2/bin/activate.fish
+-rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 sempyro-1.1.0/venv2/bin/activate.nu
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 sempyro-1.1.0/venv2/bin/activate.ps1
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 sempyro-1.1.0/venv2/bin/activate_this.py
+-rwxr-xr-x   0        0        0      300 2020-02-02 00:00:00.000000 sempyro-1.1.0/venv2/bin/coverage
+-rwxr-xr-x   0        0        0      300 2020-02-02 00:00:00.000000 sempyro-1.1.0/venv2/bin/coverage-3.9
+-rwxr-xr-x   0        0        0      300 2020-02-02 00:00:00.000000 sempyro-1.1.0/venv2/bin/coverage3
+-rwxr-xr-x   0        0        0      304 2020-02-02 00:00:00.000000 sempyro-1.1.0/venv2/bin/csv2rdf
+-rwxr-xr-x   0        0        0      308 2020-02-02 00:00:00.000000 sempyro-1.1.0/venv2/bin/email_validator
+-rwxr-xr-x   0        0        0      306 2020-02-02 00:00:00.000000 sempyro-1.1.0/venv2/bin/pip
+-rwxr-xr-x   0        0        0      306 2020-02-02 00:00:00.000000 sempyro-1.1.0/venv2/bin/pip-3.9
+-rwxr-xr-x   0        0        0      306 2020-02-02 00:00:00.000000 sempyro-1.1.0/venv2/bin/pip3
+-rwxr-xr-x   0        0        0      306 2020-02-02 00:00:00.000000 sempyro-1.1.0/venv2/bin/pip3.9
+-rwxr-xr-x   0        0        0      306 2020-02-02 00:00:00.000000 sempyro-1.1.0/venv2/bin/py.test
+-rwxr-xr-x   0        0        0      306 2020-02-02 00:00:00.000000 sempyro-1.1.0/venv2/bin/pytest
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 sempyro-1.1.0/venv2/bin/python -> /Library/Developer/CommandLineTools/Library/Frameworks/Python3.framework/Versions/3.9/Resources/Python.app/Contents/MacOS/Python
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 sempyro-1.1.0/venv2/bin/python3 -> python
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 sempyro-1.1.0/venv2/bin/python3.9 -> python
+-rwxr-xr-x   0        0        0      304 2020-02-02 00:00:00.000000 sempyro-1.1.0/venv2/bin/rdf2dot
+-rwxr-xr-x   0        0        0      313 2020-02-02 00:00:00.000000 sempyro-1.1.0/venv2/bin/rdfgraphisomorphism
+-rwxr-xr-x   0        0        0      304 2020-02-02 00:00:00.000000 sempyro-1.1.0/venv2/bin/rdfpipe
+-rwxr-xr-x   0        0        0      305 2020-02-02 00:00:00.000000 sempyro-1.1.0/venv2/bin/rdfs2dot
+-rwxr-xr-x   0        0        0      293 2020-02-02 00:00:00.000000 sempyro-1.1.0/venv2/bin/wheel
+-rwxr-xr-x   0        0        0      293 2020-02-02 00:00:00.000000 sempyro-1.1.0/venv2/bin/wheel-3.9
+-rwxr-xr-x   0        0        0      293 2020-02-02 00:00:00.000000 sempyro-1.1.0/venv2/bin/wheel3
+-rwxr-xr-x   0        0        0      293 2020-02-02 00:00:00.000000 sempyro-1.1.0/venv2/bin/wheel3.9
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 sempyro-1.1.0/.gitignore
+-rw-r--r--   0        0        0    10279 2020-02-02 00:00:00.000000 sempyro-1.1.0/LICENSE
+-rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 sempyro-1.1.0/README.md
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 sempyro-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4594 2020-02-02 00:00:00.000000 sempyro-1.1.0/PKG-INFO
```

### Comparing `sempyro-1.0.0/junk.py` & `sempyro-1.1.0/junk.py`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/poetry.lock` & `sempyro-1.1.0/poetry.lock`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/wizard.png` & `sempyro-1.1.0/wizard.png`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/.idea/workspace.xml` & `sempyro-1.1.0/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/.idea/inspectionProfiles/Project_Default.xml` & `sempyro-1.1.0/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/__tests__/test_cvard.py` & `sempyro-1.1.0/__tests__/test_cvard.py`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/__tests__/test_dcat_models.py` & `sempyro-1.1.0/__tests__/test_dcat_models.py`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/__tests__/test_hri_models.py` & `sempyro-1.1.0/__tests__/test_hri_models.py`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/__tests__/test_policy.py` & `sempyro-1.1.0/__tests__/test_policy.py`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/__tests__/test_prov.py` & `sempyro-1.1.0/__tests__/test_prov.py`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/__tests__/test_spatial.py` & `sempyro-1.1.0/__tests__/test_spatial.py`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/__tests__/test_time_models.py` & `sempyro-1.1.0/__tests__/test_time_models.py`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/__tests__/test_data/agent.ttl.license` & `sempyro-1.1.0/__tests__/test_data/agent.ttl.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/__tests__/test_data/date_time_description.json.license` & `sempyro-1.1.0/__tests__/test_data/date_time_description.json.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/__tests__/test_data/date_time_description.ttl` & `sempyro-1.1.0/__tests__/test_data/date_time_description.ttl`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/__tests__/test_data/date_time_description.ttl.license` & `sempyro-1.1.0/__tests__/test_data/date_time_description.ttl.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/__tests__/test_data/example_26.ttl` & `sempyro-1.1.0/__tests__/test_data/example_26.ttl`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/__tests__/test_data/example_26.ttl.license` & `sempyro-1.1.0/__tests__/test_data/example_26.ttl.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/__tests__/test_data/general_date_time_descr_example.ttl` & `sempyro-1.1.0/__tests__/test_data/general_date_time_descr_example.ttl`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/__tests__/test_data/general_date_time_descr_example.ttl.license` & `sempyro-1.1.0/__tests__/test_data/general_date_time_descr_example.ttl.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/__tests__/test_data/general_date_time_description.json.license` & `sempyro-1.1.0/__tests__/test_data/general_date_time_description.json.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/__tests__/test_data/period_of_time_ex23.ttl.license` & `sempyro-1.1.0/__tests__/test_data/period_of_time_ex23.ttl.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/__tests__/test_data/period_of_time_ex24.ttl` & `sempyro-1.1.0/__tests__/test_data/period_of_time_ex24.ttl`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/__tests__/test_data/period_of_time_ex24.ttl.license` & `sempyro-1.1.0/__tests__/test_data/period_of_time_ex24.ttl.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/__tests__/test_data/spatial_ex29.ttl` & `sempyro-1.1.0/__tests__/test_data/spatial_ex29.ttl`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/__tests__/test_data/spatial_ex29.ttl.license` & `sempyro-1.1.0/__tests__/test_data/spatial_ex29.ttl.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/__tests__/test_data/time_position_nominal.json.license` & `sempyro-1.1.0/__tests__/test_data/time_position_nominal.json.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/__tests__/test_data/time_position_numeric.json.license` & `sempyro-1.1.0/__tests__/test_data/time_position_numeric.json.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/__tests__/test_data/vCard.ttl.license` & `sempyro-1.1.0/__tests__/test_data/vCard.ttl.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/__tests__/test_data/vCard_as_a_node.ttl.license` & `sempyro-1.1.0/__tests__/test_data/vCard_as_a_node.ttl.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/beacon/beacon_model.json` & `sempyro-1.1.0/beacon/beacon_model.json`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/beacon/beacon_model.yaml` & `sempyro-1.1.0/beacon/beacon_model.yaml`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/beacon/commonDefinitions.py` & `sempyro-1.1.0/beacon/commonDefinitions.py`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/beacon/ind_schema.json` & `sempyro-1.1.0/beacon/ind_schema.json`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/beacon/individual.py` & `sempyro-1.1.0/beacon/individual.py`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/beacon/validate_ex.py` & `sempyro-1.1.0/beacon/validate_ex.py`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/beacon/src/common.py` & `sempyro-1.1.0/beacon/src/common.py`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/docs/Defining_extendind_a_model.md` & `sempyro-1.1.0/docs/Defining_extendind_a_model.md`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/docs/Intro.md` & `sempyro-1.1.0/docs/Intro.md`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/docs/Models.md` & `sempyro-1.1.0/docs/Models.md`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/docs/Usage_example_time_models.ipynb` & `sempyro-1.1.0/docs/Usage_example_time_models.ipynb`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/docs/Usage_example_with_test_data.ipynb` & `sempyro-1.1.0/docs/Usage_example_with_test_data.ipynb`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/docs/example_data.csv` & `sempyro-1.1.0/docs/example_data.csv`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/docs/example_data.xlsx` & `sempyro-1.1.0/docs/example_data.xlsx`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/docs/junk.py` & `sempyro-1.1.0/docs/junk.py`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/docs/imgs/minimal_catalog.png` & `sempyro-1.1.0/docs/imgs/minimal_catalog.png`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/docs/imgs/minimal_dataset.png` & `sempyro-1.1.0/docs/imgs/minimal_dataset.png`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/docs/imgs/wizard.png` & `sempyro-1.1.0/docs/imgs/wizard.png`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/dcat/DCATCatalog.json` & `sempyro-1.1.0/models/dcat/DCATCatalog.json`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/dcat/DCATCatalog.json.license` & `sempyro-1.1.0/models/dcat/DCATCatalog.json.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/dcat/DCATCatalog.yaml` & `sempyro-1.1.0/models/dcat/DCATCatalog.yaml`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/dcat/DCATCatalog.yaml.license` & `sempyro-1.1.0/models/dcat/DCATCatalog.yaml.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/dcat/DCATDataset.json` & `sempyro-1.1.0/models/dcat/DCATDataset.json`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/dcat/DCATDataset.json.license` & `sempyro-1.1.0/models/dcat/DCATDataset.json.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/dcat/DCATDataset.yaml` & `sempyro-1.1.0/models/dcat/DCATDataset.yaml`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/dcat/DCATDataset.yaml.license` & `sempyro-1.1.0/models/dcat/DCATDataset.yaml.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/dcat/DCATDistribution.json` & `sempyro-1.1.0/models/dcat/DCATDistribution.json`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/dcat/DCATDistribution.json.license` & `sempyro-1.1.0/models/dcat/DCATDistribution.json.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/dcat/DCATDistribution.yaml` & `sempyro-1.1.0/models/dcat/DCATDistribution.yaml`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/dcat/DCATDistribution.yaml.license` & `sempyro-1.1.0/models/dcat/DCATDistribution.yaml.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/dcat/DCATResource.json` & `sempyro-1.1.0/models/dcat/DCATResource.json`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/dcat/DCATResource.json.license` & `sempyro-1.1.0/models/dcat/DCATResource.json.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/dcat/DCATResource.yaml` & `sempyro-1.1.0/models/dcat/DCATResource.yaml`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/dcat/DCATResource.yaml.license` & `sempyro-1.1.0/models/dcat/DCATResource.yaml.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/dcat/DataService.json` & `sempyro-1.1.0/models/dcat/DataService.json`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/dcat/DataService.json.license` & `sempyro-1.1.0/models/dcat/DataService.json.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/dcat/DataService.yaml` & `sempyro-1.1.0/models/dcat/DataService.yaml`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/dcat/DataService.yaml.license` & `sempyro-1.1.0/models/dcat/DataService.yaml.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/dcat/DatasetSeries.json` & `sempyro-1.1.0/models/dcat/DatasetSeries.json`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/dcat/DatasetSeries.json.license` & `sempyro-1.1.0/models/dcat/DatasetSeries.json.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/dcat/DatasetSeries.yaml` & `sempyro-1.1.0/models/dcat/DatasetSeries.yaml`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/dcat/DatasetSeries.yaml.license` & `sempyro-1.1.0/models/dcat/DatasetSeries.yaml.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/dcat/dcat_catalog.png` & `sempyro-1.1.0/models/dcat/dcat_catalog.png`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/dcat/dcat_catalog.png.license` & `sempyro-1.1.0/models/dcat/dcat_catalog.png.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/dcat/dcat_data_service.png` & `sempyro-1.1.0/models/dcat/dcat_data_service.png`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/dcat/dcat_data_service.png.license` & `sempyro-1.1.0/models/dcat/dcat_data_service.png.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/dcat/dcat_dataset.png` & `sempyro-1.1.0/models/dcat/dcat_dataset.png`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/dcat/dcat_dataset.png.license` & `sempyro-1.1.0/models/dcat/dcat_dataset.png.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/dcat/dcat_dataset_series.png` & `sempyro-1.1.0/models/dcat/dcat_dataset_series.png`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/dcat/dcat_dataset_series.png.license` & `sempyro-1.1.0/models/dcat/dcat_dataset_series.png.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/dcat/dcat_distribution.png` & `sempyro-1.1.0/models/dcat/dcat_distribution.png`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/dcat/dcat_distribution.png.license` & `sempyro-1.1.0/models/dcat/dcat_distribution.png.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/dcat/dcat_resource.png` & `sempyro-1.1.0/models/dcat/dcat_resource.png`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/dcat/dcat_resource.png.license` & `sempyro-1.1.0/models/dcat/dcat_resource.png.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/foaf/Agent.json` & `sempyro-1.1.0/models/foaf/Agent.json`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/foaf/Agent.json.license` & `sempyro-1.1.0/models/foaf/Agent.json.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/foaf/Agent.yaml` & `sempyro-1.1.0/models/foaf/Agent.yaml`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/foaf/Agent.yaml.license` & `sempyro-1.1.0/models/foaf/Agent.yaml.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/foaf/Project.json` & `sempyro-1.1.0/models/foaf/Project.json`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/foaf/Project.json.license` & `sempyro-1.1.0/models/foaf/Project.json.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/foaf/Project.yaml` & `sempyro-1.1.0/models/foaf/Project.yaml`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/foaf/Project.yaml.license` & `sempyro-1.1.0/models/foaf/Project.yaml.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/geo/Geometry.json` & `sempyro-1.1.0/models/geo/Geometry.json`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/geo/Geometry.json.license` & `sempyro-1.1.0/models/geo/Geometry.json.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/geo/Geometry.yaml` & `sempyro-1.1.0/models/geo/Geometry.yaml`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/geo/Geometry.yaml.license` & `sempyro-1.1.0/models/geo/Geometry.yaml.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/geo/Location.json` & `sempyro-1.1.0/models/geo/Location.json`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/geo/Location.json.license` & `sempyro-1.1.0/models/geo/Location.json.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/geo/Location.yaml` & `sempyro-1.1.0/models/geo/Location.yaml`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/geo/Location.yaml.license` & `sempyro-1.1.0/models/geo/Location.yaml.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/hri_dcat/HRICatalog.json` & `sempyro-1.1.0/models/hri_dcat/HRICatalog.json`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/hri_dcat/HRICatalog.json.license` & `sempyro-1.1.0/models/hri_dcat/HRICatalog.json.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/hri_dcat/HRICatalog.yaml` & `sempyro-1.1.0/models/hri_dcat/HRICatalog.yaml`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/hri_dcat/HRICatalog.yaml.license` & `sempyro-1.1.0/models/hri_dcat/HRICatalog.yaml.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/hri_dcat/HRIDataService.json` & `sempyro-1.1.0/models/hri_dcat/HRIDataService.json`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/hri_dcat/HRIDataService.json.license` & `sempyro-1.1.0/models/hri_dcat/HRIDataService.json.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/hri_dcat/HRIDataService.yaml` & `sempyro-1.1.0/models/hri_dcat/HRIDataService.yaml`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/hri_dcat/HRIDataService.yaml.license` & `sempyro-1.1.0/models/hri_dcat/HRIDataService.yaml.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/hri_dcat/HRIDataset.json` & `sempyro-1.1.0/models/hri_dcat/HRIDataset.json`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/hri_dcat/HRIDataset.json.license` & `sempyro-1.1.0/models/hri_dcat/HRIDataset.json.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/hri_dcat/HRIDataset.yaml` & `sempyro-1.1.0/models/hri_dcat/HRIDataset.yaml`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/hri_dcat/HRIDataset.yaml.license` & `sempyro-1.1.0/models/hri_dcat/HRIDataset.yaml.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/hri_dcat/HRIDistribution.json` & `sempyro-1.1.0/models/hri_dcat/HRIDistribution.json`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/hri_dcat/HRIDistribution.json.license` & `sempyro-1.1.0/models/hri_dcat/HRIDistribution.json.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/hri_dcat/HRIDistribution.yaml` & `sempyro-1.1.0/models/hri_dcat/HRIDistribution.yaml`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/hri_dcat/HRIDistribution.yaml.license` & `sempyro-1.1.0/models/hri_dcat/HRIDistribution.yaml.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/hri_dcat/hri_catalog.png` & `sempyro-1.1.0/models/hri_dcat/hri_catalog.png`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/hri_dcat/hri_catalog.png.license` & `sempyro-1.1.0/models/hri_dcat/hri_catalog.png.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/hri_dcat/hri_dataservice.png` & `sempyro-1.1.0/models/hri_dcat/hri_dataservice.png`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/hri_dcat/hri_dataservice.png.license` & `sempyro-1.1.0/models/hri_dcat/hri_dataservice.png.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/hri_dcat/hri_dataset.png` & `sempyro-1.1.0/models/hri_dcat/hri_dataset.png`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/hri_dcat/hri_dataset.png.license` & `sempyro-1.1.0/models/hri_dcat/hri_dataset.png.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/hri_dcat/hri_distribution.png` & `sempyro-1.1.0/models/hri_dcat/hri_distribution.png`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/hri_dcat/hri_distribution.png.license` & `sempyro-1.1.0/models/hri_dcat/hri_distribution.png.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/odrl/ODRLPolicy.json` & `sempyro-1.1.0/models/odrl/ODRLPolicy.json`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/odrl/ODRLPolicy.json.license` & `sempyro-1.1.0/models/odrl/ODRLPolicy.json.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/odrl/ODRLPolicy.yaml` & `sempyro-1.1.0/models/odrl/ODRLPolicy.yaml`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/odrl/ODRLPolicy.yaml.license` & `sempyro-1.1.0/models/odrl/ODRLPolicy.yaml.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/prov/Activity.json` & `sempyro-1.1.0/models/prov/Activity.json`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/prov/Activity.json.license` & `sempyro-1.1.0/models/prov/Activity.json.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/prov/Activity.yaml` & `sempyro-1.1.0/models/prov/Activity.yaml`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/prov/Activity.yaml.license` & `sempyro-1.1.0/models/prov/Activity.yaml.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/prov/Association.json` & `sempyro-1.1.0/models/prov/Association.json`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/prov/Association.json.license` & `sempyro-1.1.0/models/prov/Association.json.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/prov/Association.yaml` & `sempyro-1.1.0/models/prov/Association.yaml`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/prov/Association.yaml.license` & `sempyro-1.1.0/models/prov/Association.yaml.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/prov/End.json` & `sempyro-1.1.0/models/prov/End.json`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/prov/End.json.license` & `sempyro-1.1.0/models/prov/End.json.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/prov/End.yaml` & `sempyro-1.1.0/models/prov/End.yaml`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/prov/End.yaml.license` & `sempyro-1.1.0/models/prov/End.yaml.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/prov/EntityInfluence.json` & `sempyro-1.1.0/models/prov/EntityInfluence.json`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/prov/EntityInfluence.json.license` & `sempyro-1.1.0/models/prov/EntityInfluence.json.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/prov/EntityInfluence.yaml` & `sempyro-1.1.0/models/prov/EntityInfluence.yaml`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/prov/EntityInfluence.yaml.license` & `sempyro-1.1.0/models/prov/EntityInfluence.yaml.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/prov/InstantaneousEvent.json` & `sempyro-1.1.0/models/prov/InstantaneousEvent.json`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/prov/InstantaneousEvent.json.license` & `sempyro-1.1.0/models/prov/InstantaneousEvent.json.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/prov/InstantaneousEvent.yaml` & `sempyro-1.1.0/models/prov/InstantaneousEvent.yaml`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/prov/InstantaneousEvent.yaml.license` & `sempyro-1.1.0/models/prov/InstantaneousEvent.yaml.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/prov/Start.json` & `sempyro-1.1.0/models/prov/Start.json`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/prov/Start.json.license` & `sempyro-1.1.0/models/prov/Start.json.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/prov/Start.yaml` & `sempyro-1.1.0/models/prov/Start.yaml`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/prov/Start.yaml.license` & `sempyro-1.1.0/models/prov/Start.yaml.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/spdx/Checksum.json` & `sempyro-1.1.0/models/spdx/Checksum.json`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/spdx/Checksum.json.license` & `sempyro-1.1.0/models/spdx/Checksum.json.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/spdx/Checksum.yaml` & `sempyro-1.1.0/models/spdx/Checksum.yaml`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/spdx/Checksum.yaml.license` & `sempyro-1.1.0/models/spdx/Checksum.yaml.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/time/DateTimeDescription.json` & `sempyro-1.1.0/models/time/DateTimeDescription.json`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/time/DateTimeDescription.json.license` & `sempyro-1.1.0/models/time/DateTimeDescription.json.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/time/DateTimeDescription.yaml` & `sempyro-1.1.0/models/time/DateTimeDescription.yaml`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/time/DateTimeDescription.yaml.license` & `sempyro-1.1.0/models/time/DateTimeDescription.yaml.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/time/GeneralDateTimeDescription.json` & `sempyro-1.1.0/models/time/GeneralDateTimeDescription.json`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/time/GeneralDateTimeDescription.json.license` & `sempyro-1.1.0/models/time/GeneralDateTimeDescription.json.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/time/GeneralDateTimeDescription.yaml` & `sempyro-1.1.0/models/time/GeneralDateTimeDescription.yaml`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/time/GeneralDateTimeDescription.yaml.license` & `sempyro-1.1.0/models/time/GeneralDateTimeDescription.yaml.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/time/PeriodOfTime.json` & `sempyro-1.1.0/models/time/PeriodOfTime.json`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/time/PeriodOfTime.json.license` & `sempyro-1.1.0/models/time/PeriodOfTime.json.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/time/PeriodOfTime.yaml` & `sempyro-1.1.0/models/time/PeriodOfTime.yaml`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/time/PeriodOfTime.yaml.license` & `sempyro-1.1.0/models/time/PeriodOfTime.yaml.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/time/TimeInstant.json` & `sempyro-1.1.0/models/time/TimeInstant.json`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/time/TimeInstant.json.license` & `sempyro-1.1.0/models/time/TimeInstant.json.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/time/TimeInstant.yaml` & `sempyro-1.1.0/models/time/TimeInstant.yaml`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/time/TimeInstant.yaml.license` & `sempyro-1.1.0/models/time/TimeInstant.yaml.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/time/TimePosition.json` & `sempyro-1.1.0/models/time/TimePosition.json`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/time/TimePosition.json.license` & `sempyro-1.1.0/models/time/TimePosition.json.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/time/TimePosition.yaml` & `sempyro-1.1.0/models/time/TimePosition.yaml`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/time/TimePosition.yaml.license` & `sempyro-1.1.0/models/time/TimePosition.yaml.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/time/period_of_time.png` & `sempyro-1.1.0/models/time/period_of_time.png`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/time/period_of_time.png.license` & `sempyro-1.1.0/models/time/period_of_time.png.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/time/time_instant.png` & `sempyro-1.1.0/models/time/time_instant.png`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/time/time_instant.png.license` & `sempyro-1.1.0/models/time/time_instant.png.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/vcard/VCard.json` & `sempyro-1.1.0/models/vcard/VCard.json`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/vcard/VCard.json.license` & `sempyro-1.1.0/models/vcard/VCard.json.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/vcard/VCard.yaml` & `sempyro-1.1.0/models/vcard/VCard.yaml`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/models/vcard/VCard.yaml.license` & `sempyro-1.1.0/models/vcard/VCard.yaml.license`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/sempyro/__init__.py` & `sempyro-1.1.0/sempyro/__init__.py`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/sempyro/rdf_model.py` & `sempyro-1.1.0/sempyro/rdf_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,27 +201,29 @@
                         graph.bind(bind_namespace[0], URIRef(bind_namespace[1]))
 
     @staticmethod
     def _convert_to_datetime_literal(value: Union[str, date, datetime, AwareDatetime, NaiveDatetime]) -> Literal:
         literal_format = None
         if isinstance(value, (datetime, AwareDatetime, NaiveDatetime)):
             literal_format = XSD.dateTime
+            value = value.isoformat()
         elif isinstance(value, date):
             literal_format = XSD.date
+            value = value.isoformat()
         elif isinstance(value, str):
             if re.match(year_month_pattern, value):
                 literal_format = XSD.gYearMonth
             elif re.match(year_pattern, value):
                 literal_format = XSD.gYear
             else:
                 logging.warning(f"{str} does not match neither gYear nor gYearMonth pattern")
         else:
             raise TypeError(f"Value {value} is of unsupported type {type(value)}, either str, date, datetime, "
                             f"pydantic.AwareDatetime or pydantic.NaiveDatetime are expected")
-        return Literal(str(value), datatype=literal_format)
+        return Literal(value, datatype=literal_format)
 
     def _convert_to_rdf_type(self, rdf_type: str, value: Any) -> Union[URIRef, Literal]:
         if rdf_type.startswith("xsd:"):
             xsd_attribute = getattr(XSD, rdf_type.split(":")[-1])
             return Literal(value, datatype=xsd_attribute)
         if rdf_type == "literal":
             return Literal(value)
```

### Comparing `sempyro-1.0.0/sempyro/dcat/__init__.py` & `sempyro-1.1.0/sempyro/dcat/__init__.py`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/sempyro/dcat/data_service.py` & `sempyro-1.1.0/sempyro/dcat/data_service.py`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/sempyro/dcat/dataset_series.py` & `sempyro-1.1.0/sempyro/dcat/dataset_series.py`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/sempyro/dcat/dcat_catalog.py` & `sempyro-1.1.0/sempyro/dcat/dcat_catalog.py`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/sempyro/dcat/dcat_dataset.py` & `sempyro-1.1.0/sempyro/dcat/dcat_dataset.py`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/sempyro/dcat/dcat_distribution.py` & `sempyro-1.1.0/sempyro/dcat/dcat_distribution.py`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/sempyro/dcat/dcat_resource.py` & `sempyro-1.1.0/sempyro/dcat/dcat_resource.py`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/sempyro/foaf/__init__.py` & `sempyro-1.1.0/sempyro/foaf/__init__.py`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/sempyro/foaf/agent.py` & `sempyro-1.1.0/sempyro/foaf/agent.py`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/sempyro/foaf/project.py` & `sempyro-1.1.0/sempyro/foaf/project.py`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/sempyro/geo/__init__.py` & `sempyro-1.1.0/sempyro/geo/__init__.py`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/sempyro/geo/spatial.py` & `sempyro-1.1.0/sempyro/geo/spatial.py`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/sempyro/hri_dcat/hri_catalog.py` & `sempyro-1.1.0/sempyro/hri_dcat/hri_catalog.py`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/sempyro/hri_dcat/hri_data_service.py` & `sempyro-1.1.0/sempyro/hri_dcat/hri_data_service.py`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/sempyro/hri_dcat/hri_dataset.py` & `sempyro-1.1.0/sempyro/hri_dcat/hri_dataset.py`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/sempyro/hri_dcat/hri_distribution.py` & `sempyro-1.1.0/sempyro/hri_dcat/hri_distribution.py`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/sempyro/namespaces/ADMS.py` & `sempyro-1.1.0/sempyro/namespaces/ADMS.py`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/sempyro/namespaces/DCATv3.py` & `sempyro-1.1.0/sempyro/namespaces/DCATv3.py`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/sempyro/namespaces/FREQ.py` & `sempyro-1.1.0/sempyro/namespaces/FREQ.py`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/sempyro/namespaces/GEOSPARQL.py` & `sempyro-1.1.0/sempyro/namespaces/GEOSPARQL.py`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/sempyro/namespaces/GREG.py` & `sempyro-1.1.0/sempyro/namespaces/GREG.py`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/sempyro/namespaces/LOCN.py` & `sempyro-1.1.0/sempyro/namespaces/LOCN.py`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/sempyro/namespaces/__init__.py` & `sempyro-1.1.0/sempyro/namespaces/__init__.py`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/sempyro/odrl/__init__.py` & `sempyro-1.1.0/sempyro/odrl/__init__.py`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/sempyro/odrl/policy.py` & `sempyro-1.1.0/sempyro/odrl/policy.py`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/sempyro/prov/__init__.py` & `sempyro-1.1.0/sempyro/prov/__init__.py`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/sempyro/prov/prov_classes.py` & `sempyro-1.1.0/sempyro/prov/prov_classes.py`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/sempyro/spdx/__init__.py` & `sempyro-1.1.0/sempyro/spdx/__init__.py`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/sempyro/spdx/spdx_classes.py` & `sempyro-1.1.0/sempyro/spdx/spdx_classes.py`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/sempyro/time/__init__.py` & `sempyro-1.1.0/sempyro/time/__init__.py`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/sempyro/time/dcat_time_models.py` & `sempyro-1.1.0/sempyro/time/dcat_time_models.py`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/sempyro/utils/__init__.py` & `sempyro-1.1.0/sempyro/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/sempyro/utils/constants.py` & `sempyro-1.1.0/sempyro/utils/constants.py`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/sempyro/utils/validator_functions.py` & `sempyro-1.1.0/sempyro/utils/validator_functions.py`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/sempyro/vcard/__init__.py` & `sempyro-1.1.0/sempyro/vcard/__init__.py`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/sempyro/vcard/vcard.py` & `sempyro-1.1.0/sempyro/vcard/vcard.py`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/venv2/bin/activate` & `sempyro-1.1.0/venv2/bin/activate`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/venv2/bin/activate.csh` & `sempyro-1.1.0/venv2/bin/activate.csh`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/venv2/bin/activate.fish` & `sempyro-1.1.0/venv2/bin/activate.fish`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/venv2/bin/activate.nu` & `sempyro-1.1.0/venv2/bin/activate.nu`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/venv2/bin/activate.ps1` & `sempyro-1.1.0/venv2/bin/activate.ps1`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/venv2/bin/activate_this.py` & `sempyro-1.1.0/venv2/bin/activate_this.py`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/.gitignore` & `sempyro-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/LICENSE` & `sempyro-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sempyro-1.0.0/README.md` & `sempyro-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# HRIPydanticModels
+# SeMPyRO Data Models
 
-**SeMPyRO** is a Python package containing Pydantic models representing classes of the
-DCAT-AP v3 data model. It is designed to streamline data validation, conversion to RDF, and schema generation processes.
+**SeMPyRO** (for Semantic Models Python/Pydantic RDF Ontology) is a Python package containing Pydantic models 
+representing classes of the DCAT-AP v3 data model. It is designed to streamline data validation, conversion to RDF, 
+and schema generation processes.
 
 ## Key Features
 
 - **Data Validation**: Easily validate data against schemas, ensuring its correctness, integrity and DCAT-AP compatibility.
 - **RDF Graph Conversion**: Convert data into RDF graphs effortlessly, enabling integration with RDF-based systems and applications.
 - **Schema Generation**: Generate JSON/YAML schemas compatible with the DCAT-AP v3 profile, facilitating interoperability and compliance with standards.
 - **Pedantic Integration**: Built upon the robust [Pydantic](https://docs.pydantic.dev/) library, leveraging its powerful validation capabilities and extending them for RDF handling.
```

### Comparing `sempyro-1.0.0/pyproject.toml` & `sempyro-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sempyro"
-version = "v1.0.0"
+version = "v1.1.0"
 description = "SeMPyRO (for Semantic Models Python Pydantic RDF Ontology) is a Pydantic models representing classes of DCAT-AP v3 data model."
 keywords = ["rdf", "pydantic", "DCAT", "DCAT-AP", "data model"]
 requires-python = ">= 3.9"
 authors = [
     { name = "Anastasia Nayden", email = "anastasia.nayden@health-ri.nl" },
     { name = "Mark Janse", email = "mark.janse@health-ri.nl" }
 ]
```

### Comparing `sempyro-1.0.0/PKG-INFO` & `sempyro-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sempyro
-Version: 1.0.0
+Version: 1.1.0
 Summary: SeMPyRO (for Semantic Models Python Pydantic RDF Ontology) is a Pydantic models representing classes of DCAT-AP v3 data model.
 Project-URL: Documentation, https://github.com/Health-RI/SeMPyRO/tree/main/docs
 Project-URL: Repository, https://github.com/Health-RI/SeMPyRO.git
 Project-URL: Issues, https://github.com/Health-RI/SeMPyRO/issues
 Author-email: Anastasia Nayden <anastasia.nayden@health-ri.nl>, Mark Janse <mark.janse@health-ri.nl>
 License-File: LICENSE
 Keywords: DCAT,DCAT-AP,data model,pydantic,rdf
@@ -24,18 +24,19 @@
 Requires-Dist: ruamel-yaml==0.18.5
 Provides-Extra: notebook-docs
 Requires-Dist: notebook>=7.0.6; extra == 'notebook-docs'
 Requires-Dist: pandas>=1.5.3; extra == 'notebook-docs'
 Requires-Dist: tabulate>=0.9.0; extra == 'notebook-docs'
 Description-Content-Type: text/markdown
 
-# HRIPydanticModels
+# SeMPyRO Data Models
 
-**SeMPyRO** is a Python package containing Pydantic models representing classes of the
-DCAT-AP v3 data model. It is designed to streamline data validation, conversion to RDF, and schema generation processes.
+**SeMPyRO** (for Semantic Models Python/Pydantic RDF Ontology) is a Python package containing Pydantic models 
+representing classes of the DCAT-AP v3 data model. It is designed to streamline data validation, conversion to RDF, 
+and schema generation processes.
 
 ## Key Features
 
 - **Data Validation**: Easily validate data against schemas, ensuring its correctness, integrity and DCAT-AP compatibility.
 - **RDF Graph Conversion**: Convert data into RDF graphs effortlessly, enabling integration with RDF-based systems and applications.
 - **Schema Generation**: Generate JSON/YAML schemas compatible with the DCAT-AP v3 profile, facilitating interoperability and compliance with standards.
 - **Pedantic Integration**: Built upon the robust [Pydantic](https://docs.pydantic.dev/) library, leveraging its powerful validation capabilities and extending them for RDF handling.
```

