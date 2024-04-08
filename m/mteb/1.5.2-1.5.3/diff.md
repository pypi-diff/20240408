# Comparing `tmp/mteb-1.5.2.tar.gz` & `tmp/mteb-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mteb-1.5.2.tar", last modified: Thu Apr  4 12:49:30 2024, max compression
+gzip compressed data, was "mteb-1.5.3.tar", last modified: Mon Apr  8 07:41:30 2024, max compression
```

## Comparing `mteb-1.5.2.tar` & `mteb-1.5.3.tar`

### file list

```diff
@@ -1,371 +1,381 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.124882 mteb-1.5.2/
--rw-r--r--   0 root         (0) root         (0)    11357 2024-04-04 12:49:25.000000 mteb-1.5.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)    23581 2024-04-04 12:49:30.120882 mteb-1.5.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9190 2024-04-04 12:49:25.000000 mteb-1.5.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.068882 mteb-1.5.2/mteb/
--rw-r--r--   0 root         (0) root         (0)     1917 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.072882 mteb-1.5.2/mteb/abstasks/
--rw-r--r--   0 root         (0) root         (0)     1751 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/abstasks/AbsTask.py
--rw-r--r--   0 root         (0) root         (0)     3063 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/abstasks/AbsTaskBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     5881 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/abstasks/AbsTaskClassification.py
--rw-r--r--   0 root         (0) root         (0)     2389 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/abstasks/AbsTaskClustering.py
--rw-r--r--   0 root         (0) root         (0)     2542 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/abstasks/AbsTaskPairClassification.py
--rw-r--r--   0 root         (0) root         (0)     1120 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/abstasks/AbsTaskReranking.py
--rw-r--r--   0 root         (0) root         (0)    11806 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/abstasks/AbsTaskRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2007 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/abstasks/AbsTaskSTS.py
--rw-r--r--   0 root         (0) root         (0)     2296 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/abstasks/AbsTaskSummarization.py
--rw-r--r--   0 root         (0) root         (0)      880 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/abstasks/CrosslingualTask.py
--rw-r--r--   0 root         (0) root         (0)     2831 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/abstasks/LangMapping.py
--rw-r--r--   0 root         (0) root         (0)      998 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/abstasks/MultilingualTask.py
--rw-r--r--   0 root         (0) root         (0)     6430 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/abstasks/TaskMetadata.py
--rw-r--r--   0 root         (0) root         (0)      422 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/abstasks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5296 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/cmd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.072882 mteb-1.5.2/mteb/evaluation/
--rw-r--r--   0 root         (0) root         (0)    13124 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/evaluation/MTEB.py
--rw-r--r--   0 root         (0) root         (0)       56 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/evaluation/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.072882 mteb-1.5.2/mteb/evaluation/evaluators/
--rw-r--r--   0 root         (0) root         (0)     5849 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/evaluation/evaluators/BitextMiningEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     8942 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/evaluation/evaluators/ClassificationEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     1463 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/evaluation/evaluators/ClusteringEvaluator.py
--rw-r--r--   0 root         (0) root         (0)      744 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/evaluation/evaluators/Evaluator.py
--rw-r--r--   0 root         (0) root         (0)     7140 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/evaluation/evaluators/PairClassificationEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     9613 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/evaluation/evaluators/RerankingEvaluator.py
--rw-r--r--   0 root         (0) root         (0)    12487 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/evaluation/evaluators/RetrievalEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     2394 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/evaluation/evaluators/STSEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     4841 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/evaluation/evaluators/SummarizationEvaluator.py
--rw-r--r--   0 root         (0) root         (0)      324 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/evaluation/evaluators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5482 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/evaluation/evaluators/utils.py
--rw-r--r--   0 root         (0) root         (0)      835 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/logging.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.072882 mteb-1.5.2/mteb/tasks/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.072882 mteb-1.5.2/mteb/tasks/BitextMining/
--rw-r--r--   0 root         (0) root         (0)      369 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/BitextMining/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.072882 mteb-1.5.2/mteb/tasks/BitextMining/da/
--rw-r--r--   0 root         (0) root         (0)     1398 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/BitextMining/da/BornholmskBitextMining.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/BitextMining/da/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.076882 mteb-1.5.2/mteb/tasks/BitextMining/multilingual/
--rw-r--r--   0 root         (0) root         (0)     1076 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/BitextMining/multilingual/BUCCBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     2194 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/BitextMining/multilingual/DiaBLaBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     5780 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/BitextMining/multilingual/FloresBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     1411 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/BitextMining/multilingual/NorwegianCourtsBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     2797 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/BitextMining/multilingual/TatoebaBitextMining.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/BitextMining/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.076882 mteb-1.5.2/mteb/tasks/BitextMining/nb/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/BitextMining/nb/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1351 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/BitextMining/nb/norwegian_courts_bitext_mining.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.076882 mteb-1.5.2/mteb/tasks/Classification/
--rw-r--r--   0 root         (0) root         (0)     1232 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.076882 mteb-1.5.2/mteb/tasks/Classification/da/
--rw-r--r--   0 root         (0) root         (0)     1316 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/da/AngryTweetsClassification.py
--rw-r--r--   0 root         (0) root         (0)     1615 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/da/DKHateClassification.py
--rw-r--r--   0 root         (0) root         (0)     2505 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/da/DalajClassification.py
--rw-r--r--   0 root         (0) root         (0)     1610 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/da/DanishPoliticalCommentsClassification.py
--rw-r--r--   0 root         (0) root         (0)     2937 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/da/DdiscoCohesionClassification.py
--rw-r--r--   0 root         (0) root         (0)     1255 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/da/LccSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/da/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.080882 mteb-1.5.2/mteb/tasks/Classification/en/
--rw-r--r--   0 root         (0) root         (0)     1035 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/en/AmazonPolarityClassification.py
--rw-r--r--   0 root         (0) root         (0)     1048 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/en/Banking77Classification.py
--rw-r--r--   0 root         (0) root         (0)     1368 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/en/EmotionClassification.py
--rw-r--r--   0 root         (0) root         (0)      984 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/en/ImdbClassification.py
--rw-r--r--   0 root         (0) root         (0)     1400 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/en/ToxicConversationsClassification.py
--rw-r--r--   0 root         (0) root         (0)     1275 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/en/TweetSentimentExtractionClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/en/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.080882 mteb-1.5.2/mteb/tasks/Classification/multilingual/
--rw-r--r--   0 root         (0) root         (0)     1485 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/multilingual/AmazonCounterfactualClassification.py
--rw-r--r--   0 root         (0) root         (0)     1235 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/multilingual/AmazonReviewsClassification.py
--rw-r--r--   0 root         (0) root         (0)     1164 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/multilingual/MTOPDomainClassification.py
--rw-r--r--   0 root         (0) root         (0)     1164 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/multilingual/MTOPIntentClassification.py
--rw-r--r--   0 root         (0) root         (0)     1403 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/multilingual/MasakhaNEWSClassification.py
--rw-r--r--   0 root         (0) root         (0)     1823 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/multilingual/MassiveIntentClassification.py
--rw-r--r--   0 root         (0) root         (0)     1829 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/multilingual/MassiveScenarioClassification.py
--rw-r--r--   0 root         (0) root         (0)     1468 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/multilingual/NordicLangClassification.py
--rw-r--r--   0 root         (0) root         (0)     6075 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/multilingual/ScalaClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.080882 mteb-1.5.2/mteb/tasks/Classification/nb/
--rw-r--r--   0 root         (0) root         (0)     1115 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/nb/NoRecClassification.py
--rw-r--r--   0 root         (0) root         (0)     1160 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/nb/NorwegianParliamentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/nb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.080882 mteb-1.5.2/mteb/tasks/Classification/pl/
--rw-r--r--   0 root         (0) root         (0)     4892 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/pl/PolishClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/pl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.080882 mteb-1.5.2/mteb/tasks/Classification/sv/
--rw-r--r--   0 root         (0) root         (0)     1037 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/sv/SweRecClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/sv/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.080882 mteb-1.5.2/mteb/tasks/Classification/zh/
--rw-r--r--   0 root         (0) root         (0)     6535 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/zh/CMTEBClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Classification/zh/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.084882 mteb-1.5.2/mteb/tasks/Clustering/
--rw-r--r--   0 root         (0) root         (0)     1249 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.084882 mteb-1.5.2/mteb/tasks/Clustering/de/
--rw-r--r--   0 root         (0) root         (0)     1126 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/de/BlurbsClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1118 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/de/BlurbsClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1094 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/de/TenKGnadClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1074 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/de/TenKGnadClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/de/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.084882 mteb-1.5.2/mteb/tasks/Clustering/en/
--rw-r--r--   0 root         (0) root         (0)     1095 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/en/ArxivClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1081 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/en/ArxivClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1122 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/en/BigPatentClustering.py
--rw-r--r--   0 root         (0) root         (0)     1065 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/en/BiorxivClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1055 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/en/BiorxivClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1066 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/en/MedrxivClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1056 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/en/MedrxivClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1096 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/en/RedditClustering.py
--rw-r--r--   0 root         (0) root         (0)     1085 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/en/RedditClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1121 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/en/StackExchangeClustering.py
--rw-r--r--   0 root         (0) root         (0)     1109 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/en/StackExchangeClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1078 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/en/TwentyNewsgroupsClustering.py
--rw-r--r--   0 root         (0) root         (0)     1129 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/en/WikiCitiesClustering.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/en/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.088882 mteb-1.5.2/mteb/tasks/Clustering/es/
--rw-r--r--   0 root         (0) root         (0)     1027 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/es/FloresClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1054 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/es/SpanishNewsClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/es/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.088882 mteb-1.5.2/mteb/tasks/Clustering/fr/
--rw-r--r--   0 root         (0) root         (0)     1905 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/fr/AlloProfClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1751 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/fr/AlloProfClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1619 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/fr/HALClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1926 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/fr/MLSUMClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1741 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/fr/MLSUMClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/fr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.088882 mteb-1.5.2/mteb/tasks/Clustering/multilingual/
--rw-r--r--   0 root         (0) root         (0)     2499 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     2513 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.088882 mteb-1.5.2/mteb/tasks/Clustering/nb/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/nb/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3436 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/nb/snl_clustering.py
--rw-r--r--   0 root         (0) root         (0)     3590 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/nb/vg_clustering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.088882 mteb-1.5.2/mteb/tasks/Clustering/pl/
--rw-r--r--   0 root         (0) root         (0)     1131 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/pl/PolishClustering.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/pl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.088882 mteb-1.5.2/mteb/tasks/Clustering/sv/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/sv/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3920 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/sv/swedn_clustering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.088882 mteb-1.5.2/mteb/tasks/Clustering/zh/
--rw-r--r--   0 root         (0) root         (0)     3615 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/zh/CMTEBClustering.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Clustering/zh/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.088882 mteb-1.5.2/mteb/tasks/PairClassification/
--rw-r--r--   0 root         (0) root         (0)      301 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/PairClassification/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.092882 mteb-1.5.2/mteb/tasks/PairClassification/en/
--rw-r--r--   0 root         (0) root         (0)     1146 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/PairClassification/en/SprintDuplicateQuestionsPC.py
--rw-r--r--   0 root         (0) root         (0)     1080 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/PairClassification/en/TwitterSemEval2015PC.py
--rw-r--r--   0 root         (0) root         (0)     1034 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/PairClassification/en/TwitterURLCorpusPC.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/PairClassification/en/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.092882 mteb-1.5.2/mteb/tasks/PairClassification/multilingual/
--rw-r--r--   0 root         (0) root         (0)     2687 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/PairClassification/multilingual/OpusparcusPC.py
--rw-r--r--   0 root         (0) root         (0)     1902 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/PairClassification/multilingual/PawsX.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/PairClassification/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.092882 mteb-1.5.2/mteb/tasks/PairClassification/pl/
--rw-r--r--   0 root         (0) root         (0)     3553 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/PairClassification/pl/PolishPC.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/PairClassification/pl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.092882 mteb-1.5.2/mteb/tasks/PairClassification/zh/
--rw-r--r--   0 root         (0) root         (0)     1837 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/PairClassification/zh/CMTEBPairClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/PairClassification/zh/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.092882 mteb-1.5.2/mteb/tasks/Reranking/
--rw-r--r--   0 root         (0) root         (0)      339 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Reranking/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.092882 mteb-1.5.2/mteb/tasks/Reranking/en/
--rw-r--r--   0 root         (0) root         (0)     1112 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Reranking/en/AskUbuntuDupQuestions.py
--rw-r--r--   0 root         (0) root         (0)     1097 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Reranking/en/MindSmallReranking.py
--rw-r--r--   0 root         (0) root         (0)     3010 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Reranking/en/SciDocsReranking.py
--rw-r--r--   0 root         (0) root         (0)     1131 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Reranking/en/StackOverflowDupQuestions.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Reranking/en/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.092882 mteb-1.5.2/mteb/tasks/Reranking/fr/
--rw-r--r--   0 root         (0) root         (0)     1189 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Reranking/fr/AlloprofReranking.py
--rw-r--r--   0 root         (0) root         (0)     1059 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Reranking/fr/SyntecReranking.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Reranking/fr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.096882 mteb-1.5.2/mteb/tasks/Reranking/multilingual/
--rw-r--r--   0 root         (0) root         (0)     1206 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Reranking/multilingual/MIRACLReranking.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Reranking/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.096882 mteb-1.5.2/mteb/tasks/Reranking/zh/
--rw-r--r--   0 root         (0) root         (0)     3504 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Reranking/zh/CMTEBReranking.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Reranking/zh/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.096882 mteb-1.5.2/mteb/tasks/Retrieval/
--rw-r--r--   0 root         (0) root         (0)     2462 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.096882 mteb-1.5.2/mteb/tasks/Retrieval/da/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/da/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3788 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/da/dan_fever.py
--rw-r--r--   0 root         (0) root         (0)     2577 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/da/t2nord_retrieval.py
--rw-r--r--   0 root         (0) root         (0)     3142 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/da/twitterhjerne.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.096882 mteb-1.5.2/mteb/tasks/Retrieval/de/
--rw-r--r--   0 root         (0) root         (0)     1997 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/de/GerDaLIRRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2896 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/de/GermanDPRRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2121 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/de/GermanQuADRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/de/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.100882 mteb-1.5.2/mteb/tasks/Retrieval/en/
--rw-r--r--   0 root         (0) root         (0)     1005 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/en/ArguAnaRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1059 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/en/CQADupstackAndroidRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1059 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/en/CQADupstackEnglishRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1056 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/en/CQADupstackGamingRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1047 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/en/CQADupstackGisRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1071 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/en/CQADupstackMathematicaRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1059 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/en/CQADupstackPhysicsRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1071 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/en/CQADupstackProgrammersRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1053 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/en/CQADupstackStatsRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1047 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/en/CQADupstackTexRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1050 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/en/CQADupstackUnixRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1068 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/en/CQADupstackWebmastersRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1065 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/en/CQADupstackWordpressRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1089 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/en/ClimateFEVERRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1025 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/en/DBPediaRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1169 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/en/FEVERRetrieval.py
--rw-r--r--   0 root         (0) root         (0)      977 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/en/FiQA2018Retrieval.py
--rw-r--r--   0 root         (0) root         (0)     3699 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/en/HagridRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1145 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/en/HotpotQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1003 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/en/MSMARCORetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1033 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/en/MSMARCOv2Retrieval.py
--rw-r--r--   0 root         (0) root         (0)     1018 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/en/NFCorpusRetrieval.py
--rw-r--r--   0 root         (0) root         (0)      993 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/en/NQRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2032 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/en/NarrativeQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1149 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/en/QuoraRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1108 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/en/SCIDOCSRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1040 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/en/SciFactRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1063 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/en/TRECCOVIDRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1003 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/en/Touche2020Retrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/en/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.104882 mteb-1.5.2/mteb/tasks/Retrieval/es/
--rw-r--r--   0 root         (0) root         (0)     2117 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/es/SpanishPassageRetrievalS2P.py
--rw-r--r--   0 root         (0) root         (0)     2119 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/es/SpanishPassageRetrievalS2S.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/es/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.104882 mteb-1.5.2/mteb/tasks/Retrieval/fr/
--rw-r--r--   0 root         (0) root         (0)     2182 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/fr/AlloprofRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2469 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/fr/BSARDRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2164 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/fr/SyntecRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/fr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.104882 mteb-1.5.2/mteb/tasks/Retrieval/ko/
--rw-r--r--   0 root         (0) root         (0)      900 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/ko/KoMiracl.py
--rw-r--r--   0 root         (0) root         (0)      900 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/ko/KoMrtydi.py
--rw-r--r--   0 root         (0) root         (0)      916 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/ko/KoStrategyQA.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/ko/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.104882 mteb-1.5.2/mteb/tasks/Retrieval/multilingual/
--rw-r--r--   0 root         (0) root         (0)     3248 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/multilingual/MIRACLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2905 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/multilingual/MintakaRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     3250 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/multilingual/MultiLongDocRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2921 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/multilingual/XMarketRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2925 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/multilingual/XPQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.104882 mteb-1.5.2/mteb/tasks/Retrieval/nb/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/nb/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3946 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/nb/norquad.py
--rw-r--r--   0 root         (0) root         (0)     2702 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/nb/snl_retrieval.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.108882 mteb-1.5.2/mteb/tasks/Retrieval/pl/
--rw-r--r--   0 root         (0) root         (0)      961 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/pl/ArguAnaPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1034 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/pl/DBPediaPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)      978 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/pl/FiQAPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1106 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/pl/HotpotQAPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1003 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/pl/MSMARCOPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1034 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/pl/NFCorpusPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)      991 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/pl/NQPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1157 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/pl/QuoraPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1085 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/pl/SCIDOCSPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1047 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/pl/SciFactPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1079 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/pl/TRECCOVIDPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/pl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.108882 mteb-1.5.2/mteb/tasks/Retrieval/sv/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/sv/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3213 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/sv/swedn_retrieval.py
--rw-r--r--   0 root         (0) root         (0)     2613 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/sv/swefaq_retrieval.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.108882 mteb-1.5.2/mteb/tasks/Retrieval/zh/
--rw-r--r--   0 root         (0) root         (0)    10336 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/zh/CMTEBRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Retrieval/zh/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.108882 mteb-1.5.2/mteb/tasks/STS/
--rw-r--r--   0 root         (0) root         (0)      562 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/STS/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.108882 mteb-1.5.2/mteb/tasks/STS/de/
--rw-r--r--   0 root         (0) root         (0)     1364 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/STS/de/GermanSTSBenchmarkSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/STS/de/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.112882 mteb-1.5.2/mteb/tasks/STS/en/
--rw-r--r--   0 root         (0) root         (0)     1178 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/STS/en/BiossesSTS.py
--rw-r--r--   0 root         (0) root         (0)     1147 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/STS/en/STS12STS.py
--rw-r--r--   0 root         (0) root         (0)     1144 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/STS/en/STS13STS.py
--rw-r--r--   0 root         (0) root         (0)     1178 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/STS/en/STS14STS.py
--rw-r--r--   0 root         (0) root         (0)     1142 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/STS/en/STS15STS.py
--rw-r--r--   0 root         (0) root         (0)     1142 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/STS/en/STS16STS.py
--rw-r--r--   0 root         (0) root         (0)     1202 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/STS/en/STSBenchmarkSTS.py
--rw-r--r--   0 root         (0) root         (0)     1179 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/STS/en/SickrSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/STS/en/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.112882 mteb-1.5.2/mteb/tasks/STS/es/
--rw-r--r--   0 root         (0) root         (0)     1480 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/STS/es/STSES.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/STS/es/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.112882 mteb-1.5.2/mteb/tasks/STS/fr/
--rw-r--r--   0 root         (0) root         (0)     1466 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/STS/fr/SickFrSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/STS/fr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.112882 mteb-1.5.2/mteb/tasks/STS/multilingual/
--rw-r--r--   0 root         (0) root         (0)     1362 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/STS/multilingual/STS17CrosslingualSTS.py
--rw-r--r--   0 root         (0) root         (0)     1484 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/STS/multilingual/STS22CrosslingualSTS.py
--rw-r--r--   0 root         (0) root         (0)     2528 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/STS/multilingual/STSBenchmarkMultilingualSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/STS/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.112882 mteb-1.5.2/mteb/tasks/STS/pl/
--rw-r--r--   0 root         (0) root         (0)     2256 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/STS/pl/PolishSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/STS/pl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.112882 mteb-1.5.2/mteb/tasks/STS/zh/
--rw-r--r--   0 root         (0) root         (0)     7080 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/STS/zh/CMTEBSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/STS/zh/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.112882 mteb-1.5.2/mteb/tasks/Summarization/
--rw-r--r--   0 root         (0) root         (0)      122 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Summarization/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.116882 mteb-1.5.2/mteb/tasks/Summarization/en/
--rw-r--r--   0 root         (0) root         (0)     1237 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Summarization/en/SummEvalSummarization.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Summarization/en/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.116882 mteb-1.5.2/mteb/tasks/Summarization/fr/
--rw-r--r--   0 root         (0) root         (0)     1298 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Summarization/fr/SummEvalFrSummarization.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/Summarization/fr/__init__.py
--rw-r--r--   0 root         (0) root         (0)      252 2024-04-04 12:49:25.000000 mteb-1.5.2/mteb/tasks/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.120882 mteb-1.5.2/mteb.egg-info/
--rw-r--r--   0 root         (0) root         (0)    23581 2024-04-04 12:49:30.000000 mteb-1.5.2/mteb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12579 2024-04-04 12:49:30.000000 mteb-1.5.2/mteb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 12:49:30.000000 mteb-1.5.2/mteb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2024-04-04 12:49:30.000000 mteb-1.5.2/mteb.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      234 2024-04-04 12:49:30.000000 mteb-1.5.2/mteb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2024-04-04 12:49:30.000000 mteb-1.5.2/mteb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2120 2024-04-04 12:49:26.000000 mteb-1.5.2/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.116882 mteb-1.5.2/scripts/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.116882 mteb-1.5.2/scripts/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.116882 mteb-1.5.2/scripts/data/amazon_polarity/
--rw-r--r--   0 root         (0) root         (0)      842 2024-04-04 12:49:25.000000 mteb-1.5.2/scripts/data/amazon_polarity/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.116882 mteb-1.5.2/scripts/data/amazon_reviews_multi/
--rw-r--r--   0 root         (0) root         (0)     1379 2024-04-04 12:49:25.000000 mteb-1.5.2/scripts/data/amazon_reviews_multi/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.116882 mteb-1.5.2/scripts/data/arxiv/
--rw-r--r--   0 root         (0) root         (0)     3146 2024-04-04 12:49:25.000000 mteb-1.5.2/scripts/data/arxiv/script_clustering.py
--rw-r--r--   0 root         (0) root         (0)     1451 2024-04-04 12:49:25.000000 mteb-1.5.2/scripts/data/arxiv/script_raw.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.116882 mteb-1.5.2/scripts/data/biorxiv/
--rw-r--r--   0 root         (0) root         (0)     1781 2024-04-04 12:49:25.000000 mteb-1.5.2/scripts/data/biorxiv/script_clustering.py
--rw-r--r--   0 root         (0) root         (0)     1674 2024-04-04 12:49:25.000000 mteb-1.5.2/scripts/data/biorxiv/script_raw.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.116882 mteb-1.5.2/scripts/data/bucc/
--rw-r--r--   0 root         (0) root         (0)     1171 2024-04-04 12:49:25.000000 mteb-1.5.2/scripts/data/bucc/create_data.py
--rw-r--r--   0 root         (0) root         (0)     5929 2024-04-04 12:49:25.000000 mteb-1.5.2/scripts/data/create_task_table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.116882 mteb-1.5.2/scripts/data/germanquad/
--rw-r--r--   0 root         (0) root         (0)     2132 2024-04-04 12:49:25.000000 mteb-1.5.2/scripts/data/germanquad/process_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.116882 mteb-1.5.2/scripts/data/hal/
--rw-r--r--   0 root         (0) root         (0)     1512 2024-04-04 12:49:25.000000 mteb-1.5.2/scripts/data/hal/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.116882 mteb-1.5.2/scripts/data/imdb/
--rw-r--r--   0 root         (0) root         (0)      682 2024-04-04 12:49:25.000000 mteb-1.5.2/scripts/data/imdb/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.120882 mteb-1.5.2/scripts/data/medrxiv/
--rw-r--r--   0 root         (0) root         (0)     1780 2024-04-04 12:49:25.000000 mteb-1.5.2/scripts/data/medrxiv/script_clustering.py
--rw-r--r--   0 root         (0) root         (0)     1617 2024-04-04 12:49:25.000000 mteb-1.5.2/scripts/data/medrxiv/script_raw.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.120882 mteb-1.5.2/scripts/data/mind/
--rw-r--r--   0 root         (0) root         (0)     1377 2024-04-04 12:49:25.000000 mteb-1.5.2/scripts/data/mind/prepare_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.120882 mteb-1.5.2/scripts/data/redditp2p/
--rw-r--r--   0 root         (0) root         (0)     1880 2024-04-04 12:49:25.000000 mteb-1.5.2/scripts/data/redditp2p/script_clustering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.120882 mteb-1.5.2/scripts/data/stackexchangep2p/
--rw-r--r--   0 root         (0) root         (0)     1627 2024-04-04 12:49:25.000000 mteb-1.5.2/scripts/data/stackexchangep2p/script_clustering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.120882 mteb-1.5.2/scripts/data/sts22-crosslingual-sts/
--rw-r--r--   0 root         (0) root         (0)     2436 2024-04-04 12:49:25.000000 mteb-1.5.2/scripts/data/sts22-crosslingual-sts/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.120882 mteb-1.5.2/scripts/data/summeval_fr/
--rw-r--r--   0 root         (0) root         (0)     1692 2024-04-04 12:49:25.000000 mteb-1.5.2/scripts/data/summeval_fr/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.120882 mteb-1.5.2/scripts/data/toxic_conversations_50k/
--rw-r--r--   0 root         (0) root         (0)     1151 2024-04-04 12:49:25.000000 mteb-1.5.2/scripts/data/toxic_conversations_50k/create_data.py
--rw-r--r--   0 root         (0) root         (0)     2516 2024-04-04 12:49:25.000000 mteb-1.5.2/scripts/merge_cqadupstack.py
--rw-r--r--   0 root         (0) root         (0)     5217 2024-04-04 12:49:25.000000 mteb-1.5.2/scripts/mteb_meta.py
--rw-r--r--   0 root         (0) root         (0)      673 2024-04-04 12:49:25.000000 mteb-1.5.2/scripts/run_mteb_chinese.py
--rw-r--r--   0 root         (0) root         (0)     2819 2024-04-04 12:49:25.000000 mteb-1.5.2/scripts/run_mteb_english.py
--rw-r--r--   0 root         (0) root         (0)     1852 2024-04-04 12:49:25.000000 mteb-1.5.2/scripts/run_mteb_french.py
--rw-r--r--   0 root         (0) root         (0)     1305 2024-04-04 12:49:25.000000 mteb-1.5.2/scripts/run_mteb_german.py
--rw-r--r--   0 root         (0) root         (0)     1033 2024-04-04 12:49:25.000000 mteb-1.5.2/scripts/run_mteb_korean.py
--rw-r--r--   0 root         (0) root         (0)      975 2024-04-04 12:49:25.000000 mteb-1.5.2/scripts/run_mteb_polish.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-04 12:49:30.124882 mteb-1.5.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 12:49:30.120882 mteb-1.5.2/tests/
--rw-r--r--   0 root         (0) root         (0)      632 2024-04-04 12:49:25.000000 mteb-1.5.2/tests/test_ClusteringEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     1560 2024-04-04 12:49:25.000000 mteb-1.5.2/tests/test_PairClassificationEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     1130 2024-04-04 12:49:25.000000 mteb-1.5.2/tests/test_RerankingEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     1113 2024-04-04 12:49:25.000000 mteb-1.5.2/tests/test_RetrievalEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     3471 2024-04-04 12:49:25.000000 mteb-1.5.2/tests/test_TaskMetadata.py
--rw-r--r--   0 root         (0) root         (0)     3524 2024-04-04 12:49:25.000000 mteb-1.5.2/tests/test_all_abstasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.589388 mteb-1.5.3/
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-04-08 07:41:26.000000 mteb-1.5.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    23581 2024-04-08 07:41:30.589388 mteb-1.5.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9190 2024-04-08 07:41:26.000000 mteb-1.5.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.529388 mteb-1.5.3/mteb/
+-rw-r--r--   0 root         (0) root         (0)     2135 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.533388 mteb-1.5.3/mteb/abstasks/
+-rw-r--r--   0 root         (0) root         (0)     1751 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/abstasks/AbsTask.py
+-rw-r--r--   0 root         (0) root         (0)     3063 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/abstasks/AbsTaskBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     5881 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/abstasks/AbsTaskClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2389 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/abstasks/AbsTaskClustering.py
+-rw-r--r--   0 root         (0) root         (0)     2542 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/abstasks/AbsTaskPairClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1120 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/abstasks/AbsTaskReranking.py
+-rw-r--r--   0 root         (0) root         (0)    11806 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/abstasks/AbsTaskRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2007 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/abstasks/AbsTaskSTS.py
+-rw-r--r--   0 root         (0) root         (0)     2296 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/abstasks/AbsTaskSummarization.py
+-rw-r--r--   0 root         (0) root         (0)      880 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/abstasks/CrosslingualTask.py
+-rw-r--r--   0 root         (0) root         (0)     2831 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/abstasks/LangMapping.py
+-rw-r--r--   0 root         (0) root         (0)      998 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/abstasks/MultilingualTask.py
+-rw-r--r--   0 root         (0) root         (0)     6458 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/abstasks/TaskMetadata.py
+-rw-r--r--   0 root         (0) root         (0)      422 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/abstasks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5296 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/cmd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.533388 mteb-1.5.3/mteb/evaluation/
+-rw-r--r--   0 root         (0) root         (0)    13124 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/evaluation/MTEB.py
+-rw-r--r--   0 root         (0) root         (0)       56 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/evaluation/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.533388 mteb-1.5.3/mteb/evaluation/evaluators/
+-rw-r--r--   0 root         (0) root         (0)     5849 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/evaluation/evaluators/BitextMiningEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     8942 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/evaluation/evaluators/ClassificationEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     1463 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/evaluation/evaluators/ClusteringEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)      744 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/evaluation/evaluators/Evaluator.py
+-rw-r--r--   0 root         (0) root         (0)     7140 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/evaluation/evaluators/PairClassificationEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     9613 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/evaluation/evaluators/RerankingEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)    12487 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/evaluation/evaluators/RetrievalEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     2394 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/evaluation/evaluators/STSEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     4841 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/evaluation/evaluators/SummarizationEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)      324 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/evaluation/evaluators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5482 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/evaluation/evaluators/utils.py
+-rw-r--r--   0 root         (0) root         (0)      835 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/logging.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.533388 mteb-1.5.3/mteb/tasks/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.533388 mteb-1.5.3/mteb/tasks/BitextMining/
+-rw-r--r--   0 root         (0) root         (0)      369 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/BitextMining/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.537388 mteb-1.5.3/mteb/tasks/BitextMining/da/
+-rw-r--r--   0 root         (0) root         (0)     1398 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/BitextMining/da/BornholmskBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/BitextMining/da/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.537388 mteb-1.5.3/mteb/tasks/BitextMining/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     1076 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/BitextMining/multilingual/BUCCBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     2194 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/BitextMining/multilingual/DiaBLaBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     5780 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/BitextMining/multilingual/FloresBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     1411 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/BitextMining/multilingual/NorwegianCourtsBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     2797 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/BitextMining/multilingual/TatoebaBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/BitextMining/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.537388 mteb-1.5.3/mteb/tasks/BitextMining/nb/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/BitextMining/nb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1351 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/BitextMining/nb/norwegian_courts_bitext_mining.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.537388 mteb-1.5.3/mteb/tasks/Classification/
+-rw-r--r--   0 root         (0) root         (0)     1269 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.537388 mteb-1.5.3/mteb/tasks/Classification/da/
+-rw-r--r--   0 root         (0) root         (0)     1316 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/da/AngryTweetsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1615 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/da/DKHateClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2505 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/da/DalajClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1610 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/da/DanishPoliticalCommentsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2937 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/da/DdiscoCohesionClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1255 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/da/LccSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/da/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.541388 mteb-1.5.3/mteb/tasks/Classification/en/
+-rw-r--r--   0 root         (0) root         (0)     1035 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/en/AmazonPolarityClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1048 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/en/Banking77Classification.py
+-rw-r--r--   0 root         (0) root         (0)     1368 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/en/EmotionClassification.py
+-rw-r--r--   0 root         (0) root         (0)      984 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/en/ImdbClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1063 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/en/NewsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1400 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/en/ToxicConversationsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1275 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/en/TweetSentimentExtractionClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/en/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.541388 mteb-1.5.3/mteb/tasks/Classification/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     1485 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/multilingual/AmazonCounterfactualClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1235 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/multilingual/AmazonReviewsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1164 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/multilingual/MTOPDomainClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1164 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/multilingual/MTOPIntentClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1403 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/multilingual/MasakhaNEWSClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1823 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/multilingual/MassiveIntentClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1829 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/multilingual/MassiveScenarioClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1468 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/multilingual/NordicLangClassification.py
+-rw-r--r--   0 root         (0) root         (0)     6075 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/multilingual/ScalaClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.541388 mteb-1.5.3/mteb/tasks/Classification/nb/
+-rw-r--r--   0 root         (0) root         (0)     1115 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/nb/NoRecClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1160 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/nb/NorwegianParliamentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/nb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.545388 mteb-1.5.3/mteb/tasks/Classification/pl/
+-rw-r--r--   0 root         (0) root         (0)     4892 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/pl/PolishClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/pl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.545388 mteb-1.5.3/mteb/tasks/Classification/sv/
+-rw-r--r--   0 root         (0) root         (0)     1037 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/sv/SweRecClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/sv/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.545388 mteb-1.5.3/mteb/tasks/Classification/zh/
+-rw-r--r--   0 root         (0) root         (0)     6535 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/zh/CMTEBClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Classification/zh/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.545388 mteb-1.5.3/mteb/tasks/Clustering/
+-rw-r--r--   0 root         (0) root         (0)     1249 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.545388 mteb-1.5.3/mteb/tasks/Clustering/de/
+-rw-r--r--   0 root         (0) root         (0)     1126 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/de/BlurbsClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1118 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/de/BlurbsClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1094 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/de/TenKGnadClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1074 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/de/TenKGnadClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/de/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.549388 mteb-1.5.3/mteb/tasks/Clustering/en/
+-rw-r--r--   0 root         (0) root         (0)     1095 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/en/ArxivClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1081 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/en/ArxivClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1122 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/en/BigPatentClustering.py
+-rw-r--r--   0 root         (0) root         (0)     1065 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/en/BiorxivClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1055 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/en/BiorxivClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1066 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/en/MedrxivClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1056 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/en/MedrxivClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1096 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/en/RedditClustering.py
+-rw-r--r--   0 root         (0) root         (0)     1085 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/en/RedditClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1121 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/en/StackExchangeClustering.py
+-rw-r--r--   0 root         (0) root         (0)     1109 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/en/StackExchangeClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1078 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/en/TwentyNewsgroupsClustering.py
+-rw-r--r--   0 root         (0) root         (0)     1129 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/en/WikiCitiesClustering.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/en/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.549388 mteb-1.5.3/mteb/tasks/Clustering/es/
+-rw-r--r--   0 root         (0) root         (0)     1027 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/es/FloresClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1054 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/es/SpanishNewsClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/es/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.549388 mteb-1.5.3/mteb/tasks/Clustering/fr/
+-rw-r--r--   0 root         (0) root         (0)     1905 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/fr/AlloProfClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1751 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/fr/AlloProfClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1619 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/fr/HALClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1926 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/fr/MLSUMClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1741 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/fr/MLSUMClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/fr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.553388 mteb-1.5.3/mteb/tasks/Clustering/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     2499 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     2513 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.553388 mteb-1.5.3/mteb/tasks/Clustering/nb/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/nb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3436 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/nb/snl_clustering.py
+-rw-r--r--   0 root         (0) root         (0)     3590 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/nb/vg_clustering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.553388 mteb-1.5.3/mteb/tasks/Clustering/pl/
+-rw-r--r--   0 root         (0) root         (0)     1131 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/pl/PolishClustering.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/pl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.553388 mteb-1.5.3/mteb/tasks/Clustering/sv/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/sv/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3920 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/sv/swedn_clustering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.553388 mteb-1.5.3/mteb/tasks/Clustering/zh/
+-rw-r--r--   0 root         (0) root         (0)     3615 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/zh/CMTEBClustering.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Clustering/zh/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.553388 mteb-1.5.3/mteb/tasks/PairClassification/
+-rw-r--r--   0 root         (0) root         (0)      301 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/PairClassification/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.553388 mteb-1.5.3/mteb/tasks/PairClassification/en/
+-rw-r--r--   0 root         (0) root         (0)     1146 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/PairClassification/en/SprintDuplicateQuestionsPC.py
+-rw-r--r--   0 root         (0) root         (0)     1080 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/PairClassification/en/TwitterSemEval2015PC.py
+-rw-r--r--   0 root         (0) root         (0)     1034 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/PairClassification/en/TwitterURLCorpusPC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/PairClassification/en/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.553388 mteb-1.5.3/mteb/tasks/PairClassification/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     2687 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/PairClassification/multilingual/OpusparcusPC.py
+-rw-r--r--   0 root         (0) root         (0)     1892 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/PairClassification/multilingual/PawsX.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/PairClassification/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.557388 mteb-1.5.3/mteb/tasks/PairClassification/pl/
+-rw-r--r--   0 root         (0) root         (0)     3553 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/PairClassification/pl/PolishPC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/PairClassification/pl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.557388 mteb-1.5.3/mteb/tasks/PairClassification/zh/
+-rw-r--r--   0 root         (0) root         (0)     1837 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/PairClassification/zh/CMTEBPairClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/PairClassification/zh/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.557388 mteb-1.5.3/mteb/tasks/Reranking/
+-rw-r--r--   0 root         (0) root         (0)      339 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Reranking/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.557388 mteb-1.5.3/mteb/tasks/Reranking/en/
+-rw-r--r--   0 root         (0) root         (0)     1112 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Reranking/en/AskUbuntuDupQuestions.py
+-rw-r--r--   0 root         (0) root         (0)     1097 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Reranking/en/MindSmallReranking.py
+-rw-r--r--   0 root         (0) root         (0)     3010 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Reranking/en/SciDocsReranking.py
+-rw-r--r--   0 root         (0) root         (0)     1131 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Reranking/en/StackOverflowDupQuestions.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Reranking/en/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.557388 mteb-1.5.3/mteb/tasks/Reranking/fr/
+-rw-r--r--   0 root         (0) root         (0)     1189 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Reranking/fr/AlloprofReranking.py
+-rw-r--r--   0 root         (0) root         (0)     1059 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Reranking/fr/SyntecReranking.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Reranking/fr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.557388 mteb-1.5.3/mteb/tasks/Reranking/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     1206 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Reranking/multilingual/MIRACLReranking.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Reranking/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.557388 mteb-1.5.3/mteb/tasks/Reranking/zh/
+-rw-r--r--   0 root         (0) root         (0)     3504 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Reranking/zh/CMTEBReranking.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Reranking/zh/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.557388 mteb-1.5.3/mteb/tasks/Retrieval/
+-rw-r--r--   0 root         (0) root         (0)     2813 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.561388 mteb-1.5.3/mteb/tasks/Retrieval/da/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/da/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3788 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/da/dan_fever.py
+-rw-r--r--   0 root         (0) root         (0)     2577 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/da/t2nord_retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3142 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/da/twitterhjerne.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.561388 mteb-1.5.3/mteb/tasks/Retrieval/de/
+-rw-r--r--   0 root         (0) root         (0)     1997 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/de/GerDaLIRRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1223 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/de/GerDaLIRSmallRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2896 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/de/GermanDPRRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2121 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/de/GermanQuADRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1047 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/de/LegalQuADRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/de/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.569388 mteb-1.5.3/mteb/tasks/Retrieval/en/
+-rw-r--r--   0 root         (0) root         (0)     1113 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/AILACasedocsRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1081 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/AILAStatutesRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1005 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/ArguAnaRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1059 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/CQADupstackAndroidRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1059 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/CQADupstackEnglishRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1056 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/CQADupstackGamingRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1047 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/CQADupstackGisRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1071 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/CQADupstackMathematicaRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1059 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/CQADupstackPhysicsRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1071 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/CQADupstackProgrammersRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1053 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/CQADupstackStatsRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1047 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/CQADupstackTexRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1050 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/CQADupstackUnixRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1068 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/CQADupstackWebmastersRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1065 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/CQADupstackWordpressRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1089 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/ClimateFEVERRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1025 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/DBPediaRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1169 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/FEVERRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)      977 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/FiQA2018Retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3699 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/HagridRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1145 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/HotpotQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1141 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/LegalBenchConsumerContractsQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1145 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/LegalBenchCorporateLobbyingRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1142 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/LegalSummarizationRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1003 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/MSMARCORetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/MSMARCOv2Retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1018 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/NFCorpusRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)      993 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/NQRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2032 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/NarrativeQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1149 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/QuoraRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1108 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/SCIDOCSRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/SciFactRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1063 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/TRECCOVIDRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1003 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/Touche2020Retrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/en/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.569388 mteb-1.5.3/mteb/tasks/Retrieval/es/
+-rw-r--r--   0 root         (0) root         (0)     2117 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/es/SpanishPassageRetrievalS2P.py
+-rw-r--r--   0 root         (0) root         (0)     2119 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/es/SpanishPassageRetrievalS2S.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/es/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.569388 mteb-1.5.3/mteb/tasks/Retrieval/fr/
+-rw-r--r--   0 root         (0) root         (0)     2182 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/fr/AlloprofRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2469 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/fr/BSARDRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2164 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/fr/SyntecRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/fr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.569388 mteb-1.5.3/mteb/tasks/Retrieval/ko/
+-rw-r--r--   0 root         (0) root         (0)      900 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/ko/KoMiracl.py
+-rw-r--r--   0 root         (0) root         (0)      900 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/ko/KoMrtydi.py
+-rw-r--r--   0 root         (0) root         (0)      916 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/ko/KoStrategyQA.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/ko/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.569388 mteb-1.5.3/mteb/tasks/Retrieval/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     3248 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/multilingual/MIRACLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2905 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/multilingual/MintakaRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3250 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/multilingual/MultiLongDocRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2921 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/multilingual/XMarketRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2925 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/multilingual/XPQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.573388 mteb-1.5.3/mteb/tasks/Retrieval/nb/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/nb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3946 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/nb/norquad.py
+-rw-r--r--   0 root         (0) root         (0)     2702 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/nb/snl_retrieval.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.573388 mteb-1.5.3/mteb/tasks/Retrieval/pl/
+-rw-r--r--   0 root         (0) root         (0)      961 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/pl/ArguAnaPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1034 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/pl/DBPediaPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)      978 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/pl/FiQAPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1106 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/pl/HotpotQAPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1003 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/pl/MSMARCOPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1034 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/pl/NFCorpusPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)      991 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/pl/NQPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1157 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/pl/QuoraPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1085 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/pl/SCIDOCSPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1047 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/pl/SciFactPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1079 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/pl/TRECCOVIDPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/pl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.573388 mteb-1.5.3/mteb/tasks/Retrieval/sv/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/sv/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3213 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/sv/swedn_retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2613 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/sv/swefaq_retrieval.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.573388 mteb-1.5.3/mteb/tasks/Retrieval/zh/
+-rw-r--r--   0 root         (0) root         (0)    10336 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/zh/CMTEBRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1124 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/zh/LeCaRDv2Retrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Retrieval/zh/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.573388 mteb-1.5.3/mteb/tasks/STS/
+-rw-r--r--   0 root         (0) root         (0)      562 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/STS/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.577388 mteb-1.5.3/mteb/tasks/STS/de/
+-rw-r--r--   0 root         (0) root         (0)     1364 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/STS/de/GermanSTSBenchmarkSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/STS/de/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.577388 mteb-1.5.3/mteb/tasks/STS/en/
+-rw-r--r--   0 root         (0) root         (0)     1178 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/STS/en/BiossesSTS.py
+-rw-r--r--   0 root         (0) root         (0)     1147 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/STS/en/STS12STS.py
+-rw-r--r--   0 root         (0) root         (0)     1144 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/STS/en/STS13STS.py
+-rw-r--r--   0 root         (0) root         (0)     1178 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/STS/en/STS14STS.py
+-rw-r--r--   0 root         (0) root         (0)     1142 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/STS/en/STS15STS.py
+-rw-r--r--   0 root         (0) root         (0)     1142 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/STS/en/STS16STS.py
+-rw-r--r--   0 root         (0) root         (0)     1202 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/STS/en/STSBenchmarkSTS.py
+-rw-r--r--   0 root         (0) root         (0)     1179 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/STS/en/SickrSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/STS/en/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.577388 mteb-1.5.3/mteb/tasks/STS/es/
+-rw-r--r--   0 root         (0) root         (0)     1480 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/STS/es/STSES.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/STS/es/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.577388 mteb-1.5.3/mteb/tasks/STS/fr/
+-rw-r--r--   0 root         (0) root         (0)     1466 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/STS/fr/SickFrSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/STS/fr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.577388 mteb-1.5.3/mteb/tasks/STS/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     1362 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/STS/multilingual/STS17CrosslingualSTS.py
+-rw-r--r--   0 root         (0) root         (0)     1484 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/STS/multilingual/STS22CrosslingualSTS.py
+-rw-r--r--   0 root         (0) root         (0)     2528 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/STS/multilingual/STSBenchmarkMultilingualSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/STS/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.577388 mteb-1.5.3/mteb/tasks/STS/pl/
+-rw-r--r--   0 root         (0) root         (0)     2256 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/STS/pl/PolishSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/STS/pl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.581388 mteb-1.5.3/mteb/tasks/STS/zh/
+-rw-r--r--   0 root         (0) root         (0)     7080 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/STS/zh/CMTEBSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/STS/zh/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.581388 mteb-1.5.3/mteb/tasks/Summarization/
+-rw-r--r--   0 root         (0) root         (0)      122 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Summarization/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.581388 mteb-1.5.3/mteb/tasks/Summarization/en/
+-rw-r--r--   0 root         (0) root         (0)     1237 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Summarization/en/SummEvalSummarization.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Summarization/en/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.581388 mteb-1.5.3/mteb/tasks/Summarization/fr/
+-rw-r--r--   0 root         (0) root         (0)     1298 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Summarization/fr/SummEvalFrSummarization.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/Summarization/fr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      252 2024-04-08 07:41:26.000000 mteb-1.5.3/mteb/tasks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.585388 mteb-1.5.3/mteb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    23581 2024-04-08 07:41:30.000000 mteb-1.5.3/mteb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    13078 2024-04-08 07:41:30.000000 mteb-1.5.3/mteb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 07:41:30.000000 mteb-1.5.3/mteb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2024-04-08 07:41:30.000000 mteb-1.5.3/mteb.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      234 2024-04-08 07:41:30.000000 mteb-1.5.3/mteb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-04-08 07:41:30.000000 mteb-1.5.3/mteb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2120 2024-04-08 07:41:27.000000 mteb-1.5.3/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.581388 mteb-1.5.3/scripts/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.581388 mteb-1.5.3/scripts/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.581388 mteb-1.5.3/scripts/data/amazon_polarity/
+-rw-r--r--   0 root         (0) root         (0)      842 2024-04-08 07:41:26.000000 mteb-1.5.3/scripts/data/amazon_polarity/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.581388 mteb-1.5.3/scripts/data/amazon_reviews_multi/
+-rw-r--r--   0 root         (0) root         (0)     1379 2024-04-08 07:41:26.000000 mteb-1.5.3/scripts/data/amazon_reviews_multi/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.581388 mteb-1.5.3/scripts/data/arxiv/
+-rw-r--r--   0 root         (0) root         (0)     3146 2024-04-08 07:41:26.000000 mteb-1.5.3/scripts/data/arxiv/script_clustering.py
+-rw-r--r--   0 root         (0) root         (0)     1451 2024-04-08 07:41:26.000000 mteb-1.5.3/scripts/data/arxiv/script_raw.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.585388 mteb-1.5.3/scripts/data/biorxiv/
+-rw-r--r--   0 root         (0) root         (0)     1781 2024-04-08 07:41:26.000000 mteb-1.5.3/scripts/data/biorxiv/script_clustering.py
+-rw-r--r--   0 root         (0) root         (0)     1674 2024-04-08 07:41:26.000000 mteb-1.5.3/scripts/data/biorxiv/script_raw.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.585388 mteb-1.5.3/scripts/data/bucc/
+-rw-r--r--   0 root         (0) root         (0)     1171 2024-04-08 07:41:26.000000 mteb-1.5.3/scripts/data/bucc/create_data.py
+-rw-r--r--   0 root         (0) root         (0)     5929 2024-04-08 07:41:26.000000 mteb-1.5.3/scripts/data/create_task_table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.585388 mteb-1.5.3/scripts/data/germanquad/
+-rw-r--r--   0 root         (0) root         (0)     2132 2024-04-08 07:41:26.000000 mteb-1.5.3/scripts/data/germanquad/process_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.585388 mteb-1.5.3/scripts/data/hal/
+-rw-r--r--   0 root         (0) root         (0)     1512 2024-04-08 07:41:26.000000 mteb-1.5.3/scripts/data/hal/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.585388 mteb-1.5.3/scripts/data/imdb/
+-rw-r--r--   0 root         (0) root         (0)      682 2024-04-08 07:41:26.000000 mteb-1.5.3/scripts/data/imdb/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.585388 mteb-1.5.3/scripts/data/medrxiv/
+-rw-r--r--   0 root         (0) root         (0)     1780 2024-04-08 07:41:26.000000 mteb-1.5.3/scripts/data/medrxiv/script_clustering.py
+-rw-r--r--   0 root         (0) root         (0)     1617 2024-04-08 07:41:26.000000 mteb-1.5.3/scripts/data/medrxiv/script_raw.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.585388 mteb-1.5.3/scripts/data/mind/
+-rw-r--r--   0 root         (0) root         (0)     1377 2024-04-08 07:41:26.000000 mteb-1.5.3/scripts/data/mind/prepare_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.585388 mteb-1.5.3/scripts/data/redditp2p/
+-rw-r--r--   0 root         (0) root         (0)     1880 2024-04-08 07:41:26.000000 mteb-1.5.3/scripts/data/redditp2p/script_clustering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.585388 mteb-1.5.3/scripts/data/stackexchangep2p/
+-rw-r--r--   0 root         (0) root         (0)     1627 2024-04-08 07:41:26.000000 mteb-1.5.3/scripts/data/stackexchangep2p/script_clustering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.585388 mteb-1.5.3/scripts/data/sts22-crosslingual-sts/
+-rw-r--r--   0 root         (0) root         (0)     2436 2024-04-08 07:41:26.000000 mteb-1.5.3/scripts/data/sts22-crosslingual-sts/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.585388 mteb-1.5.3/scripts/data/summeval_fr/
+-rw-r--r--   0 root         (0) root         (0)     1692 2024-04-08 07:41:26.000000 mteb-1.5.3/scripts/data/summeval_fr/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.585388 mteb-1.5.3/scripts/data/toxic_conversations_50k/
+-rw-r--r--   0 root         (0) root         (0)     1151 2024-04-08 07:41:26.000000 mteb-1.5.3/scripts/data/toxic_conversations_50k/create_data.py
+-rw-r--r--   0 root         (0) root         (0)     2516 2024-04-08 07:41:26.000000 mteb-1.5.3/scripts/merge_cqadupstack.py
+-rw-r--r--   0 root         (0) root         (0)     5217 2024-04-08 07:41:26.000000 mteb-1.5.3/scripts/mteb_meta.py
+-rw-r--r--   0 root         (0) root         (0)      673 2024-04-08 07:41:26.000000 mteb-1.5.3/scripts/run_mteb_chinese.py
+-rw-r--r--   0 root         (0) root         (0)     2819 2024-04-08 07:41:26.000000 mteb-1.5.3/scripts/run_mteb_english.py
+-rw-r--r--   0 root         (0) root         (0)     1852 2024-04-08 07:41:26.000000 mteb-1.5.3/scripts/run_mteb_french.py
+-rw-r--r--   0 root         (0) root         (0)     1305 2024-04-08 07:41:26.000000 mteb-1.5.3/scripts/run_mteb_german.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2024-04-08 07:41:26.000000 mteb-1.5.3/scripts/run_mteb_korean.py
+-rw-r--r--   0 root         (0) root         (0)      890 2024-04-08 07:41:26.000000 mteb-1.5.3/scripts/run_mteb_law.py
+-rw-r--r--   0 root         (0) root         (0)      975 2024-04-08 07:41:26.000000 mteb-1.5.3/scripts/run_mteb_polish.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-08 07:41:30.589388 mteb-1.5.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 07:41:30.585388 mteb-1.5.3/tests/
+-rw-r--r--   0 root         (0) root         (0)      632 2024-04-08 07:41:26.000000 mteb-1.5.3/tests/test_ClusteringEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     1560 2024-04-08 07:41:26.000000 mteb-1.5.3/tests/test_PairClassificationEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2024-04-08 07:41:26.000000 mteb-1.5.3/tests/test_RerankingEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     1113 2024-04-08 07:41:26.000000 mteb-1.5.3/tests/test_RetrievalEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     3471 2024-04-08 07:41:26.000000 mteb-1.5.3/tests/test_TaskMetadata.py
+-rw-r--r--   0 root         (0) root         (0)     3524 2024-04-08 07:41:26.000000 mteb-1.5.3/tests/test_all_abstasks.py
```

### Comparing `mteb-1.5.2/LICENSE` & `mteb-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/PKG-INFO` & `mteb-1.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mteb
-Version: 1.5.2
+Version: 1.5.3
 Summary: Massive Text Embedding Benchmark
 Author-email: MTEB Contributors <niklas@huggingface.co>, nouamane@huggingface.co, info@nils-reimers.de
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `mteb-1.5.2/README.md` & `mteb-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/__init__.py` & `mteb-1.5.3/mteb/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -72,7 +72,18 @@
     "Touche2020",
     "ToxicConversationsClassification",
     "TweetSentimentExtractionClassification",
     "TwentyNewsgroupsClustering",
     "TwitterSemEval2015",
     "TwitterURLCorpus",
 ]
+
+MTEB_RETRIEVAL_LAW = [
+    "LegalSummarization",
+    "LegalBenchConsumerContractsQA",
+    "LegalBenchCorporateLobbying",
+    "AILACasedocs",
+    "AILAStatutes",
+    "LeCaRDv2",
+    "LegalQuAD",
+    "GerDaLIRSmall",
+]
```

