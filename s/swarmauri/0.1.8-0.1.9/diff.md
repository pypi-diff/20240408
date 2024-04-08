# Comparing `tmp/swarmauri-0.1.8-py3-none-any.whl.zip` & `tmp/swarmauri-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 149213 bytes, number of entries: 270
--rw-rw-rw-  2.0 fat       21 b- defN 24-Mar-06 10:50 swarmauri/__init__.py
+Zip file size: 160561 bytes, number of entries: 295
+-rw-rw-rw-  2.0 fat       21 b- defN 24-Mar-06 12:54 swarmauri/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-01 11:37 swarmauri/community/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Feb-19 02:42 swarmauri/community/document_stores/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Feb-19 02:42 swarmauri/community/document_stores/base/__init__.py
 -rw-rw-rw-  2.0 fat     2873 b- defN 24-Feb-27 22:23 swarmauri/community/document_stores/concrete/RedisDocumentStore.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Feb-19 02:42 swarmauri/community/document_stores/concrete/__init__.py
 -rw-rw-rw-  2.0 fat       27 b- defN 24-Feb-20 00:24 swarmauri/community/retrievers/__init__.py
 -rw-rw-rw-  2.0 fat       27 b- defN 24-Feb-20 00:24 swarmauri/community/retrievers/base/__init__.py
@@ -19,17 +19,25 @@
 -rw-rw-rw-  2.0 fat      888 b- defN 24-Feb-25 00:17 swarmauri/community/tools/concrete/SentimentAnalysisTool.py
 -rw-rw-rw-  2.0 fat     2098 b- defN 24-Feb-26 10:14 swarmauri/community/tools/concrete/WebScrapingTool.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Feb-19 02:42 swarmauri/community/tools/concrete/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-03 23:23 swarmauri/core/__init__.py
 -rw-rw-rw-  2.0 fat     2067 b- defN 24-Feb-29 07:10 swarmauri/core/agent_apis/IAgentCommands.py
 -rw-rw-rw-  2.0 fat     1786 b- defN 24-Feb-29 07:10 swarmauri/core/agent_apis/IAgentRouterCRUD.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Feb-19 02:42 swarmauri/core/agent_apis/__init__.py
--rw-rw-rw-  2.0 fat     1869 b- defN 24-Feb-24 21:26 swarmauri/core/agents/ISwarmAgent.py
+-rw-rw-rw-  2.0 fat      477 b- defN 24-Mar-06 13:34 swarmauri/core/agents/IAgentConversation.py
+-rw-rw-rw-  2.0 fat      317 b- defN 24-Mar-06 13:37 swarmauri/core/agents/IAgentDocument.py
+-rw-rw-rw-  2.0 fat      355 b- defN 24-Mar-06 14:06 swarmauri/core/agents/IAgentName.py
+-rw-rw-rw-  2.0 fat      303 b- defN 24-Mar-06 13:37 swarmauri/core/agents/IAgentParser.py
+-rw-rw-rw-  2.0 fat      327 b- defN 24-Mar-06 13:37 swarmauri/core/agents/IAgentRetriever.py
+-rw-rw-rw-  2.0 fat      317 b- defN 24-Mar-06 13:33 swarmauri/core/agents/IAgentToolkit.py
+-rw-rw-rw-  2.0 fat      638 b- defN 24-Mar-06 13:34 swarmauri/core/agents/ISwarmAgent.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Feb-19 02:42 swarmauri/core/agents/__init__.py
 -rw-rw-rw-  2.0 fat      511 b- defN 24-Mar-06 07:13 swarmauri/core/chains/ICallableChain.py
+-rw-rw-rw-  2.0 fat     1228 b- defN 24-Mar-07 03:38 swarmauri/core/chains/IChain.py
+-rw-rw-rw-  2.0 fat      960 b- defN 24-Mar-06 22:31 swarmauri/core/chains/IChainStep.py
 -rw-rw-rw-  2.0 fat       63 b- defN 24-Mar-06 07:46 swarmauri/core/chains/__init__.py
 -rw-rw-rw-  2.0 fat     1134 b- defN 24-Mar-06 09:41 swarmauri/core/chunkers/IChunker.py
 -rw-rw-rw-  2.0 fat       93 b- defN 24-Feb-29 02:35 swarmauri/core/chunkers/__init__.py
 -rw-rw-rw-  2.0 fat     1165 b- defN 24-Feb-24 21:26 swarmauri/core/conversations/IConversation.py
 -rw-rw-rw-  2.0 fat      307 b- defN 24-Feb-24 19:48 swarmauri/core/conversations/IMaxSize.py
 -rw-rw-rw-  2.0 fat      871 b- defN 24-Feb-24 21:28 swarmauri/core/conversations/ISystemContext.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Feb-19 02:42 swarmauri/core/conversations/__init__.py
@@ -50,14 +58,15 @@
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Feb-19 02:42 swarmauri/core/prompts/__init__.py
 -rw-rw-rw-  2.0 fat      904 b- defN 24-Feb-24 21:27 swarmauri/core/retrievers/IRetriever.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-03 23:23 swarmauri/core/retrievers/__init__.py
 -rw-rw-rw-  2.0 fat     2306 b- defN 24-Feb-29 07:15 swarmauri/core/swarm_apis/IAgentRegistration.py
 -rw-rw-rw-  2.0 fat     1140 b- defN 24-Mar-03 14:20 swarmauri/core/swarm_apis/ISwarmAPI.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Feb-19 02:42 swarmauri/core/swarm_apis/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Feb-23 03:51 swarmauri/core/swarms/ISwarm.py
+-rw-rw-rw-  2.0 fat      331 b- defN 24-Mar-06 22:32 swarmauri/core/swarms/ISwarmComponent.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Feb-19 02:42 swarmauri/core/swarms/__init__.py
 -rw-rw-rw-  2.0 fat     1635 b- defN 24-Feb-24 21:26 swarmauri/core/toolkits/IToolkit.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Feb-19 02:42 swarmauri/core/toolkits/__init__.py
 -rw-rw-rw-  2.0 fat     2042 b- defN 24-Feb-24 20:06 swarmauri/core/tools/IParameter.py
 -rw-rw-rw-  2.0 fat      516 b- defN 24-Mar-03 17:27 swarmauri/core/tools/ITool.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Feb-19 02:42 swarmauri/core/tools/__init__.py
 -rw-rw-rw-  2.0 fat     1058 b- defN 24-Mar-06 05:25 swarmauri/core/tracing/IChainTracer.py
@@ -88,14 +97,24 @@
 -rw-rw-rw-  2.0 fat      624 b- defN 24-Mar-01 10:44 swarmauri/core/vectorizers/IVectorize.py
 -rw-rw-rw-  2.0 fat        1 b- defN 24-Feb-29 23:57 swarmauri/core/vectorizers/__init__.py
 -rw-rw-rw-  2.0 fat      578 b- defN 24-Mar-01 23:23 swarmauri/core/vectors/IVector.py
 -rw-rw-rw-  2.0 fat      900 b- defN 24-Feb-29 04:09 swarmauri/core/vectors/IVectorMeta.py
 -rw-rw-rw-  2.0 fat     1312 b- defN 24-Feb-29 22:50 swarmauri/core/vectors/IVectorTransform.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-03 23:24 swarmauri/core/vectors/__init__.py
 -rw-rw-rw-  2.0 fat       27 b- defN 24-Feb-20 05:28 swarmauri/experimental/__init__.py
