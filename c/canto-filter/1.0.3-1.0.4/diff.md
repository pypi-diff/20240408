# Comparing `tmp/canto-filter-1.0.3.tar.gz` & `tmp/canto-filter-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "canto-filter-1.0.3.tar", last modified: Sat Dec 23 00:19:22 2023, max compression
+gzip compressed data, was "canto-filter-1.0.4.tar", last modified: Mon Apr  8 17:38:46 2024, max compression
```

## Comparing `canto-filter-1.0.3.tar` & `canto-filter-1.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-12-23 00:19:22.460311 canto-filter-1.0.3/
--rwxrwxrwx   0 root         (0) root         (0)     1091 2023-12-22 23:56:17.000000 canto-filter-1.0.3/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)     9788 2023-12-23 00:19:22.458311 canto-filter-1.0.3/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     9018 2023-12-22 23:56:17.000000 canto-filter-1.0.3/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-12-23 00:19:22.354562 canto-filter-1.0.3/canto_filter.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     9788 2023-12-23 00:19:22.000000 canto-filter-1.0.3/canto_filter.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      334 2023-12-23 00:19:22.000000 canto-filter-1.0.3/canto_filter.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-12-23 00:19:22.000000 canto-filter-1.0.3/canto_filter.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       53 2023-12-23 00:19:22.000000 canto-filter-1.0.3/canto_filter.egg-info/entry_points.txt
--rwxrwxrwx   0 root         (0) root         (0)       18 2023-12-23 00:19:22.000000 canto-filter-1.0.3/canto_filter.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-12-23 00:19:22.412325 canto-filter-1.0.3/cantofilter/
--rwxrwxrwx   0 root         (0) root         (0)       58 2023-12-22 23:56:17.000000 canto-filter-1.0.3/cantofilter/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1395 2023-12-22 23:56:17.000000 canto-filter-1.0.3/cantofilter/cli.py
--rwxrwxrwx   0 root         (0) root         (0)     6203 2023-12-23 00:09:08.000000 canto-filter-1.0.3/cantofilter/judge.py
--rwxrwxrwx   0 root         (0) root         (0)       23 2023-12-22 23:56:17.000000 canto-filter-1.0.3/cantofilter/version.py
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-12-23 00:19:22.461312 canto-filter-1.0.3/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1578 2023-12-22 23:56:17.000000 canto-filter-1.0.3/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-12-23 00:19:22.440900 canto-filter-1.0.3/tests/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-12-22 23:56:17.000000 canto-filter-1.0.3/tests/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      859 2023-12-22 23:56:17.000000 canto-filter-1.0.3/tests/test_judge.py
+drwxr-xr-x   0 laufei   (972238) primarygroup (89939)        0 2024-04-08 17:38:46.989110 canto-filter-1.0.4/
+-rw-r--r--   0 laufei   (972238) primarygroup (89939)     1070 2023-12-08 22:39:03.000000 canto-filter-1.0.4/LICENSE
+-rw-r--r--   0 laufei   (972238) primarygroup (89939)    10004 2024-04-08 17:38:46.987827 canto-filter-1.0.4/PKG-INFO
+-rw-r--r--   0 laufei   (972238) primarygroup (89939)     9047 2024-04-08 17:32:24.000000 canto-filter-1.0.4/README.md
+drwxr-xr-x   0 laufei   (972238) primarygroup (89939)        0 2024-04-08 17:38:46.987063 canto-filter-1.0.4/canto_filter.egg-info/
+-rw-r--r--   0 laufei   (972238) primarygroup (89939)    10004 2024-04-08 17:38:46.000000 canto-filter-1.0.4/canto_filter.egg-info/PKG-INFO
+-rw-r--r--   0 laufei   (972238) primarygroup (89939)      334 2024-04-08 17:38:46.000000 canto-filter-1.0.4/canto_filter.egg-info/SOURCES.txt
+-rw-r--r--   0 laufei   (972238) primarygroup (89939)        1 2024-04-08 17:38:46.000000 canto-filter-1.0.4/canto_filter.egg-info/dependency_links.txt
+-rw-r--r--   0 laufei   (972238) primarygroup (89939)       53 2024-04-08 17:38:46.000000 canto-filter-1.0.4/canto_filter.egg-info/entry_points.txt
+-rw-r--r--   0 laufei   (972238) primarygroup (89939)       18 2024-04-08 17:38:46.000000 canto-filter-1.0.4/canto_filter.egg-info/top_level.txt
+drwxr-xr-x   0 laufei   (972238) primarygroup (89939)        0 2024-04-08 17:38:46.985150 canto-filter-1.0.4/cantofilter/
+-rw-r--r--   0 laufei   (972238) primarygroup (89939)       57 2023-12-08 23:57:19.000000 canto-filter-1.0.4/cantofilter/__init__.py
+-rw-r--r--   0 laufei   (972238) primarygroup (89939)     1354 2024-04-08 16:20:29.000000 canto-filter-1.0.4/cantofilter/cli.py
+-rw-r--r--   0 laufei   (972238) primarygroup (89939)     6659 2024-04-08 16:20:29.000000 canto-filter-1.0.4/cantofilter/judge.py
+-rw-r--r--   0 laufei   (972238) primarygroup (89939)       22 2024-04-08 16:20:29.000000 canto-filter-1.0.4/cantofilter/version.py
+-rw-r--r--   0 laufei   (972238) primarygroup (89939)       38 2024-04-08 17:38:46.989291 canto-filter-1.0.4/setup.cfg
+-rw-r--r--   0 laufei   (972238) primarygroup (89939)     1540 2023-12-11 02:48:19.000000 canto-filter-1.0.4/setup.py
+drwxr-xr-x   0 laufei   (972238) primarygroup (89939)        0 2024-04-08 17:38:46.986085 canto-filter-1.0.4/tests/
+-rw-r--r--   0 laufei   (972238) primarygroup (89939)        0 2023-12-11 02:48:19.000000 canto-filter-1.0.4/tests/__init__.py
+-rw-r--r--   0 laufei   (972238) primarygroup (89939)     1124 2024-04-08 16:20:29.000000 canto-filter-1.0.4/tests/test_judge.py
```

### Comparing `canto-filter-1.0.3/LICENSE` & `canto-filter-1.0.4/LICENSE`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 laubonghaudoi
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022 laubonghaudoi
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `canto-filter-1.0.3/PKG-INFO` & `canto-filter-1.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canto-filter
-Version: 1.0.3
+Version: 1.0.4
 Summary: 粵文分類篩選器 Cantonese text filter
 Author: CanCLID (Cantonese Computational Linguistics Infrastructure Development Workgroup)
 Author-email: support@jyutping.org
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -19,15 +19,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 粵文分類篩選器
 
