# Comparing `tmp/sapiopylib-2024.4.5a179.tar.gz` & `tmp/sapiopylib-2024.4.8a180.tar.gz`

## Comparing `sapiopylib-2024.4.5a179.tar` & `sapiopylib-2024.4.8a180.tar`

### file list

```diff
@@ -1,128 +1,129 @@
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/INSTALL.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/__init__.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/sapio_input_config.py
--rw-r--r--   0        0        0     2640 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/sapio_input_data.py
--rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/sapio_native_tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/csp/__init__.py
--rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/csp/data/PyCspFieldMap.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/csp/data/__init__.py
--rw-r--r--   0        0        0    36931 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/csp/data/plotly/PlotlyCspData.py
--rw-r--r--   0        0        0    10092 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/csp/data/plotly/PlotlyCspEnums.py
--rw-r--r--   0        0        0     8785 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/csp/data/plotly/SapioPyPlotly.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/csp/data/plotly/__init__.py
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/jarvis/JarvisDashboardWebhookContext.py
--rw-r--r--   0        0        0     4304 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/jarvis/QQPlotComputer.py
--rw-r--r--   0        0        0     7529 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/AccessionService.py
--rw-r--r--   0        0        0    12925 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/ClientCallbackService.py
--rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/CustomReportService.py
--rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/DashboardManager.py
--rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/DataMgmtService.py
--rw-r--r--   0        0        0    48718 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/DataRecordManagerService.py
--rw-r--r--   0        0        0     3015 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/DataService.py
--rw-r--r--   0        0        0     4414 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/DataTypeService.py
--rw-r--r--   0        0        0    23745 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/ELNService.py
--rw-r--r--   0        0        0     5010 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/GroupManagerService.py
--rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/MessengerService.py
--rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/PicklistService.py
--rw-r--r--   0        0        0     6824 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/ReportManager.py
--rw-r--r--   0        0        0    13871 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/User.py
--rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/UserManagerService.py
--rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/WebhookService.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/__init__.py
--rw-r--r--   0        0        0    25254 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/CustomReport.py
--rw-r--r--   0        0        0     8049 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/DataRecord.py
--rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/DataRecordBatchUpdate.py
--rw-r--r--   0        0        0     6208 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/DataRecordPaging.py
--rw-r--r--   0        0        0     6332 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/DataRecordSideLinkPaging.py
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/DateRange.py
--rw-r--r--   0        0        0     8241 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/Message.py
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/Picklist.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/SapioAccessType.py
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/Sort.py
--rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/TableColumn.py
--rw-r--r--   0        0        0     4711 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/UserInfo.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/__init__.py
--rw-r--r--   0        0        0    12264 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/chartdata/ChartData.py
--rw-r--r--   0        0        0    25239 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/chartdata/DashboardDefinition.py
--rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/chartdata/DashboardEnums.py
--rw-r--r--   0        0        0    21882 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/chartdata/DashboardSeries.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/chartdata/__init__.py
--rw-r--r--   0        0        0     7511 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/datatype/DataType.py
--rw-r--r--   0        0        0    62485 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/datatype/DataTypeComponent.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/datatype/DataTypeDescriptors.py
--rw-r--r--   0        0        0     3477 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/datatype/DataTypeEnums.py
--rw-r--r--   0        0        0    14183 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/datatype/DataTypeLayout.py
--rw-r--r--   0        0        0    55797 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/datatype/FieldDefinition.py
--rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/datatype/TemporaryDataType.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/datatype/__init__.py
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/eln/ElnEntryPosition.py
--rw-r--r--   0        0        0    19547 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/eln/ElnExperiment.py
--rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/eln/ElnExperimentRole.py
--rw-r--r--   0        0        0    29969 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/eln/ExperimentEntry.py
--rw-r--r--   0        0        0    26958 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/eln/ExperimentEntryCriteria.py
--rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/eln/SapioELNEnums.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/eln/__init__.py
--rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/eln/field_set.py
--rw-r--r--   0        0        0     6770 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/eln/protocol_template.py
--rw-r--r--   0        0        0    17530 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/reportbuilder/ReportBuilderEntryContext.py
--rw-r--r--   0        0        0    10998 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/reportbuilder/VeloxReportBuilder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/reportbuilder/__init__.py
--rw-r--r--   0        0        0    24025 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/webhook/ClientCallbackRequest.py
--rw-r--r--   0        0        0    11266 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/webhook/ClientCallbackResult.py
--rw-r--r--   0        0        0     8827 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/webhook/VeloxRules.py
--rw-r--r--   0        0        0    12323 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/webhook/WebhookContext.py
--rw-r--r--   0        0        0     3900 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/webhook/WebhookDirective.py
--rw-r--r--   0        0        0     4218 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/webhook/WebhookEnums.py
--rw-r--r--   0        0        0     6490 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/webhook/WebhookResult.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/webhook/__init__.py
--rw-r--r--   0        0        0     8809 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/CompresionUtil.py
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/DataRecordUtil.py
--rw-r--r--   0        0        0     4782 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/DataTypeCacheManager.py
--rw-r--r--   0        0        0     6499 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/FormBuilder.py
--rw-r--r--   0        0        0     5856 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/FoundationAccessioning.py
--rw-r--r--   0        0        0     5475 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/MultiMap.py
--rw-r--r--   0        0        0    16073 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/ProtocolUtils.py
--rw-r--r--   0        0        0    23715 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/Protocols.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/SapioDateUtils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/__init__.py
--rw-r--r--   0        0        0    20579 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/autopaging.py
--rw-r--r--   0        0        0     5589 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/recorddatasinks.py
--rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/plates/MultiLayerPlating.py
--rw-r--r--   0        0        0    23324 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/plates/MultiLayerPlatingUtils.py
--rw-r--r--   0        0        0     5277 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/plates/PlatingUtils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/plates/__init__.py
--rw-r--r--   0        0        0    28790 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/recordmodel/PyRecordModel.py
--rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/recordmodel/RecordModelEventBus.py
--rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/recordmodel/RecordModelEvents.py
--rw-r--r--   0        0        0    44895 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/recordmodel/RecordModelManager.py
--rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/recordmodel/RecordModelUtil.py
--rw-r--r--   0        0        0    13745 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/recordmodel/RecordModelWrapper.py
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/recordmodel/RelationshipPath.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/recordmodel/__init__.py
--rw-r--r--   0        0        0     8051 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/recordmodel/ancestry.py
--rw-r--r--   0        0        0    18003 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/recordmodel/properties.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/src/sapiopylib/utils/string.py
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/tests/EmailAttachmentDataTest.py
--rw-r--r--   0        0        0    10694 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/tests/FR-51536_test.py
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/tests/FR-51549_test.py
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/tests/FR-51551_test.py
--rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/tests/FR-51635_test.py
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/tests/FR-51821_test.py
--rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/tests/FR-51846_test.py
--rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/tests/FR-51847_test.py
--rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/tests/FR-51849_test.py
--rw-r--r--   0        0        0     6430 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/tests/FR-52100_test.py
--rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/tests/PR-51537_test.py
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/tests/PR-51547.py
--rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/tests/PR-51842_test.py
--rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/tests/PR-51853_test.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/tests/PR-51856_test.py
--rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/tests/PR-51964_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/tests/__init__.py
--rw-r--r--   0        0        0  1468866 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/tests/data_type_models.py
--rw-r--r--   0        0        0    12255 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/tests/resources/fr-51846.ssg
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/.gitignore
--rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/LICENSE
--rw-r--r--   0        0        0     5244 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/README.md
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/pyproject.toml
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 sapiopylib-2024.4.5a179/PKG-INFO
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/INSTALL.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/__init__.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/sapio_input_config.py
+-rw-r--r--   0        0        0     2640 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/sapio_input_data.py
+-rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/sapio_native_tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/csp/__init__.py
+-rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/csp/data/PyCspFieldMap.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/csp/data/__init__.py
+-rw-r--r--   0        0        0    36931 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/csp/data/plotly/PlotlyCspData.py
+-rw-r--r--   0        0        0    10092 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/csp/data/plotly/PlotlyCspEnums.py
+-rw-r--r--   0        0        0     8785 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/csp/data/plotly/SapioPyPlotly.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/csp/data/plotly/__init__.py
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/jarvis/JarvisDashboardWebhookContext.py
+-rw-r--r--   0        0        0     4304 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/jarvis/QQPlotComputer.py
+-rw-r--r--   0        0        0     7529 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/AccessionService.py
+-rw-r--r--   0        0        0    13219 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/ClientCallbackService.py
+-rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/CustomReportService.py
+-rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/DashboardManager.py
+-rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/DataMgmtService.py
+-rw-r--r--   0        0        0    48718 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/DataRecordManagerService.py
+-rw-r--r--   0        0        0     3015 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/DataService.py
+-rw-r--r--   0        0        0     4414 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/DataTypeService.py
+-rw-r--r--   0        0        0    23745 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/ELNService.py
+-rw-r--r--   0        0        0     5010 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/GroupManagerService.py
+-rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/MessengerService.py
+-rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/PicklistService.py
+-rw-r--r--   0        0        0     6824 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/ReportManager.py
+-rw-r--r--   0        0        0    14804 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/User.py
+-rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/UserManagerService.py
+-rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/WebhookService.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/__init__.py
+-rw-r--r--   0        0        0    25254 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/CustomReport.py
+-rw-r--r--   0        0        0     8049 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/DataRecord.py
+-rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/DataRecordBatchUpdate.py
+-rw-r--r--   0        0        0     6208 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/DataRecordPaging.py
+-rw-r--r--   0        0        0     6332 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/DataRecordSideLinkPaging.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/DateRange.py
+-rw-r--r--   0        0        0     8241 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/Message.py
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/Picklist.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/SapioAccessType.py
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/Sort.py
+-rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/TableColumn.py
+-rw-r--r--   0        0        0     4711 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/UserInfo.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/__init__.py
+-rw-r--r--   0        0        0    12264 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/chartdata/ChartData.py
+-rw-r--r--   0        0        0    25239 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/chartdata/DashboardDefinition.py
+-rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/chartdata/DashboardEnums.py
+-rw-r--r--   0        0        0    21882 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/chartdata/DashboardSeries.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/chartdata/__init__.py
+-rw-r--r--   0        0        0     7511 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/datatype/DataType.py
+-rw-r--r--   0        0        0    62485 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/datatype/DataTypeComponent.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/datatype/DataTypeDescriptors.py
+-rw-r--r--   0        0        0     3477 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/datatype/DataTypeEnums.py
+-rw-r--r--   0        0        0    14183 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/datatype/DataTypeLayout.py
+-rw-r--r--   0        0        0    55797 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/datatype/FieldDefinition.py
+-rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/datatype/TemporaryDataType.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/datatype/__init__.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/eln/ElnEntryPosition.py
+-rw-r--r--   0        0        0    19547 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/eln/ElnExperiment.py
+-rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/eln/ElnExperimentRole.py
+-rw-r--r--   0        0        0    29969 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/eln/ExperimentEntry.py
+-rw-r--r--   0        0        0    26958 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/eln/ExperimentEntryCriteria.py
+-rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/eln/SapioELNEnums.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/eln/__init__.py
+-rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/eln/field_set.py
+-rw-r--r--   0        0        0     6770 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/eln/protocol_template.py
+-rw-r--r--   0        0        0    17530 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/reportbuilder/ReportBuilderEntryContext.py
+-rw-r--r--   0        0        0    10998 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/reportbuilder/VeloxReportBuilder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/reportbuilder/__init__.py
+-rw-r--r--   0        0        0    24025 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/webhook/ClientCallbackRequest.py
+-rw-r--r--   0        0        0    11266 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/webhook/ClientCallbackResult.py
+-rw-r--r--   0        0        0     8827 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/webhook/VeloxRules.py
+-rw-r--r--   0        0        0    12323 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/webhook/WebhookContext.py
+-rw-r--r--   0        0        0     3900 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/webhook/WebhookDirective.py
+-rw-r--r--   0        0        0     4218 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/webhook/WebhookEnums.py
+-rw-r--r--   0        0        0     6490 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/webhook/WebhookResult.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/webhook/__init__.py
+-rw-r--r--   0        0        0     8809 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/CompresionUtil.py
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/DataRecordUtil.py
+-rw-r--r--   0        0        0     4782 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/DataTypeCacheManager.py
+-rw-r--r--   0        0        0     6499 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/FormBuilder.py
+-rw-r--r--   0        0        0     5856 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/FoundationAccessioning.py
+-rw-r--r--   0        0        0     5475 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/MultiMap.py
+-rw-r--r--   0        0        0    16073 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/ProtocolUtils.py
+-rw-r--r--   0        0        0    23715 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/Protocols.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/SapioDateUtils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/__init__.py
+-rw-r--r--   0        0        0    20579 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/autopaging.py
+-rw-r--r--   0        0        0     7225 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/recorddatasinks.py
+-rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/plates/MultiLayerPlating.py
+-rw-r--r--   0        0        0    23324 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/plates/MultiLayerPlatingUtils.py
+-rw-r--r--   0        0        0     5277 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/plates/PlatingUtils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/plates/__init__.py
+-rw-r--r--   0        0        0    28790 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/recordmodel/PyRecordModel.py
+-rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/recordmodel/RecordModelEventBus.py
+-rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/recordmodel/RecordModelEvents.py
+-rw-r--r--   0        0        0    44895 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/recordmodel/RecordModelManager.py
+-rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/recordmodel/RecordModelUtil.py
+-rw-r--r--   0        0        0    13745 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/recordmodel/RecordModelWrapper.py
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/recordmodel/RelationshipPath.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/recordmodel/__init__.py
+-rw-r--r--   0        0        0     8051 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/recordmodel/ancestry.py
+-rw-r--r--   0        0        0    18003 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/recordmodel/properties.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/utils/string.py
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/tests/EmailAttachmentDataTest.py
+-rw-r--r--   0        0        0    10694 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/tests/FR-51536_test.py
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/tests/FR-51549_test.py
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/tests/FR-51551_test.py
+-rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/tests/FR-51635_test.py
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/tests/FR-51821_test.py
+-rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/tests/FR-51846_test.py
+-rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/tests/FR-51847_test.py
+-rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/tests/FR-51849_test.py
+-rw-r--r--   0        0        0     8279 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/tests/FR-52100_test.py
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/tests/PR-51537_test.py
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/tests/PR-51547.py
+-rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/tests/PR-51842_test.py
+-rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/tests/PR-51853_test.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/tests/PR-51856_test.py
+-rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/tests/PR-51964_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/tests/__init__.py
+-rw-r--r--   0        0        0  1468866 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/tests/data_type_models.py
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/tests/resources/NAC28735.fa
+-rw-r--r--   0        0        0    12255 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/tests/resources/fr-51846.ssg
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/.gitignore
+-rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/LICENSE
+-rw-r--r--   0        0        0     5244 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/README.md
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/pyproject.toml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/PKG-INFO
```