### Comparing `mteb-1.5.2/mteb/abstasks/AbsTask.py` & `mteb-1.5.3/mteb/abstasks/AbsTask.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/abstasks/AbsTaskBitextMining.py` & `mteb-1.5.3/mteb/abstasks/AbsTaskBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/abstasks/AbsTaskClassification.py` & `mteb-1.5.3/mteb/abstasks/AbsTaskClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/abstasks/AbsTaskClustering.py` & `mteb-1.5.3/mteb/abstasks/AbsTaskClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/abstasks/AbsTaskPairClassification.py` & `mteb-1.5.3/mteb/abstasks/AbsTaskPairClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/abstasks/AbsTaskReranking.py` & `mteb-1.5.3/mteb/abstasks/AbsTaskReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/abstasks/AbsTaskRetrieval.py` & `mteb-1.5.3/mteb/abstasks/AbsTaskRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/abstasks/AbsTaskSTS.py` & `mteb-1.5.3/mteb/abstasks/AbsTaskSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/abstasks/AbsTaskSummarization.py` & `mteb-1.5.3/mteb/abstasks/AbsTaskSummarization.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/abstasks/CrosslingualTask.py` & `mteb-1.5.3/mteb/abstasks/CrosslingualTask.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/abstasks/LangMapping.py` & `mteb-1.5.3/mteb/abstasks/LangMapping.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/abstasks/MultilingualTask.py` & `mteb-1.5.3/mteb/abstasks/MultilingualTask.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/abstasks/TaskMetadata.py` & `mteb-1.5.3/mteb/abstasks/TaskMetadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     "Linguistic acceptability",
     "Political classification",
     "Question answering",
     "Sentiment/Hate speech",
     "Thematic clustering",
     "Scientific Reranking",
     "Claim verification",