+-rw-rw-rw-  2.0 fat      628 b- defN 24-Mar-06 23:57 swarmauri/experimental/chains/ChainOrderStrategy.py
+-rw-rw-rw-  2.0 fat      516 b- defN 24-Mar-06 22:36 swarmauri/experimental/chains/ChainOrderStrategyBase.py
+-rw-rw-rw-  2.0 fat      842 b- defN 24-Mar-06 23:53 swarmauri/experimental/chains/ChainProcessingStrategy.py
+-rw-rw-rw-  2.0 fat      603 b- defN 24-Mar-06 23:48 swarmauri/experimental/chains/ChainProcessingStrategyBase.py
+-rw-rw-rw-  2.0 fat      299 b- defN 24-Mar-06 22:32 swarmauri/experimental/chains/IChainOrderStrategy.py
+-rw-rw-rw-  2.0 fat      585 b- defN 24-Mar-06 22:32 swarmauri/experimental/chains/IChainProcessingStrategy.py
+-rw-rw-rw-  2.0 fat      725 b- defN 24-Mar-07 01:54 swarmauri/experimental/chains/MatrixOrderStrategy.py
+-rw-rw-rw-  2.0 fat     1073 b- defN 24-Mar-07 00:47 swarmauri/experimental/chains/MatrixProcessingStrategy.py
+-rw-rw-rw-  2.0 fat     4481 b- defN 24-Mar-06 12:26 swarmauri/experimental/chains/TypeAgnosticCallableChain.py
+-rw-rw-rw-  2.0 fat        1 b- defN 24-Mar-07 03:35 swarmauri/experimental/chains/__init__.py
 -rw-rw-rw-  2.0 fat     3471 b- defN 24-Mar-04 00:27 swarmauri/experimental/conversations/ConsensusBuildingConversation.py
 -rw-rw-rw-  2.0 fat     2219 b- defN 24-Feb-24 23:03 swarmauri/experimental/conversations/SemanticConversation.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Feb-23 04:51 swarmauri/experimental/conversations/__init__.py
 -rw-rw-rw-  2.0 fat     3556 b- defN 24-Mar-03 14:27 swarmauri/experimental/models/HierarchicalAttentionModel.py
 -rw-rw-rw-  2.0 fat     1846 b- defN 24-Feb-24 23:05 swarmauri/experimental/models/SageMaker.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Feb-23 05:01 swarmauri/experimental/models/__init__.py
 -rw-rw-rw-  2.0 fat     1508 b- defN 24-Feb-29 02:42 swarmauri/experimental/parsers/PDFToTextParser.py
@@ -120,30 +139,35 @@
 -rw-rw-rw-  2.0 fat     2643 b- defN 24-Feb-29 09:07 swarmauri/experimental/vector_stores/SSIVSimilarity.py
 -rw-rw-rw-  2.0 fat     7058 b- defN 24-Mar-03 09:40 swarmauri/experimental/vector_stores/ScannVectorStore.py
 -rw-rw-rw-  2.0 fat     2213 b- defN 24-Mar-03 14:31 swarmauri/experimental/vector_stores/SorensenDiceDistance.py
 -rw-rw-rw-  2.0 fat     1989 b- defN 24-Mar-03 14:31 swarmauri/experimental/vector_stores/SquaredEuclideanDistance.py
 -rw-rw-rw-  2.0 fat       27 b- defN 24-Feb-20 05:28 swarmauri/experimental/vector_stores/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-06 07:33 swarmauri/standard/__init__.py
 -rw-rw-rw-  2.0 fat       27 b- defN 24-Feb-20 05:28 swarmauri/standard/agents/__init__.py
--rw-rw-rw-  2.0 fat     3398 b- defN 24-Feb-26 09:36 swarmauri/standard/agents/base/SwarmAgentBase.py
+-rw-rw-rw-  2.0 fat     1650 b- defN 24-Mar-06 14:58 swarmauri/standard/agents/base/AgentBase.py
+-rw-rw-rw-  2.0 fat      913 b- defN 24-Mar-06 15:05 swarmauri/standard/agents/base/ConversationAgentBase.py
+-rw-rw-rw-  2.0 fat      546 b- defN 24-Mar-06 14:31 swarmauri/standard/agents/base/NamedAgentBase.py
+-rw-rw-rw-  2.0 fat     1061 b- defN 24-Mar-06 15:05 swarmauri/standard/agents/base/ToolAgentBase.py
 -rw-rw-rw-  2.0 fat       27 b- defN 24-Feb-20 05:28 swarmauri/standard/agents/base/__init__.py
--rw-rw-rw-  2.0 fat     2169 b- defN 24-Feb-26 14:24 swarmauri/standard/agents/concrete/ChatSwarmAgent.py
--rw-rw-rw-  2.0 fat     2404 b- defN 24-Feb-27 03:25 swarmauri/standard/agents/concrete/MultiPartyChatSwarmAgent.py
--rw-rw-rw-  2.0 fat     4086 b- defN 24-Feb-27 03:25 swarmauri/standard/agents/concrete/MultiPartyToolAgent.py
--rw-rw-rw-  2.0 fat     1428 b- defN 24-Feb-24 22:41 swarmauri/standard/agents/concrete/SimpleSwarmAgent.py
--rw-rw-rw-  2.0 fat     1135 b- defN 24-Feb-24 22:42 swarmauri/standard/agents/concrete/SingleCommandAgent.py
--rw-rw-rw-  2.0 fat     3804 b- defN 24-Mar-03 19:50 swarmauri/standard/agents/concrete/ToolAgent.py
+-rw-rw-rw-  2.0 fat     1688 b- defN 24-Mar-06 14:42 swarmauri/standard/agents/concrete/ChatSwarmAgent.py
+-rw-rw-rw-  2.0 fat     2101 b- defN 24-Mar-06 15:05 swarmauri/standard/agents/concrete/MultiPartyChatSwarmAgent.py
+-rw-rw-rw-  2.0 fat     3847 b- defN 24-Mar-06 15:06 swarmauri/standard/agents/concrete/MultiPartyToolAgent.py
+-rw-rw-rw-  2.0 fat      925 b- defN 24-Mar-06 14:55 swarmauri/standard/agents/concrete/SimpleSwarmAgent.py
+-rw-rw-rw-  2.0 fat      569 b- defN 24-Mar-06 14:55 swarmauri/standard/agents/concrete/SingleCommandAgent.py
+-rw-rw-rw-  2.0 fat     3451 b- defN 24-Mar-06 14:00 swarmauri/standard/agents/concrete/ToolAgent.py
 -rw-rw-rw-  2.0 fat       27 b- defN 24-Feb-20 05:28 swarmauri/standard/agents/concrete/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Feb-23 04:36 swarmauri/standard/apis/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Feb-23 04:36 swarmauri/standard/apis/base/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Feb-23 04:36 swarmauri/standard/apis/concrete/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-06 07:46 swarmauri/standard/chains/__init__.py
+-rw-rw-rw-  2.0 fat     2007 b- defN 24-Mar-07 03:22 swarmauri/standard/chains/base/ChainBase.py
+-rw-rw-rw-  2.0 fat     1050 b- defN 24-Mar-06 23:41 swarmauri/standard/chains/base/ChainStepBase.py
 -rw-rw-rw-  2.0 fat        1 b- defN 24-Mar-06 07:27 swarmauri/standard/chains/base/__init__.py
 -rw-rw-rw-  2.0 fat     1262 b- defN 24-Mar-06 10:26 swarmauri/standard/chains/concrete/CallableChain.py
--rw-rw-rw-  2.0 fat     4481 b- defN 24-Mar-06 12:26 swarmauri/standard/chains/concrete/TypeAgnosticCallableChain.py
+-rw-rw-rw-  2.0 fat     1594 b- defN 24-Mar-06 23:53 swarmauri/standard/chains/concrete/Chain.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-06 07:46 swarmauri/standard/chains/concrete/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Feb-23 04:36 swarmauri/standard/chunkers/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Feb-23 04:36 swarmauri/standard/chunkers/base/__init__.py
 -rw-rw-rw-  2.0 fat     1935 b- defN 24-Mar-03 14:28 swarmauri/standard/chunkers/concrete/DelimiterBasedChunker.py
 -rw-rw-rw-  2.0 fat     1477 b- defN 24-Mar-03 14:27 swarmauri/standard/chunkers/concrete/FixedLengthChunker.py
 -rw-rw-rw-  2.0 fat     2164 b- defN 24-Mar-06 09:27 swarmauri/standard/chunkers/concrete/MdSnippetChunker.py
 -rw-rw-rw-  2.0 fat     1198 b- defN 24-Mar-05 00:05 swarmauri/standard/chunkers/concrete/SimpleSentenceChunker.py
