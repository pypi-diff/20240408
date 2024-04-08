# Comparing `tmp/continuous_eval-0.3.5.tar.gz` & `tmp/continuous_eval-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "continuous_eval-0.3.5.tar", max compression
+gzip compressed data, was "continuous_eval-0.3.6.tar", max compression
```

## Comparing `continuous_eval-0.3.5.tar` & `continuous_eval-0.3.6.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0    11357 2024-01-17 21:26:45.588731 continuous_eval-0.3.5/LICENSE
--rw-r--r--   0        0        0     9138 2024-03-16 00:25:37.967576 continuous_eval-0.3.5/README.md
--rw-r--r--   0        0        0        0 2024-02-25 04:22:14.516782 continuous_eval-0.3.5/continuous_eval/__init__.py
--rw-r--r--   0        0        0       64 2024-02-17 05:39:52.426571 continuous_eval-0.3.5/continuous_eval/classifiers/__init__.py
--rw-r--r--   0        0        0     3058 2024-03-22 00:37:22.186238 continuous_eval-0.3.5/continuous_eval/classifiers/ensemble.py
--rw-r--r--   0        0        0      652 2024-03-22 00:45:46.211844 continuous_eval-0.3.5/continuous_eval/classifiers/utils.py
--rw-r--r--   0        0        0     3031 2024-02-25 04:22:14.517248 continuous_eval-0.3.5/continuous_eval/data_downloader.py
--rw-r--r--   0        0        0     3609 2024-03-22 00:37:22.186380 continuous_eval-0.3.5/continuous_eval/datatypes.py
--rw-r--r--   0        0        0      251 2024-02-25 04:22:14.517467 continuous_eval-0.3.5/continuous_eval/eval/__init__.py
--rw-r--r--   0        0        0     6328 2024-03-27 05:39:44.569863 continuous_eval-0.3.5/continuous_eval/eval/dataset.py
--rw-r--r--   0        0        0     9394 2024-03-08 08:55:45.667192 continuous_eval-0.3.5/continuous_eval/eval/manager.py
--rw-r--r--   0        0        0     1627 2024-02-28 21:52:45.358114 continuous_eval-0.3.5/continuous_eval/eval/modules.py
--rw-r--r--   0        0        0     4539 2024-02-29 19:22:06.462595 continuous_eval-0.3.5/continuous_eval/eval/pipeline.py
--rw-r--r--   0        0        0     4420 2024-03-22 00:45:46.482746 continuous_eval-0.3.5/continuous_eval/eval/result_types.py
--rw-r--r--   0        0        0     1380 2024-02-25 04:22:14.518180 continuous_eval-0.3.5/continuous_eval/eval/tests.py
--rw-r--r--   0        0        0      122 2024-02-25 04:22:14.518248 continuous_eval-0.3.5/continuous_eval/eval/types.py
--rw-r--r--   0        0        0     1107 2024-02-29 19:29:39.554407 continuous_eval-0.3.5/continuous_eval/eval/utils.py
--rw-r--r--   0        0        0       69 2024-02-17 05:39:52.427862 continuous_eval-0.3.5/continuous_eval/generators/__init__.py
--rw-r--r--   0        0        0    12800 2024-03-16 15:09:59.783830 continuous_eval-0.3.5/continuous_eval/generators/simple.py
--rw-r--r--   0        0        0    10006 2024-03-27 05:39:44.586759 continuous_eval-0.3.5/continuous_eval/llm_factory.py
--rw-r--r--   0        0        0        0 2024-03-27 04:22:00.195998 continuous_eval-0.3.5/continuous_eval/llms/__init__.py
--rw-r--r--   0        0        0      780 2024-03-27 05:39:44.227478 continuous_eval-0.3.5/continuous_eval/llms/bedrock.py
--rw-r--r--   0        0        0       48 2024-02-25 04:22:14.519065 continuous_eval-0.3.5/continuous_eval/metrics/__init__.py
--rw-r--r--   0        0        0     1732 2024-03-27 04:07:30.402986 continuous_eval-0.3.5/continuous_eval/metrics/_utils/simple_tokenizer.py
--rw-r--r--   0        0        0     2471 2024-03-08 08:55:45.593923 continuous_eval-0.3.5/continuous_eval/metrics/base.py
--rw-r--r--   0        0        0       91 2024-02-27 06:09:06.065186 continuous_eval-0.3.5/continuous_eval/metrics/classification/__init__.py
--rw-r--r--   0        0        0     2233 2024-02-27 06:09:06.065562 continuous_eval-0.3.5/continuous_eval/metrics/classification/classification.py
--rw-r--r--   0        0        0      111 2024-03-08 07:02:54.302236 continuous_eval-0.3.5/continuous_eval/metrics/code/python/__init__.py
--rw-r--r--   0        0        0    11635 2024-03-08 08:55:45.681607 continuous_eval-0.3.5/continuous_eval/metrics/code/python/code_deterministic_metrics.py
--rw-r--r--   0        0        0      678 2024-03-17 22:25:39.167477 continuous_eval-0.3.5/continuous_eval/metrics/generation/text/__init__.py
--rw-r--r--   0        0        0     3109 2024-03-16 15:32:17.406679 continuous_eval-0.3.5/continuous_eval/metrics/generation/text/bert.py
--rw-r--r--   0        0        0     2879 2024-03-27 04:56:36.204502 continuous_eval-0.3.5/continuous_eval/metrics/generation/text/custom.py
--rw-r--r--   0        0        0     4814 2024-03-08 08:55:45.614834 continuous_eval-0.3.5/continuous_eval/metrics/generation/text/deterministic.py
--rw-r--r--   0        0        0    11472 2024-03-27 05:39:44.567238 continuous_eval-0.3.5/continuous_eval/metrics/generation/text/llm_based.py
--rw-r--r--   0        0        0     5741 2024-03-17 22:25:39.168561 continuous_eval-0.3.5/continuous_eval/metrics/generation/text/semantic.py
--rw-r--r--   0        0        0     2865 2024-03-27 05:39:44.530970 continuous_eval-0.3.5/continuous_eval/metrics/generation/text/utils.py
--rw-r--r--   0        0        0      437 2024-02-25 04:22:14.520214 continuous_eval-0.3.5/continuous_eval/metrics/retrieval/__init__.py
--rw-r--r--   0        0        0     6541 2024-03-16 15:47:34.553907 continuous_eval-0.3.5/continuous_eval/metrics/retrieval/llm_based.py
--rw-r--r--   0        0        0     1918 2024-02-25 04:22:14.520478 continuous_eval-0.3.5/continuous_eval/metrics/retrieval/matching_strategy.py
--rw-r--r--   0        0        0     2267 2024-02-25 04:22:14.520567 continuous_eval-0.3.5/continuous_eval/metrics/retrieval/precision_recall_f1.py
--rw-r--r--   0        0        0     3397 2024-02-25 04:22:14.520659 continuous_eval-0.3.5/continuous_eval/metrics/retrieval/ranked.py
--rw-r--r--   0        0        0     1500 2024-02-25 04:22:14.520753 continuous_eval-0.3.5/continuous_eval/metrics/tools/match.py
--rw-r--r--   0        0        0     4013 2024-02-26 23:53:19.235416 continuous_eval-0.3.5/continuous_eval/utils/telemetry.py
--rw-r--r--   0        0        0     1832 2024-03-27 05:39:24.553037 continuous_eval-0.3.5/pyproject.toml
--rw-r--r--   0        0        0    11337 1970-01-01 00:00:00.000000 continuous_eval-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-01-17 21:26:45.588731 continuous_eval-0.3.6/LICENSE
+-rw-r--r--   0        0        0     9137 2024-04-02 16:24:12.028523 continuous_eval-0.3.6/README.md
+-rw-r--r--   0        0        0        0 2024-02-25 04:22:14.516782 continuous_eval-0.3.6/continuous_eval/__init__.py
+-rw-r--r--   0        0        0       64 2024-02-17 05:39:52.426571 continuous_eval-0.3.6/continuous_eval/classifiers/__init__.py
+-rw-r--r--   0        0        0     3058 2024-03-22 00:37:22.186238 continuous_eval-0.3.6/continuous_eval/classifiers/ensemble.py
+-rw-r--r--   0        0        0      652 2024-03-22 00:45:46.211844 continuous_eval-0.3.6/continuous_eval/classifiers/utils.py
+-rw-r--r--   0        0        0     3031 2024-02-25 04:22:14.517248 continuous_eval-0.3.6/continuous_eval/data_downloader.py
+-rw-r--r--   0        0        0     3609 2024-03-22 00:37:22.186380 continuous_eval-0.3.6/continuous_eval/datatypes.py
+-rw-r--r--   0        0        0      251 2024-02-25 04:22:14.517467 continuous_eval-0.3.6/continuous_eval/eval/__init__.py
+-rw-r--r--   0        0        0     6234 2024-04-08 17:58:05.099379 continuous_eval-0.3.6/continuous_eval/eval/dataset.py
+-rw-r--r--   0        0        0     9394 2024-03-08 08:55:45.667192 continuous_eval-0.3.6/continuous_eval/eval/manager.py
+-rw-r--r--   0        0        0     1627 2024-02-28 21:52:45.358114 continuous_eval-0.3.6/continuous_eval/eval/modules.py
+-rw-r--r--   0        0        0     4539 2024-02-29 19:22:06.462595 continuous_eval-0.3.6/continuous_eval/eval/pipeline.py
+-rw-r--r--   0        0        0     4420 2024-03-22 00:45:46.482746 continuous_eval-0.3.6/continuous_eval/eval/result_types.py
+-rw-r--r--   0        0        0     1380 2024-02-25 04:22:14.518180 continuous_eval-0.3.6/continuous_eval/eval/tests.py
+-rw-r--r--   0        0        0      122 2024-02-25 04:22:14.518248 continuous_eval-0.3.6/continuous_eval/eval/types.py
+-rw-r--r--   0        0        0     1107 2024-02-29 19:29:39.554407 continuous_eval-0.3.6/continuous_eval/eval/utils.py
+-rw-r--r--   0        0        0       69 2024-02-17 05:39:52.427862 continuous_eval-0.3.6/continuous_eval/generators/__init__.py
+-rw-r--r--   0        0        0    12800 2024-03-16 15:09:59.783830 continuous_eval-0.3.6/continuous_eval/generators/simple.py
+-rw-r--r--   0        0        0    10006 2024-03-27 05:39:44.586759 continuous_eval-0.3.6/continuous_eval/llm_factory.py
+-rw-r--r--   0        0        0        0 2024-03-27 04:22:00.195998 continuous_eval-0.3.6/continuous_eval/llms/__init__.py
+-rw-r--r--   0        0        0      780 2024-03-27 05:39:44.227478 continuous_eval-0.3.6/continuous_eval/llms/bedrock.py
+-rw-r--r--   0        0        0       48 2024-02-25 04:22:14.519065 continuous_eval-0.3.6/continuous_eval/metrics/__init__.py
+-rw-r--r--   0        0        0     1732 2024-03-27 04:07:30.402986 continuous_eval-0.3.6/continuous_eval/metrics/_utils/simple_tokenizer.py
+-rw-r--r--   0        0        0     2471 2024-03-08 08:55:45.593923 continuous_eval-0.3.6/continuous_eval/metrics/base.py
+-rw-r--r--   0        0        0       91 2024-02-27 06:09:06.065186 continuous_eval-0.3.6/continuous_eval/metrics/classification/__init__.py
+-rw-r--r--   0        0        0     2233 2024-02-27 06:09:06.065562 continuous_eval-0.3.6/continuous_eval/metrics/classification/classification.py
+-rw-r--r--   0        0        0      111 2024-03-08 07:02:54.302236 continuous_eval-0.3.6/continuous_eval/metrics/code/python/__init__.py
+-rw-r--r--   0        0        0    11635 2024-03-08 08:55:45.681607 continuous_eval-0.3.6/continuous_eval/metrics/code/python/code_deterministic_metrics.py
+-rw-r--r--   0        0        0      678 2024-03-17 22:25:39.167477 continuous_eval-0.3.6/continuous_eval/metrics/generation/text/__init__.py
+-rw-r--r--   0        0        0     3109 2024-03-16 15:32:17.406679 continuous_eval-0.3.6/continuous_eval/metrics/generation/text/bert.py
+-rw-r--r--   0        0        0     2879 2024-03-27 04:56:36.204502 continuous_eval-0.3.6/continuous_eval/metrics/generation/text/custom.py
+-rw-r--r--   0        0        0     4814 2024-03-08 08:55:45.614834 continuous_eval-0.3.6/continuous_eval/metrics/generation/text/deterministic.py
+-rw-r--r--   0        0        0    11472 2024-03-27 05:39:44.567238 continuous_eval-0.3.6/continuous_eval/metrics/generation/text/llm_based.py
+-rw-r--r--   0        0        0     5741 2024-03-17 22:25:39.168561 continuous_eval-0.3.6/continuous_eval/metrics/generation/text/semantic.py
+-rw-r--r--   0        0        0     2865 2024-03-27 05:39:44.530970 continuous_eval-0.3.6/continuous_eval/metrics/generation/text/utils.py
+-rw-r--r--   0        0        0      437 2024-02-25 04:22:14.520214 continuous_eval-0.3.6/continuous_eval/metrics/retrieval/__init__.py
+-rw-r--r--   0        0        0     6541 2024-04-05 23:59:38.533703 continuous_eval-0.3.6/continuous_eval/metrics/retrieval/llm_based.py
+-rw-r--r--   0        0        0     1918 2024-02-25 04:22:14.520478 continuous_eval-0.3.6/continuous_eval/metrics/retrieval/matching_strategy.py
+-rw-r--r--   0        0        0     2470 2024-04-02 16:24:12.028818 continuous_eval-0.3.6/continuous_eval/metrics/retrieval/precision_recall_f1.py
+-rw-r--r--   0        0        0     3394 2024-04-02 16:24:12.029049 continuous_eval-0.3.6/continuous_eval/metrics/retrieval/ranked.py
+-rw-r--r--   0        0        0     1500 2024-02-25 04:22:14.520753 continuous_eval-0.3.6/continuous_eval/metrics/tools/match.py
+-rw-r--r--   0        0        0     4013 2024-02-26 23:53:19.235416 continuous_eval-0.3.6/continuous_eval/utils/telemetry.py
+-rw-r--r--   0        0        0     1850 2024-04-08 17:57:33.865982 continuous_eval-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0    11375 1970-01-01 00:00:00.000000 continuous_eval-0.3.6/PKG-INFO
```

### Comparing `continuous_eval-0.3.5/LICENSE` & `continuous_eval-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.5/README.md` & `continuous_eval-0.3.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -218,15 +218,15 @@
 
 - `eval_manager.run_metrics()` to run all the metrics defined in the pipeline
 - `eval_manager.run_tests()` to run the tests defined in the pipeline (see the documentation [docs](docs.relari.ai) for more details)
 
 ## Synthetic Data Generation
 
 Ground truth data, or reference data, is important for evaluation as it can offer a comprehensive and consistent measurement of system performance. However, it is often costly and time-consuming to manually curate such a golden dataset.