### Comparing `sapiopylib-2024.4.5a179/INSTALL.md` & `sapiopylib-2024.4.8a180/INSTALL.md`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/sapio_input_data.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/sapio_input_data.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/sapio_native_tools.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/sapio_native_tools.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/csp/data/PyCspFieldMap.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/csp/data/PyCspFieldMap.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/csp/data/plotly/PlotlyCspData.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/csp/data/plotly/PlotlyCspData.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/csp/data/plotly/PlotlyCspEnums.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/csp/data/plotly/PlotlyCspEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/csp/data/plotly/SapioPyPlotly.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/csp/data/plotly/SapioPyPlotly.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/jarvis/JarvisDashboardWebhookContext.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/jarvis/JarvisDashboardWebhookContext.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/jarvis/QQPlotComputer.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/jarvis/QQPlotComputer.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/AccessionService.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/AccessionService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/ClientCallbackService.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/ClientCallbackService.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,33 +40,33 @@
 
     def display_info(self, msg: str) -> None:
         """
         Displays the provided method to the current user in a dialog.  This method is only available when using the credentials provided in the context of a webhook endpoint.
         :param msg: The message to be displayed.
         """
         url = '/clientcallback/display/info'
-        response = self.user.post(url, payload=msg)
+        response = self.user.post(url, payload=msg, is_payload_plain_text=True)
         self.user.raise_for_status(response)
 
     def display_warning(self, msg: str) -> None:
         """
         Displays the provided warning message to the current user in a dialog. This method is only available when using the credentials provided in the context of a webhook endpoint.
         :param msg: The warning message to be displayed.
         """
         url = '/clientcallback/display/warning'