+    "Topic classification",
 ]
 
 TASK_DOMAIN = Literal[
     "Academic",
     "Blog",
     "Encyclopaedic",
     "Fiction",
```

### Comparing `mteb-1.5.2/mteb/cmd.py` & `mteb-1.5.3/mteb/cmd.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/evaluation/MTEB.py` & `mteb-1.5.3/mteb/evaluation/MTEB.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/evaluation/evaluators/BitextMiningEvaluator.py` & `mteb-1.5.3/mteb/evaluation/evaluators/BitextMiningEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/evaluation/evaluators/ClassificationEvaluator.py` & `mteb-1.5.3/mteb/evaluation/evaluators/ClassificationEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/evaluation/evaluators/ClusteringEvaluator.py` & `mteb-1.5.3/mteb/evaluation/evaluators/ClusteringEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/evaluation/evaluators/Evaluator.py` & `mteb-1.5.3/mteb/evaluation/evaluators/Evaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/evaluation/evaluators/PairClassificationEvaluator.py` & `mteb-1.5.3/mteb/evaluation/evaluators/PairClassificationEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/evaluation/evaluators/RerankingEvaluator.py` & `mteb-1.5.3/mteb/evaluation/evaluators/RerankingEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/evaluation/evaluators/RetrievalEvaluator.py` & `mteb-1.5.3/mteb/evaluation/evaluators/RetrievalEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/evaluation/evaluators/STSEvaluator.py` & `mteb-1.5.3/mteb/evaluation/evaluators/STSEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/evaluation/evaluators/SummarizationEvaluator.py` & `mteb-1.5.3/mteb/evaluation/evaluators/SummarizationEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/evaluation/evaluators/utils.py` & `mteb-1.5.3/mteb/evaluation/evaluators/utils.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/logging.py` & `mteb-1.5.3/mteb/logging.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/BitextMining/da/BornholmskBitextMining.py` & `mteb-1.5.3/mteb/tasks/BitextMining/da/BornholmskBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/BitextMining/multilingual/BUCCBitextMining.py` & `mteb-1.5.3/mteb/tasks/BitextMining/multilingual/BUCCBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/BitextMining/multilingual/DiaBLaBitextMining.py` & `mteb-1.5.3/mteb/tasks/BitextMining/multilingual/DiaBLaBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/BitextMining/multilingual/FloresBitextMining.py` & `mteb-1.5.3/mteb/tasks/BitextMining/multilingual/FloresBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/BitextMining/multilingual/NorwegianCourtsBitextMining.py` & `mteb-1.5.3/mteb/tasks/BitextMining/multilingual/NorwegianCourtsBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/BitextMining/multilingual/TatoebaBitextMining.py` & `mteb-1.5.3/mteb/tasks/BitextMining/multilingual/TatoebaBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/BitextMining/nb/norwegian_courts_bitext_mining.py` & `mteb-1.5.3/mteb/tasks/BitextMining/nb/norwegian_courts_bitext_mining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Classification/__init__.py` & `mteb-1.5.3/mteb/tasks/Classification/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from .da.DanishPoliticalCommentsClassification import *
 from .da.DKHateClassification import *
 from .da.LccSentimentClassification import *
 from .en.AmazonPolarityClassification import *
 from .en.Banking77Classification import *
 from .en.EmotionClassification import *
 from .en.ImdbClassification import *
+from .en.NewsClassification import *
 from .en.ToxicConversationsClassification import *
 from .en.TweetSentimentExtractionClassification import *
 from .multilingual.AmazonCounterfactualClassification import *
 from .multilingual.AmazonReviewsClassification import *
 from .multilingual.MasakhaNEWSClassification import *
 from .multilingual.MassiveIntentClassification import *
 from .multilingual.MassiveScenarioClassification import *
```

### Comparing `mteb-1.5.2/mteb/tasks/Classification/da/AngryTweetsClassification.py` & `mteb-1.5.3/mteb/tasks/Classification/da/AngryTweetsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Classification/da/DKHateClassification.py` & `mteb-1.5.3/mteb/tasks/Classification/da/DKHateClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Classification/da/DalajClassification.py` & `mteb-1.5.3/mteb/tasks/Classification/da/DalajClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Classification/da/DanishPoliticalCommentsClassification.py` & `mteb-1.5.3/mteb/tasks/Classification/da/DanishPoliticalCommentsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Classification/da/DdiscoCohesionClassification.py` & `mteb-1.5.3/mteb/tasks/Classification/da/DdiscoCohesionClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Classification/da/LccSentimentClassification.py` & `mteb-1.5.3/mteb/tasks/Classification/da/LccSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Classification/en/AmazonPolarityClassification.py` & `mteb-1.5.3/mteb/tasks/Classification/en/AmazonPolarityClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Classification/en/Banking77Classification.py` & `mteb-1.5.3/mteb/tasks/Classification/en/Banking77Classification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Classification/en/EmotionClassification.py` & `mteb-1.5.3/mteb/tasks/Classification/en/EmotionClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Classification/en/ImdbClassification.py` & `mteb-1.5.3/mteb/tasks/Classification/en/ImdbClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Classification/en/ToxicConversationsClassification.py` & `mteb-1.5.3/mteb/tasks/Classification/en/ToxicConversationsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Classification/en/TweetSentimentExtractionClassification.py` & `mteb-1.5.3/mteb/tasks/Classification/en/TweetSentimentExtractionClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Classification/multilingual/AmazonCounterfactualClassification.py` & `mteb-1.5.3/mteb/tasks/Classification/multilingual/AmazonCounterfactualClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Classification/multilingual/AmazonReviewsClassification.py` & `mteb-1.5.3/mteb/tasks/Classification/multilingual/AmazonReviewsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Classification/multilingual/MTOPDomainClassification.py` & `mteb-1.5.3/mteb/tasks/Classification/multilingual/MTOPDomainClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Classification/multilingual/MTOPIntentClassification.py` & `mteb-1.5.3/mteb/tasks/Classification/multilingual/MTOPIntentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Classification/multilingual/MasakhaNEWSClassification.py` & `mteb-1.5.3/mteb/tasks/Classification/multilingual/MasakhaNEWSClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Classification/multilingual/MassiveIntentClassification.py` & `mteb-1.5.3/mteb/tasks/Classification/multilingual/MassiveIntentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Classification/multilingual/MassiveScenarioClassification.py` & `mteb-1.5.3/mteb/tasks/Classification/multilingual/MassiveScenarioClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Classification/multilingual/NordicLangClassification.py` & `mteb-1.5.3/mteb/tasks/Classification/multilingual/NordicLangClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Classification/multilingual/ScalaClassification.py` & `mteb-1.5.3/mteb/tasks/Classification/multilingual/ScalaClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Classification/nb/NoRecClassification.py` & `mteb-1.5.3/mteb/tasks/Classification/nb/NoRecClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Classification/nb/NorwegianParliamentClassification.py` & `mteb-1.5.3/mteb/tasks/Classification/nb/NorwegianParliamentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Classification/pl/PolishClassification.py` & `mteb-1.5.3/mteb/tasks/Classification/pl/PolishClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Classification/sv/SweRecClassification.py` & `mteb-1.5.3/mteb/tasks/Classification/sv/SweRecClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Classification/zh/CMTEBClassification.py` & `mteb-1.5.3/mteb/tasks/Classification/zh/CMTEBClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Clustering/__init__.py` & `mteb-1.5.3/mteb/tasks/Clustering/__init__.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Clustering/de/BlurbsClusteringP2P.py` & `mteb-1.5.3/mteb/tasks/Clustering/de/BlurbsClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Clustering/de/BlurbsClusteringS2S.py` & `mteb-1.5.3/mteb/tasks/Clustering/de/BlurbsClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Clustering/de/TenKGnadClusteringP2P.py` & `mteb-1.5.3/mteb/tasks/Clustering/de/TenKGnadClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Clustering/de/TenKGnadClusteringS2S.py` & `mteb-1.5.3/mteb/tasks/Clustering/de/TenKGnadClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Clustering/en/ArxivClusteringP2P.py` & `mteb-1.5.3/mteb/tasks/Clustering/en/ArxivClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Clustering/en/ArxivClusteringS2S.py` & `mteb-1.5.3/mteb/tasks/Clustering/en/ArxivClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Clustering/en/BigPatentClustering.py` & `mteb-1.5.3/mteb/tasks/Clustering/en/BigPatentClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Clustering/en/BiorxivClusteringP2P.py` & `mteb-1.5.3/mteb/tasks/Clustering/en/BiorxivClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Clustering/en/BiorxivClusteringS2S.py` & `mteb-1.5.3/mteb/tasks/Clustering/en/BiorxivClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Clustering/en/MedrxivClusteringP2P.py` & `mteb-1.5.3/mteb/tasks/Clustering/en/MedrxivClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Clustering/en/MedrxivClusteringS2S.py` & `mteb-1.5.3/mteb/tasks/Clustering/en/MedrxivClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Clustering/en/RedditClustering.py` & `mteb-1.5.3/mteb/tasks/Clustering/en/RedditClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Clustering/en/RedditClusteringP2P.py` & `mteb-1.5.3/mteb/tasks/Clustering/en/RedditClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Clustering/en/StackExchangeClustering.py` & `mteb-1.5.3/mteb/tasks/Clustering/en/StackExchangeClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Clustering/en/StackExchangeClusteringP2P.py` & `mteb-1.5.3/mteb/tasks/Clustering/en/StackExchangeClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Clustering/en/TwentyNewsgroupsClustering.py` & `mteb-1.5.3/mteb/tasks/Clustering/en/TwentyNewsgroupsClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Clustering/en/WikiCitiesClustering.py` & `mteb-1.5.3/mteb/tasks/Clustering/en/WikiCitiesClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Clustering/es/FloresClusteringS2S.py` & `mteb-1.5.3/mteb/tasks/Clustering/es/FloresClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Clustering/es/SpanishNewsClusteringP2P.py` & `mteb-1.5.3/mteb/tasks/Clustering/es/SpanishNewsClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Clustering/fr/AlloProfClusteringP2P.py` & `mteb-1.5.3/mteb/tasks/Clustering/fr/AlloProfClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Clustering/fr/AlloProfClusteringS2S.py` & `mteb-1.5.3/mteb/tasks/Clustering/fr/AlloProfClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Clustering/fr/HALClusteringS2S.py` & `mteb-1.5.3/mteb/tasks/Clustering/fr/HALClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Clustering/fr/MLSUMClusteringP2P.py` & `mteb-1.5.3/mteb/tasks/Clustering/fr/MLSUMClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Clustering/fr/MLSUMClusteringS2S.py` & `mteb-1.5.3/mteb/tasks/Clustering/fr/MLSUMClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringP2P.py` & `mteb-1.5.3/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringS2S.py` & `mteb-1.5.3/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Clustering/nb/snl_clustering.py` & `mteb-1.5.3/mteb/tasks/Clustering/nb/snl_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Clustering/nb/vg_clustering.py` & `mteb-1.5.3/mteb/tasks/Clustering/nb/vg_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Clustering/pl/PolishClustering.py` & `mteb-1.5.3/mteb/tasks/Clustering/pl/PolishClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Clustering/sv/swedn_clustering.py` & `mteb-1.5.3/mteb/tasks/Clustering/sv/swedn_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Clustering/zh/CMTEBClustering.py` & `mteb-1.5.3/mteb/tasks/Clustering/zh/CMTEBClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/PairClassification/en/SprintDuplicateQuestionsPC.py` & `mteb-1.5.3/mteb/tasks/PairClassification/en/SprintDuplicateQuestionsPC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/PairClassification/en/TwitterSemEval2015PC.py` & `mteb-1.5.3/mteb/tasks/PairClassification/en/TwitterSemEval2015PC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/PairClassification/en/TwitterURLCorpusPC.py` & `mteb-1.5.3/mteb/tasks/PairClassification/en/TwitterURLCorpusPC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/PairClassification/multilingual/OpusparcusPC.py` & `mteb-1.5.3/mteb/tasks/PairClassification/multilingual/OpusparcusPC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/PairClassification/multilingual/PawsX.py` & `mteb-1.5.3/mteb/tasks/PairClassification/multilingual/PawsX.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             "path": "paws-x",
             "revision": "8a04d940a42cd40658986fdd8e3da561533a3646",
         },
         description="",
         reference="https://arxiv.org/abs/1908.11828",
         category="s2s",
         type="PairClassification",