@@ -215,14 +239,15 @@
 -rw-rw-rw-  2.0 fat     1525 b- defN 24-Feb-27 13:25 swarmauri/standard/retrievers/base/DocumentRetrieverBase.py
 -rw-rw-rw-  2.0 fat       27 b- defN 24-Feb-20 00:24 swarmauri/standard/retrievers/base/__init__.py
 -rw-rw-rw-  2.0 fat       27 b- defN 24-Feb-20 00:24 swarmauri/standard/retrievers/concrete/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Feb-19 02:42 swarmauri/standard/states/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Feb-19 02:42 swarmauri/standard/states/base/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Feb-19 02:42 swarmauri/standard/states/concrete/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Feb-19 02:42 swarmauri/standard/swarms/__init__.py
+-rw-rw-rw-  2.0 fat      553 b- defN 24-Mar-06 22:40 swarmauri/standard/swarms/base/SwarmComponentBase.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Feb-19 02:42 swarmauri/standard/swarms/base/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Feb-19 02:42 swarmauri/standard/swarms/concrete/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Feb-19 02:42 swarmauri/standard/toolkits/__init__.py
 -rw-rw-rw-  2.0 fat     2430 b- defN 24-Feb-25 00:14 swarmauri/standard/toolkits/base/ToolkitBase.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Feb-19 02:42 swarmauri/standard/toolkits/base/__init__.py
 -rw-rw-rw-  2.0 fat      510 b- defN 24-Feb-25 00:14 swarmauri/standard/toolkits/concrete/Toolkit.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Feb-19 02:42 swarmauri/standard/toolkits/concrete/__init__.py
@@ -261,12 +286,12 @@
 -rw-rw-rw-  2.0 fat     2369 b- defN 24-Mar-01 10:43 swarmauri/standard/vectorizers/concrete/TFIDFVectorizer.py
 -rw-rw-rw-  2.0 fat        1 b- defN 24-Mar-01 00:01 swarmauri/standard/vectorizers/concrete/__init__.py
 -rw-rw-rw-  2.0 fat       27 b- defN 24-Feb-20 05:28 swarmauri/standard/vectors/__init__.py
 -rw-rw-rw-  2.0 fat      751 b- defN 24-Mar-01 23:28 swarmauri/standard/vectors/base/VectorBase.py
 -rw-rw-rw-  2.0 fat       27 b- defN 24-Feb-20 05:28 swarmauri/standard/vectors/base/__init__.py
 -rw-rw-rw-  2.0 fat      211 b- defN 24-Mar-01 04:52 swarmauri/standard/vectors/concrete/SimpleVector.py
 -rw-rw-rw-  2.0 fat       27 b- defN 24-Feb-20 05:28 swarmauri/standard/vectors/concrete/__init__.py
--rw-rw-rw-  2.0 fat     3536 b- defN 24-Mar-06 12:26 swarmauri-0.1.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Mar-06 12:26 swarmauri-0.1.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 24-Mar-06 12:26 swarmauri-0.1.8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat    27654 b- defN 24-Mar-06 12:26 swarmauri-0.1.8.dist-info/RECORD
-270 files, 308027 bytes uncompressed, 103363 bytes compressed:  66.4%
+-rw-rw-rw-  2.0 fat     3536 b- defN 24-Mar-07 03:39 swarmauri-0.1.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Mar-07 03:39 swarmauri-0.1.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 24-Mar-07 03:39 swarmauri-0.1.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat    30199 b- defN 24-Mar-07 03:39 swarmauri-0.1.9.dist-info/RECORD
+295 files, 322759 bytes uncompressed, 110523 bytes compressed:  65.8%
```

## zipnote {}

```diff
@@ -66,23 +66,47 @@
 
 Filename: swarmauri/core/agent_apis/IAgentRouterCRUD.py
 Comment: 
 
 Filename: swarmauri/core/agent_apis/__init__.py
 Comment: 
 
+Filename: swarmauri/core/agents/IAgentConversation.py
+Comment: 
+
+Filename: swarmauri/core/agents/IAgentDocument.py
+Comment: 
+
+Filename: swarmauri/core/agents/IAgentName.py
+Comment: 
+
+Filename: swarmauri/core/agents/IAgentParser.py
+Comment: 
+
+Filename: swarmauri/core/agents/IAgentRetriever.py
+Comment: 
+
+Filename: swarmauri/core/agents/IAgentToolkit.py
+Comment: 
+
 Filename: swarmauri/core/agents/ISwarmAgent.py
 Comment: 
 
 Filename: swarmauri/core/agents/__init__.py
 Comment: 
 
 Filename: swarmauri/core/chains/ICallableChain.py
 Comment: 
 
+Filename: swarmauri/core/chains/IChain.py
+Comment: 
+
+Filename: swarmauri/core/chains/IChainStep.py
+Comment: 
+
 Filename: swarmauri/core/chains/__init__.py
 Comment: 
 
 Filename: swarmauri/core/chunkers/IChunker.py
 Comment: 
 
 Filename: swarmauri/core/chunkers/__init__.py
@@ -159,14 +183,17 @@
 
 Filename: swarmauri/core/swarm_apis/__init__.py
 Comment: 
 
 Filename: swarmauri/core/swarms/ISwarm.py
 Comment: 
 
+Filename: swarmauri/core/swarms/ISwarmComponent.py
+Comment: 
+
 Filename: swarmauri/core/swarms/__init__.py
 Comment: 
 
 Filename: swarmauri/core/toolkits/IToolkit.py
 Comment: 
 
 Filename: swarmauri/core/toolkits/__init__.py
@@ -273,14 +300,44 @@
 
 Filename: swarmauri/core/vectors/__init__.py
 Comment: 
 
 Filename: swarmauri/experimental/__init__.py
 Comment: 
 
+Filename: swarmauri/experimental/chains/ChainOrderStrategy.py
+Comment: 
+
+Filename: swarmauri/experimental/chains/ChainOrderStrategyBase.py
+Comment: 
+
+Filename: swarmauri/experimental/chains/ChainProcessingStrategy.py
+Comment: 
+
+Filename: swarmauri/experimental/chains/ChainProcessingStrategyBase.py
+Comment: 
+
+Filename: swarmauri/experimental/chains/IChainOrderStrategy.py
+Comment: 
+
+Filename: swarmauri/experimental/chains/IChainProcessingStrategy.py
+Comment: 
+
+Filename: swarmauri/experimental/chains/MatrixOrderStrategy.py
+Comment: 
+
+Filename: swarmauri/experimental/chains/MatrixProcessingStrategy.py
+Comment: 
+
+Filename: swarmauri/experimental/chains/TypeAgnosticCallableChain.py
+Comment: 
+
+Filename: swarmauri/experimental/chains/__init__.py
+Comment: 
+
 Filename: swarmauri/experimental/conversations/ConsensusBuildingConversation.py
 Comment: 
 
 Filename: swarmauri/experimental/conversations/SemanticConversation.py
 Comment: 
 
 Filename: swarmauri/experimental/conversations/__init__.py
@@ -369,15 +426,24 @@
 
 Filename: swarmauri/standard/__init__.py
 Comment: 
 
 Filename: swarmauri/standard/agents/__init__.py
 Comment: 
 
-Filename: swarmauri/standard/agents/base/SwarmAgentBase.py
+Filename: swarmauri/standard/agents/base/AgentBase.py
+Comment: 
+
+Filename: swarmauri/standard/agents/base/ConversationAgentBase.py
+Comment: 
+
+Filename: swarmauri/standard/agents/base/NamedAgentBase.py
+Comment: 
+
+Filename: swarmauri/standard/agents/base/ToolAgentBase.py
 Comment: 
 
 Filename: swarmauri/standard/agents/base/__init__.py
 Comment: 
 
 Filename: swarmauri/standard/agents/concrete/ChatSwarmAgent.py
 Comment: 
@@ -408,21 +474,27 @@
 
 Filename: swarmauri/standard/apis/concrete/__init__.py
 Comment: 
 
 Filename: swarmauri/standard/chains/__init__.py
 Comment: 
 
+Filename: swarmauri/standard/chains/base/ChainBase.py
+Comment: 
+
+Filename: swarmauri/standard/chains/base/ChainStepBase.py
+Comment: 
+
 Filename: swarmauri/standard/chains/base/__init__.py
 Comment: 
 
 Filename: swarmauri/standard/chains/concrete/CallableChain.py
 Comment: 
 