-We have created a synthetic data pipeline that can custom generate user interaction data for a variety of use cases such as RAG, agents, copilots. They can serve a starting point for a golden dataset for evaluation or for other training purposes. Below is an example for Coding Agents. Try out this demo: [Synthetic Data Demo](https://www.relari.ai/#synthetic_data_demo)
+We have created a synthetic data pipeline that can custom generate user interaction data for a variety of use cases such as RAG, agents, copilots. They can serve a starting point for a golden dataset for evaluation or for other training purposes. Below is an example for Coding Agents. Try out this demo: [Synthetic Data Demo](https://www.relari.ai/synthetic-data-demo)
 
 <h1 align="center">
   <img
     src="docs/public/synthetic-data-demo.png"
   >
 </h1>
```

#### html2text {}

```diff
@@ -83,15 +83,15 @@
 for evaluation as it can offer a comprehensive and consistent measurement of
 system performance. However, it is often costly and time-consuming to manually
 curate such a golden dataset. We have created a synthetic data pipeline that
 can custom generate user interaction data for a variety of use cases such as
 RAG, agents, copilots. They can serve a starting point for a golden dataset for
 evaluation or for other training purposes. Below is an example for Coding
 Agents. Try out this demo: [Synthetic Data Demo](https://www.relari.ai/
-#synthetic_data_demo)
+synthetic-data-demo)
               ************ [[ddooccss//ppuubblliicc//ssyynntthheettiicc--ddaattaa--ddeemmoo..ppnngg]] ************
 ## Resources - **Docs:** [link](https://docs.relari.ai/) - **Examples Repo**:
 [end-to-end example repo](https://github.com/relari-ai/examples) - **Blog
 Posts:** - Practical Guide to RAG Pipeline Evaluation: [Part 1: Retrieval]
 (https://medium.com/relari/a-practical-guide-to-rag-pipeline-evaluation-part-1-
 27a472b09893), [Part 2: Generation](https://medium.com/relari/a-practical-
 guide-to-rag-evaluation-part-2-generation-c79b1bde0f5d) - How important is a
```

### Comparing `continuous_eval-0.3.5/continuous_eval/classifiers/ensemble.py` & `continuous_eval-0.3.6/continuous_eval/classifiers/ensemble.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.5/continuous_eval/classifiers/utils.py` & `continuous_eval-0.3.6/continuous_eval/classifiers/utils.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.5/continuous_eval/data_downloader.py` & `continuous_eval-0.3.6/continuous_eval/data_downloader.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.5/continuous_eval/datatypes.py` & `continuous_eval-0.3.6/continuous_eval/datatypes.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.5/continuous_eval/eval/dataset.py` & `continuous_eval-0.3.6/continuous_eval/eval/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import json
 import typing
-import warnings
 from dataclasses import dataclass
 from pathlib import Path
 
 import yaml
 
 from continuous_eval.eval.types import UUID, ToolCall
 from continuous_eval.eval.utils import type_hint_to_str
@@ -13,16 +12,16 @@
 _SAFE_DICT["UUID"] = UUID
 _SAFE_DICT["ToolCall"] = ToolCall
 
 
 @dataclass(frozen=True)
 class DatasetField:
     name: str
-    type: type
-    description: str
+    type: type = typing.Any  # type: ignore
+    description: str = ""
     is_ground_truth: bool = False
 
     def to_dict(self):
         return {
             "type": type_hint_to_str(self.type),
             "description": self.description,
             "ground_truth": self.is_ground_truth,
@@ -90,15 +89,14 @@
         if save_manifest:
             manifest_path = file_path.parent / "manifest.yaml"
             with open(manifest_path, "w") as manifest_file:
                 manifest_file.write(yaml.dump(self._manifest.to_yaml()))
 
     def _load_or_infer_manifest(self, manifest_path: typing.Optional[Path]) -> DatasetManifest:
         if manifest_path is None or not manifest_path.exists():
-            warnings.warn(f"Manifest file not found in {manifest_path}, it is suggested to define a manifest.")
             return self._infer_manifest()
         else:
             with open(manifest_path, "r") as manifest_file:
                 manifest = yaml.safe_load(manifest_file)
                 fields = {
                     field_name: DatasetField(
                         name=field_name,
```

### Comparing `continuous_eval-0.3.5/continuous_eval/eval/manager.py` & `continuous_eval-0.3.6/continuous_eval/eval/manager.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.5/continuous_eval/eval/modules.py` & `continuous_eval-0.3.6/continuous_eval/eval/modules.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.5/continuous_eval/eval/pipeline.py` & `continuous_eval-0.3.6/continuous_eval/eval/pipeline.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.5/continuous_eval/eval/result_types.py` & `continuous_eval-0.3.6/continuous_eval/eval/result_types.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.5/continuous_eval/eval/tests.py` & `continuous_eval-0.3.6/continuous_eval/eval/tests.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.5/continuous_eval/eval/utils.py` & `continuous_eval-0.3.6/continuous_eval/eval/utils.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.5/continuous_eval/generators/simple.py` & `continuous_eval-0.3.6/continuous_eval/generators/simple.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.5/continuous_eval/llm_factory.py` & `continuous_eval-0.3.6/continuous_eval/llm_factory.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.5/continuous_eval/llms/bedrock.py` & `continuous_eval-0.3.6/continuous_eval/llms/bedrock.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.5/continuous_eval/metrics/_utils/simple_tokenizer.py` & `continuous_eval-0.3.6/continuous_eval/metrics/_utils/simple_tokenizer.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.5/continuous_eval/metrics/base.py` & `continuous_eval-0.3.6/continuous_eval/metrics/base.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.5/continuous_eval/metrics/classification/classification.py` & `continuous_eval-0.3.6/continuous_eval/metrics/classification/classification.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.5/continuous_eval/metrics/code/python/code_deterministic_metrics.py` & `continuous_eval-0.3.6/continuous_eval/metrics/code/python/code_deterministic_metrics.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.5/continuous_eval/metrics/generation/text/__init__.py` & `continuous_eval-0.3.6/continuous_eval/metrics/generation/text/__init__.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.5/continuous_eval/metrics/generation/text/bert.py` & `continuous_eval-0.3.6/continuous_eval/metrics/generation/text/bert.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.5/continuous_eval/metrics/generation/text/custom.py` & `continuous_eval-0.3.6/continuous_eval/metrics/generation/text/custom.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.5/continuous_eval/metrics/generation/text/deterministic.py` & `continuous_eval-0.3.6/continuous_eval/metrics/generation/text/deterministic.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.5/continuous_eval/metrics/generation/text/llm_based.py` & `continuous_eval-0.3.6/continuous_eval/metrics/generation/text/llm_based.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.5/continuous_eval/metrics/generation/text/semantic.py` & `continuous_eval-0.3.6/continuous_eval/metrics/generation/text/semantic.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.5/continuous_eval/metrics/generation/text/utils.py` & `continuous_eval-0.3.6/continuous_eval/metrics/generation/text/utils.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.5/continuous_eval/metrics/retrieval/llm_based.py` & `continuous_eval-0.3.6/continuous_eval/metrics/retrieval/llm_based.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.5/continuous_eval/metrics/retrieval/matching_strategy.py` & `continuous_eval-0.3.6/continuous_eval/metrics/retrieval/matching_strategy.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.5/continuous_eval/metrics/retrieval/precision_recall_f1.py` & `continuous_eval-0.3.6/continuous_eval/metrics/retrieval/precision_recall_f1.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,20 +26,23 @@
             gt_components = ground_truth_context
         elif self.matching_strategy.type == MatchingStrategyType.SENTENCE_MATCH:
             ret_components = [sentence for chunk in retrieved_context for sentence in sent_tokenize(chunk)]
             gt_components = [sentence for chunk in ground_truth_context for sentence in sent_tokenize(chunk)]
 
         relevant_ret_components = 0
         hit_gt_components = set()
+        gt_components = set(gt_components)  # remove duplicates in ground truth context if any
         for ret_component in ret_components:
+            ret_component_matched = False
             for gt_component in gt_components:
                 if self.matching_strategy.is_relevant(ret_component, gt_component):
-                    relevant_ret_components += 1
+                    ret_component_matched = True
                     hit_gt_components.add(gt_component)
                     continue
+            relevant_ret_components += int(ret_component_matched)
         precision = relevant_ret_components / len(ret_components) if ret_components else 0.0
         recall = len(hit_gt_components) / len(gt_components) if gt_components else 0.0
 
         try:
             f1 = 2 * (precision * recall) / (precision + recall)
         except ZeroDivisionError:
             f1 = 0.0
```

### Comparing `continuous_eval-0.3.5/continuous_eval/metrics/retrieval/ranked.py` & `continuous_eval-0.3.6/continuous_eval/metrics/retrieval/ranked.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         relevant_chunks = 0
 
         for i, chunk in enumerate(retrieved_context):
             for ground_truth_chunk in ground_truth_context:
                 if self.matching_strategy.is_relevant(chunk, ground_truth_chunk):
                     relevant_chunks += 1
                     average_precision += relevant_chunks / (i + 1)
-                    continue
+                    break
 
         return average_precision / relevant_chunks if relevant_chunks else 0
 
     def calculate_reciprocal_rank(self, retrieved_context, ground_truth_context):
         # Calculate reciprocal rank for a single query retrieval
 
         # Calculate reciprocal rank for each relevant chunk
```

### Comparing `continuous_eval-0.3.5/continuous_eval/metrics/tools/match.py` & `continuous_eval-0.3.6/continuous_eval/metrics/tools/match.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.5/continuous_eval/utils/telemetry.py` & `continuous_eval-0.3.6/continuous_eval/utils/telemetry.py`

 * *Files identical despite different names*

### Comparing `continuous_eval-0.3.5/pyproject.toml` & `continuous_eval-0.3.6/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "continuous-eval"
-version = "0.3.5"
+version = "0.3.6"
 description = "Open-Source Evaluation for GenAI Application Pipelines."
 authors = ["Yi Zhang <yi@relari.ai>", "Pasquale Antonante <pasquale@relari.ai>"]
 readme = "README.md"
 license = "Apache-2.0"
 packages = [{include = "continuous_eval"}]
 
 [tool.poetry.dependencies]
@@ -17,29 +17,30 @@
 sentence-transformers = {version = "^2.2.2", optional = true}
 torch = {version = "^2.1.1", optional = true}
 anthropic = {version = "^0.7.7", optional = true}
 google-generativeai = {version = "^0.3.1", optional = true}
 mapie = "^0.7.0"
 imbalanced-learn = "^0.11.0"
 pandas = "^2.1.4"
-protobuf = "^4.25.1"
+protobuf = "^4.23.4"
 tqdm = "^4.66.1"
 requests = "^2.31.0"
 pinecone-client = {version = "^2.2.4", optional = true}
 chromadb = {version = "^0.4.21", optional = true}
 tiktoken = {version = "^0.5.2", optional = true}
 unstructured = {version = "^0.11.6", optional = true}
 appdirs = "^1.4.4"
 munkres = "^1.1.4"
 thefuzz = "^0.22.1"
 sentencepiece = "^0.2.0"
 cohere = {version = "^4.54", optional = true}
 tenacity = "^8.2.3"
 boto3 = {version = "^1.34.70", optional = true}
 langchain-community = {version = "^0.0.29", optional = true}
+pyyaml = "^6.0.1"
 
 [tool.poetry.extras]
 langchain = ["langchain-community"]
 semantic = ["transformers", "sentence-transformers", "torch"]
 anthropic = ["anthropic"]
 bedrock = ["boto3"]
 gemini = ["google-generativeai"]
```

### Comparing `continuous_eval-0.3.5/PKG-INFO` & `continuous_eval-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: continuous-eval
-Version: 0.3.5
+Version: 0.3.6
 Summary: Open-Source Evaluation for GenAI Application Pipelines.
 License: Apache-2.0
 Author: Yi Zhang
 Author-email: yi@relari.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -29,16 +29,17 @@
 Requires-Dist: langchain-community (>=0.0.29,<0.0.30) ; extra == "langchain" or extra == "generators"
 Requires-Dist: mapie (>=0.7.0,<0.8.0)
 Requires-Dist: munkres (>=1.1.4,<2.0.0)
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Requires-Dist: openai (>=1.3.7,<2.0.0)
 Requires-Dist: pandas (>=2.1.4,<3.0.0)
 Requires-Dist: pinecone-client (>=2.2.4,<3.0.0) ; extra == "generators"
-Requires-Dist: protobuf (>=4.25.1,<5.0.0)
+Requires-Dist: protobuf (>=4.23.4,<5.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
+Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: rouge (>=1.0.1,<2.0.0)
 Requires-Dist: sentence-transformers (>=2.2.2,<3.0.0) ; extra == "semantic"
 Requires-Dist: sentencepiece (>=0.2.0,<0.3.0)
 Requires-Dist: tenacity (>=8.2.3,<9.0.0)
 Requires-Dist: thefuzz (>=0.22.1,<0.23.0)
 Requires-Dist: tiktoken (>=0.5.2,<0.6.0) ; extra == "generators"
@@ -268,15 +269,15 @@
 
 - `eval_manager.run_metrics()` to run all the metrics defined in the pipeline
 - `eval_manager.run_tests()` to run the tests defined in the pipeline (see the documentation [docs](docs.relari.ai) for more details)
 
 ## Synthetic Data Generation
 
 Ground truth data, or reference data, is important for evaluation as it can offer a comprehensive and consistent measurement of system performance. However, it is often costly and time-consuming to manually curate such a golden dataset.
-We have created a synthetic data pipeline that can custom generate user interaction data for a variety of use cases such as RAG, agents, copilots. They can serve a starting point for a golden dataset for evaluation or for other training purposes. Below is an example for Coding Agents. Try out this demo: [Synthetic Data Demo](https://www.relari.ai/#synthetic_data_demo)
+We have created a synthetic data pipeline that can custom generate user interaction data for a variety of use cases such as RAG, agents, copilots. They can serve a starting point for a golden dataset for evaluation or for other training purposes. Below is an example for Coding Agents. Try out this demo: [Synthetic Data Demo](https://www.relari.ai/synthetic-data-demo)
 
 <h1 align="center">
   <img
     src="docs/public/synthetic-data-demo.png"
   >
 </h1>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: continuous-eval Version: 0.3.5 Summary: Open-Source
+Metadata-Version: 2.1 Name: continuous-eval Version: 0.3.6 Summary: Open-Source
 Evaluation for GenAI Application Pipelines. License: Apache-2.0 Author: Yi
 Zhang Author-email: yi@relari.ai Requires-Python: >=3.9,<4.0 Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: anthropic Provides-Extra: bedrock Provides-Extra: cohere
@@ -14,24 +14,25 @@
 extra == "cohere" Requires-Dist: google-generativeai (>=0.3.1,<0.4.0) ; extra
 == "gemini" Requires-Dist: imbalanced-learn (>=0.11.0,<0.12.0) Requires-Dist:
 langchain-community (>=0.0.29,<0.0.30) ; extra == "langchain" or extra ==
 "generators" Requires-Dist: mapie (>=0.7.0,<0.8.0) Requires-Dist: munkres
 (>=1.1.4,<2.0.0) Requires-Dist: nltk (>=3.8.1,<4.0.0) Requires-Dist: openai
 (>=1.3.7,<2.0.0) Requires-Dist: pandas (>=2.1.4,<3.0.0) Requires-Dist:
 pinecone-client (>=2.2.4,<3.0.0) ; extra == "generators" Requires-Dist:
-protobuf (>=4.25.1,<5.0.0) Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0) Requires-Dist: rouge (>=1.0.1,<2.0.0)
-Requires-Dist: sentence-transformers (>=2.2.2,<3.0.0) ; extra == "semantic"
-Requires-Dist: sentencepiece (>=0.2.0,<0.3.0) Requires-Dist: tenacity
-(>=8.2.3,<9.0.0) Requires-Dist: thefuzz (>=0.22.1,<0.23.0) Requires-Dist:
-tiktoken (>=0.5.2,<0.6.0) ; extra == "generators" Requires-Dist: torch
-(>=2.1.1,<3.0.0) ; extra == "semantic" Requires-Dist: tqdm (>=4.66.1,<5.0.0)
-Requires-Dist: transformers (>=4.35.2,<5.0.0) ; extra == "semantic" Requires-
-Dist: unstructured (>=0.11.6,<0.12.0) ; extra == "generators" Description-
-Content-Type: text/markdown
+protobuf (>=4.23.4,<5.0.0) Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
+Requires-Dist: pyyaml (>=6.0.1,<7.0.0) Requires-Dist: requests
+(>=2.31.0,<3.0.0) Requires-Dist: rouge (>=1.0.1,<2.0.0) Requires-Dist:
+sentence-transformers (>=2.2.2,<3.0.0) ; extra == "semantic" Requires-Dist:
+sentencepiece (>=0.2.0,<0.3.0) Requires-Dist: tenacity (>=8.2.3,<9.0.0)
+Requires-Dist: thefuzz (>=0.22.1,<0.23.0) Requires-Dist: tiktoken
+(>=0.5.2,<0.6.0) ; extra == "generators" Requires-Dist: torch (>=2.1.1,<3.0.0)
+; extra == "semantic" Requires-Dist: tqdm (>=4.66.1,<5.0.0) Requires-Dist:
+transformers (>=4.35.2,<5.0.0) ; extra == "semantic" Requires-Dist:
+unstructured (>=0.11.6,<0.12.0) ; extra == "generators" Description-Content-
+Type: text/markdown
                ******** [[ddooccss//ppuubblliicc//ccoonnttiinnuuoouuss--eevvaall--llooggoo..ppnngg]] ********
    _[_D_o_c_u_m_e_n_t_a_t_i_o_n_]_!_[_h_t_t_p_s_:_/_/_p_y_p_i_._p_y_t_h_o_n_._o_r_g_/_p_y_p_i_/_c_o_n_t_i_n_u_o_u_s_-_e_v_a_l_/_]_(_h_t_t_p_s_:_/_/
    _i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_c_o_n_t_i_n_u_o_u_s_-_e_v_a_l_._s_v_g_) _!_[_h_t_t_p_s_:_/_/_G_i_t_H_u_b_._c_o_m_/
   _r_e_l_a_r_i_-_a_i_/_c_o_n_t_i_n_u_o_u_s_-_e_v_a_l_/_r_e_l_e_a_s_e_s_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_r_e_l_e_a_s_e_/
    _r_e_l_a_r_i_-_a_i_/_c_o_n_t_i_n_u_o_u_s_-_e_v_a_l_) _!_[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_N_a_e_r_e_e_n_/_b_a_d_g_e_s_/_]_(_h_t_t_p_s_:_/_/
    _b_a_d_g_e_n_._n_e_t_/_b_a_d_g_e_/_O_p_e_n_%_2_0_S_o_u_r_c_e_%_2_0_%_3_F_/_Y_e_s_%_2_1_/_b_l_u_e_?_i_c_o_n_=_g_i_t_h_u_b_) ![https://
      pypi.python.org/pypi/continuous-eval/](https://img.shields.io/pypi/l/
@@ -113,15 +114,15 @@
 for evaluation as it can offer a comprehensive and consistent measurement of
 system performance. However, it is often costly and time-consuming to manually
 curate such a golden dataset. We have created a synthetic data pipeline that
 can custom generate user interaction data for a variety of use cases such as
 RAG, agents, copilots. They can serve a starting point for a golden dataset for
 evaluation or for other training purposes. Below is an example for Coding
 Agents. Try out this demo: [Synthetic Data Demo](https://www.relari.ai/
-#synthetic_data_demo)
+synthetic-data-demo)
               ************ [[ddooccss//ppuubblliicc//ssyynntthheettiicc--ddaattaa--ddeemmoo..ppnngg]] ************
 ## Resources - **Docs:** [link](https://docs.relari.ai/) - **Examples Repo**:
 [end-to-end example repo](https://github.com/relari-ai/examples) - **Blog
 Posts:** - Practical Guide to RAG Pipeline Evaluation: [Part 1: Retrieval]
 (https://medium.com/relari/a-practical-guide-to-rag-pipeline-evaluation-part-1-
 27a472b09893), [Part 2: Generation](https://medium.com/relari/a-practical-
 guide-to-rag-evaluation-part-2-generation-c79b1bde0f5d) - How important is a
```