-        eval_splits=["test.full", "validation.full"],
+        eval_splits=["test", "validation"],
         eval_langs=["de", "en", "es", "fr", "ja", "ko", "zh"],
         main_score="ap",
         date=None,
         form=None,
         domains=None,
         task_subtypes=None,
         license=None,
```

### Comparing `mteb-1.5.2/mteb/tasks/PairClassification/pl/PolishPC.py` & `mteb-1.5.3/mteb/tasks/PairClassification/pl/PolishPC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/PairClassification/zh/CMTEBPairClassification.py` & `mteb-1.5.3/mteb/tasks/PairClassification/zh/CMTEBPairClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Reranking/en/AskUbuntuDupQuestions.py` & `mteb-1.5.3/mteb/tasks/Reranking/en/AskUbuntuDupQuestions.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Reranking/en/MindSmallReranking.py` & `mteb-1.5.3/mteb/tasks/Reranking/en/MindSmallReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Reranking/en/SciDocsReranking.py` & `mteb-1.5.3/mteb/tasks/Reranking/en/SciDocsReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Reranking/en/StackOverflowDupQuestions.py` & `mteb-1.5.3/mteb/tasks/Reranking/en/StackOverflowDupQuestions.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Reranking/fr/AlloprofReranking.py` & `mteb-1.5.3/mteb/tasks/Reranking/fr/AlloprofReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Reranking/fr/SyntecReranking.py` & `mteb-1.5.3/mteb/tasks/Reranking/fr/SyntecReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Reranking/multilingual/MIRACLReranking.py` & `mteb-1.5.3/mteb/tasks/Reranking/multilingual/MIRACLReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Reranking/zh/CMTEBReranking.py` & `mteb-1.5.3/mteb/tasks/Reranking/zh/CMTEBReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/__init__.py` & `mteb-1.5.3/mteb/tasks/Retrieval/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 from .da.dan_fever import *
 from .da.t2nord_retrieval import *
 from .da.twitterhjerne import *
 from .de.GerDaLIRRetrieval import *
 from .de.GermanDPRRetrieval import *
 from .de.GermanQuADRetrieval import *