-Filename: swarmauri/standard/chains/concrete/TypeAgnosticCallableChain.py
+Filename: swarmauri/standard/chains/concrete/Chain.py
 Comment: 
 
 Filename: swarmauri/standard/chains/concrete/__init__.py
 Comment: 
 
 Filename: swarmauri/standard/chunkers/__init__.py
 Comment: 
@@ -654,14 +726,17 @@
 
 Filename: swarmauri/standard/states/concrete/__init__.py
 Comment: 
 
 Filename: swarmauri/standard/swarms/__init__.py
 Comment: 
 
+Filename: swarmauri/standard/swarms/base/SwarmComponentBase.py
+Comment: 
+
 Filename: swarmauri/standard/swarms/base/__init__.py
 Comment: 
 
 Filename: swarmauri/standard/swarms/concrete/__init__.py
 Comment: 
 
 Filename: swarmauri/standard/toolkits/__init__.py
@@ -792,20 +867,20 @@
 
 Filename: swarmauri/standard/vectors/concrete/SimpleVector.py
 Comment: 
 
 Filename: swarmauri/standard/vectors/concrete/__init__.py
 Comment: 
 
-Filename: swarmauri-0.1.8.dist-info/METADATA
+Filename: swarmauri-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: swarmauri-0.1.8.dist-info/WHEEL
+Filename: swarmauri-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: swarmauri-0.1.8.dist-info/top_level.txt
+Filename: swarmauri-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: swarmauri-0.1.8.dist-info/RECORD
+Filename: swarmauri-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## swarmauri/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "0.1.8"
+__version__ = "0.1.9"
```

## swarmauri/core/agents/ISwarmAgent.py

```diff
@@ -1,55 +1,26 @@
 from abc import ABC, abstractmethod
-from typing import Any, Optional, List
-from ..models.IModel import IModel
-from ..toolkits.IToolkit import IToolkit
-from ..parsers.IParser import IParser
-from ..conversations.IConversation import IConversation
-from ..documents.IDocument import IDocument
-from ..retrievers.IRetriever import IRetriever
-from ..messages.IMessage import IMessage
+from typing import Any, Optional
+from swarmauri.core.models.IModel import IModel
 
 class ISwarmAgent(ABC):
-    
-    @abstractmethod
-    def __init__(self, model: IModel, 
-                 conversation: Optional[IConversation] = None, 
-                 toolkit: Optional[IToolkit] = None, 
-                 parser: Optional[IParser] = None, 
-                 documents: Optional[List[IDocument]] = [], 
-                 retriever: Optional[IRetriever] = None):
-        pass
-    
-    @abstractmethod
-    def exec(self, input_str: Optional[Any]) -> Any:
-        pass
-    
-    @abstractmethod
-    def get_model(self) -> IModel:
-        """Returns the model component of the agent."""
-        pass
-    
-    @abstractmethod
-    def get_toolkit(self) -> Optional[IToolkit]:
-        """Returns the toolkit component of the agent, if available."""
-        pass
-    
-    @abstractmethod
-    def get_parser(self) -> Optional[IParser]:
-        """Returns the parser component of the agent, if available."""
-        pass
 
     @abstractmethod
-    def get_conversation(self) -> Optional[IConversation]:
-        """Returns the conversation manager component of the agent, if available."""
+    def exec(self, input_data: Optional[Any]) -> Any:
+        """
+        Executive method that triggers the agent's action based on the input data.
+        """
         pass
     
+    @property
     @abstractmethod
-    def get_documents(self) -> List[IDocument]:
-        """Returns the list of document components associated with the agent."""
+    def model(self) -> IModel:
+        """
+        The model property describes the computational model used by the agent.
+        """
         pass
     
+    @model.setter
     @abstractmethod
-    def get_retriever(self) -> Optional[IRetriever]:
-        """Returns the retriever component of the agent, if available."""
-        pass
+    def model(self) -> IModel:
 
+        pass
```

## swarmauri/standard/agents/concrete/ChatSwarmAgent.py

```diff
@@ -1,32 +1,21 @@
-from typing import Any, Optional, List, Union, Dict
-from ....core.models.IModel import IModel
-from ....core.toolkits.IToolkit import IToolkit
-from ....core.parsers.IParser import IParser
-from ....core.conversations.IConversation import IConversation
-from ....core.documents.IDocument import IDocument
-from ....core.retrievers.IRetriever import IRetriever
-from ....core.messages import IMessage
+from typing import Any, Optional, Union, Dict
+from swarmauri.core.models.IModel import IModel
+from swarmauri.core.messages import IMessage
+from swarmauri.core.conversations import IConversation
+from swarmauri.standard.agents.base.ConversationAgentBase import ConversationAgentBase
+from swarmauri.standard.messages.concrete import HumanMessage, AgentMessage
 
-from ..base.SwarmAgentBase import SwarmAgentBase
-from ...messages.concrete import HumanMessage, AgentMessage
-
-class ChatSwarmAgent(SwarmAgentBase):
-    def __init__(self, 
-                 model: IModel, 
-                 conversation: Optional[IConversation] = None, 
-                 toolkit: Optional[IToolkit] = None, 
-                 parser: Optional[IParser] = None,
-                 documents: Optional[List[IDocument]] = None, 
-                 retriever: Optional[IRetriever] = None):
-        super().__init__(model, conversation, toolkit, parser, documents, retriever)
+class ChatSwarmAgent(ConversationAgentBase):
+    def __init__(self, model: IModel, conversation: IConversation):
+        super().__init__(model, conversation)
 
     def exec(self, input_data: Union[str, IMessage], model_kwargs: Optional[Dict] = {}) -> Any:
-        conversation = self.get_conversation()
-        model = self.get_model()
+        conversation = self.conversation
+        model = self.model
 
         # Check if the input is a string, then wrap it in a HumanMessage
         if isinstance(input_data, str):
             human_message = HumanMessage(input_data)
         elif isinstance(input_data, IMessage):
             human_message = input_data
         else:
```

## swarmauri/standard/agents/concrete/MultiPartyChatSwarmAgent.py

```diff
@@ -1,34 +1,28 @@
-from typing import Any, Optional, List, Union, Dict
-from ....core.models.IModel import IModel
-from ....core.toolkits.IToolkit import IToolkit
-from ....core.parsers.IParser import IParser
-from ....standard.conversations.concrete.SharedConversation import SharedConversation
-from ....core.documents.IDocument import IDocument
-from ....core.retrievers.IRetriever import IRetriever
-from ....core.messages import IMessage
+from typing import Any, Optional, Union, Dict
 
-from ..base.SwarmAgentBase import SwarmAgentBase
-from ...messages.concrete import HumanMessage, AgentMessage
+from swarmauri.core.models.IModel import IModel
+from swarmauri.core.messages import IMessage
 
-class MultiPartyChatSwarmAgent(SwarmAgentBase):
+from swarmauri.standard.agents.base.ConversationAgentBase import ConversationAgentBase
+from swarmauri.standard.agents.base.NamedAgentBase import NamedAgentBase
+from swarmauri.standard.conversations.concrete.SharedConversation import SharedConversation
+from swarmauri.standard.messages.concrete import HumanMessage, AgentMessage
+
+class MultiPartyChatSwarmAgent(ConversationAgentBase, NamedAgentBase):
     def __init__(self, 
                  model: IModel, 
-                 conversation: Optional[SharedConversation] = None, 
-                 toolkit: Optional[IToolkit] = None, 
-                 parser: Optional[IParser] = None,
-                 documents: Optional[List[IDocument]] = None, 
-                 retriever: Optional[IRetriever] = None,
-                 name: str = None):
-        super().__init__(model, conversation, toolkit, parser, documents, retriever)
-        self.name = name
+                 conversation: SharedConversation,
+                 name: str):
+        ConversationAgentBase.__init__(self, model, conversation)
+        NamedAgentBase.__init__(self, name)
 
     def exec(self, input_data: Union[str, IMessage] = "", model_kwargs: Optional[Dict] = {}) -> Any:
-        conversation = self.get_conversation()
-        model = self.get_model()
+        conversation = self.conversation
+        model = self.model
 
         # Check if the input is a string, then wrap it in a HumanMessage
         if isinstance(input_data, str):
             human_message = HumanMessage(input_data)
         elif isinstance(input_data, IMessage):
             human_message = input_data
         else:
```

## swarmauri/standard/agents/concrete/MultiPartyToolAgent.py

```diff
@@ -1,38 +1,33 @@
-from typing import Any, Optional, List, Union, Dict
+from typing import Any, Optional, Union, Dict
 import json
 
-from ....core.models.IModel import IModel
-from ....core.toolkits.IToolkit import IToolkit
-from ....core.parsers.IParser import IParser
-from ....core.conversations.IConversation import IConversation
-from ....core.documents.IDocument import IDocument
-from ....core.retrievers.IRetriever import IRetriever
-from ....core.messages import IMessage
+from swarmauri.core.models.IModel import IModel
+from swarmauri.core.toolkits.IToolkit import IToolkit
+from swarmauri.core.conversations.IConversation import IConversation
+from swarmauri.core.messages import IMessage
 
-from ..base.SwarmAgentBase import SwarmAgentBase
-from ...messages.concrete import HumanMessage, AgentMessage, FunctionMessage
+from swarmauri.standard.agents.base.ToolAgentBase import ToolAgentBase
+from swarmauri.standard.agents.base.NamedAgentBase import NamedAgentBase
+from swarmauri.standard.messages.concrete import HumanMessage, AgentMessage, FunctionMessage
 
 
-class MultiPartyToolAgent(SwarmAgentBase):
+class MultiPartyToolAgent(ToolAgentBase, NamedAgentBase):
     def __init__(self, 
                  model: IModel, 
-                 conversation: Optional[IConversation] = None, 
-                 toolkit: Optional[IToolkit] = None, 
-                 parser: Optional[IParser] = None,
-                 documents: Optional[List[IDocument]] = None, 
-                 retriever: Optional[IDocument] = None,
-                 name: str = None):
-        super().__init__(model, conversation, toolkit, parser, documents, retriever)
-        self.name = name
+                 conversation: IConversation, 
+                 toolkit: IToolkit,
+                 name: str):
+        ToolAgentBase.__init__(self, model, conversation, toolkit)
+        NamedAgentBase.__init__(self, name)
 
     def exec(self, input_data: Union[str, IMessage], model_kwargs: Optional[Dict] = {}) -> Any:
-        conversation = self.get_conversation()
-        model = self.get_model()
-        tools = self.get_toolkit()
+        conversation = self.conversation
+        model = self.model
+        toolkit = self.toolkit
         
 
         # Check if the input is a string, then wrap it in a HumanMessage
         if isinstance(input_data, str):
             human_message = HumanMessage(input_data)
         elif isinstance(input_data, IMessage):
             human_message = input_data
@@ -46,15 +41,15 @@
         
         # Retrieve the conversation history and predict a response
         messages = conversation.as_dict()
         
 
         if model_kwargs:
             prediction = model.predict(messages=messages, 
-                                   tools=tools.tools, 
+                                   tools=toolkit.tools, 
                                    tool_choice="auto",
                                    **model_kwargs)
         else:
             prediction = model.predict(messages=messages)
         
         
         prediction_message = prediction.choices[0].message
@@ -66,27 +61,27 @@
         
         tool_calls = prediction.choices[0].message.tool_calls
         if tool_calls:
         
             for tool_call in tool_calls:
                 func_name = tool_call.function.name
                 
-                func_call = self.toolkit.get_tool_by_name(func_name)
+                func_call = toolkit.get_tool_by_name(func_name)
                 func_args = json.loads(tool_call.function.arguments)
                 func_result = func_call(**func_args)
                 
                 func_message = FunctionMessage(func_result, 
                                                name=func_name, 
                                                tool_call_id=tool_call.id)
                 conversation.add_message(func_message, sender_id=self.name)
             
             
             messages = conversation.as_dict()
             rag_prediction = model.predict(messages=messages, 
-                                           tools=tools.tools, 
+                                           tools=toolkit.tools, 
                                            tool_choice="none")
             
             prediction_message = rag_prediction.choices[0].message
             
             agent_response = prediction_message.content
             if agent_response != "":
                 agent_message = AgentMessage(agent_response)
```

## swarmauri/standard/agents/concrete/SimpleSwarmAgent.py

```diff
@@ -1,32 +1,24 @@
-from typing import Any, Optional, List
+from typing import Any, Optional
 
-from ....core.models.IModel import IModel
-from ....core.toolkits.IToolkit import IToolkit
-from ....core.parsers.IParser import IParser
-from ....core.conversations.IConversation import IConversation
-from ....core.documents.IDocument import IDocument
-from ....core.retrievers.IRetriever import IRetriever
-from ....core.messages import IMessage
+from swarmauri.core.models.IModel import IModel
+from swarmauri.core.conversations.IConversation import IConversation
 
-from ..base.SwarmAgentBase import SwarmAgentBase
-from ...messages.concrete import HumanMessage
 
-class SimpleSwarmAgent(SwarmAgentBase):
+from swarmauri.standard.agents.base.SwarmAgentBase import AgentBase
+from swarmauri.standard.messages.concrete import HumanMessage
+
+class SimpleSwarmAgent(AgentBase):
     def __init__(self, model: IModel, 
-                 conversation: Optional[IConversation] = None, 
-                 toolkit: Optional[IToolkit] = None, 
-                 parser: Optional[IParser] = None, 
-                 documents: Optional[List[IDocument]] = None, 
-                 retriever: Optional[IRetriever] = None):
-        super().__init__(model, conversation, toolkit, parser, documents, retriever)
+                 conversation: IConversation):
+        super().__init__(model, conversation)
 
     def exec(self, input_str: Optional[str] = None) -> Any:
-        conversation = self.get_conversation()
-        model = self.get_model()
+        conversation = self.conversation
+        model = self.model
 
         # Construct a new human message (for example purposes)
         if input_str:
             human_message = HumanMessage(input_str)
             conversation.add_message(human_message)
         
         messages = conversation.as_dict()
```

## swarmauri/standard/agents/concrete/SingleCommandAgent.py

```diff
@@ -1,27 +1,17 @@
-from typing import Any, Optional, List
+from typing import Any, Optional
 
-from ....core.models.IModel import IModel
-from ....core.toolkits.IToolkit import IToolkit
-from ....core.parsers.IParser import IParser
-from ....core.conversations.IConversation import IConversation
-from ....core.documents.IDocument import IDocument
-from ....core.retrievers.IRetriever import IRetriever
-from ....core.messages import IMessage
+from swarmauri.core.models.IModel import IModel
+from swarmauri.core.conversations.IConversation import IConversation
 
-from ..base.SwarmAgentBase import SwarmAgentBase
-from ...messages.concrete import HumanMessage
+from swarmauri.standard.agents.base.AgentBase import AgentBase
 
-class SingleCommandAgent(SwarmAgentBase):
+class SingleCommandAgent(AgentBase):
     def __init__(self, model: IModel, 
-                 conversation: Optional[IConversation] = None, 
-                 toolkit: Optional[IToolkit] = None, 
-                 parser: Optional[IParser] = None,
-                 documents: Optional[List[IDocument]] = None, 
-                 retriever: Optional[IRetriever] = None):
-        super().__init__(model, conversation, toolkit, parser, documents, retriever)
+                 conversation: IConversation):
+        super().__init__(model, conversation)
 
     def exec(self, input_str: Optional[str] = None) -> Any:
-        model = self.get_model()
+        model = self.model
         prediction = model.predict(input_str)
         
         return prediction
```

## swarmauri/standard/agents/concrete/ToolAgent.py

```diff
@@ -1,36 +1,30 @@
-from typing import Any, Optional, List, Union, Dict
+from typing import Any, Optional, Union, Dict
 import json
 
-from ....core.models.IModel import IModel
-from ....core.toolkits.IToolkit import IToolkit
-from ....core.parsers.IParser import IParser
-from ....core.conversations.IConversation import IConversation
-from ....core.documents.IDocument import IDocument
-from ....core.retrievers.IRetriever import IRetriever
-from ....core.messages import IMessage
+from swarmauri.core.models.IModel import IModel
+from swarmauri.core.toolkits.IToolkit import IToolkit
+from swarmauri.core.conversations.IConversation import IConversation
+from swarmauri.core.messages import IMessage
 