-        response = self.user.post(url, payload=msg)
+        response = self.user.post(url, payload=msg, is_payload_plain_text=True)
         self.user.raise_for_status(response)
 
     def display_error(self, msg: str) -> None:
         """
         Displays the provided error message to the current user in a dialog. This method is only available when using the credentials provided in the context of a webhook endpoint.
         :param msg: The error message to be displayed.
         """
         url = '/clientcallback/display/error'
-        response = self.user.post(url, payload=msg)
+        response = self.user.post(url, payload=msg, is_payload_plain_text=True)
         self.user.raise_for_status(response)
 
     def display_popup(self, request: DisplayPopupRequest) -> None:
         """
         Display a toastr popup message in user's log in session screen.
         :param request: The request to be displayed.
         """
@@ -77,16 +77,16 @@
     def show_file_dialog(self, request: FilePromptRequest, data_sink: Callable[[bytes], None]) -> str | None:
         """
         Displays a file prompt dialog to the current user. This method is only available when using the credentials provided in the context of a webhook endpoint.
         The file dialog will be displayed with the options provided in the request. User's browser will upload this file which will be consumed by the data sink.
         :param request: The request for the file prompt dialog.
         :param data_sink: The data sink the process the incoming data chunks in sequence.
         """
-        url = '/clientcallback/show/filedialog'
-        response = self.user.consume_octet_stream_post(url, data_sink)
+        url = '/clientcallback/filedialog'
+        response = self.user.consume_octet_stream_post(url, data_sink, payload=request.to_json())
         self.user.raise_for_status(response)
         header: str | None = response.headers.get("Content-Disposition")
         if not header:
             return None
         match = re.search("attachment; filename=\"(.+)\"", header)
         if not match:
             return None
