# Comparing `tmp/RSTAB-1.9.3.tar.gz` & `tmp/RSTAB-1.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RSTAB-1.9.3.tar", last modified: Wed Jan 31 07:50:35 2024, max compression
+gzip compressed data, was "RSTAB-1.9.5.tar", last modified: Mon Apr  8 12:33:46 2024, max compression
```

## Comparing `RSTAB-1.9.3.tar` & `RSTAB-1.9.5.tar`

### file list

```diff
@@ -1,153 +1,152 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 07:50:35.881011 RSTAB-1.9.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 07:50:35.861011 RSTAB-1.9.3/Examples/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 07:50:26.000000 RSTAB-1.9.3/Examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-01-31 07:50:26.000000 RSTAB-1.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-01-31 07:50:26.000000 RSTAB-1.9.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10615 2024-01-31 07:50:35.881011 RSTAB-1.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9988 2024-01-31 07:50:26.000000 RSTAB-1.9.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 07:50:35.865011 RSTAB-1.9.3/RSTAB/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 07:50:35.865011 RSTAB-1.9.3/RSTAB/AluminumDesign/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/AluminumDesign/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/AluminumDesign/aluminumSLSConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/AluminumDesign/aluminumULSConfiguration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 07:50:35.865011 RSTAB-1.9.3/RSTAB/BasicObjects/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/BasicObjects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13377 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/BasicObjects/coordinateSystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/BasicObjects/material.py
--rw-r--r--   0 runner    (1001) docker     (127)    89338 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/BasicObjects/member.py
--rw-r--r--   0 runner    (1001) docker     (127)     5147 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/BasicObjects/memberSet.py
--rw-r--r--   0 runner    (1001) docker     (127)    14897 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/BasicObjects/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/BasicObjects/section.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 07:50:35.869011 RSTAB-1.9.3/RSTAB/Calculate/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/Calculate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/Calculate/memberDivision.py
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/Calculate/optimizationSettings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 07:50:35.869011 RSTAB-1.9.3/RSTAB/ConcreteDesign/
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/ConcreteDesign/ConcreteServiceabilityConfigurations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/ConcreteDesign/ConcreteUltimateConfigurations.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/ConcreteDesign/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 07:50:35.869011 RSTAB-1.9.3/RSTAB/DynamicLoads/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/DynamicLoads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6414 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/DynamicLoads/responseSpectrum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 07:50:35.869011 RSTAB-1.9.3/RSTAB/GuideObjects/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/GuideObjects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5385 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/GuideObjects/note.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 07:50:35.869011 RSTAB-1.9.3/RSTAB/Imperfections/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/Imperfections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20826 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/Imperfections/imperfectionCase.py
--rw-r--r--   0 runner    (1001) docker     (127)     9351 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/Imperfections/memberImperfection.py
--rw-r--r--   0 runner    (1001) docker     (127)     9275 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/Imperfections/membersetImperfection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 07:50:35.869011 RSTAB-1.9.3/RSTAB/ImportExport/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/ImportExport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5650 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/ImportExport/exports.py
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/ImportExport/imports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 07:50:35.873011 RSTAB-1.9.3/RSTAB/LoadCasesAndCombinations/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/LoadCasesAndCombinations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/LoadCasesAndCombinations/action.py
--rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/LoadCasesAndCombinations/actionCombination.py
--rw-r--r--   0 runner    (1001) docker     (127)     8808 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/LoadCasesAndCombinations/combinationWizard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/LoadCasesAndCombinations/designSituation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9427 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/LoadCasesAndCombinations/loadCase.py
--rw-r--r--   0 runner    (1001) docker     (127)   136467 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/LoadCasesAndCombinations/loadCasesAndCombinations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/LoadCasesAndCombinations/loadCombination.py
--rw-r--r--   0 runner    (1001) docker     (127)    16929 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/LoadCasesAndCombinations/modalAnalysisSettings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/LoadCasesAndCombinations/resultCombination.py
--rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/LoadCasesAndCombinations/spectralAnalysisSettings.py
--rw-r--r--   0 runner    (1001) docker     (127)    23114 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/LoadCasesAndCombinations/stabilityAnalysisSettings.py
--rw-r--r--   0 runner    (1001) docker     (127)    14699 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/LoadCasesAndCombinations/staticAnalysisSettings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 07:50:35.873011 RSTAB-1.9.3/RSTAB/Loads/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/Loads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/Loads/imposedNodalDeformation.py
--rw-r--r--   0 runner    (1001) docker     (127)   100244 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/Loads/memberLoad.py
--rw-r--r--   0 runner    (1001) docker     (127)   113605 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/Loads/membersetload.py
--rw-r--r--   0 runner    (1001) docker     (127)    22041 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/Loads/nodalLoad.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 07:50:35.873011 RSTAB-1.9.3/RSTAB/Reports/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/Reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32882 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/Reports/favicon32.png
--rw-r--r--   0 runner    (1001) docker     (127)    10352 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/Reports/html.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/Reports/htmlScript.js
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/Reports/htmlStyles.css
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/Reports/partsList.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/Reports/printoutReport.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 07:50:35.873011 RSTAB-1.9.3/RSTAB/Results/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/Results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/Results/designOverview.py
--rw-r--r--   0 runner    (1001) docker     (127)   187103 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/Results/resultTables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 07:50:35.873011 RSTAB-1.9.3/RSTAB/SpecialObjects/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/SpecialObjects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/SpecialObjects/nodalRelease.py
--rw-r--r--   0 runner    (1001) docker     (127)    10939 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/SpecialObjects/structureModification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 07:50:35.877011 RSTAB-1.9.3/RSTAB/SteelDesign/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/SteelDesign/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/SteelDesign/steelServiceabilityConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/SteelDesign/steelUltimateConfigurations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 07:50:35.877011 RSTAB-1.9.3/RSTAB/TimberDesign/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/TimberDesign/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/TimberDesign/timberServiceLimitStateConfigurations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/TimberDesign/timberUltimateConfigurations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 07:50:35.877011 RSTAB-1.9.3/RSTAB/Tools/
--rw-r--r--   0 runner    (1001) docker     (127)    20098 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/Tools/GetObjectNumbersByType.py
--rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/Tools/ModelCheck.py
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/Tools/PlausibilityCheck.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/Tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/Tools/centreOfGravityAndObjectInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/Tools/sectionDialogue.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 07:50:35.877011 RSTAB-1.9.3/RSTAB/TypesForAluminumDesign/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/TypesForAluminumDesign/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5052 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/TypesForAluminumDesign/aluminumEffectiveLengths.py
--rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/TypesForAluminumDesign/aluminumMemberLocalSectionReduction.py
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/TypesForAluminumDesign/aluminumMemberTransverseWelds.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 07:50:35.881011 RSTAB-1.9.3/RSTAB/TypesForMembers/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/TypesForMembers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/TypesForMembers/memberDefinableStiffness.py
--rw-r--r--   0 runner    (1001) docker     (127)     6498 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/TypesForMembers/memberEccentricity.py
--rw-r--r--   0 runner    (1001) docker     (127)    33419 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/TypesForMembers/memberHinge.py
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/TypesForMembers/memberNonlinearity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/TypesForMembers/memberResultIntermediatePoints.py
--rw-r--r--   0 runner    (1001) docker     (127)    12253 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/TypesForMembers/memberRotationalRestraint.py
--rw-r--r--   0 runner    (1001) docker     (127)    16988 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/TypesForMembers/memberShearPanel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6297 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/TypesForMembers/memberStiffnessModification.py
--rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/TypesForMembers/memberSupport.py
--rw-r--r--   0 runner    (1001) docker     (127)     5723 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/TypesForMembers/memberTransverseStiffeners.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 07:50:35.881011 RSTAB-1.9.3/RSTAB/TypesForNodes/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/TypesForNodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    41218 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/TypesForNodes/nodalSupport.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 07:50:35.881011 RSTAB-1.9.3/RSTAB/TypesForSpecialObjects/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/TypesForSpecialObjects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45059 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/TypesForSpecialObjects/nodalReleaseType.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 07:50:35.881011 RSTAB-1.9.3/RSTAB/TypesForSteelDesign/
--rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/TypesForSteelDesign/SteelMemberLocalSectionReduction.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/TypesForSteelDesign/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10573 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/TypesForSteelDesign/steelBoundaryConditions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10822 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/TypesForSteelDesign/steelEffectiveLengths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 07:50:35.881011 RSTAB-1.9.3/RSTAB/TypesForTimberDesign/
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/TypesForTimberDesign/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/TypesForTimberDesign/timberEffectiveLengths.py
--rw-r--r--   0 runner    (1001) docker     (127)    11534 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/TypesForTimberDesign/timberMemberLocalSectionReduction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/TypesForTimberDesign/timberMoistureClass.py
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/TypesForTimberDesign/timberServiceClass.py
--rw-r--r--   0 runner    (1001) docker     (127)     5393 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/TypesForTimberDesign/timberServiceCondition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 07:50:35.881011 RSTAB-1.9.3/RSTAB/TypesforConcreteDesign/
--rw-r--r--   0 runner    (1001) docker     (127)     8783 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/TypesforConcreteDesign/ConcreteDurability.py
--rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/TypesforConcreteDesign/ConcreteEffectiveLength.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/TypesforConcreteDesign/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/baseData.py
--rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/baseSettings.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/connectionGlobals.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/dataTypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)   121151 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     5007 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/formula.py
--rw-r--r--   0 runner    (1001) docker     (127)     9063 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/globalParameter.py
--rw-r--r--   0 runner    (1001) docker     (127)    29744 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/initModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-01-31 07:50:26.000000 RSTAB-1.9.3/RSTAB/suds_requests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 07:50:35.881011 RSTAB-1.9.3/RSTAB.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10615 2024-01-31 07:50:35.000000 RSTAB-1.9.3/RSTAB.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4667 2024-01-31 07:50:35.000000 RSTAB-1.9.3/RSTAB.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 07:50:35.000000 RSTAB-1.9.3/RSTAB.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 07:50:35.000000 RSTAB-1.9.3/RSTAB.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-01-31 07:50:35.000000 RSTAB-1.9.3/RSTAB.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-01-31 07:50:35.000000 RSTAB-1.9.3/RSTAB.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-31 07:50:35.881011 RSTAB-1.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-01-31 07:50:26.000000 RSTAB-1.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:33:46.106858 RSTAB-1.9.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:33:46.090858 RSTAB-1.9.5/Examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 12:33:38.000000 RSTAB-1.9.5/Examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-08 12:33:38.000000 RSTAB-1.9.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-08 12:33:38.000000 RSTAB-1.9.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10666 2024-04-08 12:33:46.106858 RSTAB-1.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9988 2024-04-08 12:33:38.000000 RSTAB-1.9.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:33:46.090858 RSTAB-1.9.5/RSTAB/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:33:46.090858 RSTAB-1.9.5/RSTAB/AluminumDesign/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/AluminumDesign/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/AluminumDesign/aluminumSLSConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/AluminumDesign/aluminumULSConfiguration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:33:46.090858 RSTAB-1.9.5/RSTAB/BasicObjects/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/BasicObjects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/BasicObjects/material.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72235 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/BasicObjects/member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/BasicObjects/memberSet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14897 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/BasicObjects/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/BasicObjects/section.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:33:46.094858 RSTAB-1.9.5/RSTAB/Calculate/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/Calculate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/Calculate/optimizationSettings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:33:46.094858 RSTAB-1.9.5/RSTAB/ConcreteDesign/
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/ConcreteDesign/ConcreteServiceabilityConfigurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/ConcreteDesign/ConcreteUltimateConfigurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/ConcreteDesign/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:33:46.094858 RSTAB-1.9.5/RSTAB/DynamicLoads/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/DynamicLoads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6414 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/DynamicLoads/responseSpectrum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:33:46.094858 RSTAB-1.9.5/RSTAB/GuideObjects/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/GuideObjects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14193 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/GuideObjects/coordinateSystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5385 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/GuideObjects/note.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:33:46.094858 RSTAB-1.9.5/RSTAB/Imperfections/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/Imperfections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20826 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/Imperfections/imperfectionCase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9351 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/Imperfections/memberImperfection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9275 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/Imperfections/membersetImperfection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:33:46.094858 RSTAB-1.9.5/RSTAB/ImportExport/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/ImportExport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5650 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/ImportExport/exports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/ImportExport/imports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:33:46.098858 RSTAB-1.9.5/RSTAB/LoadCasesAndCombinations/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/LoadCasesAndCombinations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4708 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/LoadCasesAndCombinations/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/LoadCasesAndCombinations/actionCombination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8781 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/LoadCasesAndCombinations/combinationWizard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/LoadCasesAndCombinations/designSituation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9427 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/LoadCasesAndCombinations/loadCase.py
+-rw-r--r--   0 runner    (1001) docker     (127)   136467 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/LoadCasesAndCombinations/loadCasesAndCombinations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/LoadCasesAndCombinations/loadCombination.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16929 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/LoadCasesAndCombinations/modalAnalysisSettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/LoadCasesAndCombinations/resultCombination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/LoadCasesAndCombinations/spectralAnalysisSettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23114 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/LoadCasesAndCombinations/stabilityAnalysisSettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14769 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/LoadCasesAndCombinations/staticAnalysisSettings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:33:46.098858 RSTAB-1.9.5/RSTAB/Loads/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/Loads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/Loads/imposedNodalDeformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)   100244 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/Loads/memberLoad.py
+-rw-r--r--   0 runner    (1001) docker     (127)   113605 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/Loads/membersetload.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22041 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/Loads/nodalLoad.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:33:46.098858 RSTAB-1.9.5/RSTAB/Reports/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/Reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32882 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/Reports/favicon32.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10352 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/Reports/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/Reports/htmlScript.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/Reports/htmlStyles.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/Reports/partsList.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/Reports/printoutReport.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:33:46.098858 RSTAB-1.9.5/RSTAB/Results/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/Results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/Results/designOverview.py
+-rw-r--r--   0 runner    (1001) docker     (127)   201658 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/Results/resultTables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:33:46.098858 RSTAB-1.9.5/RSTAB/SpecialObjects/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/SpecialObjects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/SpecialObjects/nodalRelease.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10939 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/SpecialObjects/structureModification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:33:46.098858 RSTAB-1.9.5/RSTAB/SteelDesign/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/SteelDesign/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/SteelDesign/steelServiceabilityConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/SteelDesign/steelUltimateConfigurations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:33:46.102858 RSTAB-1.9.5/RSTAB/TimberDesign/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/TimberDesign/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/TimberDesign/timberServiceLimitStateConfigurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/TimberDesign/timberUltimateConfigurations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:33:46.102858 RSTAB-1.9.5/RSTAB/Tools/
+-rw-r--r--   0 runner    (1001) docker     (127)    20263 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/Tools/GetObjectNumbersByType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/Tools/ModelCheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/Tools/PlausibilityCheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/Tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/Tools/centreOfGravityAndObjectInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/Tools/sectionDialogue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:33:46.102858 RSTAB-1.9.5/RSTAB/TypesForAluminumDesign/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/TypesForAluminumDesign/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5052 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/TypesForAluminumDesign/aluminumEffectiveLengths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/TypesForAluminumDesign/aluminumMemberLocalSectionReduction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/TypesForAluminumDesign/aluminumMemberTransverseWelds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:33:46.102858 RSTAB-1.9.5/RSTAB/TypesForMembers/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/TypesForMembers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/TypesForMembers/memberDefinableStiffness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6498 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/TypesForMembers/memberEccentricity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33419 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/TypesForMembers/memberHinge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/TypesForMembers/memberNonlinearity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/TypesForMembers/memberResultIntermediatePoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12253 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/TypesForMembers/memberRotationalRestraint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16988 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/TypesForMembers/memberShearPanel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6297 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/TypesForMembers/memberStiffnessModification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/TypesForMembers/memberSupport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5723 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/TypesForMembers/memberTransverseStiffeners.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:33:46.102858 RSTAB-1.9.5/RSTAB/TypesForNodes/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/TypesForNodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41218 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/TypesForNodes/nodalSupport.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:33:46.102858 RSTAB-1.9.5/RSTAB/TypesForSpecialObjects/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/TypesForSpecialObjects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45059 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/TypesForSpecialObjects/nodalReleaseType.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:33:46.106858 RSTAB-1.9.5/RSTAB/TypesForSteelDesign/
+-rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/TypesForSteelDesign/SteelMemberLocalSectionReduction.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/TypesForSteelDesign/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10573 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/TypesForSteelDesign/steelBoundaryConditions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10822 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/TypesForSteelDesign/steelEffectiveLengths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:33:46.106858 RSTAB-1.9.5/RSTAB/TypesForTimberDesign/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/TypesForTimberDesign/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/TypesForTimberDesign/timberEffectiveLengths.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11534 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/TypesForTimberDesign/timberMemberLocalSectionReduction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/TypesForTimberDesign/timberMoistureClass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/TypesForTimberDesign/timberServiceClass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5393 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/TypesForTimberDesign/timberServiceCondition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:33:46.106858 RSTAB-1.9.5/RSTAB/TypesforConcreteDesign/
+-rw-r--r--   0 runner    (1001) docker     (127)     8783 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/TypesforConcreteDesign/ConcreteDurability.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/TypesforConcreteDesign/ConcreteEffectiveLength.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/TypesforConcreteDesign/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/baseData.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/baseSettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/connectionGlobals.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/dataTypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)   122071 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5007 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/formula.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9063 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/globalParameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32438 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/initModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-08 12:33:38.000000 RSTAB-1.9.5/RSTAB/suds_requests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 12:33:46.106858 RSTAB-1.9.5/RSTAB.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10666 2024-04-08 12:33:46.000000 RSTAB-1.9.5/RSTAB.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-04-08 12:33:46.000000 RSTAB-1.9.5/RSTAB.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 12:33:46.000000 RSTAB-1.9.5/RSTAB.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 12:33:46.000000 RSTAB-1.9.5/RSTAB.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-08 12:33:46.000000 RSTAB-1.9.5/RSTAB.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-08 12:33:46.000000 RSTAB-1.9.5/RSTAB.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 12:33:46.106858 RSTAB-1.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-08 12:33:38.000000 RSTAB-1.9.5/setup.py
```

### Comparing `RSTAB-1.9.3/LICENSE` & `RSTAB-1.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/PKG-INFO` & `RSTAB-1.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: RSTAB
-Version: 1.9.3
+Version: 1.9.5
 Summary: Python Framework for RSTAB9 Web Services
 Home-page: https://github.com/Dlubal-Software/RSTAB_Python_Client
 Author: Dlubal Software
 Author-email: info@dlubal.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: six
 Requires-Dist: suds-py3
 Requires-Dist: xmltodict
 Requires-Dist: pytest
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: RSTAB Version: 1.9.3 Summary: Python Framework for
+Metadata-Version: 2.1 Name: RSTAB Version: 1.9.5 Summary: Python Framework for
 RSTAB9 Web Services Home-page: https://github.com/Dlubal-Software/
 RSTAB_Python_Client Author: Dlubal Software Author-email: info@dlubal.com
 License: MIT Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.10 Description-Content-Type: text/markdown License-File: LICENSE Requires-