-from ..base.SwarmAgentBase import SwarmAgentBase
-from ...messages.concrete import HumanMessage, AgentMessage, FunctionMessage
+from swarmauri.standard.agents.base.ToolAgentBase import ToolAgentBase
+from swarmauri.standard.messages.concrete import HumanMessage, AgentMessage, FunctionMessage
 
 
-class ToolAgent(SwarmAgentBase):
+class ToolAgent(ToolAgentBase):
     def __init__(self, 
                  model: IModel, 
-                 conversation: Optional[IConversation] = None, 
-                 toolkit: Optional[IToolkit] = None, 
-                 parser: Optional[IParser] = None,
-                 documents: Optional[List[IDocument]] = None, 
-                 retriever: Optional[IDocument] = None):
-        super().__init__(model, conversation, toolkit, parser, documents, retriever)
+                 conversation: IConversation, 
+                 toolkit: IToolkit):
+        super().__init__(model, conversation, toolkit)
 
     def exec(self, input_data: Union[str, IMessage],  model_kwargs: Optional[Dict] = {}) -> Any:
-        conversation = self.get_conversation()
-        model = self.get_model()
-        tools = self.get_toolkit()
+        conversation = self.conversation
+        model = self.model
+        toolkit = self.toolkit
         
 
         # Check if the input is a string, then wrap it in a HumanMessage
         if isinstance(input_data, str):
             human_message = HumanMessage(input_data)
         elif isinstance(input_data, IMessage):
             human_message = input_data
@@ -42,15 +36,15 @@
 
             
         
         # Retrieve the conversation history and predict a response
         messages = conversation.as_dict()
         
         prediction = model.predict(messages=messages, 
-                                   tools=tools.tools, 
+                                   tools=toolkit.tools, 
                                    tool_choice="auto", 
                                    **model_kwargs)
         
         prediction_message = prediction.choices[0].message
         
         agent_response = prediction_message.content
         
@@ -60,27 +54,27 @@
         
         tool_calls = prediction.choices[0].message.tool_calls
         if tool_calls:
         
             for tool_call in tool_calls:
                 func_name = tool_call.function.name
                 
-                func_call = self.toolkit.get_tool_by_name(func_name)
+                func_call = toolkit.get_tool_by_name(func_name)
                 func_args = json.loads(tool_call.function.arguments)
                 func_result = func_call(**func_args)
                 
                 func_message = FunctionMessage(func_result, 
                                                name=func_name, 
                                                tool_call_id=tool_call.id)
                 conversation.add_message(func_message)
             
             
             messages = conversation.as_dict()
             rag_prediction = model.predict(messages=messages, 
-                                           tools=tools.tools, 
+                                           tools=toolkit.tools, 
                                            tool_choice="none",
                                            **model_kwargs)
             
             prediction_message = rag_prediction.choices[0].message
             
             agent_response = prediction_message.content
             agent_message = AgentMessage(agent_response)
```

## Comparing `swarmauri/standard/chains/concrete/TypeAgnosticCallableChain.py` & `swarmauri/experimental/chains/TypeAgnosticCallableChain.py`

 * *Files identical despite different names*

## Comparing `swarmauri-0.1.8.dist-info/METADATA` & `swarmauri-0.1.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarmauri
-Version: 0.1.8
+Version: 0.1.9
 Summary: A short description of your package
 Home-page: http://github.com/yourusername/your_package_name
 Author: Jacob Stewart
 Author-email: your_email@example.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

## Comparing `swarmauri-0.1.8.dist-info/RECORD` & `swarmauri-0.1.9.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-swarmauri/__init__.py,sha256=1CUarGSwycOh0GKIcMutmmKE9j9E4B6-Jji1lJFY5Aw,21
+swarmauri/__init__.py,sha256=248SFgOW8tTzDpyY6euJ1BwIHMa4uimdKSyc2FGEEZE,21
 swarmauri/community/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 swarmauri/community/document_stores/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 swarmauri/community/document_stores/base/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 swarmauri/community/document_stores/concrete/RedisDocumentStore.py,sha256=TnV2q6QZ-mrDnN5viHGlKODvb0mRsfHucCPzGmBrJYE,2873
 swarmauri/community/document_stores/concrete/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 swarmauri/community/retrievers/__init__.py,sha256=M9j1NuexsmXRO0O_LLRNrLF7fEfPAHWIxm90hC6gV3I,27
 swarmauri/community/retrievers/base/__init__.py,sha256=M9j1NuexsmXRO0O_LLRNrLF7fEfPAHWIxm90hC6gV3I,27
@@ -18,17 +18,25 @@
 swarmauri/community/tools/concrete/SentimentAnalysisTool.py,sha256=bvqLC0e-5gIV1Y5a6Gk3R3bsq620WW2v5XVG7Xm3XlI,888
 swarmauri/community/tools/concrete/WebScrapingTool.py,sha256=FHGEqvG-g3jMVD2X4ALvOjOwuo6pN-BuiyQCV1T2yVw,2098
 swarmauri/community/tools/concrete/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 swarmauri/core/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 swarmauri/core/agent_apis/IAgentCommands.py,sha256=6G-IQ2lih7OUA2bKWBYgY_xYhH0_E_n4xHRbYjoyq44,2067
 swarmauri/core/agent_apis/IAgentRouterCRUD.py,sha256=Sf3YqEtDHcCLSeh00M0oJbFH2xOwIz9EOG-uabJw9Og,1786
 swarmauri/core/agent_apis/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-swarmauri/core/agents/ISwarmAgent.py,sha256=wphsIF53pBiVnVSvgGHAR69wvJToF2q6nIPdZW_Yo3M,1869
+swarmauri/core/agents/IAgentConversation.py,sha256=7X0t0u74PM3VTW-rARNZysWVvUpcC5WApNmIaxeHr8c,477
+swarmauri/core/agents/IAgentDocument.py,sha256=ASOJHmXRaptiVeXLOiTigqUz13kWLIX2ei5aVxnyilI,317
+swarmauri/core/agents/IAgentName.py,sha256=rHgARhLUWqXSERbeuJ28JR3ldgAFt4QexluUn6he-sY,355
+swarmauri/core/agents/IAgentParser.py,sha256=qJnG4dUG87sfid9OGLJtFu8asgeAowwAxusPRprZoa4,303
+swarmauri/core/agents/IAgentRetriever.py,sha256=fCbiRI7hB8P5U6j4bCL4tav7b1WsVjB1rKeOcyY182M,327
+swarmauri/core/agents/IAgentToolkit.py,sha256=KKHTwj4OBneVprCvUmAyo-o-5YBLiIIXPBI3ms8sNTs,317
+swarmauri/core/agents/ISwarmAgent.py,sha256=LN9uS3YSeoPI42HljRJm3T_ZCowXvrrkRFeTSOoL0zY,638
 swarmauri/core/agents/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 swarmauri/core/chains/ICallableChain.py,sha256=E_Yz4UjhuyepQ5cG_ApXi3tPXcRra8siKrXmUIdT4Hg,511