@@ -94,15 +94,15 @@
 
     def get_file(self, fake_file_path: str, data_sink: Callable[[bytes], None]) -> None:
         """
         Retrieve a file provided by a fake file path that is only valid in this session.
         :param fake_file_path: The fake file path that points to the file content in this session.
         :param data_sink: The data sink the process the incoming data chunks in sequence.
         """
-        url = '/clientcallback/get/file'
+        url = '/clientcallback/file'
         params = {'filePath': fake_file_path}
         response = self.user.consume_octet_stream_get(url, data_sink, params=params)
         self.user.raise_for_status(response)
 
     def show_multi_file_dialog(self, request: MultiFilePromptRequest) -> list[str] | None:
         """
         Prompt the user (client) for a file path or list of file paths with a file dialog that allows multiple
@@ -111,24 +111,27 @@
 
         :param request:  the options for the file dialog
         :return: the list of file names (full paths) if the user selected something, or null if they hit cancel
         """
         url = '/clientcallback/multifiledialog'
         response = self.user.post(url, payload=request.to_json())
         self.user.raise_for_status(response)
-        return response.json()
+        return self.user.get_json_data_or_none(response)
 
     def send_file(self, default_file_name: str, request_file_name: bool, data: IO) -> None:
         """
         Send a file to the user in the system that invoked the webhook.
         This method is only available when using the credentials provided in the context of a webhook endpoint.
         :param default_file_name: The default name of the file being sent.
         :param request_file_name: Whether the callback should ask the user to provide a file name for the sent file.
-        :param data: The file stream to send to the user.
+        :param data: The file stream to send to the user. The mode of IO MUST BE 'rb' (read-binary), even if it is a text file.
         """
+        mode: str = data.mode
+        if mode != 'rb':
+            raise IOError("When sending file through sapiopylib, the open mode must be of rb (read-binary) even for text files.")
         url = '/clientcallback/sendfile'
         params = {
             "defaultFileName": default_file_name,
             "requestFileName": request_file_name
         }
         response = self.user.post_data_stream(url, data, params)
         self.user.raise_for_status(response)