-[![license](https://img.shields.io/github/license/DAVFoundation/captain-n3m0.svg?style=flat-square)](https://github.com/DAVFoundation/captain-n3m0/blob/master/LICENSE)
+[![license](https://img.shields.io/github/license/DAVFoundation/captain-n3m0.svg?style=flat-square)](https://github.com/DAVFoundation/captain-n3m0/blob/master/LICENSE) [![Publish to PyPI](https://github.com/CanCLID/canto-filter/actions/workflows/publish-to-pypi.yml/badge.svg)](https://github.com/CanCLID/canto-filter/actions/workflows/publish-to-pypi.yml)
 
 [English](https://github.com/CanCLID/cantonese-classifier#cantonese-text-classifier)
 
 ## 簡介
 
 呢個係個粵文篩選器，用嚟區分粵語同官話文本，對於篩選粵語語料好有用。個分類器會將輸入文本分成四類:
 
@@ -91,28 +91,28 @@
 cantofilter --input input.txt > output.txt
 ```
 
 噉樣會得到一個 `output.txt`，入面有由 \t 分成嘅兩列，第一列係判斷標籤，第二列係句子原文本。
 
 #### 僅輸出一類
 
-如果你想直接篩選出某一類嘅文本，噉可以加一個 `--type <LABEL>` 參數喺後面，例如
+如果你想直接篩選出某一類嘅文本，噉可以加一個 `--mode <LABEL>` 參數喺後面，例如
 
 ```bash
-cantofilter main.py --input input.txt --type cantonese > output.txt
+cantofilter main.py --input input.txt --mode cantonese > output.txt
 ```
 
-噉樣輸出嘅 `output.txt` 就會係純粵文句子。如果想剩係要官話、官粵混合或者中性文本，將個 `--type` 參數定成 `mandarin`、`mixed`、`neutral`就得。
+噉樣輸出嘅 `output.txt` 就會係純粵文句子。如果想剩係要官話、官粵混合或者中性文本，將個 `--mode` 參數定成 `mandarin`、`mixed`、`neutral`就得。
 
 #### 僅輸出標籤
 
-你亦都可以剩係輸出啲句子嘅分類結果，用 `--type label` 就得：
+你亦都可以剩係輸出啲句子嘅分類結果，用 `--mode label` 就得：
 
 ```bash
-cantofilter main.py --input input.txt --type label > output.txt
+cantofilter main.py --input input.txt --model label > output.txt
 ```
 
 噉樣嘅 `output.txt` 剩得一列，全部都係分類標籤。
 
 ## 依賴
 
 Python >= 3.6
@@ -183,28 +183,28 @@
 cantofilter --input input.txt > output.txt
 ```
 
 There will be a `output.txt` which has two columns. The first column is the language label, and the second column is the original input text.
 
 #### Output only text of one class
 
-If you want only one type of text, use the `--type <LABEL>` argument. Say if you want pure Cantonese text only:
+If you want only one class of text, use the `--mode <LABEL>` argument. Say if you want pure Cantonese text only:
 
 ```bash
-cantofilter --input input.txt --type cantonese > output.txt
+cantofilter --input input.txt --mode cantonese > output.txt
 ```
 
 The `output.txt` will contain only Cantonese text.
 
 #### Output label only
 
-If you want the classification labels, use `--type label` like this:
+If you want to include the classification labels in the output, use `--mode label` like this:
 
 ```bash
-cantofilter main.py --input input.txt --type label > output.txt
+cantofilter main.py --input input.txt --mode label > output.txt
 ```
 
 Then your `output.txt` will contain only classification results of the input sentences.
 
 ## Requirement
 
 Python >= 3.6
```

### Comparing `canto-filter-1.0.3/README.md` & `canto-filter-1.0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,187 +1,187 @@
-# 粵文分類篩選器
-
-[![license](https://img.shields.io/github/license/DAVFoundation/captain-n3m0.svg?style=flat-square)](https://github.com/DAVFoundation/captain-n3m0/blob/master/LICENSE)
-
-[English](https://github.com/CanCLID/cantonese-classifier#cantonese-text-classifier)
-
-## 簡介
-
-呢個係個粵文篩選器，用嚟區分粵語同官話文本，對於篩選粵語語料好有用。個分類器會將輸入文本分成四類:
-
-1. `cantonese`: 純粵文，僅含有粵語特徵字詞，例如“你喺邊度”
-1. `mandarin`: 純官話文，僅含有官話特徵字詞，例如“你在哪裏”
-1. `mixed`：官粵混雜文，同時含有官話同粵語特徵嘅字詞，例如“是咁的”
-1. `neutral`：無特徵漢語文，唔含有官話同粵語特徵，既可以當成粵文亦可以當成官話文，例如“去學校讀書”
-
-分類方法係官話同粵語嘅特徵字詞識別。如果同時含有官話同粵語特徵詞彙就算官粵混雜，如果唔含有任何特徵，就算冇特徵中性文本。
-
-### 設計思想同假設
-
-本篩選器嘅主要設計目標係「篩選出可以用作訓練數據嘅優質粵文」，而非「準確分類輸入文本」。所以喺判斷粵語/官話嗰陣會用偏嚴格嘅判別標準，即係會犧牲 recall 嚟換取高 precision （寧願篩漏粵文句子都唔好將官話文誤判成粵文）。
-
-本篩選器**默認所有輸入文本都用[推薦用字方案](https://jyutping.org/blog/typo/)書寫**。如果輸入文本採用其他用字方案（有錯別字），會影響分類篩選結果。例如輸入`畀本書我`分類器會輸出`cantonese`，但寫成`比本書我`會輸出`neutral`。你可以用[錯別字修正器](https://github.com/CanCLID/typo-corrector)嚟清洗被分成`neutral`嘅文本，噉樣可能會得到更多粵文。
-
-呢隻篩選器**默認所有輸入文本都係傳統漢字**。如果要分類簡化字文本，要將佢哋轉化成傳統漢字先。推薦使用 [OpenCC](https://github.com/BYVoid/OpenCC)嚟轉換。
-
-### 引用本篩選器
-
-本工具以字詞特徵抽出「純粵文」文本嘅策略同埋實踐方式。呢個策略首先喺以下場合提出。討論本分類器時，請引用：
-
-Lau, Chaak Ming (劉擇明). 2022. Lingusitic features and automatic detection of Hong Kong-style Written Chinese and Cantonese Writing (港式書面語和粵語書寫的語言學特徵和自動辨識). Paper presented at the 26th International Conference of Yue Dialects (第二十六屆國際粵方言研討會).
-
-「粵文」同「官話文」嘅定義同界線取決於使用者嘅語言意識形態，呢度嘅分類方法以下文所描述嘅粵文書寫體作為基礎。討論本工具採取嘅分類準則，請引用：
-
-Lau, Chaak Ming. 2024. Ideologically driven divergence in Cantonese vernacular writing practices. In J.-F. Dupré, editor, _Politics of Language in Hong Kong_, Routledge.
-
-## 用法
-
-首先用 pip 安裝
-
-```bash
-pip install canto-filter
-```
-
-你可以喺 Python 代碼入面用，亦都可以直接喺命令行入面用。
-
-### Python 函數用法
-
-本篩選器剩得一個函數 `judge()`，輸入一句話輸出佢嘅語言分類：
-
-```python
-from cantofilter import judge
-
-print(judge('你喺邊度')) # cantonese
-print(judge('你在哪裏')) # mandarin
-print(judge('是咁的'))  # mixed
-print(judge('去學校讀書'))  # neutral
-```
-
-### 命令行用法
-
-首先要有一個輸入文檔，例如`input.txt`，入面每行一個句子.
-
-#### 輸出標籤同原文
-
-然後運行下面命令
-
-```bash
-cantofilter --input input.txt > output.txt
-```
-
-噉樣會得到一個 `output.txt`，入面有由 \t 分成嘅兩列，第一列係判斷標籤，第二列係句子原文本。
-
-#### 僅輸出一類
-
-如果你想直接篩選出某一類嘅文本，噉可以加一個 `--type <LABEL>` 參數喺後面，例如
-
-```bash
-cantofilter main.py --input input.txt --type cantonese > output.txt
-```
-
-噉樣輸出嘅 `output.txt` 就會係純粵文句子。如果想剩係要官話、官粵混合或者中性文本，將個 `--type` 參數定成 `mandarin`、`mixed`、`neutral`就得。
-
-#### 僅輸出標籤
-
-你亦都可以剩係輸出啲句子嘅分類結果，用 `--type label` 就得：
-
-```bash
-cantofilter main.py --input input.txt --type label > output.txt
-```
-
-噉樣嘅 `output.txt` 剩得一列，全部都係分類標籤。
-
-## 依賴
-
-Python >= 3.6
-
-# Cantonese text filter
-
-## Overview
-
-This is a text filter for Cantonese, designed for filtering Cantonese text corpus. It classifies input sentences with four output labels:
-
-1. `cantonese`: Pure Cantonese text, contains Cantonese-featured words. E.g. 你喺邊度
-1. `mandarin`: Pure Mandarin text, contains Mandarin-feature words. E.g. 你在哪裏
-1. `mixed`：Mixed Cantonese-Mandarin text, contains both Cantonese and Mandarin-featured words. E.g. 是咁的
-1. `neutral`：No feature Chinese text, contains neither Cantonese nor Mandarin feature words. Such sentences can be used for both Cantonese and Mandarin text corpus. E.g. 去學校讀書
-
-The filter is regex rule-based, by detecting Mandarin and Cantonese feature characters and words. If a sentence contains both Cantonese and Mandarin feature words, then it is a mixed-Cantonese-Mandarin sentence. If it contains neither features, it is a no-feature, neutral Chinese text.
-
-### Design priciples and assumptions
-
-This filter is designed for the purpose of "obtaining high-quality Cantonese text", as opposed to "accurately classifying input texts". Therefore, it maximizes precision at the price of recall, to minimize the false positive rate / avoid including potential Mandarin sentences (we rather miss some Cantonese sentences, than mistaking potential Mandarin sentences as Cantonese).
-
-This filter **assumes all input text written in [the recommended orthography](https://jyutping.org/blog/typo/)**. Spelling errors or typos in input text might affect the classification result. For instance, `畀本書我` yields `cantonese`, while `比本書我` yields `neutral`. You can use the [spelling corrector](https://github.com/CanCLID/typo-corrector) to correct the `neutral` text, which might give you more Cantonese text.
-
-This filter **assumes all input text in Traditional Chinese characters**. If you want to filter texts written in simplified characters, please convert them into Traditional characters first. We recommend using [OpenCC](https://github.com/BYVoid/OpenCC) to do the conversion.
-
-### Citing this package
-
-The implementation and methodology of this filter was first proposed in the following contexts. below. When discussing this filter, please cite:
-
-Lau, Chaak Ming (劉擇明). 2022. Lingusitic features and automatic detection of Hong Kong-style Written Chinese and Cantonese Writing (港式書面語和粵語書寫的語言學特徵和自動辨識). Paper presented at the 26th International Conference of Yue Dialects (第二十六屆國際粵方言研討會).
-
-The definitions and boundaries of 'Cantonese text' and 'Mandarin text' depend on the user's language ideology. The classification method used here is based on the Cantonese written style described in the following text. When discussing the criteria adopted by this tool, please cite:
-
-Lau, Chaak Ming. 2024. Ideologically driven divergence in Cantonese vernacular writing practices. In J.-F. Dupré, editor, _Politics of Language in Hong Kong_, Routledge.
-
-## How to use
-
-Install the package with pip first
-
-```bash
-pip install canto-filter
-```
-
-This package can be used in python codes, or as a CLI tool.
-
-### Python function usage
-
-There is only one function in this package, `judge()`, which accepts a string input and outputs one of the labels:
-
-```python
-from cantofilter import judge
-
-print(judge('你喺邊度')) # cantonese
-print(judge('你在哪裏')) # mandarin
-print(judge('是咁的'))  # mixed
-print(judge('去學校讀書'))  # neutral
-```
-
-### CLI usage
-
-Assume an input text file, e.g. `input.txt` where each line is a sentence.
-
-#### Output both labels and original texts
-
-Then run
-
-```bash
-cantofilter --input input.txt > output.txt
-```
-
-There will be a `output.txt` which has two columns. The first column is the language label, and the second column is the original input text.
-
-#### Output only text of one class
-
-If you want only one type of text, use the `--type <LABEL>` argument. Say if you want pure Cantonese text only:
-
-```bash
-cantofilter --input input.txt --type cantonese > output.txt
-```
-
-The `output.txt` will contain only Cantonese text.
-
-#### Output label only
-
-If you want the classification labels, use `--type label` like this:
-
-```bash
-cantofilter main.py --input input.txt --type label > output.txt
-```
-
-Then your `output.txt` will contain only classification results of the input sentences.
-
-## Requirement
-
-Python >= 3.6
+# 粵文分類篩選器
+
+[![license](https://img.shields.io/github/license/DAVFoundation/captain-n3m0.svg?style=flat-square)](https://github.com/DAVFoundation/captain-n3m0/blob/master/LICENSE) [![Publish to PyPI](https://github.com/CanCLID/canto-filter/actions/workflows/publish-to-pypi.yml/badge.svg)](https://github.com/CanCLID/canto-filter/actions/workflows/publish-to-pypi.yml)
+
+[English](https://github.com/CanCLID/cantonese-classifier#cantonese-text-classifier)
+
+## 簡介
+
+呢個係個粵文篩選器，用嚟區分粵語同官話文本，對於篩選粵語語料好有用。個分類器會將輸入文本分成四類:
+
+1. `cantonese`: 純粵文，僅含有粵語特徵字詞，例如“你喺邊度”
+1. `mandarin`: 純官話文，僅含有官話特徵字詞，例如“你在哪裏”
+1. `mixed`：官粵混雜文，同時含有官話同粵語特徵嘅字詞，例如“是咁的”
+1. `neutral`：無特徵漢語文，唔含有官話同粵語特徵，既可以當成粵文亦可以當成官話文，例如“去學校讀書”
+
+分類方法係官話同粵語嘅特徵字詞識別。如果同時含有官話同粵語特徵詞彙就算官粵混雜，如果唔含有任何特徵，就算冇特徵中性文本。
+
+### 設計思想同假設
+
+本篩選器嘅主要設計目標係「篩選出可以用作訓練數據嘅優質粵文」，而非「準確分類輸入文本」。所以喺判斷粵語/官話嗰陣會用偏嚴格嘅判別標準，即係會犧牲 recall 嚟換取高 precision （寧願篩漏粵文句子都唔好將官話文誤判成粵文）。
+
+本篩選器**默認所有輸入文本都用[推薦用字方案](https://jyutping.org/blog/typo/)書寫**。如果輸入文本採用其他用字方案（有錯別字），會影響分類篩選結果。例如輸入`畀本書我`分類器會輸出`cantonese`，但寫成`比本書我`會輸出`neutral`。你可以用[錯別字修正器](https://github.com/CanCLID/typo-corrector)嚟清洗被分成`neutral`嘅文本，噉樣可能會得到更多粵文。
+
+呢隻篩選器**默認所有輸入文本都係傳統漢字**。如果要分類簡化字文本，要將佢哋轉化成傳統漢字先。推薦使用 [OpenCC](https://github.com/BYVoid/OpenCC)嚟轉換。
+
+### 引用本篩選器
+
+本工具以字詞特徵抽出「純粵文」文本嘅策略同埋實踐方式。呢個策略首先喺以下場合提出。討論本分類器時，請引用：
+
+Lau, Chaak Ming (劉擇明). 2022. Lingusitic features and automatic detection of Hong Kong-style Written Chinese and Cantonese Writing (港式書面語和粵語書寫的語言學特徵和自動辨識). Paper presented at the 26th International Conference of Yue Dialects (第二十六屆國際粵方言研討會).
+
+「粵文」同「官話文」嘅定義同界線取決於使用者嘅語言意識形態，呢度嘅分類方法以下文所描述嘅粵文書寫體作為基礎。討論本工具採取嘅分類準則，請引用：
+
+Lau, Chaak Ming. 2024. Ideologically driven divergence in Cantonese vernacular writing practices. In J.-F. Dupré, editor, _Politics of Language in Hong Kong_, Routledge.
+
+## 用法
+
+首先用 pip 安裝
+
+```bash
+pip install canto-filter
+```
+
+你可以喺 Python 代碼入面用，亦都可以直接喺命令行入面用。
+
+### Python 函數用法
+
+本篩選器剩得一個函數 `judge()`，輸入一句話輸出佢嘅語言分類：
+
+```python
+from cantofilter import judge
+
+print(judge('你喺邊度')) # cantonese
+print(judge('你在哪裏')) # mandarin
+print(judge('是咁的'))  # mixed
+print(judge('去學校讀書'))  # neutral
+```
+
+### 命令行用法
+
+首先要有一個輸入文檔，例如`input.txt`，入面每行一個句子.
+
+#### 輸出標籤同原文
+
+然後運行下面命令
+
+```bash
+cantofilter --input input.txt > output.txt
+```
+
+噉樣會得到一個 `output.txt`，入面有由 \t 分成嘅兩列，第一列係判斷標籤，第二列係句子原文本。
+
+#### 僅輸出一類
+
+如果你想直接篩選出某一類嘅文本，噉可以加一個 `--mode <LABEL>` 參數喺後面，例如
+
+```bash
+cantofilter main.py --input input.txt --mode cantonese > output.txt
+```
+
+噉樣輸出嘅 `output.txt` 就會係純粵文句子。如果想剩係要官話、官粵混合或者中性文本，將個 `--mode` 參數定成 `mandarin`、`mixed`、`neutral`就得。
+
+#### 僅輸出標籤
+
+你亦都可以剩係輸出啲句子嘅分類結果，用 `--mode label` 就得：
+
+```bash
+cantofilter main.py --input input.txt --model label > output.txt
+```
+
+噉樣嘅 `output.txt` 剩得一列，全部都係分類標籤。
+
+## 依賴
+
+Python >= 3.6
+
+# Cantonese text filter
+
+## Overview
+
+This is a text filter for Cantonese, designed for filtering Cantonese text corpus. It classifies input sentences with four output labels:
+
+1. `cantonese`: Pure Cantonese text, contains Cantonese-featured words. E.g. 你喺邊度
+1. `mandarin`: Pure Mandarin text, contains Mandarin-feature words. E.g. 你在哪裏
+1. `mixed`：Mixed Cantonese-Mandarin text, contains both Cantonese and Mandarin-featured words. E.g. 是咁的
+1. `neutral`：No feature Chinese text, contains neither Cantonese nor Mandarin feature words. Such sentences can be used for both Cantonese and Mandarin text corpus. E.g. 去學校讀書
+
+The filter is regex rule-based, by detecting Mandarin and Cantonese feature characters and words. If a sentence contains both Cantonese and Mandarin feature words, then it is a mixed-Cantonese-Mandarin sentence. If it contains neither features, it is a no-feature, neutral Chinese text.
+
+### Design priciples and assumptions
+
+This filter is designed for the purpose of "obtaining high-quality Cantonese text", as opposed to "accurately classifying input texts". Therefore, it maximizes precision at the price of recall, to minimize the false positive rate / avoid including potential Mandarin sentences (we rather miss some Cantonese sentences, than mistaking potential Mandarin sentences as Cantonese).
+
+This filter **assumes all input text written in [the recommended orthography](https://jyutping.org/blog/typo/)**. Spelling errors or typos in input text might affect the classification result. For instance, `畀本書我` yields `cantonese`, while `比本書我` yields `neutral`. You can use the [spelling corrector](https://github.com/CanCLID/typo-corrector) to correct the `neutral` text, which might give you more Cantonese text.
+
+This filter **assumes all input text in Traditional Chinese characters**. If you want to filter texts written in simplified characters, please convert them into Traditional characters first. We recommend using [OpenCC](https://github.com/BYVoid/OpenCC) to do the conversion.
+
+### Citing this package
+
+The implementation and methodology of this filter was first proposed in the following contexts. below. When discussing this filter, please cite:
+
+Lau, Chaak Ming (劉擇明). 2022. Lingusitic features and automatic detection of Hong Kong-style Written Chinese and Cantonese Writing (港式書面語和粵語書寫的語言學特徵和自動辨識). Paper presented at the 26th International Conference of Yue Dialects (第二十六屆國際粵方言研討會).
+
+The definitions and boundaries of 'Cantonese text' and 'Mandarin text' depend on the user's language ideology. The classification method used here is based on the Cantonese written style described in the following text. When discussing the criteria adopted by this tool, please cite:
+
+Lau, Chaak Ming. 2024. Ideologically driven divergence in Cantonese vernacular writing practices. In J.-F. Dupré, editor, _Politics of Language in Hong Kong_, Routledge.
+
+## How to use
+
+Install the package with pip first
+
+```bash
+pip install canto-filter
+```
+
+This package can be used in python codes, or as a CLI tool.
+
+### Python function usage
+
+There is only one function in this package, `judge()`, which accepts a string input and outputs one of the labels:
+
+```python
+from cantofilter import judge
+
+print(judge('你喺邊度')) # cantonese
+print(judge('你在哪裏')) # mandarin
+print(judge('是咁的'))  # mixed
+print(judge('去學校讀書'))  # neutral
+```
+
+### CLI usage
+
+Assume an input text file, e.g. `input.txt` where each line is a sentence.
+
+#### Output both labels and original texts
+
+Then run
+
+```bash
+cantofilter --input input.txt > output.txt
+```
+
+There will be a `output.txt` which has two columns. The first column is the language label, and the second column is the original input text.
+
+#### Output only text of one class
+
+If you want only one class of text, use the `--mode <LABEL>` argument. Say if you want pure Cantonese text only:
+
+```bash
+cantofilter --input input.txt --mode cantonese > output.txt
+```
+
+The `output.txt` will contain only Cantonese text.
+
+#### Output label only
+
+If you want to include the classification labels in the output, use `--mode label` like this:
+
+```bash
+cantofilter main.py --input input.txt --mode label > output.txt
+```
+
+Then your `output.txt` will contain only classification results of the input sentences.
+
+## Requirement
+
+Python >= 3.6
```

### Comparing `canto-filter-1.0.3/canto_filter.egg-info/PKG-INFO` & `canto-filter-1.0.4/canto_filter.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canto-filter
-Version: 1.0.3
+Version: 1.0.4
 Summary: 粵文分類篩選器 Cantonese text filter
 Author: CanCLID (Cantonese Computational Linguistics Infrastructure Development Workgroup)
 Author-email: support@jyutping.org
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -19,15 +19,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 粵文分類篩選器
 
-[![license](https://img.shields.io/github/license/DAVFoundation/captain-n3m0.svg?style=flat-square)](https://github.com/DAVFoundation/captain-n3m0/blob/master/LICENSE)
+[![license](https://img.shields.io/github/license/DAVFoundation/captain-n3m0.svg?style=flat-square)](https://github.com/DAVFoundation/captain-n3m0/blob/master/LICENSE) [![Publish to PyPI](https://github.com/CanCLID/canto-filter/actions/workflows/publish-to-pypi.yml/badge.svg)](https://github.com/CanCLID/canto-filter/actions/workflows/publish-to-pypi.yml)
 
 [English](https://github.com/CanCLID/cantonese-classifier#cantonese-text-classifier)
 
 ## 簡介
 
 呢個係個粵文篩選器，用嚟區分粵語同官話文本，對於篩選粵語語料好有用。個分類器會將輸入文本分成四類:
 
@@ -91,28 +91,28 @@
 cantofilter --input input.txt > output.txt
 ```
 
 噉樣會得到一個 `output.txt`，入面有由 \t 分成嘅兩列，第一列係判斷標籤，第二列係句子原文本。
 
 #### 僅輸出一類
 
-如果你想直接篩選出某一類嘅文本，噉可以加一個 `--type <LABEL>` 參數喺後面，例如
+如果你想直接篩選出某一類嘅文本，噉可以加一個 `--mode <LABEL>` 參數喺後面，例如
 
 ```bash
-cantofilter main.py --input input.txt --type cantonese > output.txt
+cantofilter main.py --input input.txt --mode cantonese > output.txt
 ```
 
-噉樣輸出嘅 `output.txt` 就會係純粵文句子。如果想剩係要官話、官粵混合或者中性文本，將個 `--type` 參數定成 `mandarin`、`mixed`、`neutral`就得。
+噉樣輸出嘅 `output.txt` 就會係純粵文句子。如果想剩係要官話、官粵混合或者中性文本，將個 `--mode` 參數定成 `mandarin`、`mixed`、`neutral`就得。
 
 #### 僅輸出標籤
 
-你亦都可以剩係輸出啲句子嘅分類結果，用 `--type label` 就得：
+你亦都可以剩係輸出啲句子嘅分類結果，用 `--mode label` 就得：
 
 ```bash
-cantofilter main.py --input input.txt --type label > output.txt
+cantofilter main.py --input input.txt --model label > output.txt
 ```
 
 噉樣嘅 `output.txt` 剩得一列，全部都係分類標籤。
 
 ## 依賴
 
 Python >= 3.6
@@ -183,28 +183,28 @@
 cantofilter --input input.txt > output.txt
 ```
 
 There will be a `output.txt` which has two columns. The first column is the language label, and the second column is the original input text.
 
 #### Output only text of one class
 
-If you want only one type of text, use the `--type <LABEL>` argument. Say if you want pure Cantonese text only:
+If you want only one class of text, use the `--mode <LABEL>` argument. Say if you want pure Cantonese text only:
 
 ```bash
-cantofilter --input input.txt --type cantonese > output.txt
+cantofilter --input input.txt --mode cantonese > output.txt
 ```
 
 The `output.txt` will contain only Cantonese text.
 
 #### Output label only
 
-If you want the classification labels, use `--type label` like this:
+If you want to include the classification labels in the output, use `--mode label` like this:
 
 ```bash
-cantofilter main.py --input input.txt --type label > output.txt
+cantofilter main.py --input input.txt --mode label > output.txt
 ```
 
 Then your `output.txt` will contain only classification results of the input sentences.
 
 ## Requirement
 
 Python >= 3.6
```

### Comparing `canto-filter-1.0.3/setup.py` & `canto-filter-1.0.4/setup.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-from setuptools import setup, find_packages
-from cantofilter import __version__
-
-# Read the contents of your README file
-with open("README.md", "r", encoding="utf-8") as fh:
-    long_description = fh.read()
-
-    setup(
-        name="canto-filter",
-        version=__version__,
-        author="CanCLID (Cantonese Computational Linguistics Infrastructure Development Workgroup)",
-        author_email="support@jyutping.org",
-        description="粵文分類篩選器 Cantonese text filter",
-        long_description=long_description,
-        long_description_content_type="text/markdown",
-        packages=find_packages(),
-        classifiers=[
-            "Programming Language :: Python :: 3",
-            "Programming Language :: Python :: 3.6",
-            "Programming Language :: Python :: 3.7",
-            "Programming Language :: Python :: 3.8",
-            "Programming Language :: Python :: 3.9",
-            "Programming Language :: Python :: 3.10",
-            "Programming Language :: Python :: 3.11",
-            "Programming Language :: Python :: 3.12",
-            "License :: OSI Approved :: MIT License",
-            "Intended Audience :: Developers",
-            "Topic :: Text Processing :: Linguistic",
-            "Natural Language :: Cantonese",
-            "Operating System :: OS Independent",
-        ],
-        python_requires=">=3.6",
-        entry_points={
-            "console_scripts": [
-                "cantofilter=cantofilter.cli:main",  # 'command=package.module:function'
-            ],
-        },
-    )
+from setuptools import setup, find_packages
+from cantofilter import __version__
+
+# Read the contents of your README file
+with open("README.md", "r", encoding="utf-8") as fh:
+    long_description = fh.read()
+
+    setup(
+        name="canto-filter",
+        version=__version__,
+        author="CanCLID (Cantonese Computational Linguistics Infrastructure Development Workgroup)",
+        author_email="support@jyutping.org",
+        description="粵文分類篩選器 Cantonese text filter",
+        long_description=long_description,
+        long_description_content_type="text/markdown",
+        packages=find_packages(),
+        classifiers=[
+            "Programming Language :: Python :: 3",
+            "Programming Language :: Python :: 3.6",
+            "Programming Language :: Python :: 3.7",
+            "Programming Language :: Python :: 3.8",
+            "Programming Language :: Python :: 3.9",
+            "Programming Language :: Python :: 3.10",
+            "Programming Language :: Python :: 3.11",
+            "Programming Language :: Python :: 3.12",
+            "License :: OSI Approved :: MIT License",
+            "Intended Audience :: Developers",
+            "Topic :: Text Processing :: Linguistic",
+            "Natural Language :: Cantonese",
+            "Operating System :: OS Independent",
+        ],
+        python_requires=">=3.6",
+        entry_points={
+            "console_scripts": [
+                "cantofilter=cantofilter.cli:main",  # 'command=package.module:function'
+            ],
+        },
+    )
```