+from .de.GerDaLIRSmallRetrieval import *
+from .de.LegalQuADRetrieval import *
 from .en.ArguAnaRetrieval import *
 from .en.ClimateFEVERRetrieval import *
 from .en.CQADupstackAndroidRetrieval import *
 from .en.CQADupstackEnglishRetrieval import *
 from .en.CQADupstackGamingRetrieval import *
 from .en.CQADupstackGisRetrieval import *
 from .en.CQADupstackMathematicaRetrieval import *
@@ -31,14 +33,19 @@
 from .en.NFCorpusRetrieval import *
 from .en.NQRetrieval import *
 from .en.QuoraRetrieval import *
 from .en.SCIDOCSRetrieval import *
 from .en.SciFactRetrieval import *
 from .en.Touche2020Retrieval import *
 from .en.TRECCOVIDRetrieval import *
+from .en.AILACasedocsRetrieval import *
+from .en.AILAStatutesRetrieval import *
+from .en.LegalBenchConsumerContractsQARetrieval import *
+from .en.LegalBenchCorporateLobbyingRetrieval import *
+from .en.LegalSummarizationRetrieval import *
 from .es.SpanishPassageRetrievalS2P import *
 from .es.SpanishPassageRetrievalS2S import *
 from .fr.AlloprofRetrieval import *
 from .fr.BSARDRetrieval import *
 from .fr.SyntecRetrieval import *
 from .ko.KoMiracl import *
 from .ko.KoMrtydi import *
