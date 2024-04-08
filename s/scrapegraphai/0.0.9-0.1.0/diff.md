# Comparing `tmp/scrapegraphai-0.0.9.tar.gz` & `tmp/scrapegraphai-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapegraphai-0.0.9.tar", max compression
+gzip compressed data, was "scrapegraphai-0.1.0.tar", max compression
```

## Comparing `scrapegraphai-0.0.9.tar` & `scrapegraphai-0.1.0.tar`

### file list

```diff
@@ -1,77 +1,43 @@
--rw-r--r--   0        0        0     1065 2024-03-03 14:00:51.183606 scrapegraphai-0.0.9/LICENSE
--rw-r--r--   0        0        0     5204 2024-03-14 19:54:25.107262 scrapegraphai-0.0.9/README.md
--rw-r--r--   0        0        0     1669 2024-03-14 20:02:12.175652 scrapegraphai-0.0.9/pyproject.toml
--rw-r--r--   0        0        0       54 2024-03-03 14:00:51.196394 scrapegraphai-0.0.9/scrapegraphai/__init__.py
--rw-r--r--   0        0        0       90 2024-03-03 14:00:51.196546 scrapegraphai-0.0.9/scrapegraphai/builders/__init__.py
--rw-r--r--   0        0        0      322 2024-03-07 12:18:05.846696 scrapegraphai-0.0.9/scrapegraphai/builders/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     8164 2024-03-07 12:18:05.847612 scrapegraphai-0.0.9/scrapegraphai/builders/__pycache__/graph_builder.cpython-311.pyc
--rw-r--r--   0        0        0     6476 2024-03-14 19:54:25.108991 scrapegraphai-0.0.9/scrapegraphai/builders/graph_builder.py
--rw-r--r--   0        0        0       95 2024-03-03 14:00:51.196864 scrapegraphai-0.0.9/scrapegraphai/evaluators/__init__.py
--rw-r--r--   0        0        0      330 2024-03-07 12:16:19.339413 scrapegraphai-0.0.9/scrapegraphai/evaluators/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4763 2024-03-07 12:16:19.340112 scrapegraphai-0.0.9/scrapegraphai/evaluators/__pycache__/trulens_evaluator.cpython-311.pyc
--rw-r--r--   0        0        0     2850 2024-03-03 14:00:51.196981 scrapegraphai-0.0.9/scrapegraphai/evaluators/trulens_evaluator.py
--rw-r--r--   0        0        0      182 2024-03-03 14:00:51.197129 scrapegraphai-0.0.9/scrapegraphai/graphs/__init__.py
--rw-r--r--   0        0        0      465 2024-03-03 14:05:13.267158 scrapegraphai-0.0.9/scrapegraphai/graphs/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3938 2024-03-03 14:05:13.268442 scrapegraphai-0.0.9/scrapegraphai/graphs/__pycache__/base_graph.cpython-311.pyc
--rw-r--r--   0        0        0     4878 2024-03-14 19:59:46.286501 scrapegraphai-0.0.9/scrapegraphai/graphs/__pycache__/smart_scraper_graph.cpython-311.pyc
--rw-r--r--   0        0        0     5595 2024-03-14 19:59:47.193195 scrapegraphai-0.0.9/scrapegraphai/graphs/__pycache__/speech_summary_graph.cpython-311.pyc
--rw-r--r--   0        0        0     3041 2024-03-03 14:00:51.197243 scrapegraphai-0.0.9/scrapegraphai/graphs/base_graph.py
--rw-r--r--   0        0        0     4047 2024-03-14 19:54:25.109163 scrapegraphai-0.0.9/scrapegraphai/graphs/smart_scraper_graph.py
--rw-r--r--   0        0        0     4629 2024-03-14 19:54:25.109531 scrapegraphai-0.0.9/scrapegraphai/graphs/speech_summary_graph.py
--rw-r--r--   0        0        0      164 2024-03-03 14:00:51.197634 scrapegraphai-0.0.9/scrapegraphai/helpers/__init__.py
--rw-r--r--   0        0        0      417 2024-03-07 12:18:06.972641 scrapegraphai-0.0.9/scrapegraphai/helpers/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      554 2024-03-07 12:18:06.974033 scrapegraphai-0.0.9/scrapegraphai/helpers/__pycache__/models_tokens.cpython-311.pyc
--rw-r--r--   0        0        0     2990 2024-03-12 12:09:21.919273 scrapegraphai-0.0.9/scrapegraphai/helpers/__pycache__/nodes_metadata.cpython-311.pyc
--rw-r--r--   0        0        0     1555 2024-03-07 12:18:06.973681 scrapegraphai-0.0.9/scrapegraphai/helpers/__pycache__/schemas.cpython-311.pyc
--rw-r--r--   0        0        0      406 2024-03-03 14:00:51.197724 scrapegraphai-0.0.9/scrapegraphai/helpers/models_tokens.py
--rw-r--r--   0        0        0     3446 2024-03-12 12:08:32.408444 scrapegraphai-0.0.9/scrapegraphai/helpers/nodes_metadata.py
--rw-r--r--   0        0        0     2363 2024-03-03 14:00:51.197887 scrapegraphai-0.0.9/scrapegraphai/helpers/schemas.py
--rw-r--r--   0        0        0      187 2024-03-14 19:54:25.109790 scrapegraphai-0.0.9/scrapegraphai/models/__init__.py
--rw-r--r--   0        0        0      495 2024-03-14 19:58:41.591208 scrapegraphai-0.0.9/scrapegraphai/models/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1245 2024-03-14 19:58:42.338097 scrapegraphai-0.0.9/scrapegraphai/models/__pycache__/gemini.cpython-311.pyc
--rw-r--r--   0        0        0     1173 2024-03-03 14:05:12.611162 scrapegraphai-0.0.9/scrapegraphai/models/__pycache__/openai.cpython-311.pyc
--rw-r--r--   0        0        0     2415 2024-03-03 14:05:13.261218 scrapegraphai-0.0.9/scrapegraphai/models/__pycache__/openai_itt.cpython-311.pyc
--rw-r--r--   0        0        0     2478 2024-03-03 14:05:13.265915 scrapegraphai-0.0.9/scrapegraphai/models/__pycache__/openai_tts.cpython-311.pyc
--rw-r--r--   0        0        0      715 2024-03-14 19:54:25.109898 scrapegraphai-0.0.9/scrapegraphai/models/gemini.py
--rw-r--r--   0        0        0      575 2024-03-03 14:00:51.198085 scrapegraphai-0.0.9/scrapegraphai/models/openai.py
--rw-r--r--   0        0        0     1721 2024-03-03 14:00:51.198164 scrapegraphai-0.0.9/scrapegraphai/models/openai_itt.py
--rw-r--r--   0        0        0     1647 2024-03-03 14:00:51.198245 scrapegraphai-0.0.9/scrapegraphai/models/openai_tts.py
--rw-r--r--   0        0        0      529 2024-03-14 19:54:25.110074 scrapegraphai-0.0.9/scrapegraphai/nodes/__init__.py
--rw-r--r--   0        0        0      994 2024-03-14 19:59:46.287147 scrapegraphai-0.0.9/scrapegraphai/nodes/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3390 2024-03-03 14:05:13.451022 scrapegraphai-0.0.9/scrapegraphai/nodes/__pycache__/base_node.cpython-311.pyc
--rw-r--r--   0        0        0     3903 2024-03-12 20:22:37.637898 scrapegraphai-0.0.9/scrapegraphai/nodes/__pycache__/conditional_node.cpython-311.pyc
--rw-r--r--   0        0        0     4815 2024-03-12 12:08:54.597343 scrapegraphai-0.0.9/scrapegraphai/nodes/__pycache__/fetch_html_node.cpython-311.pyc
--rw-r--r--   0        0        0     2756 2024-03-12 20:22:38.139360 scrapegraphai-0.0.9/scrapegraphai/nodes/__pycache__/fetch_text_node.cpython-311.pyc
--rw-r--r--   0        0        0     6336 2024-03-12 12:08:54.998583 scrapegraphai-0.0.9/scrapegraphai/nodes/__pycache__/generate_answer_node.cpython-311.pyc
--rw-r--r--   0        0        0     6366 2024-03-14 19:59:46.670743 scrapegraphai-0.0.9/scrapegraphai/nodes/__pycache__/generate_answer_node_from_rag.cpython-311.pyc
--rw-r--r--   0        0        0     4946 2024-03-14 19:59:47.192498 scrapegraphai-0.0.9/scrapegraphai/nodes/__pycache__/generate_answer_node_vanilla.cpython-311.pyc
--rw-r--r--   0        0        0     4783 2024-03-03 14:05:13.451945 scrapegraphai-0.0.9/scrapegraphai/nodes/__pycache__/get_probable_tags_node.cpython-311.pyc
--rw-r--r--   0        0        0     2219 2024-03-03 14:05:14.086097 scrapegraphai-0.0.9/scrapegraphai/nodes/__pycache__/image_to_text_node.cpython-311.pyc
--rw-r--r--   0        0        0     4151 2024-03-03 14:05:13.500976 scrapegraphai-0.0.9/scrapegraphai/nodes/__pycache__/parse_html_node.cpython-311.pyc
--rw-r--r--   0        0        0     4476 2024-03-12 12:08:55.003121 scrapegraphai-0.0.9/scrapegraphai/nodes/__pycache__/parse_node.cpython-311.pyc
--rw-r--r--   0        0        0     3625 2024-03-05 12:13:18.777801 scrapegraphai-0.0.9/scrapegraphai/nodes/__pycache__/parse_text_node.cpython-311.pyc
--rw-r--r--   0        0        0     5068 2024-03-12 12:08:55.011225 scrapegraphai-0.0.9/scrapegraphai/nodes/__pycache__/rag_node.cpython-311.pyc
--rw-r--r--   0        0        0     2276 2024-03-03 14:05:14.085608 scrapegraphai-0.0.9/scrapegraphai/nodes/__pycache__/text_to_speech_node.cpython-311.pyc
--rw-r--r--   0        0        0     2666 2024-03-03 14:00:51.198470 scrapegraphai-0.0.9/scrapegraphai/nodes/base_node.py
--rw-r--r--   0        0        0     2914 2024-03-12 20:22:34.352630 scrapegraphai-0.0.9/scrapegraphai/nodes/conditional_node.py
--rw-r--r--   0        0        0     3498 2024-03-12 12:08:32.408975 scrapegraphai-0.0.9/scrapegraphai/nodes/fetch_html_node.py
--rw-r--r--   0        0        0     1799 2024-03-12 20:17:38.519456 scrapegraphai-0.0.9/scrapegraphai/nodes/fetch_text_node.py
--rw-r--r--   0        0        0     5631 2024-03-14 19:54:25.110224 scrapegraphai-0.0.9/scrapegraphai/nodes/generate_answer_node_from_rag.py
--rw-r--r--   0        0        0     3938 2024-03-14 19:54:25.110334 scrapegraphai-0.0.9/scrapegraphai/nodes/generate_answer_node_vanilla.py
--rw-r--r--   0        0        0     3770 2024-03-03 14:00:51.198885 scrapegraphai-0.0.9/scrapegraphai/nodes/get_probable_tags_node.py
--rw-r--r--   0        0        0     1243 2024-03-03 14:00:51.198966 scrapegraphai-0.0.9/scrapegraphai/nodes/image_to_text_node.py
--rw-r--r--   0        0        0     3395 2024-03-12 12:08:32.409631 scrapegraphai-0.0.9/scrapegraphai/nodes/parse_node.py
--rw-r--r--   0        0        0     4130 2024-03-12 12:08:32.411047 scrapegraphai-0.0.9/scrapegraphai/nodes/rag_node.py
--rw-r--r--   0        0        0     1258 2024-03-03 14:00:51.199293 scrapegraphai-0.0.9/scrapegraphai/nodes/text_to_speech_node.py
--rw-r--r--   0        0        0      191 2024-03-03 14:00:51.199414 scrapegraphai-0.0.9/scrapegraphai/utils/__init__.py
--rw-r--r--   0        0        0      417 2024-03-03 14:05:14.087703 scrapegraphai-0.0.9/scrapegraphai/utils/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2134 2024-03-03 14:05:14.088401 scrapegraphai-0.0.9/scrapegraphai/utils/__pycache__/convert_to_csv.cpython-311.pyc
--rw-r--r--   0        0        0     2291 2024-03-03 14:05:14.674154 scrapegraphai-0.0.9/scrapegraphai/utils/__pycache__/convert_to_json.cpython-311.pyc
--rw-r--r--   0        0        0     1559 2024-03-12 12:08:54.888761 scrapegraphai-0.0.9/scrapegraphai/utils/__pycache__/remover.cpython-311.pyc
--rw-r--r--   0        0        0     1159 2024-03-03 14:05:14.088008 scrapegraphai-0.0.9/scrapegraphai/utils/__pycache__/save_audio_from_bytes.cpython-311.pyc
--rw-r--r--   0        0        0     1271 2024-03-03 14:00:51.199500 scrapegraphai-0.0.9/scrapegraphai/utils/convert_to_csv.py
--rw-r--r--   0        0        0     1268 2024-03-03 14:00:51.199592 scrapegraphai-0.0.9/scrapegraphai/utils/convert_to_json.py
--rw-r--r--   0        0        0      877 2024-03-12 12:08:32.411492 scrapegraphai-0.0.9/scrapegraphai/utils/remover.py
--rw-r--r--   0        0        0      574 2024-03-03 14:00:51.199769 scrapegraphai-0.0.9/scrapegraphai/utils/save_audio_from_bytes.py
--rw-r--r--   0        0        0      990 2024-03-03 14:00:51.199840 scrapegraphai-0.0.9/scrapegraphai/utils/token_calculator.py
--rw-r--r--   0        0        0     6881 1970-01-01 00:00:00.000000 scrapegraphai-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-03-03 14:00:51.183606 scrapegraphai-0.1.0/LICENSE
+-rw-r--r--   0        0        0     5590 2024-04-06 12:43:33.708461 scrapegraphai-0.1.0/README.md
+-rw-r--r--   0        0        0     1621 2024-04-08 16:14:52.864798 scrapegraphai-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0       54 2024-03-03 14:00:51.196394 scrapegraphai-0.1.0/scrapegraphai/__init__.py
+-rw-r--r--   0        0        0       90 2024-03-03 14:00:51.196546 scrapegraphai-0.1.0/scrapegraphai/builders/__init__.py
+-rw-r--r--   0        0        0     6670 2024-03-24 19:34:24.965713 scrapegraphai-0.1.0/scrapegraphai/builders/graph_builder.py
+-rw-r--r--   0        0        0      205 2024-04-06 12:46:22.006551 scrapegraphai-0.1.0/scrapegraphai/graphs/__init__.py
+-rw-r--r--   0        0        0     2887 2024-04-08 16:13:44.450904 scrapegraphai-0.1.0/scrapegraphai/graphs/abstract_graph.py
+-rw-r--r--   0        0        0     3041 2024-03-18 13:23:07.402624 scrapegraphai-0.1.0/scrapegraphai/graphs/base_graph.py
+-rw-r--r--   0        0        0     2160 2024-04-08 16:13:44.451088 scrapegraphai-0.1.0/scrapegraphai/graphs/search_graph.py
+-rw-r--r--   0        0        0     2300 2024-04-08 16:13:44.451433 scrapegraphai-0.1.0/scrapegraphai/graphs/smart_scraper_graph.py
+-rw-r--r--   0        0        0     3024 2024-04-08 16:13:44.451625 scrapegraphai-0.1.0/scrapegraphai/graphs/speech_graph.py
+-rw-r--r--   0        0        0      164 2024-03-03 14:00:51.197634 scrapegraphai-0.1.0/scrapegraphai/helpers/__init__.py
+-rw-r--r--   0        0        0      607 2024-04-08 16:13:44.452326 scrapegraphai-0.1.0/scrapegraphai/helpers/models_tokens.py
+-rw-r--r--   0        0        0     3793 2024-04-08 16:13:44.452862 scrapegraphai-0.1.0/scrapegraphai/helpers/nodes_metadata.py
+-rw-r--r--   0        0        0     2363 2024-03-03 14:00:51.197887 scrapegraphai-0.1.0/scrapegraphai/helpers/schemas.py
+-rw-r--r--   0        0        0      252 2024-04-08 16:13:44.453206 scrapegraphai-0.1.0/scrapegraphai/models/__init__.py
+-rw-r--r--   0        0        0      600 2024-04-08 16:13:44.453638 scrapegraphai-0.1.0/scrapegraphai/models/azure_openai.py
+-rw-r--r--   0        0        0      651 2024-04-06 12:44:56.957059 scrapegraphai-0.1.0/scrapegraphai/models/gemini.py
+-rw-r--r--   0        0        0      590 2024-04-08 16:13:44.454004 scrapegraphai-0.1.0/scrapegraphai/models/ollama.py
+-rw-r--r--   0        0        0      575 2024-03-03 14:00:51.198085 scrapegraphai-0.1.0/scrapegraphai/models/openai.py
+-rw-r--r--   0        0        0     1721 2024-03-18 13:23:25.826441 scrapegraphai-0.1.0/scrapegraphai/models/openai_itt.py
+-rw-r--r--   0        0        0     1657 2024-03-24 19:34:24.967643 scrapegraphai-0.1.0/scrapegraphai/models/openai_tts.py
+-rw-r--r--   0        0        0      448 2024-04-06 12:46:22.007377 scrapegraphai-0.1.0/scrapegraphai/nodes/__init__.py
+-rw-r--r--   0        0        0     7544 2024-04-08 16:13:44.454956 scrapegraphai-0.1.0/scrapegraphai/nodes/base_node.py
+-rw-r--r--   0        0        0     2914 2024-03-12 20:22:34.352630 scrapegraphai-0.1.0/scrapegraphai/nodes/conditional_node.py
+-rw-r--r--   0        0        0     3225 2024-04-08 16:13:44.455216 scrapegraphai-0.1.0/scrapegraphai/nodes/fetch_node.py
+-rw-r--r--   0        0        0     5602 2024-04-08 16:13:44.455773 scrapegraphai-0.1.0/scrapegraphai/nodes/generate_answer_node.py
+-rw-r--r--   0        0        0     4023 2024-03-27 19:54:31.570449 scrapegraphai-0.1.0/scrapegraphai/nodes/get_probable_tags_node.py
+-rw-r--r--   0        0        0     1592 2024-04-08 16:13:44.455987 scrapegraphai-0.1.0/scrapegraphai/nodes/image_to_text_node.py
+-rw-r--r--   0        0        0     3337 2024-04-08 16:13:44.456540 scrapegraphai-0.1.0/scrapegraphai/nodes/parse_node.py
+-rw-r--r--   0        0        0     4691 2024-04-08 16:13:44.456936 scrapegraphai-0.1.0/scrapegraphai/nodes/rag_node.py
+-rw-r--r--   0        0        0     4525 2024-04-08 16:13:44.457372 scrapegraphai-0.1.0/scrapegraphai/nodes/search_internet_node.py
+-rw-r--r--   0        0        0     1635 2024-04-08 16:13:44.457753 scrapegraphai-0.1.0/scrapegraphai/nodes/text_to_speech_node.py
+-rw-r--r--   0        0        0      191 2024-03-03 14:00:51.199414 scrapegraphai-0.1.0/scrapegraphai/utils/__init__.py
+-rw-r--r--   0        0        0     1856 2024-04-03 10:39:06.250892 scrapegraphai-0.1.0/scrapegraphai/utils/convert_to_csv.py
+-rw-r--r--   0        0        0     1437 2024-04-03 10:39:06.251121 scrapegraphai-0.1.0/scrapegraphai/utils/convert_to_json.py
+-rw-r--r--   0        0        0     3630 2024-04-06 12:43:33.712449 scrapegraphai-0.1.0/scrapegraphai/utils/parse_state_keys.py
+-rw-r--r--   0        0        0      767 2024-04-06 12:43:33.712605 scrapegraphai-0.1.0/scrapegraphai/utils/remover.py
+-rw-r--r--   0        0        0     1118 2024-04-06 12:46:22.008255 scrapegraphai-0.1.0/scrapegraphai/utils/research_web.py
+-rw-r--r--   0        0        0      631 2024-04-06 12:44:50.349656 scrapegraphai-0.1.0/scrapegraphai/utils/save_audio_from_bytes.py
+-rw-r--r--   0        0        0      990 2024-03-18 13:23:59.117686 scrapegraphai-0.1.0/scrapegraphai/utils/token_calculator.py
+-rw-r--r--   0        0        0     7177 1970-01-01 00:00:00.000000 scrapegraphai-0.1.0/PKG-INFO
```

### Comparing `scrapegraphai-0.0.9/LICENSE` & `scrapegraphai-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.0.9/README.md` & `scrapegraphai-0.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 
 
 # 🕷️ ScrapeGraphAI: You Only Scrape Once
 [![Downloads](https://static.pepy.tech/badge/scrapegraphai)](https://pepy.tech/project/scrapegraphai)
 [![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/pylint-dev/pylint)
 [![Pylint](https://github.com/VinciGit00/Scrapegraph-ai/actions/workflows/pylint.yml/badge.svg)](https://github.com/VinciGit00/Scrapegraph-ai/actions/workflows/pylint.yml)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![](https://dcbadge.vercel.app/api/server/gkxQDAjfeX)](https://discord.gg/gkxQDAjfeX)
 
 
-ScrapeGraphAI is a *web scraping* python library based on LangChain which uses LLM and direct graph logic to create scraping pipelines for websites and documents.
+ScrapeGraphAI is a *web scraping* python library which uses LLM and direct graph logic to create scraping pipelines for websites, documents and XML files.
 Just say which information you want to extract and the library will do it for you!
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/VinciGit00/Scrapegraph-ai/main/docs/assets/scrapegraphai_logo.png" alt="Scrapegraph-ai Logo" style="width: 50%;">
 </p>
 
 
@@ -45,28 +46,34 @@
 ### Case 1: Extracting information using a prompt
 
 You can use the `SmartScraper` class to extract information from a website using a prompt.
 
 The `SmartScraper` class is a direct graph implementation that uses the most common nodes present in a web scraping pipeline. For more information, please see the [documentation](https://scrapegraph-ai.readthedocs.io/en/latest/).
 
 ```python
-from scrapegraphai.graphs import SmartScraper
-
+from scrapegraphai.graphs import SmartScraperGraph
 OPENAI_API_KEY = "YOUR_API_KEY"
 
-llm_config = {
-    "api_key": OPENAI_API_KEY,
-    "model_name": "gpt-3.5-turbo",
+# Define the configuration for the graph
+graph_config = {
+    "llm": {
+        "api_key": OPENAI_API_KEY,
+        "model": "gpt-3.5-turbo",
+    },
 }
 
-smart_scraper = SmartScraper("List me all the titles and project descriptions",
-                             "https://perinim.github.io/projects/", llm_config)
+# Create the SmartScraperGraph instance
+smart_scraper_graph = SmartScraperGraph(
+    prompt="List me all the news with their description.",
+    file_source="https://perinim.github.io/projects/",  # also accepts a string with the already downloaded HTML code as string format
+    config=graph_config
+)
 
-answer = smart_scraper.run()
-print(answer)
+result = smart_scraper_graph.run()
+print(result)
 ```
 
 The output will be a dictionary with the extracted information, for example:
 
 ```bash
 {
     'titles': [
@@ -80,16 +87,17 @@
 
 ## 🤝 Contributing
 
 Fell free to contribute and join our Discord server to discuss with us improvements and give us suggestions!
 
 For more information, please see the [contributing guidelines](https://github.com/VinciGit00/Scrapegraph-ai/blob/main/CONTRIBUTING.md).
 
-[![My Skills](https://skillicons.dev/icons?i=discord)](https://discord.gg/DujC7HG8)
+[![My Skills](https://skillicons.dev/icons?i=discord)](https://discord.gg/gkxQDAjfeX)
 [![My Skills](https://skillicons.dev/icons?i=linkedin)](https://www.linkedin.com/company/scrapegraphai/)
+[![My Skills](https://skillicons.dev/icons?i=twitter)](https://twitter.com/scrapegraph)
 
 ## ❤️ Contributors
 [![Contributors](https://contrib.rocks/image?repo=VinciGit00/Scrapegraph-ai)](https://github.com/VinciGit00/Scrapegraph-ai/graphs/contributors)
 
 ## 🎓 Citations
 If you have used our library for research purposes please quote us with the following reference:
 ```text
```

### Comparing `scrapegraphai-0.0.9/pyproject.toml` & `scrapegraphai-0.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scrapegraphai"
-version = "0.0.9"
+version = "0.1.0"
 description = "A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines."
 authors = [
     "Marco Vinciguerra <mvincig11@gmail.com>",
     "Marco Perini <perinim.98@gmail.com>",
     "Lorenzo Padoan <lorenzo.padoan977@gmail.com>"
 ]
 license = "MIT"
@@ -17,28 +17,27 @@
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 
 [tool.poetry.dependencies]
-python = ">3.9,<3.9.7 || >3.9.7,<3.12"
-langchain = "0.1.6"
-langchain_community = "0.0.19"
-langchain_core = "0.1.22"
-langchain_openai = "0.0.5"
+python = ">3.9,<4.0"
+langchain = "0.1.14"
+langchain-openai = "0.1.1"
+langchain-google-genai = "1.0.1"
 html2text = "2020.1.16"
 faiss-cpu = "1.7.4"
 beautifulsoup4 = "4.12.3"
-trulens_eval = "0.23.0"
 pandas = "2.0.3"
 python-dotenv = "1.0.1"
 tiktoken = {version = ">=0.5.2,<0.6.0"}
 tqdm = "4.66.1"
 graphviz = "0.20.1"
+google = "3.0.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "8.0.0"
 
 [tool.poetry.group.docs]
 optional = true
```

### Comparing `scrapegraphai-0.0.9/scrapegraphai/builders/graph_builder.py` & `scrapegraphai-0.1.0/scrapegraphai/builders/graph_builder.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ 
 Module for making the graph building
 """
-import graphviz
+
 from langchain_core.prompts import ChatPromptTemplate
 from langchain.chains import create_extraction_chain
 from ..models import OpenAI, Gemini
 from ..helpers import nodes_metadata, graph_schema
 
 
 class GraphBuilder:
@@ -35,51 +35,49 @@
             language model, where 'api_key' is mandatory, 
             and 'model_name', 'temperature', and 'streaming' can be optionally included.
 
     Raises:
         ValueError: If 'api_key' is not included in llm_config.
     """
 
-    def __init__(self, user_prompt: str, llm_config: dict):
+    def __init__(self, user_prompt: str, config: dict):
         """
         Initializes the GraphBuilder with a user prompt and language model configuration.
         """
         self.user_prompt = user_prompt
-        self.llm_config = llm_config
-        self.llm = self._create_llm()
+        self.config = config
+        self.llm = self._create_llm(config["llm"])
         self.nodes_description = self._generate_nodes_description()
         self.chain = self._create_extraction_chain()
 
-    def _create_llm(self):
+    def _create_llm(self, llm_config: dict):
         """
         Creates an instance of the OpenAI class with the provided language model configuration.
 
         Returns:
             OpenAI: An instance of the OpenAI class.
 
         Raises:
             ValueError: If 'api_key' is not provided in llm_config.
         """
         llm_defaults = {
-            "model_name": "gpt-3.5-turbo",
             "temperature": 0,
             "streaming": True
         }
         # Update defaults with any LLM parameters that were provided
-        llm_params = {**llm_defaults, **self.llm_config}
+        llm_params = {**llm_defaults, **llm_config}
         if "api_key" not in llm_params:
             raise ValueError("LLM configuration must include an 'api_key'.")
-        
+
         # select the model based on the model name
-        if "gpt-" in llm_params["model_name"]:
+        if "gpt-" in llm_params["model"]:
             return OpenAI(llm_params)
-        elif "gemini" in llm_params["model_name"]:
+        elif "gemini" in llm_params["model"]:
             return Gemini(llm_params)
-        
-        return OpenAI(llm_params)
+        raise ValueError("Model not supported")
 
     def _generate_nodes_description(self):
         """
         Generates a string description of all available nodes and their arguments.
 
         Returns:
             str: A string description of all available nodes and their arguments.
@@ -130,14 +128,19 @@
 
         Args:
             json_data (dict): A JSON representation of the graph configuration.
 
         Returns:
             graphviz.Digraph: A Graphviz object representing the graph configuration.
         """
+        try:
+            import graphviz
+        except ImportError:
+            raise ImportError("The 'graphviz' library is required for this functionality. "
+                              "Please install it from 'https://graphviz.org/download/'.")
 
         graph = graphviz.Digraph(comment='ScrapeGraphAI Generated Graph', format=format,
                                  node_attr={'color': 'lightblue2', 'style': 'filled'})
 
         graph_config = json_data["text"][0]
 
         # Retrieve nodes, edges, and the entry point from the JSON data
```

### Comparing `scrapegraphai-0.0.9/scrapegraphai/graphs/base_graph.py` & `scrapegraphai-0.1.0/scrapegraphai/graphs/base_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.0.9/scrapegraphai/helpers/nodes_metadata.py` & `scrapegraphai-0.1.0/scrapegraphai/helpers/nodes_metadata.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 """
 Nodes metadata for the scrapegraphai package.
 """
 
 nodes_metadata = {
-    "FetchHTMLNode": {
-        "description": "Fetches HTML content from a given URL.",
+    "SearchInternetNode": {
+        "description": "Refactors the user's query into a search query and fetches the search result URLs.",
+        "type": "node",
+        "args": {
+            "user_input": "User's query or question."
+        },
+        "returns": "Updated state with the URL of the search result under 'url' key."
+    },
+    "FetchNode": {
+        "description": "Fetches input content from a given URL or file path.",
         "type": "node",
         "args": {
             "url": "The URL from which to fetch HTML content."
         },
         "returns": "Updated state with fetched HTML content under 'document' key."
     },
     "GetProbableTagsNode": {
```

### Comparing `scrapegraphai-0.0.9/scrapegraphai/helpers/schemas.py` & `scrapegraphai-0.1.0/scrapegraphai/helpers/schemas.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.0.9/scrapegraphai/models/gemini.py` & `scrapegraphai-0.1.0/scrapegraphai/models/gemini.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""
+Gemini module configuration
+"""
 from langchain_google_genai import ChatGoogleGenerativeAI
 
 
 class Gemini(ChatGoogleGenerativeAI):
     """Class for wrapping gemini module"""
 
     def __init__(self, llm_config: dict):
@@ -9,11 +12,9 @@
         A wrapper for the Gemini class that provides default configuration
         and could be extended with additional methods if needed.
 
         Args:
             llm_config (dict): Configuration parameters for the language model.
             such as model="gemini-pro" and api_key 
         """
-        # change the key model_name to model
-        llm_config["model"] = llm_config["model_name"]
         # Initialize the superclass (ChatOpenAI) with provided config parameters
         super().__init__(**llm_config)
```

### Comparing `scrapegraphai-0.0.9/scrapegraphai/models/openai.py` & `scrapegraphai-0.1.0/scrapegraphai/models/openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.0.9/scrapegraphai/models/openai_itt.py` & `scrapegraphai-0.1.0/scrapegraphai/models/openai_itt.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.0.9/scrapegraphai/models/openai_tts.py` & `scrapegraphai-0.1.0/scrapegraphai/models/openai_tts.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,30 +18,30 @@
         voice (str): The voice model to use for generating speech.
 
     Methods:
         run(text): Converts the provided text to speech and returns the
         bytes of the generated speech.
     """
 
-    def __init__(self, llm_config: dict, model: str = "tts-1", voice: str = "alloy"):
+    def __init__(self, tts_config: dict):
         """
         Initializes an instance of the OpenAITextToSpeech class.
 
         Args:
             llm_config (dict): The configuration for the language model.
             model (str, optional): The model to use for text-to-speech conversion. 
             Defaults to "tts-1".
             voice (str, optional): The voice model to use for generating speech. 
             Defaults to "alloy".
         """
 
         # convert model_name to model
-        self.client = OpenAI(api_key=llm_config.get("api_key"))
-        self.model = model
-        self.voice = voice
+        self.client = OpenAI(api_key=tts_config.get("api_key"))
+        self.model = tts_config.get("model", "tts-1")
+        self.voice = tts_config.get("voice", "alloy")
 
     def run(self, text):
         """
         Converts the provided text to speech and returns the bytes of the generated speech.
 
         Args:
             text (str): The text to convert to speech.
```

### Comparing `scrapegraphai-0.0.9/scrapegraphai/nodes/base_node.py` & `scrapegraphai-0.1.0/scrapegraphai/nodes/fetch_node.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,66 +1,84 @@
 """ 
-Module for creating the basic node
+Module for fetching the HTML node
 """
-from abc import ABC, abstractmethod
 
+from typing import List
+from langchain_community.document_loaders import AsyncHtmlLoader
+from langchain_core.documents import Document
+from .base_node import BaseNode
 
-class BaseNode(ABC):
+
+class FetchNode(BaseNode):
     """
-    An abstract base class for nodes in a graph-based workflow. Each node is 
-    intended to perform a specific action when executed as part of the graph's 
-    processing flow.
+    A node responsible for fetching the HTML content of a specified URL and updating
+    the graph's state with this content. It uses the AsyncHtmlLoader for asynchronous
+    document loading.
 
-    Attributes:
-        node_name (str): A unique identifier for the node.
-        node_type (str): Specifies the node's type, which influences how the 
-                         node interacts within the graph. Valid values are 
-                         "node" for standard nodes and "conditional_node" for 
-                         nodes that determine the flow based on conditions.
+    This node acts as a starting point in many scraping workflows, preparing the state
+    with the necessary HTML content for further processing by subsequent nodes in the graph.
 
-    Methods:
-        execute(state): An abstract method that subclasses must implement. This 
-                        method should contain the logic that the node executes 
-                        when it is reached in the graph's flow. It takes the 
-                        graph's current state as input and returns the updated 
-                        state after execution.
+    Attributes:
+        node_name (str): The unique identifier name for the node.
+        node_type (str): The type of the node, defaulting to "node". This categorization
+                         helps in determining the node's role and behavior within the graph.
+                         The "node" type is used for standard operational nodes.
 
     Args:
-        node_name (str): The unique identifier name for the node. This name is 
-                         used to reference the node within the graph.
-        node_type (str): The type of the node, limited to "node" or 
-                         "conditional_node". This categorization helps in 
-                         determining the node's role and behavior within the 
-                         graph.
-
-    Raises:
-        ValueError: If the provided `node_type` is not one of the allowed 
-                    values ("node" or "conditional_node"), a ValueError is 
-                    raised to indicate the incorrect usage.
+        node_name (str): The unique identifier name for the node. This name is used to
+                         reference the node within the graph.
+        node_type (str, optional): The type of the node, limited to "node" or
+                                   "conditional_node". Defaults to "node".
+
+    Methods:
+        execute(state): Fetches the HTML content for the URL specified in the state and
+                        updates the state with this content under the 'document' key.
+                        The 'url' key must be present in the state for the operation
+                        to succeed.
     """
 
-    def __init__(self, node_name: str, node_type: str):
+    def __init__(self, input: str, output: List[str], node_name: str = "Fetch"):
+        """
+        Initializes the FetchHTMLNode with a node name and node type.
+        Arguments:
+            node_name (str): name of the node
+        """
+        super().__init__(node_name, "node", input, output, 1)
+
+    def execute(self, state):
         """
-        Initialize the node with a unique identifier and a specified node type.
+        Executes the node's logic to fetch HTML content from a specified URL and
+        update the state with this content.
 
         Args:
-            node_name (str): The unique identifier name for the node.
-            node_type (str): The type of the node, limited to "node" or "conditional_node".
+            state (dict): The current state of the graph, expected to contain a 'url' key.
+
+        Returns:
+            dict: The updated state with a new 'document' key containing the fetched HTML content.
 
         Raises:
-            ValueError: If node_type is not "node" or "conditional_node".
+            KeyError: If the 'url' key is not found in the state, indicating that the
+                      necessary information to perform the operation is missing.
         """
-        self.node_name = node_name
-        if node_type not in ["node", "conditional_node"]:
-            raise ValueError(
-                f"node_type must be 'node' or 'conditional_node', got '{node_type}'")
-        self.node_type = node_type
+        print(f"--- Executing {self.node_name} Node ---")
 
-    @abstractmethod
-    def execute(self, state: dict):
-        """
-        Execute the node's logic and return the updated state.
-        Args:
-            state (dict): The current state of the graph.
-        :return: The updated state after executing this node.
-        """
-        pass
+        # Interpret input keys based on the provided input expression
+        input_keys = self.get_input_keys(state)
+
+        # Fetching data from the state based on the input keys
+        input_data = [state[key] for key in input_keys]
+
+        source = input_data[0]        
+        
+        # if it is a local directory
+        if not source.startswith("http"):
+            document = [Document(page_content=source, metadata={
+                "source": "local_dir"
+            })]
+
+        # if it is a URL
+        else:
+            loader = AsyncHtmlLoader(source)
+            document = loader.load()
+
+        state.update({self.output[0]: document})
+        return state
```

### Comparing `scrapegraphai-0.0.9/scrapegraphai/nodes/conditional_node.py` & `scrapegraphai-0.1.0/scrapegraphai/nodes/conditional_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.0.9/scrapegraphai/nodes/fetch_html_node.py` & `scrapegraphai-0.1.0/scrapegraphai/nodes/parse_node.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,91 +1,84 @@
-""" 
-Module for fetching the HTML node
 """
-from typing import Any
-from langchain_community.document_loaders import AsyncHtmlLoader
-from langchain_core.documents import Document
+Module for parsing the HTML node
+"""
+from typing import List
+from langchain.text_splitter import RecursiveCharacterTextSplitter
+from langchain_community.document_transformers import Html2TextTransformer
 from .base_node import BaseNode
-from ..utils.remover import remover
-
-
-def _build_metadata(soup: Any, url: str) -> dict:
-    """Build metadata from BeautifulSoup output."""
-    metadata = {"source": url}
-    if title := soup.find("title"):
-        metadata["title"] = title.get_text()
-    if description := soup.find("meta", attrs={"name": "description"}):
-        metadata["description"] = description.get(
-            "content", "No description found.")
-    if html := soup.find("html"):
-        metadata["language"] = html.get("lang", "No language found.")
-    return metadata
 
 
-class FetchHTMLNode(BaseNode):
+class ParseNode(BaseNode):
     """
-    A node responsible for fetching the HTML content of a specified URL and updating
-    the graph's state with this content. It uses the AsyncHtmlLoader for asynchronous
-    document loading.
+    A node responsible for parsing HTML content from a document. 
+    It uses BeautifulSoupTransformer for parsing, providing flexibility in extracting
+    specific parts of an HTML document.
 
-    This node acts as a starting point in many scraping workflows, preparing the state
-    with the necessary HTML content for further processing by subsequent nodes in the graph.
+    This node enhances the scraping workflow by allowing for targeted extraction of 
+    content, thereby optimizing the processing of large HTML documents.
 
     Attributes:
-        node_name (str): The unique identifier name for the node.
-        node_type (str): The type of the node, defaulting to "node". This categorization
-                         helps in determining the node's role and behavior within the graph.
-                         The "node" type is used for standard operational nodes.
+        node_name (str): The unique identifier name for the node, defaulting to "ParseHTMLNode".
+        node_type (str): The type of the node, set to "node" indicating a standard operational node.
 
     Args:
-        node_name (str): The unique identifier name for the node. This name is used to
-                         reference the node within the graph.
-        node_type (str, optional): The type of the node, limited to "node" or
-                                   "conditional_node". Defaults to "node".
+        node_name (str, optional): The unique identifier name for the node. 
+        Defaults to "ParseHTMLNode".
 
     Methods:
-        execute(state): Fetches the HTML content for the URL specified in the state and
-                        updates the state with this content under the 'document' key.
-                        The 'url' key must be present in the state for the operation
-                        to succeed.
+        execute(state): Parses the HTML document contained within the state using 
+        the specified tags, if provided, and updates the state with the parsed content.
     """
 
-    def __init__(self, node_name: str):
+    def __init__(self, input: str, output: List[str], node_config: dict, node_name: str = "Parse"):
         """
-        Initializes the FetchHTMLNode with a node name and node type.
-        Arguments:
+        Initializes the ParseHTMLNode with a node name.
+        Args:
+            doc_type (str): type of the input document
+            chunks_size (int): size of the chunks to split the document
             node_name (str): name of the node
+            node_type (str, optional): type of the node
         """
-        super().__init__(node_name, "node")
+        super().__init__(node_name, "node", input, output, 1, node_config)
 
-    def execute(self, state: dict) -> dict:
+    def execute(self,  state):
         """
-        Executes the node's logic to fetch HTML content from a specified URL and
-        update the state with this content.
+        Executes the node's logic to parse the HTML document based on specified tags. 
+        If tags are provided in the state, the document is parsed accordingly; otherwise, 
+        the document remains unchanged. The method updates the state with either the original 
+        or parsed document under the 'parsed_document' key.
 
         Args:
-            state (dict): The current state of the graph, expected to contain a 'url' key.
+            state (dict): The current state of the graph, expected to contain 
+            'document' within 'keys', and optionally 'tags' for targeted parsing.
 
         Returns:
-            dict: The updated state with a new 'document' key containing the fetched HTML content.
+            dict: The updated state with the 'parsed_document' key containing the parsed content,
+                  if tags were provided, or the original document otherwise.
 
         Raises:
-            KeyError: If the 'url' key is not found in the state, indicating that the
-                      necessary information to perform the operation is missing.
+            KeyError: If 'document' is not found in the state, indicating that the necessary 
+                      information for parsing is missing.
         """
-        print("---FETCHING HTML CODE---")
-        try:
-            url = state["url"]
-        except KeyError as e:
-            print(f"Error: {e} not found in state.")
-            raise
-
-        loader = AsyncHtmlLoader(url)
-        document = loader.load()
-        # metadata = document[0].metadata
-        # document = remover(str(document[0]))
-
-        # state["document"] = [
-        #     Document(page_content=document, metadata=metadata)]
-        state["document"] = document
+
+        print(f"--- Executing {self.node_name} Node ---")
+
+        # Interpret input keys based on the provided input expression
+        input_keys = self.get_input_keys(state)
+
+        # Fetching data from the state based on the input keys
+        input_data = [state[key] for key in input_keys]
+
+        text_splitter = RecursiveCharacterTextSplitter.from_tiktoken_encoder(
+            chunk_size=self.node_config.get("chunk_size", 4096),
+            chunk_overlap=0,
+        )
+
+        # Parse the document
+        docs_transformed = Html2TextTransformer(
+        ).transform_documents(input_data[0])[0]
+
+        chunks = text_splitter.split_text(docs_transformed.page_content)
+
+        state.update({self.output[0]: chunks})
 
         return state
```

### Comparing `scrapegraphai-0.0.9/scrapegraphai/nodes/generate_answer_node_from_rag.py` & `scrapegraphai-0.1.0/scrapegraphai/nodes/generate_answer_node.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """
 Module for generating the answer node
 """
 # Imports from standard library
+from typing import List
 from tqdm import tqdm
 
 # Imports from Langchain
 from langchain.prompts import PromptTemplate
 from langchain_core.output_parsers import JsonOutputParser
 from langchain_core.runnables import RunnableParallel
 
 # Imports from the library
 from .base_node import BaseNode
 
 
-class GenerateAnswerNodeFromRag(BaseNode):
+class GenerateAnswerNode(BaseNode):
     """
     A node that generates an answer using a language model (LLM) based on the user's input
     and the content extracted from a webpage. It constructs a prompt from the user's input
     and the scraped content, feeds it to the LLM, and parses the LLM's response to produce
     an answer.
 
     Attributes:
@@ -34,25 +35,26 @@
         Defaults to "GenerateAnswerNode".
 
     Methods:
         execute(state): Processes the input and document from the state to generate an answer,
                         updating the state with the generated answer under the 'answer' key.
     """
 
-    def __init__(self, llm, node_name: str):
+    def __init__(self, input: str, output: List[str], node_config: dict,
+                 node_name: str = "GenerateAnswer"):
         """
         Initializes the GenerateAnswerNode with a language model client and a node name.
         Args:
             llm (OpenAIImageToText): An instance of the OpenAIImageToText class.
             node_name (str): name of the node
         """
-        super().__init__(node_name, "node")
-        self.llm = llm
+        super().__init__(node_name, "node", input, output, 2, node_config)
+        self.llm_model = node_config["llm"]
 
-    def execute(self, state: dict) -> dict:
+    def execute(self, state):
         """
         Generates an answer by constructing a prompt from the user's input and the scraped
         content, querying the language model, and parsing its response.
 
         The method updates the state with the generated answer under the 'answer' key.
 
         Args:
@@ -63,31 +65,24 @@
             dict: The updated state with the 'answer' key containing the generated answer.
 
         Raises:
             KeyError: If 'user_input' or 'document' is not found in the state, indicating
                       that the necessary information for generating an answer is missing.
         """
 
-        print("---GENERATING ANSWER---")
-        try:
-            user_input = state["user_input"]
-            document = state["document"]
-        except KeyError as e:
-            print(f"Error: {e} not found in state.")
-            raise
-
-        parsed_document = state.get("parsed_document", None)
-        relevant_chunks = state.get("relevant_chunks", None)
-
-        if relevant_chunks:
-            context = relevant_chunks
-        elif parsed_document:
-            context = parsed_document
-        else:
-            context = document
+        print(f"--- Executing {self.node_name} Node ---")
+
+        # Interpret input keys based on the provided input expression
+        input_keys = self.get_input_keys(state)
+
+        # Fetching data from the state based on the input keys
+        input_data = [state[key] for key in input_keys]
+
+        user_prompt = input_data[0]
+        doc = input_data[1]
 
         output_parser = JsonOutputParser()
         format_instructions = output_parser.get_format_instructions()
 
         template_chunks = """You are a website scraper and you have just scraped the
         following content from a website.
         You are now asked to answer a question about the content you have scraped.\n {format_instructions} \n
@@ -102,36 +97,36 @@
         Content to merge: {context}
         Question: {question}
                 """
 
         chains_dict = {}
 
         # Use tqdm to add progress bar
-        for i, chunk in enumerate(tqdm(context, desc="Processing chunks")):
+        for i, chunk in enumerate(tqdm(doc, desc="Processing chunks")):
             prompt = PromptTemplate(
                 template=template_chunks,
                 input_variables=["question"],
                 partial_variables={"context": chunk.page_content,
                                    "chunk_id": i + 1, "format_instructions": format_instructions},
             )
             # Dynamically name the chains based on their index
             chain_name = f"chunk{i+1}"
-            chains_dict[chain_name] = prompt | self.llm | output_parser
+            chains_dict[chain_name] = prompt | self.llm_model | output_parser
 
         # Use dictionary unpacking to pass the dynamically named chains to RunnableParallel
         map_chain = RunnableParallel(**chains_dict)
         # Chain
-        answer_map = map_chain.invoke({"question": user_input})
+        answer_map = map_chain.invoke({"question": user_prompt})
 
         # Merge the answers from the chunks
         merge_prompt = PromptTemplate(
             template=template_merge,
             input_variables=["context", "question"],
             partial_variables={"format_instructions": format_instructions},
         )
-        merge_chain = merge_prompt | self.llm | output_parser
+        merge_chain = merge_prompt | self.llm_model | output_parser
         answer = merge_chain.invoke(
-            {"context": answer_map, "question": user_input})
+            {"context": answer_map, "question": user_prompt})
 
         # Update the state with the generated answer
-        state.update({"answer": answer})
-        return state
+        state.update({self.output[0]: answer})
+        return state
```

### Comparing `scrapegraphai-0.0.9/scrapegraphai/nodes/get_probable_tags_node.py` & `scrapegraphai-0.1.0/scrapegraphai/nodes/get_probable_tags_node.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Module for proobable tags
 """
+from typing import List
 from langchain.output_parsers import CommaSeparatedListOutputParser
 from langchain.prompts import PromptTemplate
 from .base_node import BaseNode
 
 
 class GetProbableTagsNode(BaseNode):
     """
@@ -25,25 +26,26 @@
         Defaults to "GetProbableTagsNode".
 
     Methods:
         execute(state): Processes the user's input and the URL from the state to generate a list of 
                         probable HTML tags, updating the state with these tags under the 'tags' key.
     """
 
-    def __init__(self, llm, node_name: str):
+    def __init__(self, input: str, output: List[str], model_config: dict,
+                 node_name: str = "GetProbableTags"):
         """
         Initializes the GetProbableTagsNode with a language model client and a node name.
         Args:
             llm (OpenAIImageToText): An instance of the OpenAIImageToText class.
             node_name (str): name of the node
         """
-        super().__init__(node_name, "node")
-        self.llm = llm
+        super().__init__(node_name, "node", input, output, 2, model_config)
+        self.llm_model = model_config["llm_model"]
 
-    def execute(self, state: dict):
+    def execute(self, state):
         """
         Generates a list of probable HTML tags based on the user's input and updates the state 
         with this list. The method constructs a prompt for the language model, submits it, and 
         parses the output to identify probable tags.
 
         Args:
             state (dict): The current state of the graph, expected to contain 'user_input', 'url',
@@ -53,21 +55,24 @@
             dict: The updated state with the 'tags' key containing a list of probable HTML tags.
 
         Raises:
             KeyError: If 'user_input' or 'url' is not found in the state, indicating that the
                       necessary information for generating tag predictions is missing.
         """
 
-        print("---GETTING PROBABLE TAGS---")
-        try:
-            user_input = state["user_input"]
-            url = state["url"]
-        except KeyError as e:
-            print(f"Error: {e} not found in state.")
-            raise
+        print(f"--- Executing {self.node_name} Node ---")
+
+        # Interpret input keys based on the provided input expression
+        input_keys = self.get_input_keys(state)
+
+        # Fetching data from the state based on the input keys
+        input_data = [state[key] for key in input_keys]
+
+        user_prompt = input_data[0]
+        url = input_data[1]
 
         output_parser = CommaSeparatedListOutputParser()
         format_instructions = output_parser.get_format_instructions()
 
         template = """You are a website scraper that knows all the types of html tags.
          You are now asked to list all the html tags where you think you can find the information of the asked question.\n 
          {format_instructions} \n  The webpage is: {webpage} \n The asked question is the following: {question}
@@ -77,15 +82,13 @@
             template=template,
             input_variables=["question"],
             partial_variables={
                 "format_instructions": format_instructions, "webpage": url},
         )
 
         # Execute the chain to get probable tags
-        tag_answer = tag_prompt | self.llm | output_parser
-        probable_tags = tag_answer.invoke({"question": user_input})
-
-        print("Possible tags: ", *probable_tags)
+        tag_answer = tag_prompt | self.llm_model | output_parser
+        probable_tags = tag_answer.invoke({"question": user_prompt})
 
         # Update the dictionary with probable tags
-        state.update({"tags": probable_tags})
+        state.update({self.output[0]: probable_tags})
         return state
```

### Comparing `scrapegraphai-0.0.9/scrapegraphai/nodes/image_to_text_node.py` & `scrapegraphai-0.1.0/scrapegraphai/nodes/image_to_text_node.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,52 @@
-""" 
+"""
 Module for the ImageToTextNode class.
 """
-
+from typing import List
 from .base_node import BaseNode
 
 
 class ImageToTextNode(BaseNode):
     """
     A class representing a node that processes an image and returns the text description.
 
     Attributes:
-        llm (OpenAIImageToText): An instance of the OpenAIImageToText class.
+        llm_model (OpenAIImageToText): An instance of the OpenAIImageToText class.
 
     Methods:
         execute(state, url): Execute the node's logic and return the updated state.
     """
 
-    def __init__(self, llm, node_name: str):
+    def __init__(self, input: str, output: List[str], node_config: dict,
+                 node_name: str = "ImageToText"):
         """
         Initializes an instance of the ImageToTextNode class.
 
         Args:
-            llm (OpenAIImageToText): An instance of the OpenAIImageToText class.
-            node_name (str): name of the node
+            input (str): The input for the node.
+            output (List[str]): The output of the node.
+            node_config (dict): Configuration for the model.
+            node_name (str): Name of the node.
         """
-        super().__init__(node_name, "node")
-        self.llm = llm
+        super().__init__(node_name, "node", input, output, 1, node_config)
+        self.llm_model = node_config["llm_model"]
 
-    def execute(self, state: dict, url: str) -> dict:
+    def execute(self, state: dict) -> dict:
         """
         Execute the node's logic and return the updated state.
+
         Args:
             state (dict): The current state of the graph.
-            url (str): url of the image where to 
-        :return: The updated state after executing this node.
-        """
 
+        Returns:
+            dict: The updated state after executing this node.
+        """
         print("---GENERATING TEXT FROM IMAGE---")
-        text_answer = self.llm.run(url)
+        input_keys = self.get_input_keys(state)
+
+        input_data = [state[key] for key in input_keys]
+        url = input_data[0]
+
+        text_answer = self.llm_model.run(url)
 
         state.update({"image_text": text_answer})
         return state
```

### Comparing `scrapegraphai-0.0.9/scrapegraphai/nodes/rag_node.py` & `scrapegraphai-0.1.0/scrapegraphai/nodes/rag_node.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """
 Module for parsing the HTML node
 """
 
+from typing import List
 from langchain.docstore.document import Document
 from langchain.retrievers import ContextualCompressionRetriever
 from langchain.retrievers.document_compressors import EmbeddingsFilter, DocumentCompressorPipeline
 from langchain_community.document_transformers import EmbeddingsRedundantFilter
 from langchain_community.vectorstores import FAISS
-from langchain_openai import OpenAIEmbeddings
-
-
+from ..models import OpenAI, Gemini, Ollama, AzureOpenAI
+from langchain_openai import OpenAIEmbeddings, AzureOpenAIEmbeddings
+from langchain_community.embeddings import OllamaEmbeddings
 from .base_node import BaseNode
 
 
 class RAGNode(BaseNode):
     """
     A node responsible for compressing the input tokens and storing the document
     in a vector database for retrieval.
@@ -29,20 +30,21 @@
         Defaults to "ParseHTMLNode".
 
     Methods:
         execute(state): Parses the HTML document contained within the state using 
         the specified tags, if provided, and updates the state with the parsed content.
     """
 
-    def __init__(self, llm, node_name="RagNode"):
+    def __init__(self, input: str, output: List[str], node_config: dict, node_name: str = "RAG"):
         """
         Initializes the ParseHTMLNode with a node name.
         """
-        super().__init__(node_name, "node")
-        self.llm = llm
+        super().__init__(node_name, "node", input, output, 2, node_config)
+        self.llm_model = node_config["llm"]
+        self.embedder_model = node_config.get("embedder_model", None)
 
     def execute(self, state):
         """
         Executes the node's logic to implement RAG (Retrieval-Augmented Generation) 
         The method updates the state with relevant chunks of the document.
 
         Args:
@@ -52,65 +54,68 @@
             dict: The updated state containing the 'relevant_chunks' key with the relevant chunks.
 
         Raises:
             KeyError: If 'document' is not found in the state, indicating that the necessary 
                       information for parsing is missing.
         """
 
-        print("---RAG STARTED---")
-        try:
-            user_input = state["user_input"]
-            document = state["document"]
-        except KeyError as e:
-            print(f"Error: {e} not found in state.")
-            raise
+        print(f"--- Executing {self.node_name} Node ---")
 
-        parsed_document = state.get("parsed_document", None)
+        # Interpret input keys based on the provided input expression
+        input_keys = self.get_input_keys(state)
 
-        if parsed_document:
-            chunks = parsed_document
-        else:
-            print("Parsed document not found. Using original document.")
-            chunks = document
+        # Fetching data from the state based on the input keys
+        input_data = [state[key] for key in input_keys]
+
+        user_prompt = input_data[0]
+        doc = input_data[1]
 
         chunked_docs = []
 
-        for i, chunk in enumerate(chunks):
+        for i, chunk in enumerate(doc):
             doc = Document(
                 page_content=chunk,
                 metadata={
                     "chunk": i + 1,
                 },
             )
             chunked_docs.append(doc)
 
-        print("---UPDATED CHUNKS METADATA---")
+        print("--- (updated chunks metadata) ---")
+
+        # check if embedder_model is provided, if not use llm_model
+        embedding_model = self.embedder_model if self.embedder_model else self.llm_model
 
-        openai_key = self.llm.openai_api_key
-        retriever = FAISS.from_documents(chunked_docs,
-                                         OpenAIEmbeddings(api_key=openai_key)).as_retriever()
-        # could be any embedding of your choice
-        embeddings = OpenAIEmbeddings(api_key=openai_key)
+        if isinstance(embedding_model, OpenAI):
+            embeddings = OpenAIEmbeddings(api_key=embedding_model.openai_api_key)
+        elif isinstance(embedding_model, AzureOpenAI):
+            embeddings = AzureOpenAIEmbeddings()
+        elif isinstance(embedding_model, Ollama):
+            embeddings = OllamaEmbeddings()
+        else:
+            raise ValueError("Embedding Model missing or not supported")
+        
+        retriever = FAISS.from_documents(chunked_docs, embeddings).as_retriever()
+    
         redundant_filter = EmbeddingsRedundantFilter(embeddings=embeddings)
         # similarity_threshold could be set, now k=20
         relevant_filter = EmbeddingsFilter(embeddings=embeddings)
         pipeline_compressor = DocumentCompressorPipeline(
             transformers=[redundant_filter, relevant_filter]
         )
-        
         # redundant + relevant filter compressor
         compression_retriever = ContextualCompressionRetriever(
             base_compressor=pipeline_compressor, base_retriever=retriever
         )
 
         # relevant filter compressor only
         # compression_retriever = ContextualCompressionRetriever(
         #     base_compressor=relevant_filter, base_retriever=retriever
         # )
 
         compressed_docs = compression_retriever.get_relevant_documents(
-            user_input)
-        
-        print("---TOKENS COMPRESSED AND VECTOR STORED---")
-        
-        state.update({"relevant_chunks": compressed_docs})
+            user_prompt)
+
+        print("--- (tokens compressed and vector stored) ---")
+
+        state.update({self.output[0]: compressed_docs})
         return state
```

### Comparing `scrapegraphai-0.0.9/scrapegraphai/utils/convert_to_csv.py` & `scrapegraphai-0.1.0/scrapegraphai/utils/convert_to_json.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 """
-Module that given a filename and a position saves the file in the csv format
+Convert to json module
 """
+import json
 import os
-import pandas as pd
+import sys
 
 
-def convert_to_csv(data: dict, filename: str, position: str):
+def convert_to_json(data: dict, filename: str, position: str = None):
     """
     Convert data to JSON format and save it to a file.
 
     Args:
-        data (dict): Data to save.
-        filename (str): Name of the file to save without .csv extension.
-        position (str): Directory where the file should be saved.
+    data (dict): Data to save.
+    filename (str): Name of the file to save without .json extension.
+    position (str): Directory where the file should be saved. If None, 
+    the directory of the caller script will be used.
 
     Raises:
-        ValueError: If filename contains '.csv'.
-        FileNotFoundError: If the specified directory does not exist.
-        PermissionError: If the program does not have permission to write to the directory.
+    ValueError: If filename contains '.json'.
+    FileNotFoundError: If the specified directory does not exist.
+    PermissionError: If the program does not have permission to write to the directory.
     """
-    if ".csv" in filename:
-        raise ValueError("The filename should not contain '.csv'")
+    if ".json" in filename:
+        raise ValueError("The filename should not contain '.json'")
+
+  # Get the directory of the caller script
+    if position is None:
+        # Get directory of the main script
+        caller_dir = os.path.dirname(os.path.abspath(sys.argv[0]))
+        position = caller_dir
 
     try:
         os.makedirs(position, exist_ok=True)
-        pd.DataFrame.from_dict(data, orient='index').to_csv(
-            os.path.join(position, f"{filename}.csv"), index=False)
+        with open(os.path.join(position, f"{filename}.json"), "w", encoding="utf-8") as f:
+            f.write(json.dumps(data))
     except FileNotFoundError as fnfe:
         raise FileNotFoundError(
             f"The specified directory '{position}' does not exist.") from fnfe
     except PermissionError as pe:
         raise PermissionError(
             f"You don't have permission to write to '{position}'.") from pe
-    except Exception as e:
-        raise e
```

### Comparing `scrapegraphai-0.0.9/scrapegraphai/utils/remover.py` & `scrapegraphai-0.1.0/scrapegraphai/utils/remover.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,19 +14,16 @@
 
     Returns:
         str: the parsed title followed by the body content without script tags
     """
 
     soup = BeautifulSoup(html_content, 'html.parser')
 
-    # Estrai il titolo
     title_tag = soup.find('title')
     title = title_tag.get_text() if title_tag else ""
 
-    # Rimuovi i tag <script> in tutto il documento
     [script.extract() for script in soup.find_all('script')]
 
-    # Estrai il corpo del documento
     body_content = soup.find('body')
     body = str(body_content) if body_content else ""
 
     return "Title: " + title + ", Body: " + body
```

### Comparing `scrapegraphai-0.0.9/scrapegraphai/utils/save_audio_from_bytes.py` & `scrapegraphai-0.1.0/scrapegraphai/utils/save_audio_from_bytes.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 This utility function saves the byte response as an audio file.
 """
-
 from pathlib import Path
+from typing import Union
 
 
-def save_audio_from_bytes(byte_response, output_path):
+def save_audio_from_bytes(byte_response: bytes, output_path: Union[str, Path]) -> None:
     """
     Saves the byte response as an audio file.
 
     Args:
         byte_response (bytes): The byte response containing the generated speech.
         output_path (str or Path): The file path where the generated speech should be saved.
     """
```

### Comparing `scrapegraphai-0.0.9/scrapegraphai/utils/token_calculator.py` & `scrapegraphai-0.1.0/scrapegraphai/utils/token_calculator.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.0.9/PKG-INFO` & `scrapegraphai-0.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,52 +1,53 @@
 Metadata-Version: 2.1
 Name: scrapegraphai
-Version: 0.0.9
+Version: 0.1.0
 Summary: A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines.
 Home-page: https://scrapegraph-ai.readthedocs.io/
 License: MIT
 Keywords: scrapegraph,scrapegraphai,langchain,ai,artificial intelligence,gpt,machine learning,rag,nlp,natural language processing,openai,scraping,web scraping,web scraping library,web scraping tool,webscraping,graph
 Author: Marco Vinciguerra
 Author-email: mvincig11@gmail.com
-Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*, !=3.12.*
+Requires-Python: >3.9,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: beautifulsoup4 (==4.12.3)
 Requires-Dist: faiss-cpu (==1.7.4)
+Requires-Dist: google (==3.0.0)
 Requires-Dist: graphviz (==0.20.1)
 Requires-Dist: html2text (==2020.1.16)
-Requires-Dist: langchain (==0.1.6)
-Requires-Dist: langchain_community (==0.0.19)
-Requires-Dist: langchain_core (==0.1.22)
-Requires-Dist: langchain_openai (==0.0.5)
+Requires-Dist: langchain (==0.1.14)
+Requires-Dist: langchain-google-genai (==1.0.1)
+Requires-Dist: langchain-openai (==0.1.1)
 Requires-Dist: pandas (==2.0.3)
 Requires-Dist: python-dotenv (==1.0.1)
 Requires-Dist: tiktoken (>=0.5.2,<0.6.0)
 Requires-Dist: tqdm (==4.66.1)
-Requires-Dist: trulens_eval (==0.23.0)
 Project-URL: Documentation, https://scrapegraph-doc.onrender.com/
 Project-URL: Repository, https://github.com/VinciGit00/Scrapegraph-ai
 Description-Content-Type: text/markdown
 
 
 
 
 # 🕷️ ScrapeGraphAI: You Only Scrape Once
 [![Downloads](https://static.pepy.tech/badge/scrapegraphai)](https://pepy.tech/project/scrapegraphai)
 [![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/pylint-dev/pylint)
 [![Pylint](https://github.com/VinciGit00/Scrapegraph-ai/actions/workflows/pylint.yml/badge.svg)](https://github.com/VinciGit00/Scrapegraph-ai/actions/workflows/pylint.yml)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![](https://dcbadge.vercel.app/api/server/gkxQDAjfeX)](https://discord.gg/gkxQDAjfeX)
 
 
-ScrapeGraphAI is a *web scraping* python library based on LangChain which uses LLM and direct graph logic to create scraping pipelines for websites and documents.
+ScrapeGraphAI is a *web scraping* python library which uses LLM and direct graph logic to create scraping pipelines for websites, documents and XML files.
 Just say which information you want to extract and the library will do it for you!
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/VinciGit00/Scrapegraph-ai/main/docs/assets/scrapegraphai_logo.png" alt="Scrapegraph-ai Logo" style="width: 50%;">
 </p>
 
 
@@ -79,28 +80,34 @@
 ### Case 1: Extracting information using a prompt
 
 You can use the `SmartScraper` class to extract information from a website using a prompt.
 
 The `SmartScraper` class is a direct graph implementation that uses the most common nodes present in a web scraping pipeline. For more information, please see the [documentation](https://scrapegraph-ai.readthedocs.io/en/latest/).
 
 ```python
-from scrapegraphai.graphs import SmartScraper
-
+from scrapegraphai.graphs import SmartScraperGraph
 OPENAI_API_KEY = "YOUR_API_KEY"
 
-llm_config = {
-    "api_key": OPENAI_API_KEY,
-    "model_name": "gpt-3.5-turbo",
+# Define the configuration for the graph
+graph_config = {
+    "llm": {
+        "api_key": OPENAI_API_KEY,
+        "model": "gpt-3.5-turbo",
+    },
 }
 
-smart_scraper = SmartScraper("List me all the titles and project descriptions",
-                             "https://perinim.github.io/projects/", llm_config)
+# Create the SmartScraperGraph instance
+smart_scraper_graph = SmartScraperGraph(
+    prompt="List me all the news with their description.",
+    file_source="https://perinim.github.io/projects/",  # also accepts a string with the already downloaded HTML code as string format
+    config=graph_config
+)
 
-answer = smart_scraper.run()
-print(answer)
+result = smart_scraper_graph.run()
+print(result)
 ```
 
 The output will be a dictionary with the extracted information, for example:
 
 ```bash
 {
     'titles': [
@@ -114,16 +121,17 @@
 
 ## 🤝 Contributing
 
 Fell free to contribute and join our Discord server to discuss with us improvements and give us suggestions!
 
 For more information, please see the [contributing guidelines](https://github.com/VinciGit00/Scrapegraph-ai/blob/main/CONTRIBUTING.md).
 
-[![My Skills](https://skillicons.dev/icons?i=discord)](https://discord.gg/DujC7HG8)
+[![My Skills](https://skillicons.dev/icons?i=discord)](https://discord.gg/gkxQDAjfeX)
 [![My Skills](https://skillicons.dev/icons?i=linkedin)](https://www.linkedin.com/company/scrapegraphai/)
+[![My Skills](https://skillicons.dev/icons?i=twitter)](https://twitter.com/scrapegraph)
 
 ## ❤️ Contributors
 [![Contributors](https://contrib.rocks/image?repo=VinciGit00/Scrapegraph-ai)](https://github.com/VinciGit00/Scrapegraph-ai/graphs/contributors)
 
 ## 🎓 Citations
 If you have used our library for research purposes please quote us with the following reference:
 ```text
```