+swarmauri/core/chains/IChain.py,sha256=LixpmvWacgYHWv4j7uRtCPYyPeqzv9qhib_Ak6xbn6s,1228
+swarmauri/core/chains/IChainStep.py,sha256=8bIzAZaHU_xn8Jcx1KnuAOK7N-Q8aBKfAz_YUkb2f_g,960
 swarmauri/core/chains/__init__.py,sha256=2VUTSB4i5lyvBGtidOAzfRN-fNeqIVDTax916aY7CuY,63
 swarmauri/core/chunkers/IChunker.py,sha256=Fd0_uBEY8xPGTSTM_CSqi3Bk5KctC2PwYcMGhb-jH6Y,1134
 swarmauri/core/chunkers/__init__.py,sha256=duO2de8fQ-apsK7K-_O23kl1A-MKAeMUth8jGNkaFgk,93
 swarmauri/core/conversations/IConversation.py,sha256=e2pa38RBAI6LcCSOkD4cdENjEb470wPfwOmZUqMYef4,1165
 swarmauri/core/conversations/IMaxSize.py,sha256=qpIAsMVrrPlqNLOm4gZ-OeB6puFORBQS6lzpJc7L8DA,307
 swarmauri/core/conversations/ISystemContext.py,sha256=pM09Q6tQ892DGXeavbSHnlBaYKpfedyO3Nu2NY2Trzg,871
 swarmauri/core/conversations/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -49,14 +57,15 @@
 swarmauri/core/prompts/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 swarmauri/core/retrievers/IRetriever.py,sha256=JvV6mxZkeLGINvQMSFu1FS7S20fW_bguYHkl517AceY,904
 swarmauri/core/retrievers/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 swarmauri/core/swarm_apis/IAgentRegistration.py,sha256=N_hn4gA79HVztqYJr4iuCWSLfdtlg3617ClSjoaoBAo,2306
 swarmauri/core/swarm_apis/ISwarmAPI.py,sha256=wjJXe0XHHUglB5IFnKpG7kS2jj7S9RCmV7YYIWgk_8Q,1140
 swarmauri/core/swarm_apis/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 swarmauri/core/swarms/ISwarm.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+swarmauri/core/swarms/ISwarmComponent.py,sha256=eXRaK1tRV-14IkKOVI0dXZuiNC3NZ8HUjBrNKSsHvhM,331
 swarmauri/core/swarms/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 swarmauri/core/toolkits/IToolkit.py,sha256=eYsLgCNw50-CRMjhcdxwWgquXPz87umr0XQCh9FTIdk,1635
 swarmauri/core/toolkits/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 swarmauri/core/tools/IParameter.py,sha256=tovQX3WTG_UK0bIdQPaEHknepaJuoRkW5u5ewCzbFHw,2042
 swarmauri/core/tools/ITool.py,sha256=ztiJ0fPDgUPu3zQOg3QjkIzDCXRO82X3MNXl8AZ6BpY,516
 swarmauri/core/tools/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 swarmauri/core/tracing/IChainTracer.py,sha256=YXwzj1_00d2-QXL4Hk2UilfBn_p5N1KZ_itR78C0d8o,1058
@@ -87,14 +96,24 @@
 swarmauri/core/vectorizers/IVectorize.py,sha256=_nV2GTeJsxnPXF1h6fvh38oN2VkYJOQzRDqgFQ5nSB4,624
 swarmauri/core/vectorizers/__init__.py,sha256=M0NZuQ7-112l8K2h1eayVvSmvQrufrOcD5AYKgIf_Is,1
 swarmauri/core/vectors/IVector.py,sha256=luyz7XgOEWaZ6fXFopYXnQBN-NIZd3U2q-sHWQntoKA,578
 swarmauri/core/vectors/IVectorMeta.py,sha256=XTezOiHe1qtD5bw_2MZ35t8HK7K6e5CfCA6Qq3FU45U,900
 swarmauri/core/vectors/IVectorTransform.py,sha256=uHq2oDqNCeM48Tz5jcWQRsXScQaO_YFDpGpnorKpkZ0,1312
 swarmauri/core/vectors/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 swarmauri/experimental/__init__.py,sha256=M9j1NuexsmXRO0O_LLRNrLF7fEfPAHWIxm90hC6gV3I,27
+swarmauri/experimental/chains/ChainOrderStrategy.py,sha256=GTwzwuLv0tEnHSVo6MiSEPuRsJva8BDjniGIs9IVXMg,628
+swarmauri/experimental/chains/ChainOrderStrategyBase.py,sha256=N7MiXjVmOKaUgQyubH3359sJ5aiXCARh3Fav-w0RKRE,516
+swarmauri/experimental/chains/ChainProcessingStrategy.py,sha256=lOTQZuUGU0x8TUjlcqj3a9dT47jnLkURJP8fEJCw2bw,842
+swarmauri/experimental/chains/ChainProcessingStrategyBase.py,sha256=6OjrtHIQWT2mrdNoh2Vum2XcSYI87kH79F26cEq-t7s,603
+swarmauri/experimental/chains/IChainOrderStrategy.py,sha256=xccq0a1UNDgXDq_expueSJd4XBNYTf8EJGBfa4cKGUY,299
+swarmauri/experimental/chains/IChainProcessingStrategy.py,sha256=F-0P260A0-iADz3w4YqnlHPVfbmpIHeWby2KJNoMnd8,585
+swarmauri/experimental/chains/MatrixOrderStrategy.py,sha256=073NQudWwWgF2ncyCkyW2a359z2BfNuHw2eAm9_7h8k,725
+swarmauri/experimental/chains/MatrixProcessingStrategy.py,sha256=9Eofj2on_9qKEZh2hzU1PhS_g0c5dSL99i1lg7wtsEw,1073
+swarmauri/experimental/chains/TypeAgnosticCallableChain.py,sha256=wRd4WdyPSsZQZFdsafkwzsOxDzu1Ecjg4hnk-pbiHrU,4481
+swarmauri/experimental/chains/__init__.py,sha256=M0NZuQ7-112l8K2h1eayVvSmvQrufrOcD5AYKgIf_Is,1
 swarmauri/experimental/conversations/ConsensusBuildingConversation.py,sha256=-oqhf1NroCKMIUoizzBVqapgO9F2qDcS7vGtG5PaDe4,3471
 swarmauri/experimental/conversations/SemanticConversation.py,sha256=RWcnEImggOl3jDatVnr7AZDiHKNRSFuLlWh1AxfdV-g,2219
 swarmauri/experimental/conversations/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 swarmauri/experimental/models/HierarchicalAttentionModel.py,sha256=2oPh6MPccjSY5gG6eHMdWAuocjVHYQ9f7WaonvOoDIA,3556
 swarmauri/experimental/models/SageMaker.py,sha256=oH4n19dDStuqgsnTeNQY_C7HrpdrCcQ_LDat8rDe9QI,1846
 swarmauri/experimental/models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 swarmauri/experimental/parsers/PDFToTextParser.py,sha256=OMAj2BF0_cjCndZmZxBqzLJXaCvarDzZVHfH7eyfAdk,1508
@@ -119,30 +138,35 @@
 swarmauri/experimental/vector_stores/SSIVSimilarity.py,sha256=_DofUiu6ImT4HYk9Y0YnlJIP79JC8uB9gPgibM03wwQ,2643
 swarmauri/experimental/vector_stores/ScannVectorStore.py,sha256=Ikb0aG6SSZR_Mop4aelMOxwOt3XroLd0NzFmDseJjzg,7058
 swarmauri/experimental/vector_stores/SorensenDiceDistance.py,sha256=QaIS4h3VCFRsX_-tDgsw3Phzs4Sb4792rvkUUkl5MZg,2213
 swarmauri/experimental/vector_stores/SquaredEuclideanDistance.py,sha256=5Y64P1qaJscnWKx0d483pGUoJIhOwq_u5-U51JwcNqU,1989
 swarmauri/experimental/vector_stores/__init__.py,sha256=M9j1NuexsmXRO0O_LLRNrLF7fEfPAHWIxm90hC6gV3I,27
 swarmauri/standard/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 swarmauri/standard/agents/__init__.py,sha256=M9j1NuexsmXRO0O_LLRNrLF7fEfPAHWIxm90hC6gV3I,27
-swarmauri/standard/agents/base/SwarmAgentBase.py,sha256=NWhMnXCICQtI7bFjSh1LV2Lpxxk_XD-ru4jkWQ_zhgw,3398
+swarmauri/standard/agents/base/AgentBase.py,sha256=oOQPOhkFAydwqEptnehSTaWXTpNy6zkgEajcPAqP5GY,1650
+swarmauri/standard/agents/base/ConversationAgentBase.py,sha256=j9OpsqV4tvLSM3ouYnmAoWIF2BMVrQ-5AcwPouVSZSY,913
+swarmauri/standard/agents/base/NamedAgentBase.py,sha256=qyLvF5IIcgrK1SALEj0io9txnTBAWALnrGvrLbI6Z-8,546
+swarmauri/standard/agents/base/ToolAgentBase.py,sha256=QUAUt_urHgU4w_hySsTt35tzJ2rat_YXHnrdKxLDBQs,1061
 swarmauri/standard/agents/base/__init__.py,sha256=M9j1NuexsmXRO0O_LLRNrLF7fEfPAHWIxm90hC6gV3I,27