@@ -60,7 +67,8 @@
 from .pl.QuoraPLRetrieval import *
 from .pl.SCIDOCSPLRetrieval import *
 from .pl.SciFactPLRetrieval import *
 from .pl.TRECCOVIDPLRetrieval import *
 from .sv.swedn_retrieval import *
 from .sv.swefaq_retrieval import *
 from .zh.CMTEBRetrieval import *
+from .zh.LeCaRDv2Retrieval import *
```

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/da/dan_fever.py` & `mteb-1.5.3/mteb/tasks/Retrieval/da/dan_fever.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/da/t2nord_retrieval.py` & `mteb-1.5.3/mteb/tasks/Retrieval/da/t2nord_retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/da/twitterhjerne.py` & `mteb-1.5.3/mteb/tasks/Retrieval/da/twitterhjerne.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/de/GerDaLIRRetrieval.py` & `mteb-1.5.3/mteb/tasks/Retrieval/de/GerDaLIRRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/de/GermanDPRRetrieval.py` & `mteb-1.5.3/mteb/tasks/Retrieval/de/GermanDPRRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/de/GermanQuADRetrieval.py` & `mteb-1.5.3/mteb/tasks/Retrieval/de/GermanQuADRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/en/ArguAnaRetrieval.py` & `mteb-1.5.3/mteb/tasks/Retrieval/en/ArguAnaRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/en/CQADupstackAndroidRetrieval.py` & `mteb-1.5.3/mteb/tasks/Retrieval/en/CQADupstackAndroidRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/en/CQADupstackEnglishRetrieval.py` & `mteb-1.5.3/mteb/tasks/Retrieval/en/CQADupstackEnglishRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/en/CQADupstackGamingRetrieval.py` & `mteb-1.5.3/mteb/tasks/Retrieval/en/CQADupstackGamingRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/en/CQADupstackGisRetrieval.py` & `mteb-1.5.3/mteb/tasks/Retrieval/en/CQADupstackGisRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/en/CQADupstackMathematicaRetrieval.py` & `mteb-1.5.3/mteb/tasks/Retrieval/en/CQADupstackMathematicaRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/en/CQADupstackPhysicsRetrieval.py` & `mteb-1.5.3/mteb/tasks/Retrieval/en/CQADupstackPhysicsRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/en/CQADupstackProgrammersRetrieval.py` & `mteb-1.5.3/mteb/tasks/Retrieval/en/CQADupstackProgrammersRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/en/CQADupstackStatsRetrieval.py` & `mteb-1.5.3/mteb/tasks/Retrieval/en/CQADupstackStatsRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/en/CQADupstackTexRetrieval.py` & `mteb-1.5.3/mteb/tasks/Retrieval/en/CQADupstackTexRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/en/CQADupstackUnixRetrieval.py` & `mteb-1.5.3/mteb/tasks/Retrieval/en/CQADupstackUnixRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/en/CQADupstackWebmastersRetrieval.py` & `mteb-1.5.3/mteb/tasks/Retrieval/en/CQADupstackWebmastersRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/en/CQADupstackWordpressRetrieval.py` & `mteb-1.5.3/mteb/tasks/Retrieval/en/CQADupstackWordpressRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/en/ClimateFEVERRetrieval.py` & `mteb-1.5.3/mteb/tasks/Retrieval/en/ClimateFEVERRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/en/DBPediaRetrieval.py` & `mteb-1.5.3/mteb/tasks/Retrieval/en/DBPediaRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/en/FEVERRetrieval.py` & `mteb-1.5.3/mteb/tasks/Retrieval/en/FEVERRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/en/FiQA2018Retrieval.py` & `mteb-1.5.3/mteb/tasks/Retrieval/en/FiQA2018Retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/en/HagridRetrieval.py` & `mteb-1.5.3/mteb/tasks/Retrieval/en/HagridRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/en/HotpotQARetrieval.py` & `mteb-1.5.3/mteb/tasks/Retrieval/en/HotpotQARetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/en/MSMARCORetrieval.py` & `mteb-1.5.3/mteb/tasks/Retrieval/en/MSMARCORetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/en/MSMARCOv2Retrieval.py` & `mteb-1.5.3/mteb/tasks/Retrieval/en/MSMARCOv2Retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/en/NFCorpusRetrieval.py` & `mteb-1.5.3/mteb/tasks/Retrieval/en/NFCorpusRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/en/NQRetrieval.py` & `mteb-1.5.3/mteb/tasks/Retrieval/en/NQRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/en/NarrativeQARetrieval.py` & `mteb-1.5.3/mteb/tasks/Retrieval/en/NarrativeQARetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/en/QuoraRetrieval.py` & `mteb-1.5.3/mteb/tasks/Retrieval/en/QuoraRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/en/SCIDOCSRetrieval.py` & `mteb-1.5.3/mteb/tasks/Retrieval/en/SCIDOCSRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/en/SciFactRetrieval.py` & `mteb-1.5.3/mteb/tasks/Retrieval/en/SciFactRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/en/TRECCOVIDRetrieval.py` & `mteb-1.5.3/mteb/tasks/Retrieval/en/TRECCOVIDRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/en/Touche2020Retrieval.py` & `mteb-1.5.3/mteb/tasks/Retrieval/en/Touche2020Retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/es/SpanishPassageRetrievalS2P.py` & `mteb-1.5.3/mteb/tasks/Retrieval/es/SpanishPassageRetrievalS2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/es/SpanishPassageRetrievalS2S.py` & `mteb-1.5.3/mteb/tasks/Retrieval/es/SpanishPassageRetrievalS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/fr/AlloprofRetrieval.py` & `mteb-1.5.3/mteb/tasks/Retrieval/fr/AlloprofRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/fr/BSARDRetrieval.py` & `mteb-1.5.3/mteb/tasks/Retrieval/fr/BSARDRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/fr/SyntecRetrieval.py` & `mteb-1.5.3/mteb/tasks/Retrieval/fr/SyntecRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/ko/KoMiracl.py` & `mteb-1.5.3/mteb/tasks/Retrieval/ko/KoMiracl.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/ko/KoMrtydi.py` & `mteb-1.5.3/mteb/tasks/Retrieval/ko/KoMrtydi.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/ko/KoStrategyQA.py` & `mteb-1.5.3/mteb/tasks/Retrieval/ko/KoStrategyQA.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/multilingual/MIRACLRetrieval.py` & `mteb-1.5.3/mteb/tasks/Retrieval/multilingual/MIRACLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/multilingual/MintakaRetrieval.py` & `mteb-1.5.3/mteb/tasks/Retrieval/multilingual/MintakaRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/multilingual/MultiLongDocRetrieval.py` & `mteb-1.5.3/mteb/tasks/Retrieval/multilingual/MultiLongDocRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/multilingual/XMarketRetrieval.py` & `mteb-1.5.3/mteb/tasks/Retrieval/multilingual/XMarketRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/multilingual/XPQARetrieval.py` & `mteb-1.5.3/mteb/tasks/Retrieval/multilingual/XPQARetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/nb/norquad.py` & `mteb-1.5.3/mteb/tasks/Retrieval/nb/norquad.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/nb/snl_retrieval.py` & `mteb-1.5.3/mteb/tasks/Retrieval/nb/snl_retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/pl/ArguAnaPLRetrieval.py` & `mteb-1.5.3/mteb/tasks/Retrieval/pl/ArguAnaPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/pl/DBPediaPLRetrieval.py` & `mteb-1.5.3/mteb/tasks/Retrieval/pl/DBPediaPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/pl/FiQAPLRetrieval.py` & `mteb-1.5.3/mteb/tasks/Retrieval/pl/FiQAPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/pl/HotpotQAPLRetrieval.py` & `mteb-1.5.3/mteb/tasks/Retrieval/pl/HotpotQAPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/pl/MSMARCOPLRetrieval.py` & `mteb-1.5.3/mteb/tasks/Retrieval/pl/MSMARCOPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/pl/NFCorpusPLRetrieval.py` & `mteb-1.5.3/mteb/tasks/Retrieval/pl/NFCorpusPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/pl/NQPLRetrieval.py` & `mteb-1.5.3/mteb/tasks/Retrieval/pl/NQPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/pl/QuoraPLRetrieval.py` & `mteb-1.5.3/mteb/tasks/Retrieval/pl/QuoraPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/pl/SCIDOCSPLRetrieval.py` & `mteb-1.5.3/mteb/tasks/Retrieval/pl/SCIDOCSPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/pl/SciFactPLRetrieval.py` & `mteb-1.5.3/mteb/tasks/Retrieval/pl/SciFactPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/pl/TRECCOVIDPLRetrieval.py` & `mteb-1.5.3/mteb/tasks/Retrieval/pl/TRECCOVIDPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/sv/swedn_retrieval.py` & `mteb-1.5.3/mteb/tasks/Retrieval/sv/swedn_retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/sv/swefaq_retrieval.py` & `mteb-1.5.3/mteb/tasks/Retrieval/sv/swefaq_retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Retrieval/zh/CMTEBRetrieval.py` & `mteb-1.5.3/mteb/tasks/Retrieval/zh/CMTEBRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/STS/__init__.py` & `mteb-1.5.3/mteb/tasks/STS/__init__.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/STS/de/GermanSTSBenchmarkSTS.py` & `mteb-1.5.3/mteb/tasks/STS/de/GermanSTSBenchmarkSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/STS/en/BiossesSTS.py` & `mteb-1.5.3/mteb/tasks/STS/en/BiossesSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/STS/en/STS12STS.py` & `mteb-1.5.3/mteb/tasks/STS/en/STS12STS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/STS/en/STS13STS.py` & `mteb-1.5.3/mteb/tasks/STS/en/STS13STS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/STS/en/STS14STS.py` & `mteb-1.5.3/mteb/tasks/STS/en/STS14STS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/STS/en/STS15STS.py` & `mteb-1.5.3/mteb/tasks/STS/en/STS15STS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/STS/en/STS16STS.py` & `mteb-1.5.3/mteb/tasks/STS/en/STS16STS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/STS/en/STSBenchmarkSTS.py` & `mteb-1.5.3/mteb/tasks/STS/en/STSBenchmarkSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/STS/en/SickrSTS.py` & `mteb-1.5.3/mteb/tasks/STS/en/SickrSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/STS/es/STSES.py` & `mteb-1.5.3/mteb/tasks/STS/es/STSES.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/STS/fr/SickFrSTS.py` & `mteb-1.5.3/mteb/tasks/STS/fr/SickFrSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/STS/multilingual/STS17CrosslingualSTS.py` & `mteb-1.5.3/mteb/tasks/STS/multilingual/STS17CrosslingualSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/STS/multilingual/STS22CrosslingualSTS.py` & `mteb-1.5.3/mteb/tasks/STS/multilingual/STS22CrosslingualSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/STS/multilingual/STSBenchmarkMultilingualSTS.py` & `mteb-1.5.3/mteb/tasks/STS/multilingual/STSBenchmarkMultilingualSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/STS/pl/PolishSTS.py` & `mteb-1.5.3/mteb/tasks/STS/pl/PolishSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/STS/zh/CMTEBSTS.py` & `mteb-1.5.3/mteb/tasks/STS/zh/CMTEBSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Summarization/en/SummEvalSummarization.py` & `mteb-1.5.3/mteb/tasks/Summarization/en/SummEvalSummarization.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb/tasks/Summarization/fr/SummEvalFrSummarization.py` & `mteb-1.5.3/mteb/tasks/Summarization/fr/SummEvalFrSummarization.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/mteb.egg-info/PKG-INFO` & `mteb-1.5.3/mteb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mteb
-Version: 1.5.2
+Version: 1.5.3
 Summary: Massive Text Embedding Benchmark
 Author-email: MTEB Contributors <niklas@huggingface.co>, nouamane@huggingface.co, info@nils-reimers.de
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `mteb-1.5.2/mteb.egg-info/SOURCES.txt` & `mteb-1.5.3/mteb.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 mteb/tasks/Classification/da/DdiscoCohesionClassification.py
 mteb/tasks/Classification/da/LccSentimentClassification.py
 mteb/tasks/Classification/da/__init__.py
 mteb/tasks/Classification/en/AmazonPolarityClassification.py
 mteb/tasks/Classification/en/Banking77Classification.py
 mteb/tasks/Classification/en/EmotionClassification.py
 mteb/tasks/Classification/en/ImdbClassification.py