@@ -139,101 +142,92 @@
         using the dialog and returns their selection to the user. This method is only available when using the credentials provided in the context of a webhook endpoint.
         :param request: The request containing the available records to select.
         :return: A list of the selected records.  If no records are selected, an empty list is returned.  If the user cancels the dialog, then None will be returned.
         """
         url = '/clientcallback/datarecordselectiondialog'
         response = self.user.post(url, payload=request.to_json())
         self.user.raise_for_status(response)
-        if not response.json():
-            return None
-        return response.json()
+        return self.user.get_json_data_or_none(response)
 
     def show_table_entry_dialog(self, request: TableEntryDialogRequest) -> list[dict[str, Any]] | None:
         """
         Show a table dialog with the specified title, optional message and a table populated with default values
         that returns value entered by the user for each cell on the table.  The table is defined through attributes
         specified on the request provided to the method.
         The request defines the structure of the table and the request's field map list defines the data that will be displayed in the table when it is first displayed to the user.
         This method is only available when using the credentials provided in the context of a webhook endpoint.
         :param request: the criteria object defining how the table should appear and function.
         :return: map of data entered by user keyed by data field name
         """
         url = '/clientcallback/tableentrydialog'
         response = self.user.post(url, payload=request.to_json())
         self.user.raise_for_status(response)
-        if not response.json():
-            return None
-        return response.json()
+        return self.user.get_json_data_or_none(response)
 
     def data_record_form_view_dialog(self, request: DataRecordDialogRequest) -> bool:
         """
         Show a dialog with the specified title.  The dialog will display the given dataRecord using the provided
         DataTypeLayout.  This dialog can display all normal record toolbar buttons including save and cancel.  Use this
         when it is safe for the user transaction to be committed or rolled back. This method is only available when using the
         credentials provided in the context of a webhook endpoint.
         :param request: The criteria object that defines how this dialog will be displayed.  This criteria
         includes options to enable or disable core features, specify plugins that should be displayed, set the layout that should be used, set the title of the dialog, etc.
         :return: true if the OK button was pressed. false if the Cancel button was pressed by user.
         """
         url = '/clientcallback/dataRecordFormViewDialog'
         response = self.user.post(url, payload=request.to_json())
         self.user.raise_for_status(response)
-        return response.json()
+        return self.user.get_json_data_or_none(response)
 
     def show_form_entry_dialog(self, request: FormEntryDialogRequest) -> dict[str, Any] | None:
         """
         Show a dialog with the specified title, optional message and list of controls that returns value entered by the
         user for each control.  The controls are built off of the TemporaryDataType that is created by the developer or
         that mirrors actual an actual type in the system, but the type does not have actual data record mappings.
         This method is only available when using the credentials provided in the context of a webhook endpoint.
         :param request: options to use when displaying the dialog
         :return: map of data entered by user keyed by data field name. If user did not respond by existing the dialog, None is returned.
         """
         url = '/clientcallback/formentrydialog'
         response = self.user.post(url, payload=request.to_json())
         self.user.raise_for_status(response)
-        if not response.json():
-            return None
-        return response.json()
+        return self.user.get_json_data_or_none(response)
 
     def show_list_dialog(self, request: ListDialogRequest) -> list[str] | None:
         """
         Show a list box to the user to make a selection from a list of choices.
         This method is only available when using the credentials provided in the context of a webhook endpoint.
         :param request: the details about how the dialog should be displayed
         :return: the list of selected strings, or None if they hit cancel
         """
         url = '/clientcallback/selectionlistdialog'
         response = self.user.post(url, payload=request.to_json())
         self.user.raise_for_status(response)
-        if not response.json():
-            return None
-        return response.json()
+        return self.user.get_json_data_or_none(response)
 
     def show_option_dialog(self, request: OptionDialogRequest) -> int | None:
         """
         Show a dialog with the specified title, message and list of buttons that returns index of selected button.
         This method is only available when using the credentials provided in the context of a webhook endpoint.
 
         :param request: options to use when displaying the dialog
         :return: the index of the button that the user choose or {@code null} if the user cancelled the dialog.
         """
         url = '/clientcallback/custombuttondialog'
         response = self.user.post(url, payload=request.to_json())
         self.user.raise_for_status(response)
-        if not response.json():
-            return None
-        return response.json()
+        return self.user.get_json_data_or_none(response)
 
     def show_input_selection_dialog(self, request: InputSelectionRequest) -> InputSelectionResult | None:
         """
         Shows an input-selection dialog with configurations for enabling tabs for tree navigation, reports, and quick search.
         Allows the user to select records using the dialog and returns their selection to the user.
         :param request: The request defining the options for the dialog
         :return: A list of the selected data records.  If no records are selected, an empty list is returned.  If the user cancels the dialog, then None will be returned.
         """
         url = '/clientcallback/inputselectiondialog'
         response = self.user.post(url, payload=request.to_json())
         self.user.raise_for_status(response)
-        if not response.json():
+        json = self.user.get_json_data_or_none(response)
+        if not json:
             return None
-        return cast(InputSelectionResult, ClientCallbackResultParser.parse_client_callback_result(response.json()))
+        return cast(InputSelectionResult, ClientCallbackResultParser.parse_client_callback_result(json))
```

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/CustomReportService.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/CustomReportService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/DashboardManager.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/DashboardManager.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/DataMgmtService.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/DataMgmtService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/DataRecordManagerService.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/DataRecordManagerService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/DataService.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/DataService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/DataTypeService.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/DataTypeService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/ELNService.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/ELNService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/GroupManagerService.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/GroupManagerService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/MessengerService.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/MessengerService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/PicklistService.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/PicklistService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/ReportManager.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/ReportManager.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/User.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/User.py`

 * *Files 4% similar despite different names*

```diff
@@ -173,18 +173,25 @@
     @staticmethod
     def is_null_response(response: Response):
         text_response = response.text
         if text_response and text_response.strip():
             return False
         return True
 
-    def post(self, url_sub_path: str, params: Optional[dict] = None, payload=None) -> Response:
-        return requests.post(self.url + url_sub_path, params=params, json=payload,
-                             headers=self.get_http_headers(), verify=self.verify_ssl_cert,
-                             timeout=self.timeout_seconds)
+    def post(self, url_sub_path: str, params: Optional[dict] = None, payload=None, is_payload_plain_text: bool = False) -> Response:
+        headers = self.get_http_headers()
+        if is_payload_plain_text:
+            headers['Content-Type'] = 'application/json'
+            return requests.post(self.url + url_sub_path, params=params, data=payload,
+                                 headers=headers, verify=self.verify_ssl_cert,
+                                 timeout=self.timeout_seconds)
+        else:
+            return requests.post(self.url + url_sub_path, params=params, json=payload,
+                                 headers=headers, verify=self.verify_ssl_cert,
+                                 timeout=self.timeout_seconds)
 
     def post_data_stream(self, url_sub_path: str, data_stream: IO, params: Optional[dict] = None):
         headers = self.get_http_headers()
         headers['Content-Type'] = 'application/octet-stream'
         return requests.post(self.url + url_sub_path, params=params, data=data_stream,
                              headers=headers, verify=self.verify_ssl_cert,
                              timeout=self.timeout_seconds)
@@ -244,14 +251,25 @@
     def raise_for_status(response: Response):
         try:
             response.raise_for_status()
         except requests.exceptions.HTTPError as e:
             raise SapioServerException(e)
 
     @staticmethod
+    def get_json_data_or_none(response: Response) -> Any | None:
+        """
+        If the response's content can be parsed into json, return its JSON representation Otherwise, return None object.
+        :param response: The REST response to parse.
+        :return: Return None object if the "requests" API would be unable to parse the response into a JSON structure. Otherwise, return the JSON structure.
+        """
+        if not response.text:
+            return None
+        return response.json()
+
+    @staticmethod
     def build_url(url_list: List[str]) -> str:
         url = '/'.join(urllib.parse.quote(x) for x in url_list)
         if not url.startswith('/'):
             url = '/' + url
         return url
 
     def log_info(self, msg: str) -> None:
```

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/UserManagerService.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/UserManagerService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/WebhookService.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/WebhookService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/CustomReport.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/CustomReport.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/DataRecord.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/DataRecord.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/DataRecordBatchUpdate.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/DataRecordBatchUpdate.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/DataRecordPaging.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/DataRecordPaging.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/DataRecordSideLinkPaging.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/DataRecordSideLinkPaging.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/DateRange.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/DateRange.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/Message.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/Message.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/Picklist.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/Picklist.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/Sort.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/Sort.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/TableColumn.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/TableColumn.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/UserInfo.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/UserInfo.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/chartdata/ChartData.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/chartdata/ChartData.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/chartdata/DashboardDefinition.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/chartdata/DashboardDefinition.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/chartdata/DashboardEnums.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/chartdata/DashboardEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/chartdata/DashboardSeries.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/chartdata/DashboardSeries.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/datatype/DataType.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/datatype/DataType.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/datatype/DataTypeComponent.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/datatype/DataTypeComponent.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/datatype/DataTypeDescriptors.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/datatype/DataTypeDescriptors.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/datatype/DataTypeEnums.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/datatype/DataTypeEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/datatype/DataTypeLayout.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/datatype/DataTypeLayout.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/datatype/FieldDefinition.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/datatype/FieldDefinition.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/datatype/TemporaryDataType.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/datatype/TemporaryDataType.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/eln/ElnEntryPosition.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/eln/ElnEntryPosition.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/eln/ElnExperiment.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/eln/ElnExperiment.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/eln/ElnExperimentRole.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/eln/ElnExperimentRole.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/eln/ExperimentEntry.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/eln/ExperimentEntry.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/eln/ExperimentEntryCriteria.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/eln/ExperimentEntryCriteria.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/eln/SapioELNEnums.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/eln/SapioELNEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/eln/field_set.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/eln/field_set.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/eln/protocol_template.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/eln/protocol_template.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/reportbuilder/ReportBuilderEntryContext.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/reportbuilder/ReportBuilderEntryContext.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/reportbuilder/VeloxReportBuilder.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/reportbuilder/VeloxReportBuilder.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/webhook/ClientCallbackRequest.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/webhook/ClientCallbackRequest.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/webhook/ClientCallbackResult.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/webhook/ClientCallbackResult.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/webhook/VeloxRules.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/webhook/VeloxRules.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/webhook/WebhookContext.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/webhook/WebhookContext.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/webhook/WebhookDirective.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/webhook/WebhookDirective.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/webhook/WebhookEnums.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/webhook/WebhookEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/pojo/webhook/WebhookResult.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/webhook/WebhookResult.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/CompresionUtil.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/CompresionUtil.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/DataRecordUtil.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/DataRecordUtil.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/DataTypeCacheManager.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/DataTypeCacheManager.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/FormBuilder.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/FormBuilder.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/FoundationAccessioning.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/FoundationAccessioning.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/MultiMap.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/MultiMap.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/ProtocolUtils.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/ProtocolUtils.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/Protocols.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/Protocols.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/SapioDateUtils.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/SapioDateUtils.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/autopaging.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/autopaging.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/recorddatasinks.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/recorddatasinks.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # FR-51549 Added class
 # Holds utility classes to handle data record streaming common operations.
 from abc import ABC, abstractmethod
 from io import BytesIO
 from pathlib import Path
 from typing import IO
 
+from sapiopylib.rest.pojo.webhook.ClientCallbackRequest import FilePromptRequest
+
 from sapiopylib.rest.DataService import DataManager
 
 from sapiopylib.rest.DataMgmtService import DataMgmtServer
 from sapiopylib.rest.DataRecordManagerService import DataRecordManager
 from sapiopylib.rest.User import SapioUser
 from sapiopylib.rest.pojo.DataRecord import DataRecord
 
@@ -35,42 +37,74 @@
     def __exit__(self, exc_type, exc_val, exc_tb):
         pass
 
     @abstractmethod
     def consume_data(self, chunk: bytes, context_obj: IO) -> None:
         pass
 
-    def get_record_image(self, record: DataRecord):
+    def get_record_image(self, record: DataRecord) -> None:
         """
         Consume the record image using the specified data sink's method.
         """
         with self as io:
             def do_consume(chunk: bytes) -> None:
                 return self.consume_data(chunk, io)
+
             self._data_record_manager.get_record_image(record, do_consume)
 
-    def get_attachment_data(self, record: DataRecord):
+    def get_attachment_data(self, record: DataRecord) -> None:
         """
         Consume the attachment data using the specified data sink's method.
         """
         with self as io:
             def do_consume(chunk: bytes) -> None:
                 return self.consume_data(chunk, io)
+
             self._data_record_manager.get_attachment_data(record, do_consume)
 
-    def export_to_xml(self, records: list[DataRecord], recursive: bool = True, data_types_to_exclude: list[str | None] = None):
+    def export_to_xml(self, records: list[DataRecord], recursive: bool = True,
+                      data_types_to_exclude: list[str | None] = None):
         """
         Export the selected files into an .xml.zip file format, to be able to be imported later via data manager.
         """
         with self as io:
             def do_consume(chunk: bytes) -> None:
                 return self.consume_data(chunk, io)
+
             self._data_manager.export_to_xml(records, do_consume,
                                              recursive=recursive, data_types_to_exclude=data_types_to_exclude)
 
+    def upload_single_file_to_webhook_server(self, request: FilePromptRequest) -> None:
+        """
+        Requests user to upload a single file in a browser file window, and then receive the file into the sink.
+        This method requires the session to have active client callback object (such as from webhook).
+        :param request The file prompt client callback request object.
+        """
+        with self as io:
+            def do_consume(chunk: bytes) -> None:
+                return self.consume_data(chunk, io)
+
+            client_callback = DataMgmtServer.get_client_callback(self._user)
+            client_callback.show_file_dialog(request, do_consume)
+
+    def consume_client_callback_file_path_data(self, fake_file_path: str) -> None:
+        """
+        To be used together with a multi-file dialog. When a multi-file dialog returns sucessfully, a list of fake file paths are given to the webhook server as a response object.
+        For every one of these fake file paths, we should be able to read the data inside.
+
+        This method requires the session to have active client callback object (such as from webhook).
+        :param fake_file_path: The particular fake file path we are reading in the list.
+        """
+        with self as io:
+            def do_consume(chunk: bytes) -> None:
+                return self.consume_data(chunk, io)
+
+            client_callback = DataMgmtServer.get_client_callback(self._user)
+            client_callback.get_file(fake_file_path, do_consume)
+
 
 class FileSaveRecordDataSink(AbstractRecordDataSink):
     """
     This data sink stores the data into a specific file path.
     """
     _file_path_to_save: Path
     _file_obj: IO
```

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/plates/MultiLayerPlating.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/plates/MultiLayerPlating.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/plates/MultiLayerPlatingUtils.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/plates/MultiLayerPlatingUtils.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/plates/PlatingUtils.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/plates/PlatingUtils.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/recordmodel/PyRecordModel.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/recordmodel/PyRecordModel.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/recordmodel/RecordModelEventBus.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/recordmodel/RecordModelEventBus.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/recordmodel/RecordModelEvents.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/recordmodel/RecordModelEvents.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/recordmodel/RecordModelManager.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/recordmodel/RecordModelManager.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/recordmodel/RecordModelUtil.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/recordmodel/RecordModelUtil.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/recordmodel/RecordModelWrapper.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/recordmodel/RecordModelWrapper.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/recordmodel/RelationshipPath.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/recordmodel/RelationshipPath.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/recordmodel/ancestry.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/recordmodel/ancestry.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/rest/utils/recordmodel/properties.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/recordmodel/properties.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/src/sapiopylib/utils/string.py` & `sapiopylib-2024.4.8a180/src/sapiopylib/utils/string.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/tests/EmailAttachmentDataTest.py` & `sapiopylib-2024.4.8a180/tests/EmailAttachmentDataTest.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/tests/FR-51536_test.py` & `sapiopylib-2024.4.8a180/tests/FR-51536_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/tests/FR-51549_test.py` & `sapiopylib-2024.4.8a180/tests/FR-51549_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/tests/FR-51551_test.py` & `sapiopylib-2024.4.8a180/tests/FR-51551_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/tests/FR-51635_test.py` & `sapiopylib-2024.4.8a180/tests/FR-51635_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/tests/FR-51821_test.py` & `sapiopylib-2024.4.8a180/tests/FR-51821_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/tests/FR-51846_test.py` & `sapiopylib-2024.4.8a180/tests/FR-51846_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/tests/FR-51847_test.py` & `sapiopylib-2024.4.8a180/tests/FR-51847_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/tests/FR-51849_test.py` & `sapiopylib-2024.4.8a180/tests/FR-51849_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/tests/FR-52100_test.py` & `sapiopylib-2024.4.8a180/tests/FR-52100_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # This test needs to be run by a webhook user. So it doesn't fit the regular unittest.testcase.
+from sapiopylib.rest.utils.recorddatasinks import InMemoryRecordDataSink, InMemoryStringDataSink
+
 from sapiopylib.rest.pojo.datatype.FieldDefinition import *
 
 from sapiopylib.rest.utils.FormBuilder import FormBuilder
 
 from sapiopylib.rest.DataMgmtService import DataMgmtServer
 from sapiopylib.rest.pojo.webhook.ClientCallbackRequest import *
 
@@ -14,38 +16,45 @@
 
 
 class TestDisplayInfo(AbstractWebhookHandler):
 
     def run(self, context: SapioWebhookContext) -> SapioWebhookResult:
         user = context.user
         client_callback = DataMgmtServer.get_client_callback(user)
-        client_callback.display_info("Info message 1")
-        client_callback.display_warning("Info message 2")
-        client_callback.display_error("Info message 3")
+        client_callback.display_info("Info message 1\nInfo message 2")
+        client_callback.display_warning("Info message 1\nInfo message 2")
+        client_callback.display_error("Info message 1\nInfo message 2")
         client_callback.display_popup(DisplayPopupRequest("Test Title", "Test Message", PopupType.Success))
         return SapioWebhookResult(True)
 
 class TestUserInputDialogs(AbstractWebhookHandler):
 
     def run(self, context: SapioWebhookContext) -> SapioWebhookResult:
         user = context.user
         client_callback = DataMgmtServer.get_client_callback(user)
         selected_option: int | None = client_callback.show_option_dialog(OptionDialogRequest("Select Input Dialog Option",
                                                                "Please make a selection in one of these options to test ^_^.",
-                                                               ['Abort', 'Field Entry', 'Table Entry', 'List', 'Record IDV', 'Record Selection']))
+                                                               ['Abort', 'Field Entry', 'Table Entry', 'List', 'Record IDV', 'Record Selection',
+                                                                "Download", "Upload", "Upload Multiple"]))
         if selected_option == 1:
             self.test_field_entry(context)
         elif selected_option == 2:
             self.test_table_entry(context)
         elif selected_option == 3:
             self.test_list(context)
         elif selected_option == 4:
             self.test_record_idv(context)
         elif selected_option == 5:
             self.test_record_selection(context)
+        elif selected_option == 6:
+            self.test_download_file_to_user(context)
+        elif selected_option == 7:
+            self.test_upload_file_from_user(context)
+        elif selected_option == 8:
+            self.test_multi_upload_file_from_user(context)
         return SapioWebhookResult(True)
 
     def test_field_entry(self, context):
         user = context.user
         client_callback = DataMgmtServer.get_client_callback(user)
         fb: FormBuilder = FormBuilder()
         fb.add_field(VeloxStringFieldDefinition(fb.get_data_type_name(), "Test1", "Test 1"))
@@ -103,18 +112,44 @@
         fb.add_field(VeloxBooleanFieldDefinition(fb.get_data_type_name(), "Test2", "Test 2"))
         temp_dt: TemporaryDataType = fb.get_temporary_data_type()
         initial_field_map_list: list[dict[str, Any]] = []
         initial_field_map_list.append({"Test1": "aaa", "Test2": True})
         initial_field_map_list.append({"Test1": "bbb", "Test2": False})
         selection_result = client_callback.show_data_record_selection_dialog(DataRecordSelectionRequest(
             "Test", "Tests", temp_dt.get_field_def_list(), initial_field_map_list, multi_select=True))
-        if not selection_result:
+        if selection_result is None:
             client_callback.display_info("User has cancelled record selection.")
         else:
             client_callback.display_info("User has selected: " + str(selection_result))
 
+    def test_download_file_to_user(self, context):
+        user = context.user
+        client_callback = DataMgmtServer.get_client_callback(user)
+
+        with open('resources/NAC28735.fa', 'rb') as io:
+            client_callback.send_file("downloaded.fa", True, io)
+
+    def test_upload_file_from_user(self, context):
+        user = context.user
+        sink = InMemoryStringDataSink(user)
+        sink.upload_single_file_to_webhook_server(FilePromptRequest("Upload me a text file please...", file_extension=".txt"))
+        client_callback = DataMgmtServer.get_client_callback(user)
+        client_callback.display_info("Here is what you have uploaded: \n" + sink.text)
+
+    def test_multi_upload_file_from_user(self, context):
+        user = context.user
+        client_callback = DataMgmtServer.get_client_callback(user)
+        fake_file_path_list = client_callback.show_multi_file_dialog(MultiFilePromptRequest("Upload me multiple text files please...", file_extension=".txt"))
+        if not fake_file_path_list:
+            return
+        for fake_file_path in fake_file_path_list:
+            sink = InMemoryStringDataSink(user)
+            sink.consume_client_callback_file_path_data(fake_file_path)
+            client_callback.display_info("Received file content for '" + fake_file_path + "':\n" + sink.text)
+
+
 config: WebhookConfiguration = WebhookConfiguration(verify_sapio_cert=False, debug=True)
 config.register('/display_info_test', TestDisplayInfo)
 config.register('/dialog_test', TestUserInputDialogs)
 
 app = WebhookServerFactory.configure_flask_app(app=None, config=config)
-app.run(host="0.0.0.0", port=8099)
+app.run(host="0.0.0.0", port=8099)
```

### Comparing `sapiopylib-2024.4.5a179/tests/PR-51537_test.py` & `sapiopylib-2024.4.8a180/tests/PR-51537_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/tests/PR-51547.py` & `sapiopylib-2024.4.8a180/tests/PR-51547.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/tests/PR-51842_test.py` & `sapiopylib-2024.4.8a180/tests/PR-51842_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/tests/PR-51853_test.py` & `sapiopylib-2024.4.8a180/tests/PR-51853_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/tests/PR-51856_test.py` & `sapiopylib-2024.4.8a180/tests/PR-51856_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/tests/PR-51964_test.py` & `sapiopylib-2024.4.8a180/tests/PR-51964_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/tests/data_type_models.py` & `sapiopylib-2024.4.8a180/tests/data_type_models.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/tests/resources/fr-51846.ssg` & `sapiopylib-2024.4.8a180/tests/resources/fr-51846.ssg`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/LICENSE` & `sapiopylib-2024.4.8a180/LICENSE`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/README.md` & `sapiopylib-2024.4.8a180/README.md`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.5a179/pyproject.toml` & `sapiopylib-2024.4.8a180/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sapiopylib"
-version='2024.04.05a179'
+version='2024.04.08a180'
 authors = [
     { name="Yechen Qiao", email="yqiao@sapiosciences.com" },
 ]
 description = "Official Sapio Informatics Platform Python API"
 license = "MPL-2.0"
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `sapiopylib-2024.4.5a179/PKG-INFO` & `sapiopylib-2024.4.8a180/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sapiopylib
-Version: 2024.4.5a179
+Version: 2024.4.8a180
 Summary: Official Sapio Informatics Platform Python API
 Project-URL: Homepage, https://github.com/sapiosciences
 Project-URL: Bug Tracker, https://github.com/sapiosciences/sapio-py-tutorials/issues
 Author-email: Yechen Qiao <yqiao@sapiosciences.com>
 License-Expression: MPL-2.0
 License-File: LICENSE
 Keywords: eln,lims,rest,sapio
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: sapiopylib Version: 2024.4.5a179 Summary: Official
+Metadata-Version: 2.3 Name: sapiopylib Version: 2024.4.8a180 Summary: Official
 Sapio Informatics Platform Python API Project-URL: Homepage, https://
 github.com/sapiosciences Project-URL: Bug Tracker, https://github.com/
 sapiosciences/sapio-py-tutorials/issues Author-email: Yechen Qiao
 sapiosciences.com> License-Expression: MPL-2.0 License-File: LICENSE Keywords:
 eln,lims,rest,sapio Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Healthcare Industry Classifier: Intended Audience :: Science/Research
```