-swarmauri/standard/agents/concrete/ChatSwarmAgent.py,sha256=CuD7dD38-Ji9f5hjnyvDhDN9KkLDaOWswRH98cbGMQw,2169
-swarmauri/standard/agents/concrete/MultiPartyChatSwarmAgent.py,sha256=QimDlSVqfjf-rUm5rUlheCAE1gT1tamy1wcBC2s_RqQ,2404
-swarmauri/standard/agents/concrete/MultiPartyToolAgent.py,sha256=k-p6gN6ihS2F8OprPDAZQabZIHIL4SEMmDHW-_vyXgI,4086
-swarmauri/standard/agents/concrete/SimpleSwarmAgent.py,sha256=0k7K-35jcnb2CCS4odtf5CqJJALVa2fGdwGyIJmsSNQ,1428
-swarmauri/standard/agents/concrete/SingleCommandAgent.py,sha256=sIjI_qnpDcMCeLmVGwHhmIX60SAEak07lg2LrxMY2xY,1135
-swarmauri/standard/agents/concrete/ToolAgent.py,sha256=7egEMiSnlfHfplv5iYLe5WSMoVoaO0zkYsPloaN5yeI,3804
+swarmauri/standard/agents/concrete/ChatSwarmAgent.py,sha256=41N2s-VnpRX0o_ZAPKr8K0WmaYzQt7ls338QyY90rUo,1688
+swarmauri/standard/agents/concrete/MultiPartyChatSwarmAgent.py,sha256=SOxyxm59ZniP6eU4XNWdIA8g5h7yE1jWhClfQgWM4p8,2101
+swarmauri/standard/agents/concrete/MultiPartyToolAgent.py,sha256=RAgwwWSX_FJ0w5UAVYysLzbSloA1Uu1GXmctatSLZ44,3847
+swarmauri/standard/agents/concrete/SimpleSwarmAgent.py,sha256=aE5fQQNwm8YLPXaUPwr97eqzAcYBYSNczAxDHaScoPg,925
+swarmauri/standard/agents/concrete/SingleCommandAgent.py,sha256=5hHOMnVcvdPFUJbLRlpD0z4ntdRe_Qpt6F5zIVy6ZL8,569
+swarmauri/standard/agents/concrete/ToolAgent.py,sha256=EWwVeYbcvK3KgvcCawOLpwf69f3orvVhsuKR9PQubmE,3451
 swarmauri/standard/agents/concrete/__init__.py,sha256=M9j1NuexsmXRO0O_LLRNrLF7fEfPAHWIxm90hC6gV3I,27
 swarmauri/standard/apis/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 swarmauri/standard/apis/base/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 swarmauri/standard/apis/concrete/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 swarmauri/standard/chains/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+swarmauri/standard/chains/base/ChainBase.py,sha256=oDi-kkYVf1JIy6e0cX7F7rLtOuKJluOEdU-8W2GW4X4,2007
+swarmauri/standard/chains/base/ChainStepBase.py,sha256=PxaI0c8YhEI4bFevXrPBYF8F7dOVN2OMzklcpwTJrkU,1050
 swarmauri/standard/chains/base/__init__.py,sha256=M0NZuQ7-112l8K2h1eayVvSmvQrufrOcD5AYKgIf_Is,1
 swarmauri/standard/chains/concrete/CallableChain.py,sha256=F743Nm4tQW_2A-qKSWHT5VcLF9ZZzxy26hvBiqrrbko,1262
-swarmauri/standard/chains/concrete/TypeAgnosticCallableChain.py,sha256=wRd4WdyPSsZQZFdsafkwzsOxDzu1Ecjg4hnk-pbiHrU,4481
+swarmauri/standard/chains/concrete/Chain.py,sha256=zNm1Sjx41dJoORrdAySyPmD50RprJ59NqBCs4ZCginM,1594
 swarmauri/standard/chains/concrete/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 swarmauri/standard/chunkers/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 swarmauri/standard/chunkers/base/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 swarmauri/standard/chunkers/concrete/DelimiterBasedChunker.py,sha256=NiNMoUxqaBBfUQm93voNhlOmgNy06ZFvbovq3PGDC4Q,1935
 swarmauri/standard/chunkers/concrete/FixedLengthChunker.py,sha256=Pv839vpyA-iabHypzFuazp52An7vjHNK7ux73zSZ2vk,1477
 swarmauri/standard/chunkers/concrete/MdSnippetChunker.py,sha256=qsdPVLgvSXdjNm1qodRI4UfvHfXXQWQ6miqrasWgOMY,2164
 swarmauri/standard/chunkers/concrete/SimpleSentenceChunker.py,sha256=l445gizpV9VO7v2FlZECUlNhAtVLxhjaiRl01i5tO5A,1198
@@ -214,14 +238,15 @@
 swarmauri/standard/retrievers/base/DocumentRetrieverBase.py,sha256=zW6wdCX4SdlBF-pWFbRLCjsv9HGnomJIyuWwXvgQi5I,1525
 swarmauri/standard/retrievers/base/__init__.py,sha256=M9j1NuexsmXRO0O_LLRNrLF7fEfPAHWIxm90hC6gV3I,27
 swarmauri/standard/retrievers/concrete/__init__.py,sha256=M9j1NuexsmXRO0O_LLRNrLF7fEfPAHWIxm90hC6gV3I,27
 swarmauri/standard/states/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 swarmauri/standard/states/base/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 swarmauri/standard/states/concrete/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 swarmauri/standard/swarms/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+swarmauri/standard/swarms/base/SwarmComponentBase.py,sha256=EpjyA9eLJxE6zvvO7ds6nhleKGcGDXUo8qHB2gs5rxA,553
 swarmauri/standard/swarms/base/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 swarmauri/standard/swarms/concrete/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 swarmauri/standard/toolkits/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 swarmauri/standard/toolkits/base/ToolkitBase.py,sha256=FkpjkOnz_hqL7CBIsJ6FyDNiR8b2bQifu4T30TFMMjk,2430
 swarmauri/standard/toolkits/base/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 swarmauri/standard/toolkits/concrete/Toolkit.py,sha256=zsbSSeiTffqe-YBNesouqImGtnFP7vgebjxhIa0YWlU,510
 swarmauri/standard/toolkits/concrete/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -260,11 +285,11 @@
 swarmauri/standard/vectorizers/concrete/TFIDFVectorizer.py,sha256=MiLfu3WeQGL3iTdqwCU-D1lZqRqG7IKgTHRGF2J0lLo,2369
 swarmauri/standard/vectorizers/concrete/__init__.py,sha256=M0NZuQ7-112l8K2h1eayVvSmvQrufrOcD5AYKgIf_Is,1
 swarmauri/standard/vectors/__init__.py,sha256=M9j1NuexsmXRO0O_LLRNrLF7fEfPAHWIxm90hC6gV3I,27
 swarmauri/standard/vectors/base/VectorBase.py,sha256=eByYtB5eulHGHtoUdANqXSPEfuf86ZukQPXnfEZ2_nA,751
 swarmauri/standard/vectors/base/__init__.py,sha256=M9j1NuexsmXRO0O_LLRNrLF7fEfPAHWIxm90hC6gV3I,27
 swarmauri/standard/vectors/concrete/SimpleVector.py,sha256=p3gJ5kCFkJtl_5ekwvdIOUvlq2qboLzxZxFvlCQ-Ick,211
 swarmauri/standard/vectors/concrete/__init__.py,sha256=M9j1NuexsmXRO0O_LLRNrLF7fEfPAHWIxm90hC6gV3I,27
-swarmauri-0.1.8.dist-info/METADATA,sha256=VzkXti8sjuoGaaL_Ph6xD0wMQgPr4uXsUIZ17YjUTVY,3536
-swarmauri-0.1.8.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-swarmauri-0.1.8.dist-info/top_level.txt,sha256=IOPRWqByQ7oueIepbzL8LuDShkB-qYxRAtgHxgvO4ug,10
-swarmauri-0.1.8.dist-info/RECORD,,
+swarmauri-0.1.9.dist-info/METADATA,sha256=eNraFIUivfBA_21qYzisaYicv9VB8rH07xPloUpkND4,3536
+swarmauri-0.1.9.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+swarmauri-0.1.9.dist-info/top_level.txt,sha256=IOPRWqByQ7oueIepbzL8LuDShkB-qYxRAtgHxgvO4ug,10
+swarmauri-0.1.9.dist-info/RECORD,,
```