+mteb/tasks/Classification/en/NewsClassification.py
 mteb/tasks/Classification/en/ToxicConversationsClassification.py
 mteb/tasks/Classification/en/TweetSentimentExtractionClassification.py
 mteb/tasks/Classification/en/__init__.py
 mteb/tasks/Classification/multilingual/AmazonCounterfactualClassification.py
 mteb/tasks/Classification/multilingual/AmazonReviewsClassification.py
 mteb/tasks/Classification/multilingual/MTOPDomainClassification.py
 mteb/tasks/Classification/multilingual/MTOPIntentClassification.py
@@ -151,17 +152,21 @@
 mteb/tasks/Reranking/zh/__init__.py
 mteb/tasks/Retrieval/__init__.py
 mteb/tasks/Retrieval/da/__init__.py
 mteb/tasks/Retrieval/da/dan_fever.py
 mteb/tasks/Retrieval/da/t2nord_retrieval.py
 mteb/tasks/Retrieval/da/twitterhjerne.py
 mteb/tasks/Retrieval/de/GerDaLIRRetrieval.py
+mteb/tasks/Retrieval/de/GerDaLIRSmallRetrieval.py
 mteb/tasks/Retrieval/de/GermanDPRRetrieval.py
 mteb/tasks/Retrieval/de/GermanQuADRetrieval.py