-Dist: requests Requires-Dist: six Requires-Dist: suds-py3 Requires-Dist:
-xmltodict Requires-Dist: pytest Requires-Dist: psutil Requires-Dist: mock
-Requires-Dist: setuptools
+:: 3.10 Classifier: Programming Language :: Python :: 3.11 Description-Content-
+Type: text/markdown License-File: LICENSE Requires-Dist: requests Requires-
+Dist: six Requires-Dist: suds-py3 Requires-Dist: xmltodict Requires-Dist:
+pytest Requires-Dist: psutil Requires-Dist: mock Requires-Dist: setuptools
 ************ _[[_DD_ll_uu_bb_aa_ll_ _SS_oo_ff_tt_ww_aa_rr_ee_]]DDlluubbaall SSooffttwwaarree GGmmbbHH [[!![[iimmaaggee]]((hhttttppss::////iimmgg..sshhiieellddss..iioo//
 ttwwiitttteerr//ffoollllooww//ddlluubbaall__eenn??ssttyyllee==ssoocciiaall))]]((hhttttppss::////ttwwiitttteerr..ccoomm//ddlluubbaall__eenn ""TTwwiitttteerr
     FFoollllooww"")) [[!![[iimmaaggee]]((hhttttppss::////iimmgg..sshhiieellddss..iioo//bbaaddggee//GGiittHHuubb--DDlluubbaall__SSooffttwwaarree--
 ddaarrkkbblluuee??llooggoo==ggiitthhuubb&&))]]((hhttttppss::////ggiitthhuubb..ccoomm//DDlluubbaall--SSooffttwwaarree ""GGiitthhuubb FFoollllooww"")) [[!!
   [[iimmaaggee]]((hhttttppss::////iimmgg..sshhiieellddss..iioo//bbaaddggee//hhttttpp::////--ddlluubbaall..ccoomm--ddaarrkkbblluuee))]]((hhttttppss::////
 wwwwww..ddlluubbaall..ccoomm//eenn--UUSS ""DDlluubbaall WWeebbssiittee"")) [[!![[iimmaaggee]]((hhttttppss::////iimmgg..sshhiieellddss..iioo//bbaaddggee//
     ddooccss--AAPPII--ddaarrkkbblluuee??llooggoo==rreeaadd--tthhee--ddooccss&&llooggooCCoolloorr==wwhhiittee))]]((hhttttppss::////ddlluubbaall--
```

### Comparing `RSTAB-1.9.3/README.md` & `RSTAB-1.9.5/README.md`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/AluminumDesign/aluminumSLSConfiguration.py` & `RSTAB-1.9.5/RSTAB/AluminumDesign/aluminumSLSConfiguration.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/AluminumDesign/aluminumULSConfiguration.py` & `RSTAB-1.9.5/RSTAB/AluminumDesign/aluminumULSConfiguration.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/BasicObjects/coordinateSystem.py` & `RSTAB-1.9.5/RSTAB/GuideObjects/coordinateSystem.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,53 +1,52 @@
 from RSTAB.initModel import Model, clearAttributes, deleteEmptyAttributes
 from RSTAB.enums import CoordinateSystemType, CoordinateSystemRotationAnglesSequence
 
 class CoordinateSystem():
     def __init__(self,
                  no: int = 1,
-                 type = CoordinateSystemType.TYPE_OFFSET_XYZ,
                  origin_coordinate_x: float = 0.0,
                  origin_coordinate_y: float = 0.0,
                  origin_coordinate_z: float = 0.0,
                  name: str = 'Coord1',
                  comment: str = '',
                  params: dict = None,
                  model = Model):
 
         '''
          Args:
             no (int): Coordinate System Tag
-            type (enum): Coordinate System Type
             origin_coordinate_x (float): X-Coordinate
             origin_coordinate_y (float): Y-Coordinate
             origin_coordinate_z (float): Z-Coordinate
-            name (str): Name
+            name (str, optional): User Defined Coordinate System Name
             comment (str, optional): Comments
             params (dict, optional): Any WS Parameter relevant to the object and its value in form of a dictionary
             model (RSTAB Class, optional): Model to be edited
         '''
         # Client model | Coordinate System
         clientObject = model.clientModel.factory.create('ns0:coordinate_system')
 
         # Clears object atributes | Sets all atributes to None
         clearAttributes(clientObject)
 
         # Coordinate System No.
         clientObject.no = no
 
         # Coordinate System Type
-        clientObject.type = type.name
+        clientObject.type = CoordinateSystemType.TYPE_OFFSET_XYZ.name
 
         # Coordinates
         clientObject.origin_coordinate_x = origin_coordinate_x
         clientObject.origin_coordinate_y = origin_coordinate_y
         clientObject.origin_coordinate_z = origin_coordinate_z
 
         # Name
         if name:
+            clientObject.user_defined_name_enabled = True
             clientObject.name = name
 
         # Comment
         clientObject.comment = comment
 
         # Adding optional parameters via dictionary
         if params:
@@ -72,15 +71,15 @@
 
         '''
          Args:
             no (int): Coordinate System Tag
             origin_coordinate_x (float): X-Coordinate
             origin_coordinate_y (float): Y-Coordinate
             origin_coordinate_z (float): Z-Coordinate
-            name (str): Name
+            name (str, optional): User Defined Coordinate System Name
             comment (str, optional): Comments
             params (dict, optional): Any WS Parameter relevant to the object and its value in form of a dictionary
             model (RSTAB Class, optional): Model to be edited
         '''
         # Client model | Coordinate System
         clientObject = model.clientModel.factory.create('ns0:coordinate_system')
 
@@ -96,14 +95,15 @@
         # Coordinates
         clientObject.origin_coordinate_x = origin_coordinate_x
         clientObject.origin_coordinate_y = origin_coordinate_y
         clientObject.origin_coordinate_z = origin_coordinate_z
 
         # Name
         if name:
+            clientObject.user_defined_name_enabled = True
             clientObject.name = name
 
         # Comment
         clientObject.comment = comment
 
         # Adding optional parameters via dictionary
         if params:
@@ -140,15 +140,15 @@
             origin_coordinate_z (float): Origin Point Z-Coordinate
             u_axis_point_coordinate_x (float): Point on +U-Axis - 1st point X-Coordinate
             u_axis_point_coordinate_y (float): Point on +U-Axis - 1st point Y-Coordinate
             u_axis_point_coordinate_z (float): Point on +U-Axis - 1st point Z-Coordinate
             uw_plane_point_coordinate_x (float): Point in +UW-Plane - 2nd Point X-Coordinate
             uw_plane_point_coordinate_y (float): Point in +UW-Plane - 2nd Point Y-Coordinate
             uw_plane_point_coordinate_z (float): Point in +UW-Plane - 2nd Point Z-Coordinate
-            name (str): Name
+            name (str, optional): User Defined Coordinate System Name
             comment (str, optional): Comments
             params (dict, optional): Any WS Parameter relevant to the object and its value in form of a dictionary
             model (RSTAB Class, optional): Model to be edited
         '''
         # Client model | Coordinate System
         clientObject = model.clientModel.factory.create('ns0:coordinate_system')
 
@@ -172,14 +172,15 @@
 
         clientObject.uw_plane_point_coordinate_x = uw_plane_point_coordinate_x
         clientObject.uw_plane_point_coordinate_y = uw_plane_point_coordinate_y
         clientObject.uw_plane_point_coordinate_z = uw_plane_point_coordinate_z
 
         # Name
         if name:
+            clientObject.user_defined_name_enabled = True
             clientObject.name = name
 
         # Comment
         clientObject.comment = comment
 
         # Adding optional parameters via dictionary
         if params:
@@ -212,15 +213,15 @@
             origin_coordinate_x (float): Origin Point X-Coordinate
             origin_coordinate_y (float): Origin Point Y-Coordinate
             origin_coordinate_z (float): Origin Point Z-Coordinate
             u_axis_point_coordinate_x (float): Point on +U-Axis - 1st point X-Coordinate
             u_axis_point_coordinate_y (float): Point on +U-Axis - 1st point Y-Coordinate
             u_axis_point_coordinate_z (float): Point on +U-Axis - 1st point Z-Coordinate
             uw_plane_angle (float): Rotation About U-Axis
-            name (str): Name
+            name (str, optional): User Defined Coordinate System Name
             comment (str, optional): Comments
             params (dict, optional): Any WS Parameter relevant to the object and its value in form of a dictionary
             model (RSTAB Class, optional): Model to be edited
         '''
         # Client model | Coordinate System
         clientObject = model.clientModel.factory.create('ns0:coordinate_system')
 
@@ -242,14 +243,15 @@
         clientObject.u_axis_point_coordinate_y = u_axis_point_coordinate_y
         clientObject.u_axis_point_coordinate_z = u_axis_point_coordinate_z
 
         clientObject.uw_plane_angle = uw_plane_angle
 
         # Name
         if name:
+            clientObject.user_defined_name_enabled = True
             clientObject.name = name
 
         # Comment
         clientObject.comment = comment
 
         # Adding optional parameters via dictionary
         if params:
@@ -278,33 +280,32 @@
 
         '''
          Args:
             no (int): Coordinate System Tag
             origin_coordinate_x (float): Origin Point X-Coordinate
             origin_coordinate_y (float): Origin Point Y-Coordinate
             origin_coordinate_z (float): Origin Point Z-Coordinate
-            rotation_angles_sequence (float): Rotation Angles Sequesce
+            rotation_angles_sequence (enum): Coordinate System Rotation Angles Sequence Enumeration
             rotation_angle_1 (float): Rotation about X Axes
             rotation_angle_2 (float): Rotation about Y Axes
             rotation_angle_3 (float): Rotation about Z Axes
-            name (str): Name
+            name (str, optional): User Defined Coordinate System Name
             comment (str, optional): Comments
             params (dict, optional): Any WS Parameter relevant to the object and its value in form of a dictionary
             model (RSTAB Class, optional): Model to be edited
         '''
         # Client model | Coordinate System
         clientObject = model.clientModel.factory.create('ns0:coordinate_system')
 
         # Clears object atributes | Sets all atributes to None
         clearAttributes(clientObject)
 
         # Coordinate System No.
         clientObject.no = no
 
-
         # Coordinate System Type
         clientObject.type = CoordinateSystemType.TYPE_POINT_AND_3_ANGLES.name
 
         # Coordinates
         clientObject.origin_coordinate_x = origin_coordinate_x
         clientObject.origin_coordinate_y = origin_coordinate_y
         clientObject.origin_coordinate_z = origin_coordinate_z
@@ -314,14 +315,15 @@
 
         clientObject.rotation_angle_1 = rotation_angle_1
         clientObject.rotation_angle_2 = rotation_angle_2
         clientObject.rotation_angle_3 = rotation_angle_3
 
         # Name
         if name:
+            clientObject.user_defined_name_enabled = True
             clientObject.name = name
 
         # Comment
         clientObject.comment = comment
 
         # Adding optional parameters via dictionary
         if params:
@@ -329,7 +331,19 @@
                 clientObject[key] = params[key]
 
         # Delete None attributes for improved performance
         deleteEmptyAttributes(clientObject)
 
         # Add Coordinate System to client model
         model.clientModel.service.set_coordinate_system(clientObject)
+
+    @staticmethod
+    def GetCoordinateSystem(object_index: int = 1, model = Model):
+
+        '''
+        Args:
+            obejct_index (int): Coordinate System Index
+            model (RSTAB Class, optional): Model to be edited
+        '''
+
+        # Get Coordinate System from client model
+        return model.clientModel.service.get_coordinate_system(object_index)
```

### Comparing `RSTAB-1.9.3/RSTAB/BasicObjects/material.py` & `RSTAB-1.9.5/RSTAB/ConcreteDesign/ConcreteServiceabilityConfigurations.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,71 +1,67 @@
-from RSTAB.initModel import clearAttributes, deleteEmptyAttributes, Model, ConvertStrToListOfInt
-from RSTAB.enums import ObjectTypes
+from RSTAB.initModel import Model, clearAttributes, deleteEmptyAttributes, ConvertToDlString
 
 
-class Material():
-    def __init__(self,
-                 no: int = 1,
-                 name: str = 'S235',
-                 comment: str = '',
-                 params: dict = None,
-                 model = Model):
+class ConcreteServiceabilityConfiguration():
 
-        '''
+    def __init__(self,
+                no: int = 1,
+                name: str = 'SLS',
+                members: str = 'All',
+                member_sets: str = 'All',
+                comment: str = '',
+                params: dict = None,
+                model = Model):
+        """
         Args:
-            no (int): Material Tag
-            name (str): Name of Desired Material (As Named in RSTAB Database)
-            comment (str, optional): Comments
+            no (int): Configuration Tag
+            name (str): User Defined Name
+            members (str): Assigned Members
+            member_sets (str): Assigned Member Sets
+            comment (str, optional): Comment
             params (dict, optional): Any WS Parameter relevant to the object and its value in form of a dictionary
             model (RSTAB Class, optional): Model to be edited
-        '''
+        """
 
-        # Client model | Material
-        clientObject = model.clientModel.factory.create('ns0:material')
+        # Client model | Concrete Durabilities
+        clientObject = model.clientModel.factory.create('ns0:concrete_design_sls_configuration')
 
         # Clears object atributes | Sets all atributes to None
         clearAttributes(clientObject)
 
-        # Material No.
+        # Concrete Durability No.
         clientObject.no = no
 
-        # Material Name
-        clientObject.name = name
+        # User Defined Name
+        if name:
+            clientObject.user_defined_name_enabled = True
+            clientObject.name = name
+
+        # Assigned Members
+        if members == 'All':
+            clientObject.assigned_to_all_members = True
+
+        else:
+            clientObject.assigned_to_all_members = False
+            clientObject.assigned_to_members = ConvertToDlString(members)
+
+        # Assigned Member Sets
+        if member_sets == 'All':
+            clientObject.assigned_to_all_member_sets = True
+
+        else:
+            clientObject.assigned_to_all_member_sets = False
+            clientObject.assigned_to_member_sets = ConvertToDlString(member_sets)
 
         # Comment
         clientObject.comment = comment
 
         # Adding optional parameters via dictionary
         if params:
             for key in params:
                 clientObject[key] = params[key]
 
         # Delete None attributes for improved performance
         deleteEmptyAttributes(clientObject)
 
-        # Add material to client model
-        model.clientModel.service.set_material(clientObject)
-
-    @staticmethod
-    def DeleteMaterial(materials_no: str = '1 2', model = Model):
-
-        '''
-        Args:
-            materials_no (str): Numbers of Materials to be deleted
-            model (RSTAB Class, optional): Model to be edited
-        '''
-
-        # Delete from client model
-        for material in ConvertStrToListOfInt(materials_no):
-            model.clientModel.service.delete_object(ObjectTypes.E_OBJECT_TYPE_MATERIAL.name, material)
-
-    @staticmethod
-    def GetMaterial(object_index: int = 1, model = Model):
-
-        '''
-        Args:
-            obejct_index (int): Material Index
-            model (RSTAB Class, optional): Model to be edited
-        '''
-
-        # Get Material from client model
-        return model.clientModel.service.get_material(object_index)
+        # Add Global Parameter to client model
+        model.clientModel.service.set_concrete_design_sls_configuration(clientObject)
```

### Comparing `RSTAB-1.9.3/RSTAB/BasicObjects/member.py` & `RSTAB-1.9.5/RSTAB/BasicObjects/member.py`

 * *Files 22% similar despite different names*

```diff
@@ -282,64 +282,20 @@
             clientObject.rotation_plane_type = rotation_parameters[1].name
         elif rotation_specification_type == MemberRotationSpecificationType.COORDINATE_SYSTEM_ROTATION_VIA_INSIDE_NODE:
             clientObject.rotation_plane_type = rotation_parameters[0].name
         elif rotation_specification_type == MemberRotationSpecificationType.COORDINATE_SYSTEM_ROTATION_VIA_SURFACE:
             clientObject.rotation_surface = rotation_parameters[0]
             clientObject.rotation_surface_plane_type = rotation_parameters[1].name
 
-
         # Start Section No.
         clientObject.section_start = start_section_no
 
         # End Section No.
         clientObject.section_end = end_section_no
 
-        # Update parameters
-        params_up: dict = {'member_hinge_start':0, 'member_hinge_end': 0,
-                        'member_eccentricity_start': 0, 'member_eccentricity_end': 0,
-                        'support':0, 'member_nonlinearity': 0,
-                        'end_modifications_member_start_extension': 0,
-                        'end_modifications_member_start_slope_y': 0,
-                        'end_modifications_member_start_slope_z': 0,
-                        'end_modifications_member_end_extension': 0,
-                        'end_modifications_member_end_slope_y': 0,
-                        'end_modifications_member_end_slope_z': 0,
-                        'member_result_intermediate_point' : 0,
-                        'is_deactivated_for_calculation' : False }
-
-        params_up.update(params)
-
-        # Member Hinges
-        clientObject.member_hinge_start = params_up['member_hinge_start']
-        clientObject.member_hinge_end = params_up['member_hinge_end']
-
-        # Member Eccentricity
-        clientObject.member_eccentricity_start = params_up['member_eccentricity_start']
-        clientObject.member_eccentricity_end = params_up['member_eccentricity_end']
-
-        # Member Support
-        clientObject.support = params_up['support']
-
-        # Member Nonlinearity
-        clientObject.member_nonlinearity = params_up['member_nonlinearity']
-
-        # End Modifications
-        clientObject.end_modifications_member_start_extension = params_up['end_modifications_member_start_extension']
-        clientObject.end_modifications_member_start_slope_y = params_up['end_modifications_member_start_slope_y']
-        clientObject.end_modifications_member_start_slope_z = params_up['end_modifications_member_start_slope_z']
-        clientObject.end_modifications_member_end_extension = params_up['end_modifications_member_end_extension']
-        clientObject.end_modifications_member_end_slope_y = params_up['end_modifications_member_end_slope_y']
-        clientObject.end_modifications_member_end_slope_z = params_up['end_modifications_member_end_slope_z']
-
-        # Result Intermediate Points
-        clientObject.member_result_intermediate_point = params_up['member_result_intermediate_point']
-
-        # Deactivation for Calculation
-        clientObject.is_deactivated_for_calculation = params_up['is_deactivated_for_calculation']
-
         # Comment
         clientObject.comment = comment
 
         # Adding optional parameters via dictionary
         if params:
             for key in params:
                 clientObject[key] = params[key]
@@ -414,44 +370,14 @@
             clientObject.rotation_plane_type = rotation_parameters[1].name
         elif rotation_specification_type == MemberRotationSpecificationType.COORDINATE_SYSTEM_ROTATION_VIA_INSIDE_NODE:
             clientObject.rotation_plane_type = rotation_parameters[0].name
         elif rotation_specification_type == MemberRotationSpecificationType.COORDINATE_SYSTEM_ROTATION_VIA_SURFACE:
             clientObject.rotation_surface = rotation_parameters[0]
             clientObject.rotation_surface_plane_type = rotation_parameters[1].name
 
-        # Update parameters
-        params_up: dict = {'member_hinge_start':0, 'member_hinge_end': 0,
-                          'member_eccentricity_start': 0, 'member_eccentricity_end': 0,
-                          'support':0, 'member_nonlinearity': 0,
-                          'member_result_intermediate_point' : 0,
-                          'is_deactivated_for_calculation' : False }
-
-        params_up.update(params)
-
-        # Member Hinges
-        clientObject.member_hinge_start = params_up['member_hinge_start']
-        clientObject.member_hinge_end = params_up['member_hinge_end']
-
-        # Member Eccentricity
-        clientObject.member_eccentricity_start = params_up['member_eccentricity_start']
-        clientObject.member_eccentricity_end = params_up['member_eccentricity_end']
-
-        # Member Support
-        clientObject.support = params_up['support']
-
-        # Member Nonlinearity
-        clientObject.member_nonlinearity = params_up['member_nonlinearity']
-
-        # Result Intermediate Points
-        clientObject.member_result_intermediate_point = params_up['member_result_intermediate_point']
-
-        # Deactivation for Calculation
-        clientObject.is_deactivated_for_calculation = params_up['is_deactivated_for_calculation']
-
-
         # Comment
         clientObject.comment = comment
 
         # Adding optional parameters via dictionary
         if params:
             for key in params:
                 clientObject[key] = params[key]
@@ -540,46 +466,14 @@
 
         # Start Section No.
         clientObject.section_start = section_no
 
         # End Section No.
         clientObject.section_end = section_no
 
-        # Update parameters
-        params_up: dict = {'member_eccentricity_start': 0, 'member_eccentricity_end': 0,
-                            'member_nonlinearity': 0,
-                            'end_modifications_member_start_extension': 0,
-                            'end_modifications_member_start_slope_y': 0,
-                            'end_modifications_member_start_slope_z': 0,
-                            'end_modifications_member_end_extension': 0,
-                            'end_modifications_member_end_slope_y': 0,
-                            'end_modifications_member_end_slope_z': 0,
-                            'is_deactivated_for_calculation' : False }
-
-        params_up.update(params)
-
-        # Member Eccentricity
-        clientObject.member_eccentricity_start = params_up['member_eccentricity_start']
-        clientObject.member_eccentricity_end = params_up['member_eccentricity_end']
-
-        # Member Nonlinearity
-        clientObject.member_nonlinearity = params_up['member_nonlinearity']
-
-        # End Modifications
-        clientObject.end_modifications_member_start_extension = params_up['end_modifications_member_start_extension']
-        clientObject.end_modifications_member_start_slope_y = params_up['end_modifications_member_start_slope_y']
-        clientObject.end_modifications_member_start_slope_z = params_up['end_modifications_member_start_slope_z']
-        clientObject.end_modifications_member_end_extension = params_up['end_modifications_member_end_extension']
-        clientObject.end_modifications_member_end_slope_y = params_up['end_modifications_member_end_slope_y']
-        clientObject.end_modifications_member_end_slope_z = params_up['end_modifications_member_end_slope_z']
-
-        # Deactivation for Calculation
-        clientObject.is_deactivated_for_calculation = params_up['is_deactivated_for_calculation']
-
-
         # Comment
         clientObject.comment = comment
 
         # Adding optional parameters via dictionary
         if params:
             for key in params:
                 clientObject[key] = params[key]
@@ -668,45 +562,14 @@
 
         # Start Section No.
         clientObject.section_start = section_no
 
         # End Section No.
         clientObject.section_end = section_no
 
-        # Update parameters
-        params_up: dict = {'member_eccentricity_start': 0, 'member_eccentricity_end': 0,
-                            'member_nonlinearity': 0,
-                            'end_modifications_member_start_extension': 0,
-                            'end_modifications_member_start_slope_y': 0,
-                            'end_modifications_member_start_slope_z': 0,
-                            'end_modifications_member_end_extension': 0,
-                            'end_modifications_member_end_slope_y': 0,
-                            'end_modifications_member_end_slope_z': 0,
-                            'is_deactivated_for_calculation' : False }
-
-        params_up.update(params)
-
-        # Member Eccentricity
-        clientObject.member_eccentricity_start = params_up['member_eccentricity_start']
-        clientObject.member_eccentricity_end = params_up['member_eccentricity_end']
-
-        # Member Nonlinearity
-        clientObject.member_nonlinearity = params_up['member_nonlinearity']
-
-        # End Modifications
-        clientObject.end_modifications_member_start_extension = params_up['end_modifications_member_start_extension']
-        clientObject.end_modifications_member_start_slope_y = params_up['end_modifications_member_start_slope_y']
-        clientObject.end_modifications_member_start_slope_z = params_up['end_modifications_member_start_slope_z']
-        clientObject.end_modifications_member_end_extension = params_up['end_modifications_member_end_extension']
-        clientObject.end_modifications_member_end_slope_y = params_up['end_modifications_member_end_slope_y']
-        clientObject.end_modifications_member_end_slope_z = params_up['end_modifications_member_end_slope_z']
-
-        # Deactivation for Calculation
-        clientObject.is_deactivated_for_calculation = params_up['is_deactivated_for_calculation']
-
         # Comment
         clientObject.comment = comment
 
         # Adding optional parameters via dictionary
         if params:
             for key in params:
                 clientObject[key] = params[key]
@@ -795,45 +658,14 @@
 
         # Start Section No.
         clientObject.section_start = section_no
 
         # End Section No.
         clientObject.section_end = section_no
 
-        # Update parameters
-        params_up: dict = {'member_eccentricity_start': 0, 'member_eccentricity_end': 0,
-                            'member_nonlinearity': 0,
-                            'end_modifications_member_start_extension': 0,
-                            'end_modifications_member_start_slope_y': 0,
-                            'end_modifications_member_start_slope_z': 0,
-                            'end_modifications_member_end_extension': 0,
-                            'end_modifications_member_end_slope_y': 0,
-                            'end_modifications_member_end_slope_z': 0,
-                            'is_deactivated_for_calculation' : False }
-
-        params_up.update(params)
-
-        # Member Eccentricity
-        clientObject.member_eccentricity_start = params_up['member_eccentricity_start']
-        clientObject.member_eccentricity_end = params_up['member_eccentricity_end']
-
-        # Member Nonlinearity
-        clientObject.member_nonlinearity = params_up['member_nonlinearity']
-
-        # End Modifications
-        clientObject.end_modifications_member_start_extension = params_up['end_modifications_member_start_extension']
-        clientObject.end_modifications_member_start_slope_y = params_up['end_modifications_member_start_slope_y']
-        clientObject.end_modifications_member_start_slope_z = params_up['end_modifications_member_start_slope_z']
-        clientObject.end_modifications_member_end_extension = params_up['end_modifications_member_end_extension']
-        clientObject.end_modifications_member_end_slope_y = params_up['end_modifications_member_end_slope_y']
-        clientObject.end_modifications_member_end_slope_z = params_up['end_modifications_member_end_slope_z']
-
-        # Deactivation for Calculation
-        clientObject.is_deactivated_for_calculation = params_up['is_deactivated_for_calculation']
-
         # Comment
         clientObject.comment = comment
 
         # Adding optional parameters via dictionary
         if params:
             for key in params:
                 clientObject[key] = params[key]
@@ -922,45 +754,14 @@
 
         # Start Section No.
         clientObject.section_start = section_no
 
         # End Section No.
         clientObject.section_end = section_no
 
-        # Update parameters
-        params_up: dict = {'member_eccentricity_start': 0, 'member_eccentricity_end': 0,
-                            'member_nonlinearity': 0,
-                            'end_modifications_member_start_extension': 0,
-                            'end_modifications_member_start_slope_y': 0,
-                            'end_modifications_member_start_slope_z': 0,
-                            'end_modifications_member_end_extension': 0,
-                            'end_modifications_member_end_slope_y': 0,
-                            'end_modifications_member_end_slope_z': 0,
-                            'is_deactivated_for_calculation' : False }
-
-        params_up.update(params)
-
-        # Member Eccentricity
-        clientObject.member_eccentricity_start = params_up['member_eccentricity_start']
-        clientObject.member_eccentricity_end = params_up['member_eccentricity_end']
-
-        # Member Nonlinearity
-        clientObject.member_nonlinearity = params_up['member_nonlinearity']
-
-        # End Modifications
-        clientObject.end_modifications_member_start_extension = params_up['end_modifications_member_start_extension']
-        clientObject.end_modifications_member_start_slope_y = params_up['end_modifications_member_start_slope_y']
-        clientObject.end_modifications_member_start_slope_z = params_up['end_modifications_member_start_slope_z']
-        clientObject.end_modifications_member_end_extension = params_up['end_modifications_member_end_extension']
-        clientObject.end_modifications_member_end_slope_y = params_up['end_modifications_member_end_slope_y']
-        clientObject.end_modifications_member_end_slope_z = params_up['end_modifications_member_end_slope_z']
-
-        # Deactivation for Calculation
-        clientObject.is_deactivated_for_calculation = params_up['is_deactivated_for_calculation']
-
         # Comment
         clientObject.comment = comment
 
         # Adding optional parameters via dictionary
         if params:
             for key in params:
                 clientObject[key] = params[key]
@@ -1049,45 +850,14 @@
 
         # Start Section No.
         clientObject.section_start = section_no
 
         # End Section No.
         clientObject.section_end = section_no
 
-        # Update parameters
-        params_up: dict = {'member_eccentricity_start': 0, 'member_eccentricity_end': 0,
-                            'member_nonlinearity': 0,
-                            'end_modifications_member_start_extension': 0,
-                            'end_modifications_member_start_slope_y': 0,
-                            'end_modifications_member_start_slope_z': 0,
-                            'end_modifications_member_end_extension': 0,
-                            'end_modifications_member_end_slope_y': 0,
-                            'end_modifications_member_end_slope_z': 0,
-                            'is_deactivated_for_calculation' : False }
-
-        params_up.update(params)
-
-        # Member Eccentricity
-        clientObject.member_eccentricity_start = params_up['member_eccentricity_start']
-        clientObject.member_eccentricity_end = params_up['member_eccentricity_end']
-
-        # Member Nonlinearity
-        clientObject.member_nonlinearity = params_up['member_nonlinearity']
-
-        # End Modifications
-        clientObject.end_modifications_member_start_extension = params_up['end_modifications_member_start_extension']
-        clientObject.end_modifications_member_start_slope_y = params_up['end_modifications_member_start_slope_y']
-        clientObject.end_modifications_member_start_slope_z = params_up['end_modifications_member_start_slope_z']
-        clientObject.end_modifications_member_end_extension = params_up['end_modifications_member_end_extension']
-        clientObject.end_modifications_member_end_slope_y = params_up['end_modifications_member_end_slope_y']
-        clientObject.end_modifications_member_end_slope_z = params_up['end_modifications_member_end_slope_z']
-
-        # Deactivation for Calculation
-        clientObject.is_deactivated_for_calculation = params_up['is_deactivated_for_calculation']
-
         # Comment
         clientObject.comment = comment
 
         # Adding optional parameters via dictionary
         if params:
             for key in params:
                 clientObject[key] = params[key]
@@ -1173,36 +943,14 @@
 
         # Start Section No.
         clientObject.section_start = section_no
 
         # End Section No.
         clientObject.section_end = section_no
 
-        # Update parameters
-        params_up: dict = {'end_modifications_member_start_extension': 0,
-                            'end_modifications_member_start_slope_y': 0,
-                            'end_modifications_member_start_slope_z': 0,
-                            'end_modifications_member_end_extension': 0,
-                            'end_modifications_member_end_slope_y': 0,
-                            'end_modifications_member_end_slope_z': 0,
-                            'is_deactivated_for_calculation' : False }
-
-        params_up.update(params)
-
-        # End Modifications
-        clientObject.end_modifications_member_start_extension = params_up['end_modifications_member_start_extension']
-        clientObject.end_modifications_member_start_slope_y = params_up['end_modifications_member_start_slope_y']
-        clientObject.end_modifications_member_start_slope_z = params_up['end_modifications_member_start_slope_z']
-        clientObject.end_modifications_member_end_extension = params_up['end_modifications_member_end_extension']
-        clientObject.end_modifications_member_end_slope_y = params_up['end_modifications_member_end_slope_y']
-        clientObject.end_modifications_member_end_slope_z = params_up['end_modifications_member_end_slope_z']
-
-        # Deactivation for Calculation
-        clientObject.is_deactivated_for_calculation = params_up['is_deactivated_for_calculation']
-
         # Comment
         clientObject.comment = comment
 
         # Adding optional parameters via dictionary
         if params:
             for key in params:
                 clientObject[key] = params[key]
@@ -1285,40 +1033,14 @@
             clientObject.rotation_plane_type = rotation_parameters[1].name
         elif rotation_specification_type == MemberRotationSpecificationType.COORDINATE_SYSTEM_ROTATION_VIA_INSIDE_NODE:
             clientObject.rotation_plane_type = rotation_parameters[0].name
         elif rotation_specification_type == MemberRotationSpecificationType.COORDINATE_SYSTEM_ROTATION_VIA_SURFACE:
             clientObject.rotation_surface = rotation_parameters[0]
             clientObject.rotation_surface_plane_type = rotation_parameters[1].name
 
-        # Update parameters
-        params_up: dict = {'member_hinge_start':0, 'member_hinge_end': 0,
-                        'member_eccentricity_start': 0, 'member_eccentricity_end': 0,
-                        'member_nonlinearity': 0,
-                        'member_result_intermediate_point' : 0,
-                        'is_deactivated_for_calculation' : False}
-
-        params_up.update(params)
-
-        # Member Hinges
-        clientObject.member_hinge_start = params_up['member_hinge_start']
-        clientObject.member_hinge_end = params_up['member_hinge_end']
-
-        # Member Eccentricity
-        clientObject.member_eccentricity_start = params_up['member_eccentricity_start']
-        clientObject.member_eccentricity_end = params_up['member_eccentricity_end']
-
-        # Member Nonlinearity
-        clientObject.member_nonlinearity = params_up['member_nonlinearity']
-
-        # Result Intermediate Points
-        clientObject.member_result_intermediate_point = params_up['member_result_intermediate_point']
-
-        # Deactivation for Calculation
-        clientObject.is_deactivated_for_calculation = params_up['is_deactivated_for_calculation']
-
         # Comment
         clientObject.comment = comment
 
         # Adding optional parameters via dictionary
         if params:
             for key in params:
                 clientObject[key] = params[key]
@@ -1387,22 +1109,14 @@
             clientObject.rotation_plane_type = rotation_parameters[1].name
         elif rotation_specification_type == MemberRotationSpecificationType.COORDINATE_SYSTEM_ROTATION_VIA_INSIDE_NODE:
             clientObject.rotation_plane_type = rotation_parameters[0].name
         elif rotation_specification_type == MemberRotationSpecificationType.COORDINATE_SYSTEM_ROTATION_VIA_SURFACE:
             clientObject.rotation_surface = rotation_parameters[0]
             clientObject.rotation_surface_plane_type = rotation_parameters[1].name
 
-        # Update parameters
-        params_up: dict = {'is_deactivated_for_calculation' : False}
-
-        params_up.update(params)
-
-        # Deactivation for Calculation
-        clientObject.is_deactivated_for_calculation = params_up['is_deactivated_for_calculation']
-
         # Comment
         clientObject.comment = comment
 
         # Adding optional parameters via dictionary
         if params:
             for key in params:
                 clientObject[key] = params[key]
@@ -1471,22 +1185,14 @@
             clientObject.rotation_plane_type = rotation_parameters[1].name
         elif rotation_specification_type == MemberRotationSpecificationType.COORDINATE_SYSTEM_ROTATION_VIA_INSIDE_NODE:
             clientObject.rotation_plane_type = rotation_parameters[0].name
         elif rotation_specification_type == MemberRotationSpecificationType.COORDINATE_SYSTEM_ROTATION_VIA_SURFACE:
             clientObject.rotation_surface = rotation_parameters[0]
             clientObject.rotation_surface_plane_type = rotation_parameters[1].name
 
-        # Update parameters
-        params_up: dict = {'is_deactivated_for_calculation' : False}
-
-        params_up.update(params)
-
-        # Deactivation for Calculation
-        clientObject.is_deactivated_for_calculation = params_up['is_deactivated_for_calculation']
-
         # Comment
         clientObject.comment = comment
 
         # Adding optional parameters via dictionary
         if params:
             for key in params:
                 clientObject[key] = params[key]
@@ -1549,27 +1255,14 @@
         # Member Rotation
         clientObject.rotation_specification_type = rotation_specification_type.name
         if rotation_specification_type == MemberRotationSpecificationType.COORDINATE_SYSTEM_ROTATION_VIA_ANGLE:
             clientObject.rotation_angle = rotation_parameters[0]
         elif rotation_specification_type == MemberRotationSpecificationType.COORDINATE_SYSTEM_ROTATION_VIA_HELP_NODE:
             clientObject.rotation_help_node = rotation_parameters[0]
             clientObject.rotation_plane_type = rotation_parameters[1].name
-        elif rotation_specification_type == MemberRotationSpecificationType.COORDINATE_SYSTEM_ROTATION_VIA_INSIDE_NODE:
-            clientObject.rotation_plane_type = rotation_parameters[0].name
-        elif rotation_specification_type == MemberRotationSpecificationType.COORDINATE_SYSTEM_ROTATION_VIA_SURFACE:
-            clientObject.rotation_surface = rotation_parameters[0]
-            clientObject.rotation_surface_plane_type = rotation_parameters[1].name
-
-        # Update parameters
-        params_up: dict = {'is_deactivated_for_calculation' : False}
-
-        params_up.update(params)
-
-        # Deactivation for Calculation
-        clientObject.is_deactivated_for_calculation = params_up['is_deactivated_for_calculation']
 
         # Comment
         clientObject.comment = comment
 
         # Adding optional parameters via dictionary
         if params:
             for key in params:
@@ -1639,22 +1332,14 @@
             clientObject.rotation_plane_type = rotation_parameters[1].name
         elif rotation_specification_type == MemberRotationSpecificationType.COORDINATE_SYSTEM_ROTATION_VIA_INSIDE_NODE:
             clientObject.rotation_plane_type = rotation_parameters[0].name
         elif rotation_specification_type == MemberRotationSpecificationType.COORDINATE_SYSTEM_ROTATION_VIA_SURFACE:
             clientObject.rotation_surface = rotation_parameters[0]
             clientObject.rotation_surface_plane_type = rotation_parameters[1].name
 
-        # Update parameters
-        params_up: dict = {'is_deactivated_for_calculation' : False}
-
-        params_up.update(params)
-
-        # Deactivation for Calculation
-        clientObject.is_deactivated_for_calculation = params_up['is_deactivated_for_calculation']
-
         # Comment
         clientObject.comment = comment
 
         # Adding optional parameters via dictionary
         if params:
             for key in params:
                 clientObject[key] = params[key]
```

### Comparing `RSTAB-1.9.3/RSTAB/BasicObjects/memberSet.py` & `RSTAB-1.9.5/RSTAB/BasicObjects/memberSet.py`

 * *Files 8% similar despite different names*

```diff
@@ -138,14 +138,27 @@
         # Delete None attributes for improved performance
         deleteEmptyAttributes(clientObject)
 
         # Add Member Set to client model
         model.clientModel.service.set_member_set(clientObject)
 
     @staticmethod
+    def DeleteMemberSet(members_no: str = '1 2', model = Model):
+
+        '''
+        Args:
+            members_no (str): Numbers of Members Sets to be deleted
+            model (RSTAB Class, optional): Model to be edited
+        '''
+
+        # Delete from client model
+        for member in ConvertStrToListOfInt(members_no):
+            model.clientModel.service.delete_object(ObjectTypes.E_OBJECT_TYPE_MEMBER_SET.name, member)
+
+    @staticmethod
     def GetMemberSet(object_index: int = 1, model = Model):
 
         '''
         Args:
             obejct_index (int): Member Set Index
             model (RSTAB Class, optional): Model to be edited
         '''
```

### Comparing `RSTAB-1.9.3/RSTAB/BasicObjects/node.py` & `RSTAB-1.9.5/RSTAB/BasicObjects/node.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/BasicObjects/section.py` & `RSTAB-1.9.5/RSTAB/BasicObjects/section.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/Calculate/optimizationSettings.py` & `RSTAB-1.9.5/RSTAB/Calculate/optimizationSettings.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/ConcreteDesign/ConcreteServiceabilityConfigurations.py` & `RSTAB-1.9.5/RSTAB/ConcreteDesign/ConcreteUltimateConfigurations.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from RSTAB.initModel import Model, clearAttributes, deleteEmptyAttributes, ConvertToDlString
 
 
-class ConcreteServiceabilityConfiguration():
+class ConcreteUltimateConfiguration():
 
     def __init__(self,
                 no: int = 1,
-                name: str = 'SLS',
+                name: str = 'ULS',
                 members: str = 'All',
                 member_sets: str = 'All',
                 comment: str = '',
                 params: dict = None,
                 model = Model):
         """
         Args:
@@ -19,15 +19,15 @@
             member_sets (str): Assigned Member Sets
             comment (str, optional): Comment
             params (dict, optional): Any WS Parameter relevant to the object and its value in form of a dictionary
             model (RSTAB Class, optional): Model to be edited
         """
 
         # Client model | Concrete Durabilities
-        clientObject = model.clientModel.factory.create('ns0:concrete_design_sls_configuration')
+        clientObject = model.clientModel.factory.create('ns0:concrete_design_uls_configuration')
 
         # Clears object atributes | Sets all atributes to None
         clearAttributes(clientObject)
 
         # Concrete Durability No.
         clientObject.no = no
 
@@ -60,8 +60,8 @@
             for key in params:
                 clientObject[key] = params[key]
 
         # Delete None attributes for improved performance
         deleteEmptyAttributes(clientObject)
 
         # Add Global Parameter to client model
-        model.clientModel.service.set_concrete_design_sls_configuration(clientObject)
+        model.clientModel.service.set_concrete_design_uls_configuration(clientObject)
```

### Comparing `RSTAB-1.9.3/RSTAB/ConcreteDesign/ConcreteUltimateConfigurations.py` & `RSTAB-1.9.5/RSTAB/SteelDesign/steelUltimateConfigurations.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,67 +1,68 @@
 from RSTAB.initModel import Model, clearAttributes, deleteEmptyAttributes, ConvertToDlString
 
-
-class ConcreteUltimateConfiguration():
+class SteelDesignUltimateConfigurations():
 
     def __init__(self,
-                no: int = 1,
-                name: str = 'ULS',
-                members: str = 'All',
-                member_sets: str = 'All',
-                comment: str = '',
-                params: dict = None,
-                model = Model):
+                 no: int = 1,
+                 name: str = 'ULS1',
+                 members_no: str = 'All',
+                 member_sets_no: str = 'All',
+                 comment: str = '',
+                 params: dict = None,
+                 model = Model):
+
         """
         Args:
-            no (int): Configuration Tag
-            name (str): User Defined Name
-            members (str): Assigned Members
-            member_sets (str): Assigned Member Sets
+            no (int): Steel Design Ultimate Configuration Tag
+            name (str): User Defined Configuration Name
+            members_no (str): Assign Configuration to Selected Members
+            member_sets_no (str): Assign Configuration to Selected Member Sets
             comment (str, optional): Comment
             params (dict, optional): Any WS Parameter relevant to the object and its value in form of a dictionary
             model (RSTAB Class, optional): Model to be edited
         """
 
-        # Client model | Concrete Durabilities
-        clientObject = model.clientModel.factory.create('ns0:concrete_design_uls_configuration')
+        # Client Model | Steel Design Ultimate Configurations
+        clientObject = model.clientModel.factory.create('ns0:steel_design_uls_configuration')
 
         # Clears object atributes | Sets all atributes to None
         clearAttributes(clientObject)
 
-        # Concrete Durability No.
+        # ULS Configuration No.
         clientObject.no = no
 
         # User Defined Name
         if name:
             clientObject.user_defined_name_enabled = True
             clientObject.name = name
 
         # Assigned Members
-        if members == 'All':
+        if members_no == 'All':
             clientObject.assigned_to_all_members = True
 
         else:
             clientObject.assigned_to_all_members = False
-            clientObject.assigned_to_members = ConvertToDlString(members)
+            clientObject.assigned_to_members = ConvertToDlString(members_no)
 
         # Assigned Member Sets
-        if member_sets == 'All':
+        if member_sets_no == 'All':
             clientObject.assigned_to_all_member_sets = True
 
         else:
             clientObject.assigned_to_all_member_sets = False
-            clientObject.assigned_to_member_sets = ConvertToDlString(member_sets)
+            clientObject.assigned_to_member_sets = ConvertToDlString(member_sets_no)
 
         # Comment
         clientObject.comment = comment
 
         # Adding optional parameters via dictionary
         if params:
             for key in params:
                 clientObject[key] = params[key]
 
         # Delete None attributes for improved performance
         deleteEmptyAttributes(clientObject)
 
-        # Add Global Parameter to client model
-        model.clientModel.service.set_concrete_design_uls_configuration(clientObject)
+        # Add Global Parameters to Client Model
+        model.clientModel.service.set_steel_design_uls_configuration(clientObject)
+
```

### Comparing `RSTAB-1.9.3/RSTAB/DynamicLoads/responseSpectrum.py` & `RSTAB-1.9.5/RSTAB/DynamicLoads/responseSpectrum.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/GuideObjects/note.py` & `RSTAB-1.9.5/RSTAB/GuideObjects/note.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/Imperfections/imperfectionCase.py` & `RSTAB-1.9.5/RSTAB/Imperfections/imperfectionCase.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/Imperfections/memberImperfection.py` & `RSTAB-1.9.5/RSTAB/Imperfections/memberImperfection.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/Imperfections/membersetImperfection.py` & `RSTAB-1.9.5/RSTAB/Imperfections/membersetImperfection.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/ImportExport/exports.py` & `RSTAB-1.9.5/RSTAB/ImportExport/exports.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/ImportExport/imports.py` & `RSTAB-1.9.5/RSTAB/ImportExport/imports.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/LoadCasesAndCombinations/action.py` & `RSTAB-1.9.5/RSTAB/LoadCasesAndCombinations/action.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,21 +12,23 @@
                  comment: str = '',
                  params: dict = None,
                  model = Model):
         '''
         Combination Wizard Action
 
         Args:
-            no (int, optional): Action number
-            action_category (enum, optional): Action category
-            action_type (enum, optional): Action type
-            action_items (list or list of lists, optional):
-                - if action_type == 'ACTING_DIFFERENTLY': [[Load_case, acting_group], ...]
-                - else: [Load_case, Load_case, ...]
-            name (str, optional): Action name
+            no (int, optional): Action Tag
+            action_category (enum, optional): Action Category Type Enumeration
+            action_type (enum, optional): Action Type Enumeration
+            action_items (list or list of lists, optional): Action Items
+                if action_type == 'ACTING_DIFFERENTLY':
+                    action_items = [[Load_case, acting_group], ...]
+                else:
+                    action_items = [Load_case, Load_case, ...]
+            name (str, optional): User Defined Action Name
             is_active (bool, optional): Define if active
             comment (str, optional): Comments
             params (dict, optional): Any WS Parameter relevant to the object and its value in form of a dictionary
             model (RSTAB Class, optional): Model to be edited
         '''
 
         # Client model | Action
```

### Comparing `RSTAB-1.9.3/RSTAB/LoadCasesAndCombinations/actionCombination.py` & `RSTAB-1.9.5/RSTAB/LoadCasesAndCombinations/actionCombination.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def ActionCombinationItem(model = Model, **kwargs):
     '''
     Set Action Combination Item.
 
     Args:
         model (RSTAB Class): Model to be edited
-        **kwargs - pass a keyworded, variable-length argument list. Following are all possible keywords:
+        **kwargs - Pass a keyworded, variable-length argument list. Following are all possible keywords:
 
         action_item, operator_type, left_parenthesis, right_parenthesis, group_factor, action_factor,
         action_load_type, group_load_type, action, is_leading, gamma, psi, xi, k_fi, c_esl, k_def,
         psi_0, psi_1, psi_2, fi, gamma_0, alfa, k_f, phi, omega_0, gamma_l_1, k_creep, gamma_n, j_2
     Usage:
         aci1 = ActionCombinationItem(Model, action_item=1, operator_type=OperatorType.OPERATOR_AND.name, action_factor=1.0, action=1)
 
@@ -43,18 +43,18 @@
         '''
         Action Combination
 
         Attribute: Design Situation
         WARNING: Only design situations with an assigned combination wizard where a user-defined action combination is set are valid.
 
         Args:
-            no (int, mandatory): Action number
-            design_situation (int, mandatory): Design Situation
-            action_combination_items (list, mandatory): Action Combination Items list
-            name (str, optional): Action Combination name
+            no (int): Action Combination Tag
+            design_situation (int): Design Situation
+            action_combination_items (list): Action Combination Items list
+            name (str, optional): User Defined Action Combination Name
             active (bool, optional): Define if Active
             comment (str, optional): Comments
             params (dict, optional): Any WS Parameter relevant to the object and its value in form of a dictionary
             model (RSTAB Class, optional): Model to be edited
         '''
 
         # Client model | Action
@@ -104,15 +104,15 @@
 
     @staticmethod
     def DeleteActionCombination(action_combination_no: str = '1 2', model = Model):
         '''
         Delete Action Combination object(s)
 
         Args:
-            actions_no (str): Numbers of Action Combinations to be deleted
+            action_combination_no (str): Numbers of Action Combinations to be deleted
             model (RSTAB Class, optional): Model to be edited
         '''
 
         # Delete Action Combinations from client model
         for ac in ConvertStrToListOfInt(action_combination_no):
             model.clientModel.service.delete_object(ObjectTypes.E_OBJECT_TYPE_ACTION_COMBINATION.name, ac)
```

### Comparing `RSTAB-1.9.3/RSTAB/LoadCasesAndCombinations/combinationWizard.py` & `RSTAB-1.9.5/RSTAB/LoadCasesAndCombinations/combinationWizard.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from RSTAB.initModel import Model, clearAttributes, deleteEmptyAttributes
-from RSTAB.enums import LoadWizardType, InitialStateDefintionType
+from RSTAB.enums import LoadWizardType
 
 class CombinationWizard():
     def __init__(self,
                 no: int = 1,
                 name: str = '',
                 static_analysis_settings: int = 1,
                 stability_analysis_setting: int = 1,
```

### Comparing `RSTAB-1.9.3/RSTAB/LoadCasesAndCombinations/designSituation.py` & `RSTAB-1.9.5/RSTAB/LoadCasesAndCombinations/designSituation.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/LoadCasesAndCombinations/loadCase.py` & `RSTAB-1.9.5/RSTAB/LoadCasesAndCombinations/loadCase.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/LoadCasesAndCombinations/loadCasesAndCombinations.py` & `RSTAB-1.9.5/RSTAB/LoadCasesAndCombinations/loadCasesAndCombinations.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/LoadCasesAndCombinations/loadCombination.py` & `RSTAB-1.9.5/RSTAB/LoadCasesAndCombinations/loadCombination.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/LoadCasesAndCombinations/modalAnalysisSettings.py` & `RSTAB-1.9.5/RSTAB/LoadCasesAndCombinations/modalAnalysisSettings.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/LoadCasesAndCombinations/resultCombination.py` & `RSTAB-1.9.5/RSTAB/LoadCasesAndCombinations/resultCombination.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,29 +16,29 @@
                  name: str = '',
                  comment: str = '',
                  params: dict = None,
                  model = Model):
 
         '''
         Args:
-            no (int, mandatory): Result combination tag
-            design_situation (int, mandatory): Design situation
-            combination_type (enum, mandatory): Combination type
-            combination_items (list of lists, mandatory): Combination items
+            no (int): Result Combination tag
+            design_situation (int): Assign Design Situation
+            combination_type (enum): Result Combination Type Enumeration
+            combination_items (list of lists): Combination Items Table
                 combination_item[0](int) = case_object_item
                 combination_item[1](enum) = operator_type enumeration
                 combination_item[2](float) = case_object_factor
                 combination_item[3](enum) = case_object_load_type enumeration
                 combination_item[4](bool) = left_parenthesis (if parenthesis active in LoadCaseandCombination)
                 combination_item[5](bool) = right_parenthesis (if parenthesis active in LoadCaseandCombination)
                 combination_item[6](float) = group_factor (if left_parenthesis is True then value else None)
                 combination_item[7](enum) = group_load_type (if right_parenthesis is True then enumeration else None)
             srss_combination (list, optional): SRSS Combination. If None then False.
-                [srss_use_equivalent_linear_combination[bool], ]
-            name (str, optional): Result combination name
+                srss_combination = [srss_use_equivalent_linear_combination(bool), srss_extreme_value_sign(enum), srss_according_load_case_or_combination(int)]
+            name (str, optional): User Defined Result Combination Name
             comment (str, optional): Comments
             params (dict, optional): Any WS Parameter relevant to the object and its value in form of a dictionary
             model (RSTAB Class, optional): Model to be edited
         '''
 
         # Client model | Result Combination
         clientObject = model.clientModel.factory.create('ns0:result_combination')
```

### Comparing `RSTAB-1.9.3/RSTAB/LoadCasesAndCombinations/spectralAnalysisSettings.py` & `RSTAB-1.9.5/RSTAB/LoadCasesAndCombinations/spectralAnalysisSettings.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/LoadCasesAndCombinations/stabilityAnalysisSettings.py` & `RSTAB-1.9.5/RSTAB/LoadCasesAndCombinations/stabilityAnalysisSettings.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/LoadCasesAndCombinations/staticAnalysisSettings.py` & `RSTAB-1.9.5/RSTAB/LoadCasesAndCombinations/staticAnalysisSettings.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,18 +60,18 @@
                   comment: str = '',
                   params: dict = None,
                   model = Model):
 
         """
         Args:
             no (int): Static Analysis Setting Tag
-            name (str): Static Analysis Setting Name
-            load_modification (list): Load Modification Parameters
+            name (str, optional): Static Analysis Setting Name
+            load_modification (list, optional): Load Modification Parameters
                 load_modification = [loading_by_multiplier_factor, multiplier_factor, dividing_results]
-            mass_conversion (list): Mass Conversion Parameters
+            mass_conversion (list, optional): Mass Conversion Parameters
                 mass_conversion = [mass_conversion_enabled, mass_conversion_factor_in_direction_x, mass_conversion_factor_in_direction_y, mass_conversion_factor_in_direction_z]
             comment (str, optional): Comments
             params (dict, optional): Any WS Parameter relevant to the object and its value in form of a dictionary
             model (RSTAB Class, optional): Model to be edited
         """
 
         # Client model
@@ -134,23 +134,23 @@
                   comment: str = '',
                   params: dict = {'save_results_of_all_load_increments': False},
                   model = Model):
 
         """
         Args:
             no (int): Static Analysis Setting Tag
-            name (str):  Static Analysis Setting Name
+            name (str, optional):  Static Analysis Setting Name
             iterative_method (enum): Static Analysis Settings Iterative Method for Non-linear Analysis Enumeration
             precision_of_convergence_criteria_for_nonlinear_calculation (float): Precision of Convergence defaults to 0
             max_number_of_iterations (float): Maximum Number of Iterations
             number_of_load_increments (float): Number of Load Increments
-            load_modification (list): Load Modification Parameters
+            load_modification (list, optional): Load Modification Parameters
                 load_modification = [loading_by_multiplier_factor, multiplier_factor, dividing_results]
-            bourdon_effect (bool): Bourdon Effect Boolean
-            mass_conversion (list): Mass Conversion Parameters
+            bourdon_effect (bool, optional): Bourdon Effect Boolean
+            mass_conversion (list, optional): Mass Conversion Parameters
                 mass_conversion = [mass_conversion_enabled, mass_conversion_factor_in_direction_x, mass_conversion_factor_in_direction_y, mass_conversion_factor_in_direction_z]
             comment (str, optional): Comments
             params (dict, optional): Any WS Parameter relevant to the object and its value in form of a dictionary
             model (RSTAB Class, optional): Model to be edited
         """
 
         # Client model
```

### Comparing `RSTAB-1.9.3/RSTAB/Loads/imposedNodalDeformation.py` & `RSTAB-1.9.5/RSTAB/Loads/imposedNodalDeformation.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/Loads/memberLoad.py` & `RSTAB-1.9.5/RSTAB/Loads/memberLoad.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/Loads/membersetload.py` & `RSTAB-1.9.5/RSTAB/Loads/membersetload.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/Loads/nodalLoad.py` & `RSTAB-1.9.5/RSTAB/Loads/nodalLoad.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/Reports/favicon32.png` & `RSTAB-1.9.5/RSTAB/Reports/favicon32.png`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/Reports/html.py` & `RSTAB-1.9.5/RSTAB/Reports/html.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/Reports/htmlScript.js` & `RSTAB-1.9.5/RSTAB/Reports/htmlScript.js`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/Reports/htmlStyles.css` & `RSTAB-1.9.5/RSTAB/Reports/htmlStyles.css`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/Reports/partsList.py` & `RSTAB-1.9.5/RSTAB/Reports/partsList.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/Reports/printoutReport.py` & `RSTAB-1.9.5/RSTAB/Reports/printoutReport.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/Results/designOverview.py` & `RSTAB-1.9.5/RSTAB/Results/designOverview.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/Results/resultTables.py` & `RSTAB-1.9.5/RSTAB/Results/resultTables.py`

 * *Files 7% similar despite different names*

```diff
@@ -4762,7 +4762,451 @@
          Args:
             loading_type (emun): Loading type (LC2 = E_OBJECT_TYPE_LOAD_CASE)
             loading_no (int): Loading Number (CO2 = 2)
             model (class, optional): Model instance
         '''
 
         return model.clientModel.service.has_results(loading_type.name, loading_no)
+
+    @staticmethod
+    def AluminumDesignDesignRatiosMemberRepresentativesByConstructionStage(
+        include_base: bool = False,
+        model = Model):
+
+        '''
+        Args:
+            model(class, optional): Model instance
+        '''
+
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_aluminum_design_design_ratios_member_representatives_by_construction_stage(), include_base)
+
+    @staticmethod
+    def AluminumDesignDesignRatiosMemberRepresentativesByDesignSituation(
+        include_base: bool = False,
+        model = Model):
+
+        '''
+        Args:
+            model(class, optional): Model instance
+        '''
+
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_aluminum_design_design_ratios_member_representatives_by_design_situation(), include_base)
+
+    @staticmethod
+    def AluminumDesignDesignRatiosMemberRepresentativesByLoading(
+        include_base: bool = False,
+        model = Model):
+
+        '''
+        Args:
+            model(class, optional): Model instance
+        '''
+
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_aluminum_design_design_ratios_member_representatives_by_loading(), include_base)
+
+    @staticmethod
+    def AluminumDesignDesignRatiosMemberRepresentativesByLocation(
+        include_base: bool = False,
+        model = Model):
+
+        '''
+        Args:
+            model(class, optional): Model instance
+        '''
+
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_aluminum_design_design_ratios_member_representatives_by_location(), include_base)
+
+    @staticmethod
+    def AluminumDesignDesignRatiosMemberRepresentativesByMaterial(
+        include_base: bool = False,
+        model = Model):
+
+        '''
+        Args:
+            model(class, optional): Model instance
+        '''
+
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_aluminum_design_design_ratios_member_representatives_by_material(), include_base)
+
+    @staticmethod
+    def AluminumDesignDesignRatiosMemberRepresentativesByMemberRepresentative(
+        include_base: bool = False,
+        model = Model):
+
+        '''
+        Args:
+            model(class, optional): Model instance
+        '''
+
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_aluminum_design_design_ratios_member_representatives_by_member_representative(), include_base)
+
+    @staticmethod
+    def AluminumDesignDesignRatiosMemberRepresentativesBySection(
+        include_base: bool = False,
+        model = Model):
+
+        '''
+        Args:
+            model(class, optional): Model instance
+        '''
+
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_aluminum_design_design_ratios_member_representatives_by_section(), include_base)
+
+    @staticmethod
+    def AluminumDesignDesignRatiosMemberSetRepresentativesByConstructionStage(
+        include_base: bool = False,
+        model = Model):
+
+        '''
+        Args:
+            model(class, optional): Model instance
+        '''
+
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_aluminum_design_design_ratios_member_set_representatives_by_construction_stage(), include_base)
+
+    @staticmethod
+    def AluminumDesignDesignRatiosMemberSetRepresentativesByDesignSituation(
+        include_base: bool = False,
+        model = Model):
+
+        '''
+        Args:
+            model(class, optional): Model instance
+        '''
+
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_aluminum_design_design_ratios_member_set_representatives_by_design_situation(), include_base)
+
+    @staticmethod
+    def AluminumDesignDesignRatiosMemberSetRepresentativesByLoading(
+        include_base: bool = False,
+        model = Model):
+
+        '''
+        Args:
+            model(class, optional): Model instance
+        '''
+
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_aluminum_design_design_ratios_member_set_representatives_by_loading(), include_base)
+
+    @staticmethod
+    def AluminumDesignDesignRatiosMemberSetRepresentativesByLocation(
+        include_base: bool = False,
+        model = Model):
+
+        '''
+        Args:
+            model(class, optional): Model instance
+        '''
+
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_aluminum_design_design_ratios_member_set_representatives_by_location(), include_base)
+
+    @staticmethod
+    def AluminumDesignDesignRatiosMemberSetRepresentativesByMaterial(
+        include_base: bool = False,
+        model = Model):
+
+        '''
+        Args:
+            model(class, optional): Model instance
+        '''
+
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_aluminum_design_design_ratios_member_set_representatives_by_material(), include_base)
+
+    @staticmethod
+    def AluminumDesignDesignRatiosMemberSetRepresentativesByMemberSetRepresentative(
+        include_base: bool = False,
+        model = Model):
+
+        '''
+        Args:
+            model(class, optional): Model instance
+        '''
+
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_aluminum_design_design_ratios_member_set_representatives_by_member_set_representative(), include_base)
+
+    @staticmethod
+    def AluminumDesignDesignRatiosMemberSetRepresentativesBySection(
+        include_base: bool = False,
+        model = Model):
+
+        '''
+        Args:
+            model(class, optional): Model instance
+        '''
+
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_aluminum_design_design_ratios_member_set_representatives_by_section(), include_base)
+
+    @staticmethod
+    def AluminumDesignDesignRatiosMembersByConstructionStage(
+        include_base: bool = False,
+        model = Model):
+
+        '''
+        Args:
+            model(class, optional): Model instance
+        '''
+
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_aluminum_design_design_ratios_members_by_construction_stage(), include_base)
+
+    @staticmethod
+    def AluminumDesignDesignRatiosMembersByDesignSituation(
+        include_base: bool = False,
+        model = Model):
+
+        '''
+        Args:
+            model(class, optional): Model instance
+        '''
+
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_aluminum_design_design_ratios_members_by_design_situation(), include_base)
+
+    @staticmethod
+    def AluminumDesignDesignRatiosMembersByLoading(
+        include_base: bool = False,
+        model = Model):
+
+        '''
+        Args:
+            model(class, optional): Model instance
+        '''
+
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_aluminum_design_design_ratios_members_by_loading(), include_base)
+
+    @staticmethod
+    def AluminumDesignDesignRatiosMembersByLocation(
+        include_base: bool = False,
+        model = Model):
+
+        '''
+        Args:
+            model(class, optional): Model instance
+        '''
+
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_aluminum_design_design_ratios_members_by_location(), include_base)
+
+    @staticmethod
+    def AluminumDesignDesignRatiosMembersByMaterial(
+        include_base: bool = False,
+        model = Model):
+
+        '''
+        Args:
+            model(class, optional): Model instance
+        '''
+
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_aluminum_design_design_ratios_members_by_material(), include_base)
+
+    @staticmethod
+    def AluminumDesignDesignRatiosMembersByMember(
+        include_base: bool = False,
+        model = Model):
+
+        '''
+        Args:
+            model(class, optional): Model instance
+        '''
+
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_aluminum_design_design_ratios_members_by_member(), include_base)
+
+    @staticmethod
+    def AluminumDesignDesignRatiosMembersByMemberSet(
+        include_base: bool = False,
+        model = Model):
+
+        '''
+        Args:
+            model(class, optional): Model instance
+        '''
+
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_aluminum_design_design_ratios_members_by_member_set(), include_base)
+
+    @staticmethod
+    def AluminumDesignDesignRatiosMembersBySection(
+        include_base: bool = False,
+        model = Model):
+
+        '''
+        Args:
+            model(class, optional): Model instance
+        '''
+
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_aluminum_design_design_ratios_members_by_section(), include_base)
+
+    @staticmethod
+    def AluminumDesignGoverningInternalForcesByMember(
+        include_base: bool = False,
+        model = Model):
+
+        '''
+        Args:
+            model(class, optional): Model instance
+        '''
+
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_aluminum_design_governing_internal_forces_by_member(), include_base)
+
+    @staticmethod
+    def AluminumDesignGoverningInternalForcesByMemberEnds(
+        include_base: bool = False,
+        model = Model):
+
+        '''
+        Args:
+            model(class, optional): Model instance
+        '''
+
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_aluminum_design_governing_internal_forces_by_member_ends(), include_base)
+
+    @staticmethod
+    def AluminumDesignGoverningInternalForcesByMemberRepresentative(
+        include_base: bool = False,
+        model = Model):
+
+        '''
+        Args:
+            model(class, optional): Model instance
+        '''
+
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_aluminum_design_governing_internal_forces_by_member_representative(), include_base)
+
+    @staticmethod
+    def AluminumDesignGoverningInternalForcesByMemberRepresentativeEnds(
+        include_base: bool = False,
+        model = Model):
+
+        '''
+        Args:
+            model(class, optional): Model instance
+        '''
+
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_aluminum_design_governing_internal_forces_by_member_representative_ends(), include_base)
+
+    @staticmethod
+    def AluminumDesignGoverningInternalForcesByMemberSet(
+        include_base: bool = False,
+        model = Model):
+
+        '''
+        Args:
+            model(class, optional): Model instance
+        '''
+
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_aluminum_design_governing_internal_forces_by_member_set(), include_base)
+
+    @staticmethod
+    def AluminumDesignGoverningInternalForcesByMemberSetEnds(
+        include_base: bool = False,
+        model = Model):
+
+        '''
+        Args:
+            model(class, optional): Model instance
+        '''
+
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_aluminum_design_governing_internal_forces_by_member_set_ends(), include_base)
+
+    @staticmethod
+    def AluminumDesignGoverningInternalForcesByMemberSetRepresentative(
+        include_base: bool = False,
+        model = Model):
+
+        '''
+        Args:
+            model(class, optional): Model instance
+        '''
+
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_aluminum_design_governing_internal_forces_by_member_set_representative(), include_base)
+
+    @staticmethod
+    def AluminumDesignGoverningInternalForcesByMemberSetRepresentativeEnds(
+        include_base: bool = False,
+        model = Model):
+
+        '''
+        Args:
+            model(class, optional): Model instance
+        '''
+
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_aluminum_design_governing_internal_forces_by_member_set_representative_ends(), include_base)
+
+    @staticmethod
+    def AluminumDesignGoverningLoading(
+        include_base: bool = False,
+        model = Model):
+
+        '''
+        Args:
+            model(class, optional): Model instance
+        '''
+
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_aluminum_design_governing_loading(), include_base)
+
+    @staticmethod
+    def AluminumDesignOverviewErrorsAndWarnings(
+        include_base: bool = False,
+        model = Model):
+
+        '''
+        Args:
+            model(class, optional): Model instance
+        '''
+
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_aluminum_design_overview_errors_and_warnings(), include_base)
+
+    @staticmethod
+    def AluminumDesignOverviewNotValidDeactivated(
+        include_base: bool = False,
+        model = Model):
+
+        '''
+        Args:
+            model(class, optional): Model instance
+        '''
+
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_aluminum_design_overview_not_valid_deactivated(), include_base)
+
+    @staticmethod
+    def AluminumDesignSlendernessByMember(
+        include_base: bool = False,
+        model = Model):
+
+        '''
+        Args:
+            model(class, optional): Model instance
+        '''
+
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_aluminum_design_slenderness_by_member(), include_base)
+
+    @staticmethod
+    def AluminumDesignSlendernessByMemberRepresentative(
+        include_base: bool = False,
+        model = Model):
+
+        '''
+        Args:
+            model(class, optional): Model instance
+        '''
+
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_aluminum_design_slenderness_by_member_representative(), include_base)
+
+    @staticmethod
+    def AluminumDesignSlendernessByMemberSet(
+        include_base: bool = False,
+        model = Model):
+
+        '''
+        Args:
+            model(class, optional): Model instance
+        '''
+
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_aluminum_design_slenderness_by_member_set(), include_base)
+
+    @staticmethod
+    def AluminumDesignSlendernessByMemberSetRepresentative(
+        include_base: bool = False,
+        model = Model):
+
+        '''
+        Args:
+            model(class, optional): Model instance
+        '''
+
+        return ConvertResultsToListOfDct(model.clientModel.service.get_results_for_aluminum_design_slenderness_by_member_set_representative(), include_base)
```

### Comparing `RSTAB-1.9.3/RSTAB/SpecialObjects/nodalRelease.py` & `RSTAB-1.9.5/RSTAB/SpecialObjects/nodalRelease.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/SpecialObjects/structureModification.py` & `RSTAB-1.9.5/RSTAB/SpecialObjects/structureModification.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/SteelDesign/steelServiceabilityConfiguration.py` & `RSTAB-1.9.5/RSTAB/SteelDesign/steelServiceabilityConfiguration.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/SteelDesign/steelUltimateConfigurations.py` & `RSTAB-1.9.5/RSTAB/TimberDesign/timberUltimateConfigurations.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from RSTAB.initModel import Model, clearAttributes, deleteEmptyAttributes, ConvertToDlString
 
-class SteelDesignUltimateConfigurations():
+class TimberDesignUltimateConfigurations():
 
     def __init__(self,
                  no: int = 1,
                  name: str = 'ULS1',
                  members_no: str = 'All',
                  member_sets_no: str = 'All',
                  comment: str = '',
                  params: dict = None,
                  model = Model):
 
         """
         Args:
-            no (int): Steel Design Ultimate Configuration Tag
+            no (int): Timber Design Ultimate Configuration Tag
             name (str): User Defined Configuration Name
             members_no (str): Assign Configuration to Selected Members
             member_sets_no (str): Assign Configuration to Selected Member Sets
             comment (str, optional): Comment
             params (dict, optional): Any WS Parameter relevant to the object and its value in form of a dictionary
             model (RSTAB Class, optional): Model to be edited
         """
 
-        # Client Model | Steel Design Ultimate Configurations
-        clientObject = model.clientModel.factory.create('ns0:steel_design_uls_configuration')
+        # Client Model | Timber Design Ultimate Configurations
+        clientObject = model.clientModel.factory.create('ns0:timber_design_uls_configuration')
 
         # Clears object atributes | Sets all atributes to None
         clearAttributes(clientObject)
 
         # ULS Configuration No.
         clientObject.no = no
 
@@ -60,9 +60,9 @@
             for key in params:
                 clientObject[key] = params[key]
 
         # Delete None attributes for improved performance
         deleteEmptyAttributes(clientObject)
 
         # Add Global Parameters to Client Model
-        model.clientModel.service.set_steel_design_uls_configuration(clientObject)
+        model.clientModel.service.set_timber_design_uls_configuration(clientObject)
```

### Comparing `RSTAB-1.9.3/RSTAB/TimberDesign/timberServiceLimitStateConfigurations.py` & `RSTAB-1.9.5/RSTAB/TimberDesign/timberServiceLimitStateConfigurations.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/TimberDesign/timberUltimateConfigurations.py` & `RSTAB-1.9.5/RSTAB/TypesForTimberDesign/timberMoistureClass.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,68 +1,61 @@
 from RSTAB.initModel import Model, clearAttributes, deleteEmptyAttributes, ConvertToDlString
+from RSTAB.enums import TimberMoistureClassType
 
-class TimberDesignUltimateConfigurations():
-
+class TimberMoistureClass():
     def __init__(self,
-                 no: int = 1,
-                 name: str = 'ULS1',
-                 members_no: str = 'All',
-                 member_sets_no: str = 'All',
-                 comment: str = '',
-                 params: dict = None,
-                 model = Model):
-
+                no: int = 1,
+                name: str = '',
+                members: str = '',
+                member_sets: str = '',
+                moisture_class = TimberMoistureClassType.TIMBER_MOISTURE_CLASS_TYPE_1,
+                comment: str = '',
+                params: dict = None,
+                model = Model):
         """
         Args:
-            no (int): Timber Design Ultimate Configuration Tag
-            name (str): User Defined Configuration Name
-            members_no (str): Assign Configuration to Selected Members
-            member_sets_no (str): Assign Configuration to Selected Member Sets
+            no (int): Timber Moisture Class Tag
+            name (str): User Defined Moisture Class Name
+            members (str): Assigned Members
+            member_sets (str): Assigned Member Sets
+            moisture_class (enum): Timber Moisture Class Enumeration
             comment (str, optional): Comment
             params (dict, optional): Any WS Parameter relevant to the object and its value in form of a dictionary
             model (RSTAB Class, optional): Model to be edited
         """
 
-        # Client Model | Timber Design Ultimate Configurations
-        clientObject = model.clientModel.factory.create('ns0:timber_design_uls_configuration')
+         # Client Model | Types For Timber Design Moisture Class
+        clientObject = model.clientModel.factory.create('ns0:timber_moisture_class')
 
         # Clears object atributes | Sets all atributes to None
         clearAttributes(clientObject)
 
-        # ULS Configuration No.
+        # Member Service Class
         clientObject.no = no
 
-        # User Defined Name
-        if name:
-            clientObject.user_defined_name_enabled = True
-            clientObject.name = name
-
         # Assigned Members
-        if members_no == 'All':
-            clientObject.assigned_to_all_members = True
-
-        else:
-            clientObject.assigned_to_all_members = False
-            clientObject.assigned_to_members = ConvertToDlString(members_no)
+        clientObject.member = ConvertToDlString(members)
 
         # Assigned Member Sets
-        if member_sets_no == 'All':
-            clientObject.assigned_to_all_member_sets = True
+        clientObject.member_sets = ConvertToDlString(member_sets)
 
-        else:
-            clientObject.assigned_to_all_member_sets = False
-            clientObject.assigned_to_member_sets = ConvertToDlString(member_sets_no)
+        # Moisture Class
+        clientObject.moisture_class = moisture_class.name
+
+        # User Defined Name
+        if name:
+            clientObject.user_defined_name_enabled = True
+            clientObject.name = name
 
         # Comment
         clientObject.comment = comment
 
         # Adding optional parameters via dictionary
         if params:
             for key in params:
                 clientObject[key] = params[key]
 
         # Delete None attributes for improved performance
         deleteEmptyAttributes(clientObject)
 
-        # Add Global Parameters to Client Model
-        model.clientModel.service.set_timber_design_uls_configuration(clientObject)
-
+        # Add Service Class to client model
+        model.clientModel.service.set_timber_moisture_class(clientObject)
```

### Comparing `RSTAB-1.9.3/RSTAB/Tools/GetObjectNumbersByType.py` & `RSTAB-1.9.5/RSTAB/Tools/GetObjectNumbersByType.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         func_vec = [[ObjectTypes.E_OBJECT_TYPE_COORDINATE_SYSTEM, lambda i: model.clientModel.service.get_coordinate_system(i), 'from RSTAB.BasicObjects.coordinateSystem import CoordinateSystem\n', 'CoordinateSystem'],
 			[ObjectTypes.E_OBJECT_TYPE_MATERIAL, lambda i: model.clientModel.service.get_material(i), 'from RSTAB.BasicObjects.material import Material\n', 'Material'],
             [ObjectTypes.E_OBJECT_TYPE_SECTION, lambda i: model.clientModel.service.get_section(i), 'from RSTAB.BasicObjects.section import Section\n', 'Section'],
             [ObjectTypes.E_OBJECT_TYPE_NODE, lambda i: model.clientModel.service.get_node(i), 'from RSTAB.BasicObjects.node import Node\n', 'Node'],
             [ObjectTypes.E_OBJECT_TYPE_MEMBER, lambda i: model.clientModel.service.get_member(i), 'from RSTAB.BasicObjects.member import Member\n', 'Member'],
             [ObjectTypes.E_OBJECT_TYPE_MEMBER_SET, lambda i: model.clientModel.service.get_member_set(i), 'from RSTAB.BasicObjects.memberSet import MemberSet\n', 'MemberSet'],
             [ObjectTypes.E_OBJECT_TYPE_STRUCTURE_MODIFICATION, lambda i: model.clientModel.service.get_structure_modification(i), 'from RSTAB.SpecialObjects.structureModification import StructureModification\n', 'StructureModification'],
-            # nodal_release
+            [ObjectTypes.E_OBJECT_TYPE_NODAL_RELEASE, lambda i: model.clientModel.service.get_nodal_release(i), 'from RSTAB.SpecialObjects.nodalRelease import NodalRelease\n', 'NodalRelease'],
             # blocks
 
             [ObjectTypes.E_OBJECT_TYPE_NODAL_SUPPORT, lambda i: model.clientModel.service.get_nodal_support(i), 'from RSTAB.TypesForNodes.nodalSupport import NodalSupport\n', 'NodalSupport'],
 
             [ObjectTypes.E_OBJECT_TYPE_MEMBER_HINGE, lambda i: model.clientModel.service.get_member_hinge(i), 'from RSTAB.TypesForMembers.memberHinge import MemberHinge\n', 'MemberHinge'],
             [ObjectTypes.E_OBJECT_TYPE_MEMBER_ECCENTRICITY, lambda i: model.clientModel.service.get_member_eccentricity(i), 'from RSTAB.TypesForMembers.memberEccentricity import MemberEccentricity\n', 'MemberEccentricity'],
             [ObjectTypes.E_OBJECT_TYPE_MEMBER_SUPPORT, lambda i: model.clientModel.service.get_member_support(i), 'from RSTAB.TypesForMembers.memberSupport import MemberSupport\n', 'MemberSupport'],
```

### Comparing `RSTAB-1.9.3/RSTAB/Tools/ModelCheck.py` & `RSTAB-1.9.5/RSTAB/Tools/ModelCheck.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/Tools/centreOfGravityAndObjectInfo.py` & `RSTAB-1.9.5/RSTAB/Tools/centreOfGravityAndObjectInfo.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/Tools/sectionDialogue.py` & `RSTAB-1.9.5/RSTAB/Tools/sectionDialogue.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/TypesForAluminumDesign/aluminumEffectiveLengths.py` & `RSTAB-1.9.5/RSTAB/TypesForAluminumDesign/aluminumEffectiveLengths.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/TypesForAluminumDesign/aluminumMemberLocalSectionReduction.py` & `RSTAB-1.9.5/RSTAB/TypesForAluminumDesign/aluminumMemberLocalSectionReduction.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/TypesForAluminumDesign/aluminumMemberTransverseWelds.py` & `RSTAB-1.9.5/RSTAB/TypesForAluminumDesign/aluminumMemberTransverseWelds.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/TypesForMembers/memberDefinableStiffness.py` & `RSTAB-1.9.5/RSTAB/TypesForMembers/memberDefinableStiffness.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/TypesForMembers/memberEccentricity.py` & `RSTAB-1.9.5/RSTAB/TypesForMembers/memberEccentricity.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/TypesForMembers/memberHinge.py` & `RSTAB-1.9.5/RSTAB/TypesForMembers/memberHinge.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/TypesForMembers/memberNonlinearity.py` & `RSTAB-1.9.5/RSTAB/TypesForMembers/memberNonlinearity.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/TypesForMembers/memberResultIntermediatePoints.py` & `RSTAB-1.9.5/RSTAB/TypesForMembers/memberResultIntermediatePoints.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/TypesForMembers/memberRotationalRestraint.py` & `RSTAB-1.9.5/RSTAB/TypesForMembers/memberRotationalRestraint.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/TypesForMembers/memberShearPanel.py` & `RSTAB-1.9.5/RSTAB/TypesForMembers/memberShearPanel.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/TypesForMembers/memberStiffnessModification.py` & `RSTAB-1.9.5/RSTAB/TypesForMembers/memberStiffnessModification.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/TypesForMembers/memberSupport.py` & `RSTAB-1.9.5/RSTAB/TypesForMembers/memberSupport.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/TypesForMembers/memberTransverseStiffeners.py` & `RSTAB-1.9.5/RSTAB/TypesForMembers/memberTransverseStiffeners.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/TypesForNodes/nodalSupport.py` & `RSTAB-1.9.5/RSTAB/TypesForNodes/nodalSupport.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/TypesForSpecialObjects/nodalReleaseType.py` & `RSTAB-1.9.5/RSTAB/TypesForSpecialObjects/nodalReleaseType.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/TypesForSteelDesign/SteelMemberLocalSectionReduction.py` & `RSTAB-1.9.5/RSTAB/TypesForSteelDesign/SteelMemberLocalSectionReduction.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/TypesForSteelDesign/steelBoundaryConditions.py` & `RSTAB-1.9.5/RSTAB/TypesForSteelDesign/steelBoundaryConditions.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/TypesForSteelDesign/steelEffectiveLengths.py` & `RSTAB-1.9.5/RSTAB/TypesForSteelDesign/steelEffectiveLengths.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/TypesForTimberDesign/timberEffectiveLengths.py` & `RSTAB-1.9.5/RSTAB/TypesForTimberDesign/timberEffectiveLengths.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/TypesForTimberDesign/timberMemberLocalSectionReduction.py` & `RSTAB-1.9.5/RSTAB/TypesForTimberDesign/timberMemberLocalSectionReduction.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/TypesForTimberDesign/timberServiceClass.py` & `RSTAB-1.9.5/RSTAB/TypesForTimberDesign/timberServiceClass.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/TypesForTimberDesign/timberServiceCondition.py` & `RSTAB-1.9.5/RSTAB/TypesForTimberDesign/timberServiceCondition.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/TypesforConcreteDesign/ConcreteDurability.py` & `RSTAB-1.9.5/RSTAB/TypesforConcreteDesign/ConcreteDurability.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/TypesforConcreteDesign/ConcreteEffectiveLength.py` & `RSTAB-1.9.5/RSTAB/TypesforConcreteDesign/ConcreteEffectiveLength.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/baseData.py` & `RSTAB-1.9.5/RSTAB/baseData.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/baseSettings.py` & `RSTAB-1.9.5/RSTAB/baseSettings.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/dependencies.py` & `RSTAB-1.9.5/RSTAB/dependencies.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 except:
     print('One of the required modules is not installed in your Python env.')
     instSUDS = input('\nDo you want to install all dependencies and check all their versions (y/n)? ')
     instSUDS = instSUDS.lower()
     if instSUDS == 'y':
         # Subprocess will be opened in cmd and closed automaticaly after installation.
         # Prevents invoking pip by an old script wrapper (https://github.com/pypa/pip/issues/5599)
+        import os
         import subprocess
         try:
             subprocess.call('python -m pip install --upgrade pip')
             subprocess.call('python -m pip install psutil requests six suds-py3 xmltodict pytest mock --user')
             os.execv(sys.executable, ['python'] + sys.argv)
         except:
             print('WARNING: Installation of modules failed!')
```

### Comparing `RSTAB-1.9.3/RSTAB/enums.py` & `RSTAB-1.9.5/RSTAB/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -2376,7 +2376,32 @@
     STIFFNESS_DIAGRAM_DEPENDS_ON_P, STIFFNESS_DIAGRAM_DEPENDS_ON_PX, STIFFNESS_DIAGRAM_DEPENDS_ON_PY, STIFFNESS_DIAGRAM_DEPENDS_ON_PZ = range(4)
 
 class NodalSupportStiffnessDiagramType(Enum):
     '''
     Nodal Support Stiffness Diagram Type Enumeration
     '''
     STIFFNESS_DIAGRAM_ENDING_TYPE_CONTINUOUS, STIFFNESS_DIAGRAM_ENDING_TYPE_FAILURE, STIFFNESS_DIAGRAM_ENDING_TYPE_YIELDING = range(3)
+
+class MaterialType(Enum):
+    '''
+    Material Type Enumeration
+    '''
+    TYPE_ALUMINUM, TYPE_BASIC, TYPE_CONCRETE, TYPE_FABRIC, TYPE_FIBER_CONCRETE, TYPE_FOIL, TYPE_GAS, TYPE_GLASS,\
+    TYPE_MASONRY, TYPE_METAL, TYPE_REINFORCING_STEEL, TYPE_SOIL, TYPE_STEEL, TYPE_TIMBER, TYPE_VIRTUAL_JOIST_GIRDER = range(15)
+
+class MaterialDefinitionType(Enum):
+    '''
+    Material Definition Type Enumeration
+    '''
+    DERIVED_G, DERIVED_NU, E_G_NO_NU, E_G_NU, NONE = range(5)
+
+class MaterialStiffnessModificationType(Enum):
+    '''
+    Material Stiffness Modification Type Enumeration
+    '''
+    STIFFNESS_MODIFICATION_TYPE_DIVISION, STIFFNESS_MODIFICATION_TYPE_MULTIPLICATION = range(2)
+
+class PoissonRatioEditableGroupType(Enum):
+    '''
+    Poisson Ratio Editable Group Type
+    '''
+    POISSON_RATIOS_GROUP_MAJOR_2D, POISSON_RATIOS_GROUP_MAJOR_3D, POISSON_RATIOS_GROUP_MINOR_2D, POISSON_RATIOS_GROUP_MINOR_3D = range(4)
```

### Comparing `RSTAB-1.9.3/RSTAB/formula.py` & `RSTAB-1.9.5/RSTAB/formula.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/globalParameter.py` & `RSTAB-1.9.5/RSTAB/globalParameter.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB/initModel.py` & `RSTAB-1.9.5/RSTAB/initModel.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import os
 import sys
 import RSTAB.dependencies # dependency check ahead of imports
 import socket
 import requests
+import xmltodict
+from urllib import request
 from suds import WebFault
 from suds.client import Client
 from RSTAB.enums import ObjectTypes, ModelType, AddOn
 from RSTAB.suds_requests import RequestsTransport
 from suds.cache import DocumentCache
 from tempfile import gettempdir
 import time
@@ -38,22 +40,31 @@
     else:
         print(f'Error: Port {urlAndPort} is not open.')
         print('Please check:')
         print('- If you have started RSTAB application at the remote destination correctly.')
         a_socket.close()
         sys.exit()
 
-    # Delete cached WSDL older than 1 day to reflect newer version of RSTAB
+    # Delete old cache if the version or mode doesn't correlate
     connectionGlobals.cacheLoc = os.path.join(gettempdir(), 'WSDL')
-    currentTime = time.time()
+    new_wsdl = request.urlopen(urlAndPort+'/wsdl')
+    new_wsdl_data = new_wsdl.read()
+    new_wsdl.close()
+    new_tns = xmltodict.parse(new_wsdl_data)['definitions']['@targetNamespace']
+
     if os.path.exists(connectionGlobals.cacheLoc):
         for file in os.listdir(connectionGlobals.cacheLoc):
             filePath = os.path.join(connectionGlobals.cacheLoc, file)
-            if (currentTime - os.path.getmtime(filePath)) > 86400:
-                os.remove(filePath)
+            if file.endswith('.xml'):
+                with open(filePath,'r', encoding='utf-8') as old_wsdl:
+                    old_wsdl_data = old_wsdl.read()
+                    old_wsdl.close()
+                    old_tns = xmltodict.parse(old_wsdl_data)['definitions']['@targetNamespace']
+                    if new_tns != old_tns:
+                        os.remove(filePath)
 
     # Check for issues locally and remotely
     try:
         connectionGlobals.ca = DocumentCache(location=connectionGlobals.cacheLoc)
         connectionGlobals.client = Client(urlAndPort+'/wsdl', location = urlAndPort, cache=connectionGlobals.ca)
         connectionGlobals.connected = True
 
@@ -118,76 +129,96 @@
 
         # The model suffix is omitted in modelLs, so it must be omitted in model_name to match exactly
         original_model_name = model_name
         if '.' in model_name:
             model_name = model_name.split('.')[0]
 
         if new_model:
-            # Requested new model but the model with given name was already connected
+            # Requested new model but the model with given name is already connected
             if model_name in self.clientModelDct:
                 cModel = self.clientModelDct[model_name]
+                # Asuming the existing model should be recycled everything have to be deleted,
+                # so the script won't add new objects on top of the old ones.
+                # Mainly used in cycles.
                 cModel.service.delete_all_results()
                 cModel.service.delete_all()
 
-            # Requested new model, model with given name DOESN'T exist yet
             else:
                 modelPath = ''
-                # Requested new model, model with given name was NOT connected yet but file with the same name was opened
+                # Requested new model, model with given name was NOT connected yet but file with the same name is opened in RSTAB
                 if model_name in modelLst:
                     id = 0
                     for i,j in enumerate(modelLst):
                         if modelLst[i] == model_name:
                             id = i
                     modelPath =  connectionGlobals.client.service.get_model(id)
-                elif model_name == "":
-                    modelPath =  connectionGlobals.client.service.get_active_model()
+
+                # Requested new model, model with given name DOESN'T exist yet
                 else:
-                    modelPath =  connectionGlobals.client.service.new_model(original_model_name)
+                    # If name is empty, active will be selected
+                    if model_name == "":
+                        modelPath =  connectionGlobals.client.service.get_active_model()
+                    # If there is no nodel with given name, new RFEM model will be created
+                    else:
+                        modelPath =  connectionGlobals.client.service.new_model(original_model_name)
+
                 modelPort = modelPath[-5:-1]
                 modelUrlPort = connectionGlobals.url+':'+modelPort
                 modelCompletePath = modelUrlPort+'/wsdl'
 
                 connectionGlobals.session = requests.Session()
                 adapter = requests.adapters.HTTPAdapter(pool_connections=1, pool_maxsize=1)
                 connectionGlobals.session.mount('http://', adapter)
                 trans = RequestsTransport(connectionGlobals.session)
 
                 cModel = Client(modelCompletePath, transport=trans, location = modelUrlPort, cache=connectionGlobals.ca, timeout=360)
 
-                cModel.service.delete_all_results()
-                cModel.service.delete_all()
-
                 self.clientModelDct[model_name] = cModel
 
         else:
-            # Requested model which was already connected
-            #assert model_name in self.clientModelDct or model_name in modelLst, 'WARNING: '+model_name +' is not connected neither opened in RSTAB.'
+            # Requested model is already opened in RFEM or even connected in self.clientModelDct.
+            # In this statement RFEM doesn't create new model in RFEM via new_model().
+
+            # assert model_name in self.clientModelDct or model_name in modelLst, 'WARNING: '+model_name +' is not connected neither opened in RFEM.'
 
+            # If model with same name is opened and alredy in clientModelDct.
+            # This is typicaly model created by RFEM Python Client.
             if model_name in self.clientModelDct:
                 cModel = self.clientModelDct[model_name]
+            # If opening new file.
+            # Model is opened in RFEM (model in modelLst) but it is not in clientModelDct yet to be edited or closed.
             elif model_name in modelLst:
                 id = 0
                 for i,j in enumerate(modelLst):
                     if modelLst[i] == model_name:
                         id = i
                 modelPath =  connectionGlobals.client.service.get_model(id)
+                self.clientModelDct[model_name] = cModel
                 modelPort = modelPath[-5:-1]
                 modelUrlPort = connectionGlobals.url+':'+modelPort
                 modelCompletePath = modelUrlPort+'/wsdl'
 
                 connectionGlobals.session = requests.Session()
                 adapter = requests.adapters.HTTPAdapter(pool_connections=1, pool_maxsize=1)
                 connectionGlobals.session.mount('http://', adapter)
                 trans = RequestsTransport(connectionGlobals.session)
 
                 cModel = Client(modelCompletePath, transport=trans, location = modelUrlPort, cache=connectionGlobals.ca, timeout=360)
-
-                self.clientModelDct[model_name] = cModel
             elif model_name == "":
                 modelPath =  connectionGlobals.client.service.get_active_model()
+                modelPort = modelPath[-5:-1]
+                modelUrlPort = connectionGlobals.url+':'+modelPort
+                modelCompletePath = modelUrlPort+'/wsdl'
+
+                connectionGlobals.session = requests.Session()
+                adapter = requests.adapters.HTTPAdapter(pool_connections=1, pool_maxsize=1)
+                connectionGlobals.session.mount('http://', adapter)
+                trans = RequestsTransport(connectionGlobals.session)
+
+                cModel = Client(modelCompletePath, transport=trans, location = modelUrlPort, cache=connectionGlobals.ca, timeout=360)
             else:
                 print('Model name "'+model_name+'" is not created in RSTAB. Consider changing new_model parameter in Model class from False to True.')
                 sys.exit()
 
         if delete:
             print('Deleting results...')
             cModel.service.delete_all_results()
@@ -279,15 +310,15 @@
 
     return obj
 
 def openFile(model_path):
     '''
     Open file with a name.
     This routine primarily adds client instance into
-    Model.clientModelLst which manages all connections to the models.
+    Model.clientModelDct which manages all connections to the models.
     New Model class instance is invoked.
     It should be used when opening a file.
 
     Args:
         model_path (str): Path to RSTAB9 model.
     Returns:
         model (client instance): RSTAB model instance
@@ -358,26 +389,30 @@
 def insertSpaces(lst: list):
     '''
     Add spaces between list of numbers.
     Returns list of values.
     '''
     return ' '.join(str(item) for item in lst)
 
-def Calculate_all(generateXmlSolverInput: bool = False, model = Model):
+def Calculate_all(skipWarnings: bool = False, model = Model):
     '''
     Calculates model.
     CAUTION: Don't use it in unit tests!
     It works when executing tests individually but when running all of them
     it causes RSTAB to stuck and generates failures, which are hard to investigate.
 
     Args:
-        generateXmlSolverInput (bool): Generate XML Solver Input
+        skipWarnings (bool): Warnings will be skipped
         model (RSTAB Class, optional): Model to be edited
     '''
-    calculationMessages = model.clientModel.service.calculate_all(generateXmlSolverInput)
+
+    from RSTAB.Tools.PlausibilityCheck import PlausibilityCheck
+    PlausibilityCheck()
+
+    calculationMessages = model.clientModel.service.calculate_all(skipWarnings)
     return calculationMessages
 
 def CalculateInCloud(machine_id, run_plausibility_check, calculate_despite_warnings_and_errors, email_notification, model = Model):
     '''
     Sends the current model to the defined server to be calculated in the cloud. Plausibility check before and email notification after the cloud calculation are optional.
     CAUTION: Don't use it in unit tests!
     It works when executing tests individually but when running all of them
@@ -648,20 +683,32 @@
 
     if loadCombinations:
         for loadCombination in loadCombinations:
             specificObjectsToCalculateCC = model.clientModel.factory.create('ns0:calculate_specific_loadings.loading')
             specificObjectsToCalculateCC.no = loadCombination
             specificObjectsToCalculateCC.type = ObjectTypes.E_OBJECT_TYPE_LOAD_COMBINATION.name
             specificObjectsToCalculate.loading.append(specificObjectsToCalculateCC)
+
+    errors_and_warnings = []
+    calculationMessages = []
+
     try:
-        calculationMessages = model.clientModel.service.calculate_specific(specificObjectsToCalculate,skipWarnings)
+        calculationMessages = model.clientModel.service.calculate_specific(specificObjectsToCalculate, skipWarnings)
     except Exception as exp:
-        calculationMessages = "Calculation was unsuccessful: " + repr(exp)
+        errors_and_warnings = ["Calculation was unsuccessful: " + repr(exp)]
 
-    return calculationMessages
+    if calculationMessages["errors_and_warnings"] and calculationMessages["errors_and_warnings"]["message"]:
+        errors_and_warnings = ["".join([message.message_type,\
+                                        ": Input field: ", message.input_field,\
+                                            ", object: ", message.object,\
+                                                ", current value: ", message.current_value,\
+                                                    ". Message: ", message.message]) if message.message_type == "ERROR"\
+                                                        else "".join([message.message_type, ": ", message.message]) if not skipWarnings else None for message in calculationMessages["errors_and_warnings"]["message"]]
+
+    return errors_and_warnings
 
 def FirstFreeIdNumber(memType = ObjectTypes.E_OBJECT_TYPE_MEMBER, parent_no: int = 0, model = Model):
     '''
     This method returns the next available Id Number for the selected object type
 
     Args:
         memType (enum): Object Type Enumeration
```

### Comparing `RSTAB-1.9.3/RSTAB/suds_requests.py` & `RSTAB-1.9.5/RSTAB/suds_requests.py`

 * *Files identical despite different names*

### Comparing `RSTAB-1.9.3/RSTAB.egg-info/PKG-INFO` & `RSTAB-1.9.5/RSTAB.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: RSTAB
-Version: 1.9.3
+Version: 1.9.5
 Summary: Python Framework for RSTAB9 Web Services
 Home-page: https://github.com/Dlubal-Software/RSTAB_Python_Client
 Author: Dlubal Software
 Author-email: info@dlubal.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: six
 Requires-Dist: suds-py3
 Requires-Dist: xmltodict
 Requires-Dist: pytest
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: RSTAB Version: 1.9.3 Summary: Python Framework for
+Metadata-Version: 2.1 Name: RSTAB Version: 1.9.5 Summary: Python Framework for
 RSTAB9 Web Services Home-page: https://github.com/Dlubal-Software/
 RSTAB_Python_Client Author: Dlubal Software Author-email: info@dlubal.com
 License: MIT Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.10 Description-Content-Type: text/markdown License-File: LICENSE Requires-
-Dist: requests Requires-Dist: six Requires-Dist: suds-py3 Requires-Dist:
-xmltodict Requires-Dist: pytest Requires-Dist: psutil Requires-Dist: mock
-Requires-Dist: setuptools
+:: 3.10 Classifier: Programming Language :: Python :: 3.11 Description-Content-
+Type: text/markdown License-File: LICENSE Requires-Dist: requests Requires-
+Dist: six Requires-Dist: suds-py3 Requires-Dist: xmltodict Requires-Dist:
+pytest Requires-Dist: psutil Requires-Dist: mock Requires-Dist: setuptools
 ************ _[[_DD_ll_uu_bb_aa_ll_ _SS_oo_ff_tt_ww_aa_rr_ee_]]DDlluubbaall SSooffttwwaarree GGmmbbHH [[!![[iimmaaggee]]((hhttttppss::////iimmgg..sshhiieellddss..iioo//
 ttwwiitttteerr//ffoollllooww//ddlluubbaall__eenn??ssttyyllee==ssoocciiaall))]]((hhttttppss::////ttwwiitttteerr..ccoomm//ddlluubbaall__eenn ""TTwwiitttteerr
     FFoollllooww"")) [[!![[iimmaaggee]]((hhttttppss::////iimmgg..sshhiieellddss..iioo//bbaaddggee//GGiittHHuubb--DDlluubbaall__SSooffttwwaarree--
 ddaarrkkbblluuee??llooggoo==ggiitthhuubb&&))]]((hhttttppss::////ggiitthhuubb..ccoomm//DDlluubbaall--SSooffttwwaarree ""GGiitthhuubb FFoollllooww"")) [[!!
   [[iimmaaggee]]((hhttttppss::////iimmgg..sshhiieellddss..iioo//bbaaddggee//hhttttpp::////--ddlluubbaall..ccoomm--ddaarrkkbblluuee))]]((hhttttppss::////
 wwwwww..ddlluubbaall..ccoomm//eenn--UUSS ""DDlluubbaall WWeebbssiittee"")) [[!![[iimmaaggee]]((hhttttppss::////iimmgg..sshhiieellddss..iioo//bbaaddggee//
     ddooccss--AAPPII--ddaarrkkbblluuee??llooggoo==rreeaadd--tthhee--ddooccss&&llooggooCCoolloorr==wwhhiittee))]]((hhttttppss::////ddlluubbaall--
```

### Comparing `RSTAB-1.9.3/RSTAB.egg-info/SOURCES.txt` & `RSTAB-1.9.5/RSTAB.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -20,29 +20,28 @@
 RSTAB.egg-info/not-zip-safe
 RSTAB.egg-info/requires.txt
 RSTAB.egg-info/top_level.txt
 RSTAB/AluminumDesign/__init__.py
 RSTAB/AluminumDesign/aluminumSLSConfiguration.py
 RSTAB/AluminumDesign/aluminumULSConfiguration.py
 RSTAB/BasicObjects/__init__.py
-RSTAB/BasicObjects/coordinateSystem.py
 RSTAB/BasicObjects/material.py
 RSTAB/BasicObjects/member.py
 RSTAB/BasicObjects/memberSet.py
 RSTAB/BasicObjects/node.py
 RSTAB/BasicObjects/section.py
 RSTAB/Calculate/__init__.py
-RSTAB/Calculate/memberDivision.py
 RSTAB/Calculate/optimizationSettings.py
 RSTAB/ConcreteDesign/ConcreteServiceabilityConfigurations.py
 RSTAB/ConcreteDesign/ConcreteUltimateConfigurations.py
 RSTAB/ConcreteDesign/__init__.py
 RSTAB/DynamicLoads/__init__.py
 RSTAB/DynamicLoads/responseSpectrum.py
 RSTAB/GuideObjects/__init__.py
+RSTAB/GuideObjects/coordinateSystem.py
 RSTAB/GuideObjects/note.py
 RSTAB/Imperfections/__init__.py
 RSTAB/Imperfections/imperfectionCase.py
 RSTAB/Imperfections/memberImperfection.py
 RSTAB/Imperfections/membersetImperfection.py
 RSTAB/ImportExport/__init__.py
 RSTAB/ImportExport/exports.py
```

### Comparing `RSTAB-1.9.3/setup.py` & `RSTAB-1.9.5/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,26 +3,27 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent
 readme = (here/"README.md").read_text(encoding="utf-8")
 
 setup(
     name='RSTAB',
-    version='1.09.3',
+    version='1.09.5',
     description='Python Framework for RSTAB9 Web Services',
     long_description=readme,
     long_description_content_type = "text/markdown",
     url="https://github.com/Dlubal-Software/RSTAB_Python_Client",
     author="Dlubal Software",
     author_email="info@dlubal.com",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.10"
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11"
     ],
     packages=find_packages(),
     package_dir={"RSTAB":"RSTAB"},
     include_package_data=True,
     install_requires=["requests", "six", "suds-py3", "xmltodict", "pytest", "psutil", "mock", "setuptools"],
     zip_safe = False
 )
```