+mteb/tasks/Retrieval/de/LegalQuADRetrieval.py
 mteb/tasks/Retrieval/de/__init__.py
+mteb/tasks/Retrieval/en/AILACasedocsRetrieval.py
+mteb/tasks/Retrieval/en/AILAStatutesRetrieval.py
 mteb/tasks/Retrieval/en/ArguAnaRetrieval.py
 mteb/tasks/Retrieval/en/CQADupstackAndroidRetrieval.py
 mteb/tasks/Retrieval/en/CQADupstackEnglishRetrieval.py
 mteb/tasks/Retrieval/en/CQADupstackGamingRetrieval.py
 mteb/tasks/Retrieval/en/CQADupstackGisRetrieval.py
 mteb/tasks/Retrieval/en/CQADupstackMathematicaRetrieval.py
 mteb/tasks/Retrieval/en/CQADupstackPhysicsRetrieval.py
@@ -173,14 +178,17 @@
 mteb/tasks/Retrieval/en/CQADupstackWordpressRetrieval.py
 mteb/tasks/Retrieval/en/ClimateFEVERRetrieval.py
 mteb/tasks/Retrieval/en/DBPediaRetrieval.py
 mteb/tasks/Retrieval/en/FEVERRetrieval.py
 mteb/tasks/Retrieval/en/FiQA2018Retrieval.py
 mteb/tasks/Retrieval/en/HagridRetrieval.py
 mteb/tasks/Retrieval/en/HotpotQARetrieval.py
+mteb/tasks/Retrieval/en/LegalBenchConsumerContractsQARetrieval.py
+mteb/tasks/Retrieval/en/LegalBenchCorporateLobbyingRetrieval.py
+mteb/tasks/Retrieval/en/LegalSummarizationRetrieval.py
 mteb/tasks/Retrieval/en/MSMARCORetrieval.py
 mteb/tasks/Retrieval/en/MSMARCOv2Retrieval.py
 mteb/tasks/Retrieval/en/NFCorpusRetrieval.py
 mteb/tasks/Retrieval/en/NQRetrieval.py
 mteb/tasks/Retrieval/en/NarrativeQARetrieval.py
 mteb/tasks/Retrieval/en/QuoraRetrieval.py
 mteb/tasks/Retrieval/en/SCIDOCSRetrieval.py
@@ -220,14 +228,15 @@
 mteb/tasks/Retrieval/pl/SciFactPLRetrieval.py
 mteb/tasks/Retrieval/pl/TRECCOVIDPLRetrieval.py
 mteb/tasks/Retrieval/pl/__init__.py
 mteb/tasks/Retrieval/sv/__init__.py
 mteb/tasks/Retrieval/sv/swedn_retrieval.py
 mteb/tasks/Retrieval/sv/swefaq_retrieval.py
 mteb/tasks/Retrieval/zh/CMTEBRetrieval.py
+mteb/tasks/Retrieval/zh/LeCaRDv2Retrieval.py
 mteb/tasks/Retrieval/zh/__init__.py
 mteb/tasks/STS/__init__.py
 mteb/tasks/STS/de/GermanSTSBenchmarkSTS.py
 mteb/tasks/STS/de/__init__.py
 mteb/tasks/STS/en/BiossesSTS.py
 mteb/tasks/STS/en/STS12STS.py
 mteb/tasks/STS/en/STS13STS.py
@@ -257,14 +266,15 @@
 scripts/merge_cqadupstack.py
 scripts/mteb_meta.py
 scripts/run_mteb_chinese.py
 scripts/run_mteb_english.py
 scripts/run_mteb_french.py
 scripts/run_mteb_german.py
 scripts/run_mteb_korean.py
+scripts/run_mteb_law.py
 scripts/run_mteb_polish.py
 scripts/data/create_task_table.py
 scripts/data/amazon_polarity/create_data.py
 scripts/data/amazon_reviews_multi/create_data.py
 scripts/data/arxiv/script_clustering.py
 scripts/data/arxiv/script_raw.py
 scripts/data/biorxiv/script_clustering.py
```

### Comparing `mteb-1.5.2/pyproject.toml` & `mteb-1.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mteb"
-version = "1.5.2"
+version = "1.5.3"
 description = "Massive Text Embedding Benchmark"
 readme = "README.md"
 authors = [
     { name = "MTEB Contributors", email = "niklas@huggingface.co" },
     { email = "nouamane@huggingface.co" },
     { email = "info@nils-reimers.de" },
 ]
```

### Comparing `mteb-1.5.2/scripts/data/amazon_polarity/create_data.py` & `mteb-1.5.3/scripts/data/amazon_polarity/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/scripts/data/amazon_reviews_multi/create_data.py` & `mteb-1.5.3/scripts/data/amazon_reviews_multi/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/scripts/data/arxiv/script_clustering.py` & `mteb-1.5.3/scripts/data/arxiv/script_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/scripts/data/arxiv/script_raw.py` & `mteb-1.5.3/scripts/data/arxiv/script_raw.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/scripts/data/biorxiv/script_clustering.py` & `mteb-1.5.3/scripts/data/biorxiv/script_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/scripts/data/biorxiv/script_raw.py` & `mteb-1.5.3/scripts/data/biorxiv/script_raw.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/scripts/data/bucc/create_data.py` & `mteb-1.5.3/scripts/data/bucc/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/scripts/data/create_task_table.py` & `mteb-1.5.3/scripts/data/create_task_table.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/scripts/data/germanquad/process_data.py` & `mteb-1.5.3/scripts/data/germanquad/process_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/scripts/data/hal/create_data.py` & `mteb-1.5.3/scripts/data/hal/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/scripts/data/imdb/create_data.py` & `mteb-1.5.3/scripts/data/imdb/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/scripts/data/medrxiv/script_clustering.py` & `mteb-1.5.3/scripts/data/medrxiv/script_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/scripts/data/medrxiv/script_raw.py` & `mteb-1.5.3/scripts/data/medrxiv/script_raw.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/scripts/data/mind/prepare_data.py` & `mteb-1.5.3/scripts/data/mind/prepare_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/scripts/data/redditp2p/script_clustering.py` & `mteb-1.5.3/scripts/data/redditp2p/script_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/scripts/data/stackexchangep2p/script_clustering.py` & `mteb-1.5.3/scripts/data/stackexchangep2p/script_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/scripts/data/sts22-crosslingual-sts/create_data.py` & `mteb-1.5.3/scripts/data/sts22-crosslingual-sts/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/scripts/data/summeval_fr/create_data.py` & `mteb-1.5.3/scripts/data/summeval_fr/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/scripts/data/toxic_conversations_50k/create_data.py` & `mteb-1.5.3/scripts/data/toxic_conversations_50k/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/scripts/merge_cqadupstack.py` & `mteb-1.5.3/scripts/merge_cqadupstack.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/scripts/mteb_meta.py` & `mteb-1.5.3/scripts/mteb_meta.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/scripts/run_mteb_chinese.py` & `mteb-1.5.3/scripts/run_mteb_chinese.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/scripts/run_mteb_english.py` & `mteb-1.5.3/scripts/run_mteb_english.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/scripts/run_mteb_french.py` & `mteb-1.5.3/scripts/run_mteb_french.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/scripts/run_mteb_german.py` & `mteb-1.5.3/scripts/run_mteb_german.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/scripts/run_mteb_korean.py` & `mteb-1.5.3/scripts/run_mteb_korean.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/scripts/run_mteb_polish.py` & `mteb-1.5.3/scripts/run_mteb_polish.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/tests/test_ClusteringEvaluator.py` & `mteb-1.5.3/tests/test_ClusteringEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/tests/test_PairClassificationEvaluator.py` & `mteb-1.5.3/tests/test_PairClassificationEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/tests/test_RerankingEvaluator.py` & `mteb-1.5.3/tests/test_RerankingEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/tests/test_RetrievalEvaluator.py` & `mteb-1.5.3/tests/test_RetrievalEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/tests/test_TaskMetadata.py` & `mteb-1.5.3/tests/test_TaskMetadata.py`

 * *Files identical despite different names*

### Comparing `mteb-1.5.2/tests/test_all_abstasks.py` & `mteb-1.5.3/tests/test_all_abstasks.py`

 * *Files identical despite different names*

