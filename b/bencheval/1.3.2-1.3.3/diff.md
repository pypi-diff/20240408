# Comparing `tmp/bencheval-1.3.2.tar.gz` & `tmp/bencheval-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bencheval-1.3.2.tar", last modified: Tue Apr  2 13:58:06 2024, max compression
+gzip compressed data, was "bencheval-1.3.3.tar", last modified: Mon Apr  8 13:06:14 2024, max compression
```

## Comparing `bencheval-1.3.2.tar` & `bencheval-1.3.3.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-04-02 13:58:06.409004 bencheval-1.3.2/
--rw-r--r--   0 gzhang    (3204)     1040     1068 2024-03-18 09:00:38.000000 bencheval-1.3.2/LICENSE.txt
--rw-r--r--   0 gzhang    (3204)     1040       52 2024-03-18 09:00:38.000000 bencheval-1.3.2/MANIFEST.in
--rw-r--r--   0 gzhang    (3204)     1040     3315 2024-04-02 13:58:06.408818 bencheval-1.3.2/PKG-INFO
--rw-r--r--   0 gzhang    (3204)     1040     2282 2024-03-18 09:00:38.000000 bencheval-1.3.2/README.md
-drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-04-02 13:58:06.396232 bencheval-1.3.2/bencheval/
--rw-r--r--   0 gzhang    (3204)     1040        0 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/__init__.py
-drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-04-02 13:58:06.396932 bencheval-1.3.2/bencheval/data/
--rw-r--r--   0 gzhang    (3204)     1040     4171 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/__init__.py
-drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-04-02 13:58:06.397188 bencheval-1.3.2/bencheval/data/__pycache__/
--rw-r--r--   0 gzhang    (3204)     1040     5711 2024-03-27 13:57:41.000000 bencheval-1.3.2/bencheval/data/__pycache__/__init__.cpython-311.pyc
-drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-04-02 13:58:06.398193 bencheval-1.3.2/bencheval/data/bbh/
--rw-r--r--   0 gzhang    (3204)     1040      208 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/bbh/__init__.py
--rw-r--r--   0 gzhang    (3204)     1040      636 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/bbh/cols.txt
--rw-r--r--   0 gzhang    (3204)     1040      542 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/bbh/format.py
--rw-r--r--   0 gzhang    (3204)     1040    18964 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/bbh/leaderboard.tsv
--rw-r--r--   0 gzhang    (3204)     1040     1021 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/bbh/statistic.py
--rw-r--r--   0 gzhang    (3204)     1040    18436 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/bbh/vanilla.tsv
-drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-04-02 13:58:06.398764 bencheval-1.3.2/bencheval/data/bigcode/
--rw-r--r--   0 gzhang    (3204)     1040      338 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/bigcode/__init__.py
--rw-r--r--   0 gzhang    (3204)     1040      430 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/bigcode/format.py
--rw-r--r--   0 gzhang    (3204)     1040     2169 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/bigcode/leaderboard.tsv
--rw-r--r--   0 gzhang    (3204)     1040     2226 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/bigcode/vanilla.txt
-drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-04-02 13:58:06.398895 bencheval-1.3.2/bencheval/data/dummy/
--rw-r--r--   0 gzhang    (3204)     1040     1404 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/dummy/__init__.py
-drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-04-02 13:58:06.399303 bencheval-1.3.2/bencheval/data/glue/
--rw-r--r--   0 gzhang    (3204)     1040     1077 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/glue/__init__.py
--rw-r--r--   0 gzhang    (3204)     1040     9876 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/glue/leaderboard.tsv
-drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-04-02 13:58:06.401373 bencheval-1.3.2/bencheval/data/heim/
--rw-r--r--   0 gzhang    (3204)     1040      767 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/heim/__init__.py
--rw-r--r--   0 gzhang    (3204)     1040    13934 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/heim/aesthetics_auto.tsv
--rw-r--r--   0 gzhang    (3204)     1040     5206 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/heim/aesthetics_human.tsv
--rw-r--r--   0 gzhang    (3204)     1040    10394 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/heim/alignment_auto.tsv
--rw-r--r--   0 gzhang    (3204)     1040     5830 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/heim/alignment_human.tsv
--rw-r--r--   0 gzhang    (3204)     1040     3765 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/heim/black_out.tsv
--rw-r--r--   0 gzhang    (3204)     1040     4494 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/heim/nsfw.tsv
--rw-r--r--   0 gzhang    (3204)     1040     4809 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/heim/nudity.tsv
--rw-r--r--   0 gzhang    (3204)     1040     3643 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/heim/originality.tsv
--rw-r--r--   0 gzhang    (3204)     1040     3343 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/heim/quality_auto.tsv
--rw-r--r--   0 gzhang    (3204)     1040     2554 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/heim/quality_human.tsv
-drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-04-02 13:58:06.403214 bencheval-1.3.2/bencheval/data/helm/
--rw-r--r--   0 gzhang    (3204)     1040      890 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/helm/__init__.py
--rw-r--r--   0 gzhang    (3204)     1040     7516 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/helm/accuracy.tsv
--rw-r--r--   0 gzhang    (3204)     1040    14741 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/helm/bias.tsv
--rw-r--r--   0 gzhang    (3204)     1040     5563 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/helm/calibration.tsv
--rw-r--r--   0 gzhang    (3204)     1040     5858 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/helm/efficiency.tsv
--rw-r--r--   0 gzhang    (3204)     1040     6993 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/helm/fairness.tsv
--rw-r--r--   0 gzhang    (3204)     1040     7035 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/helm/robustness.tsv
--rw-r--r--   0 gzhang    (3204)     1040     6495 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/helm/summarization.tsv
--rw-r--r--   0 gzhang    (3204)     1040     4663 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/helm/toxicity.tsv
-drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-04-02 13:58:06.404636 bencheval-1.3.2/bencheval/data/imagenet/
--rw-r--r--   0 gzhang    (3204)     1040     1435 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/imagenet/__init__.py
--rw-r--r--   0 gzhang    (3204)     1040     1058 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/imagenet/format.py
--rw-r--r--   0 gzhang    (3204)     1040   554910 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/imagenet/leaderboard.tsv
--rw-r--r--   0 gzhang    (3204)     1040     7562 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/imagenet/leaderboard_raw.tsv
--rw-r--r--   0 gzhang    (3204)     1040    11304 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/imagenet/run.sh
--rw-r--r--   0 gzhang    (3204)     1040     2587 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/imagenet/run_imagenet.py
--rw-r--r--   0 gzhang    (3204)     1040     8324 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/imagenet/vanilla.txt
-drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-04-02 13:58:06.405220 bencheval-1.3.2/bencheval/data/mmlu/
--rw-r--r--   0 gzhang    (3204)     1040      367 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/mmlu/__init__.py
--rw-r--r--   0 gzhang    (3204)     1040     2113 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/mmlu/format.py
--rw-r--r--   0 gzhang    (3204)     1040   101533 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/mmlu/leaderboard.tsv
--rw-r--r--   0 gzhang    (3204)     1040     5831 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/mmlu/leaderboard_raw.csv
-drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-04-02 13:58:06.405966 bencheval-1.3.2/bencheval/data/mteb/
--rw-r--r--   0 gzhang    (3204)     1040      810 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/mteb/__init__.py
--rw-r--r--   0 gzhang    (3204)     1040      430 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/mteb/format.py
--rw-r--r--   0 gzhang    (3204)     1040     7313 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/mteb/leaderboard.tsv
--rw-r--r--   0 gzhang    (3204)     1040     7199 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/mteb/vanilla.txt
-drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-04-02 13:58:06.406839 bencheval-1.3.2/bencheval/data/openllm/
--rw-r--r--   0 gzhang    (3204)     1040      456 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/openllm/__init__.py
--rw-r--r--   0 gzhang    (3204)     1040      431 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/openllm/format.py
--rw-r--r--   0 gzhang    (3204)     1040     7511 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/openllm/leaderboard.tsv
--rw-r--r--   0 gzhang    (3204)     1040      196 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/openllm/statistic.py
--rw-r--r--   0 gzhang    (3204)     1040     8119 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/openllm/vanilla.txt
-drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-04-02 13:58:06.407196 bencheval-1.3.2/bencheval/data/superglue/
--rw-r--r--   0 gzhang    (3204)     1040      958 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/superglue/__init__.py
--rw-r--r--   0 gzhang    (3204)     1040     3297 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/superglue/leaderboard.tsv
-drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-04-02 13:58:06.407429 bencheval-1.3.2/bencheval/data/vtab/
--rw-r--r--   0 gzhang    (3204)     1040      331 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/vtab/__init__.py
--rw-r--r--   0 gzhang    (3204)     1040     1970 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/data/vtab/leaderboard.tsv
-drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-04-02 13:58:06.407779 bencheval-1.3.2/bencheval/measures/
--rw-r--r--   0 gzhang    (3204)     1040     4697 2024-04-02 13:14:28.000000 bencheval-1.3.2/bencheval/measures/cardinal.py
--rw-r--r--   0 gzhang    (3204)     1040     5334 2024-04-02 11:52:38.000000 bencheval-1.3.2/bencheval/measures/ordinal.py
-drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-04-02 13:58:06.408467 bencheval-1.3.2/bencheval/utils/
--rw-r--r--   0 gzhang    (3204)     1040        0 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/utils/__init__.py
--rw-r--r--   0 gzhang    (3204)     1040     2077 2024-04-02 11:55:56.000000 bencheval-1.3.2/bencheval/utils/base.py
--rw-r--r--   0 gzhang    (3204)     1040     4158 2024-03-19 15:00:57.000000 bencheval-1.3.2/bencheval/utils/metric.py
--rw-r--r--   0 gzhang    (3204)     1040     1358 2024-03-16 13:21:55.000000 bencheval-1.3.2/bencheval/utils/win_rate.py
-drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-04-02 13:58:06.408619 bencheval-1.3.2/bencheval.egg-info/
--rw-r--r--   0 gzhang    (3204)     1040     3315 2024-04-02 13:58:06.000000 bencheval-1.3.2/bencheval.egg-info/PKG-INFO
--rw-r--r--   0 gzhang    (3204)     1040     2480 2024-04-02 13:58:06.000000 bencheval-1.3.2/bencheval.egg-info/SOURCES.txt
--rw-r--r--   0 gzhang    (3204)     1040        1 2024-04-02 13:58:06.000000 bencheval-1.3.2/bencheval.egg-info/dependency_links.txt
--rw-r--r--   0 gzhang    (3204)     1040       62 2024-04-02 13:58:06.000000 bencheval-1.3.2/bencheval.egg-info/requires.txt
--rw-r--r--   0 gzhang    (3204)     1040       10 2024-04-02 13:58:06.000000 bencheval-1.3.2/bencheval.egg-info/top_level.txt
--rw-r--r--   0 gzhang    (3204)     1040     1176 2024-04-02 08:41:37.000000 bencheval-1.3.2/pyproject.toml
--rw-r--r--   0 gzhang    (3204)     1040      129 2024-03-16 13:21:55.000000 bencheval-1.3.2/requirements.txt
--rw-r--r--   0 gzhang    (3204)     1040       38 2024-04-02 13:58:06.409040 bencheval-1.3.2/setup.cfg
+drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-04-08 13:06:14.432786 bencheval-1.3.3/
+-rw-r--r--   0 gzhang    (3204)     1040     1068 2024-03-18 09:00:38.000000 bencheval-1.3.3/LICENSE.txt
+-rw-r--r--   0 gzhang    (3204)     1040       52 2024-03-18 09:00:38.000000 bencheval-1.3.3/MANIFEST.in
+-rw-r--r--   0 gzhang    (3204)     1040     3315 2024-04-08 13:06:14.432609 bencheval-1.3.3/PKG-INFO
+-rw-r--r--   0 gzhang    (3204)     1040     2282 2024-03-18 09:00:38.000000 bencheval-1.3.3/README.md
+drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-04-08 13:06:14.412484 bencheval-1.3.3/bencheval/
+-rw-r--r--   0 gzhang    (3204)     1040        0 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/__init__.py
+drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-04-08 13:06:14.413223 bencheval-1.3.3/bencheval/data/
+-rw-r--r--   0 gzhang    (3204)     1040     4171 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/data/__init__.py
+drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-04-08 13:06:14.413602 bencheval-1.3.3/bencheval/data/__pycache__/
+-rw-r--r--   0 gzhang    (3204)     1040     5711 2024-03-27 13:57:41.000000 bencheval-1.3.3/bencheval/data/__pycache__/__init__.cpython-311.pyc
+drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-04-08 13:06:14.415597 bencheval-1.3.3/bencheval/data/bbh/
+-rw-r--r--   0 gzhang    (3204)     1040      208 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/data/bbh/__init__.py
+-rw-r--r--   0 gzhang    (3204)     1040      636 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/data/bbh/cols.txt
+-rw-r--r--   0 gzhang    (3204)     1040      542 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/data/bbh/format.py
+-rw-r--r--   0 gzhang    (3204)     1040    18964 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/data/bbh/leaderboard.tsv
+-rw-r--r--   0 gzhang    (3204)     1040     1021 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/data/bbh/statistic.py
+-rw-r--r--   0 gzhang    (3204)     1040    18436 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/data/bbh/vanilla.tsv
+drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-04-08 13:06:14.416908 bencheval-1.3.3/bencheval/data/bigcode/
+-rw-r--r--   0 gzhang    (3204)     1040      338 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/data/bigcode/__init__.py
+-rw-r--r--   0 gzhang    (3204)     1040      430 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/data/bigcode/format.py
+-rw-r--r--   0 gzhang    (3204)     1040     2169 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/data/bigcode/leaderboard.tsv
+-rw-r--r--   0 gzhang    (3204)     1040     2226 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/data/bigcode/vanilla.txt
+drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-04-08 13:06:14.417049 bencheval-1.3.3/bencheval/data/dummy/
+-rw-r--r--   0 gzhang    (3204)     1040     1404 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/data/dummy/__init__.py
+drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-04-08 13:06:14.417466 bencheval-1.3.3/bencheval/data/glue/
+-rw-r--r--   0 gzhang    (3204)     1040     1077 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/data/glue/__init__.py
+-rw-r--r--   0 gzhang    (3204)     1040     9876 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/data/glue/leaderboard.tsv
+drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-04-08 13:06:14.420490 bencheval-1.3.3/bencheval/data/heim/
+-rw-r--r--   0 gzhang    (3204)     1040      767 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/data/heim/__init__.py
+-rw-r--r--   0 gzhang    (3204)     1040    13934 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/data/heim/aesthetics_auto.tsv
+-rw-r--r--   0 gzhang    (3204)     1040     5206 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/data/heim/aesthetics_human.tsv
+-rw-r--r--   0 gzhang    (3204)     1040    10394 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/data/heim/alignment_auto.tsv
+-rw-r--r--   0 gzhang    (3204)     1040     5830 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/data/heim/alignment_human.tsv
+-rw-r--r--   0 gzhang    (3204)     1040     3765 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/data/heim/black_out.tsv
+-rw-r--r--   0 gzhang    (3204)     1040     4494 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/data/heim/nsfw.tsv
+-rw-r--r--   0 gzhang    (3204)     1040     4809 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/data/heim/nudity.tsv
+-rw-r--r--   0 gzhang    (3204)     1040     3643 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/data/heim/originality.tsv
+-rw-r--r--   0 gzhang    (3204)     1040     3343 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/data/heim/quality_auto.tsv
+-rw-r--r--   0 gzhang    (3204)     1040     2554 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/data/heim/quality_human.tsv
+drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-04-08 13:06:14.423426 bencheval-1.3.3/bencheval/data/helm/
+-rw-r--r--   0 gzhang    (3204)     1040      890 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/data/helm/__init__.py
+-rw-r--r--   0 gzhang    (3204)     1040     7516 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/data/helm/accuracy.tsv
+-rw-r--r--   0 gzhang    (3204)     1040    14741 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/data/helm/bias.tsv
+-rw-r--r--   0 gzhang    (3204)     1040     5563 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/data/helm/calibration.tsv
+-rw-r--r--   0 gzhang    (3204)     1040     5858 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/data/helm/efficiency.tsv
+-rw-r--r--   0 gzhang    (3204)     1040     6993 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/data/helm/fairness.tsv
+-rw-r--r--   0 gzhang    (3204)     1040     7035 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/data/helm/robustness.tsv
+-rw-r--r--   0 gzhang    (3204)     1040     6495 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/data/helm/summarization.tsv
+-rw-r--r--   0 gzhang    (3204)     1040     4663 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/data/helm/toxicity.tsv
+drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-04-08 13:06:14.426106 bencheval-1.3.3/bencheval/data/imagenet/
+-rw-r--r--   0 gzhang    (3204)     1040     1435 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/data/imagenet/__init__.py
+-rw-r--r--   0 gzhang    (3204)     1040     1058 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/data/imagenet/format.py
+-rw-r--r--   0 gzhang    (3204)     1040   554910 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/data/imagenet/leaderboard.tsv
+-rw-r--r--   0 gzhang    (3204)     1040     7562 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/data/imagenet/leaderboard_raw.tsv
+-rw-r--r--   0 gzhang    (3204)     1040    11304 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/data/imagenet/run.sh
+-rw-r--r--   0 gzhang    (3204)     1040     2587 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/data/imagenet/run_imagenet.py
+-rw-r--r--   0 gzhang    (3204)     1040     8324 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/data/imagenet/vanilla.txt
+drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-04-08 13:06:14.427694 bencheval-1.3.3/bencheval/data/mmlu/
+-rw-r--r--   0 gzhang    (3204)     1040      367 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/data/mmlu/__init__.py
+-rw-r--r--   0 gzhang    (3204)     1040     2113 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/data/mmlu/format.py
+-rw-r--r--   0 gzhang    (3204)     1040   101533 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/data/mmlu/leaderboard.tsv
+-rw-r--r--   0 gzhang    (3204)     1040     5831 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/data/mmlu/leaderboard_raw.csv
+drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-04-08 13:06:14.428668 bencheval-1.3.3/bencheval/data/mteb/
+-rw-r--r--   0 gzhang    (3204)     1040      810 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/data/mteb/__init__.py
+-rw-r--r--   0 gzhang    (3204)     1040      430 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/data/mteb/format.py
+-rw-r--r--   0 gzhang    (3204)     1040     7313 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/data/mteb/leaderboard.tsv
+-rw-r--r--   0 gzhang    (3204)     1040     7199 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/data/mteb/vanilla.txt
+drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-04-08 13:06:14.429845 bencheval-1.3.3/bencheval/data/openllm/
+-rw-r--r--   0 gzhang    (3204)     1040      456 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/data/openllm/__init__.py
+-rw-r--r--   0 gzhang    (3204)     1040      431 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/data/openllm/format.py
+-rw-r--r--   0 gzhang    (3204)     1040     7511 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/data/openllm/leaderboard.tsv
+-rw-r--r--   0 gzhang    (3204)     1040      196 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/data/openllm/statistic.py
+-rw-r--r--   0 gzhang    (3204)     1040     8119 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/data/openllm/vanilla.txt
+drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-04-08 13:06:14.430278 bencheval-1.3.3/bencheval/data/superglue/
+-rw-r--r--   0 gzhang    (3204)     1040      958 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/data/superglue/__init__.py
+-rw-r--r--   0 gzhang    (3204)     1040     3297 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/data/superglue/leaderboard.tsv
+drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-04-08 13:06:14.430770 bencheval-1.3.3/bencheval/data/vtab/
+-rw-r--r--   0 gzhang    (3204)     1040      331 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/data/vtab/__init__.py
+-rw-r--r--   0 gzhang    (3204)     1040     1970 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/data/vtab/leaderboard.tsv
+drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-04-08 13:06:14.431259 bencheval-1.3.3/bencheval/measures/
+-rw-r--r--   0 gzhang    (3204)     1040     4663 2024-04-08 12:21:46.000000 bencheval-1.3.3/bencheval/measures/cardinal.py
+-rw-r--r--   0 gzhang    (3204)     1040     5334 2024-04-02 11:52:38.000000 bencheval-1.3.3/bencheval/measures/ordinal.py
+drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-04-08 13:06:14.432151 bencheval-1.3.3/bencheval/utils/
+-rw-r--r--   0 gzhang    (3204)     1040        0 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/utils/__init__.py
+-rw-r--r--   0 gzhang    (3204)     1040     2077 2024-04-02 11:55:56.000000 bencheval-1.3.3/bencheval/utils/base.py
+-rw-r--r--   0 gzhang    (3204)     1040     4158 2024-03-19 15:00:57.000000 bencheval-1.3.3/bencheval/utils/metric.py
+-rw-r--r--   0 gzhang    (3204)     1040     1358 2024-03-16 13:21:55.000000 bencheval-1.3.3/bencheval/utils/win_rate.py
+drwxr-xr-x   0 gzhang    (3204)     1040        0 2024-04-08 13:06:14.432418 bencheval-1.3.3/bencheval.egg-info/
+-rw-r--r--   0 gzhang    (3204)     1040     3315 2024-04-08 13:06:14.000000 bencheval-1.3.3/bencheval.egg-info/PKG-INFO
+-rw-r--r--   0 gzhang    (3204)     1040     2480 2024-04-08 13:06:14.000000 bencheval-1.3.3/bencheval.egg-info/SOURCES.txt
+-rw-r--r--   0 gzhang    (3204)     1040        1 2024-04-08 13:06:14.000000 bencheval-1.3.3/bencheval.egg-info/dependency_links.txt
+-rw-r--r--   0 gzhang    (3204)     1040       62 2024-04-08 13:06:14.000000 bencheval-1.3.3/bencheval.egg-info/requires.txt
+-rw-r--r--   0 gzhang    (3204)     1040       10 2024-04-08 13:06:14.000000 bencheval-1.3.3/bencheval.egg-info/top_level.txt
+-rw-r--r--   0 gzhang    (3204)     1040     1176 2024-04-08 11:00:58.000000 bencheval-1.3.3/pyproject.toml
+-rw-r--r--   0 gzhang    (3204)     1040      129 2024-03-16 13:21:55.000000 bencheval-1.3.3/requirements.txt
+-rw-r--r--   0 gzhang    (3204)     1040       38 2024-04-08 13:06:14.432821 bencheval-1.3.3/setup.cfg
```

### Comparing `bencheval-1.3.2/LICENSE.txt` & `bencheval-1.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.2/PKG-INFO` & `bencheval-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bencheval
-Version: 1.3.2
+Version: 1.3.3
 Summary: Tools for measuring sensitivity and diversity of multi-task benchmarks.
 Author: Guanhua Zhang
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `bencheval-1.3.2/README.md` & `bencheval-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.2/bencheval/data/__init__.py` & `bencheval-1.3.3/bencheval/data/__init__.py`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.2/bencheval/data/__pycache__/__init__.cpython-311.pyc` & `bencheval-1.3.3/bencheval/data/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.2/bencheval/data/bbh/cols.txt` & `bencheval-1.3.3/bencheval/data/bbh/cols.txt`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.2/bencheval/data/bbh/format.py` & `bencheval-1.3.3/bencheval/data/bbh/format.py`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.2/bencheval/data/bbh/leaderboard.tsv` & `bencheval-1.3.3/bencheval/data/bbh/leaderboard.tsv`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.2/bencheval/data/bbh/statistic.py` & `bencheval-1.3.3/bencheval/data/bbh/statistic.py`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.2/bencheval/data/bbh/vanilla.tsv` & `bencheval-1.3.3/bencheval/data/bbh/vanilla.tsv`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.2/bencheval/data/bigcode/leaderboard.tsv` & `bencheval-1.3.3/bencheval/data/bigcode/leaderboard.tsv`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.2/bencheval/data/bigcode/vanilla.txt` & `bencheval-1.3.3/bencheval/data/bigcode/vanilla.txt`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.2/bencheval/data/dummy/__init__.py` & `bencheval-1.3.3/bencheval/data/dummy/__init__.py`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.2/bencheval/data/glue/__init__.py` & `bencheval-1.3.3/bencheval/data/glue/__init__.py`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.2/bencheval/data/glue/leaderboard.tsv` & `bencheval-1.3.3/bencheval/data/glue/leaderboard.tsv`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.2/bencheval/data/heim/__init__.py` & `bencheval-1.3.3/bencheval/data/heim/__init__.py`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.2/bencheval/data/heim/aesthetics_auto.tsv` & `bencheval-1.3.3/bencheval/data/heim/aesthetics_auto.tsv`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.2/bencheval/data/heim/aesthetics_human.tsv` & `bencheval-1.3.3/bencheval/data/heim/aesthetics_human.tsv`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.2/bencheval/data/heim/alignment_auto.tsv` & `bencheval-1.3.3/bencheval/data/heim/alignment_auto.tsv`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.2/bencheval/data/heim/alignment_human.tsv` & `bencheval-1.3.3/bencheval/data/heim/alignment_human.tsv`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.2/bencheval/data/heim/black_out.tsv` & `bencheval-1.3.3/bencheval/data/heim/black_out.tsv`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.2/bencheval/data/heim/nsfw.tsv` & `bencheval-1.3.3/bencheval/data/heim/nsfw.tsv`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.2/bencheval/data/heim/nudity.tsv` & `bencheval-1.3.3/bencheval/data/heim/nudity.tsv`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.2/bencheval/data/heim/originality.tsv` & `bencheval-1.3.3/bencheval/data/heim/originality.tsv`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.2/bencheval/data/heim/quality_auto.tsv` & `bencheval-1.3.3/bencheval/data/heim/quality_auto.tsv`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.2/bencheval/data/heim/quality_human.tsv` & `bencheval-1.3.3/bencheval/data/heim/quality_human.tsv`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.2/bencheval/data/helm/__init__.py` & `bencheval-1.3.3/bencheval/data/helm/__init__.py`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.2/bencheval/data/helm/accuracy.tsv` & `bencheval-1.3.3/bencheval/data/helm/accuracy.tsv`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.2/bencheval/data/helm/bias.tsv` & `bencheval-1.3.3/bencheval/data/helm/bias.tsv`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.2/bencheval/data/helm/calibration.tsv` & `bencheval-1.3.3/bencheval/data/helm/calibration.tsv`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.2/bencheval/data/helm/efficiency.tsv` & `bencheval-1.3.3/bencheval/data/helm/efficiency.tsv`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.2/bencheval/data/helm/fairness.tsv` & `bencheval-1.3.3/bencheval/data/helm/fairness.tsv`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.2/bencheval/data/helm/robustness.tsv` & `bencheval-1.3.3/bencheval/data/helm/robustness.tsv`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.2/bencheval/data/helm/summarization.tsv` & `bencheval-1.3.3/bencheval/data/helm/summarization.tsv`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.2/bencheval/data/helm/toxicity.tsv` & `bencheval-1.3.3/bencheval/data/helm/toxicity.tsv`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.2/bencheval/data/imagenet/__init__.py` & `bencheval-1.3.3/bencheval/data/imagenet/__init__.py`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.2/bencheval/data/imagenet/format.py` & `bencheval-1.3.3/bencheval/data/imagenet/format.py`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.2/bencheval/data/imagenet/leaderboard.tsv` & `bencheval-1.3.3/bencheval/data/imagenet/leaderboard.tsv`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.2/bencheval/data/imagenet/leaderboard_raw.tsv` & `bencheval-1.3.3/bencheval/data/imagenet/leaderboard_raw.tsv`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.2/bencheval/data/imagenet/run.sh` & `bencheval-1.3.3/bencheval/data/imagenet/run.sh`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.2/bencheval/data/imagenet/run_imagenet.py` & `bencheval-1.3.3/bencheval/data/imagenet/run_imagenet.py`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.2/bencheval/data/imagenet/vanilla.txt` & `bencheval-1.3.3/bencheval/data/imagenet/vanilla.txt`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.2/bencheval/data/mmlu/format.py` & `bencheval-1.3.3/bencheval/data/mmlu/format.py`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.2/bencheval/data/mmlu/leaderboard.tsv` & `bencheval-1.3.3/bencheval/data/mmlu/leaderboard.tsv`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.2/bencheval/data/mmlu/leaderboard_raw.csv` & `bencheval-1.3.3/bencheval/data/mmlu/leaderboard_raw.csv`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.2/bencheval/data/mteb/__init__.py` & `bencheval-1.3.3/bencheval/data/mteb/__init__.py`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.2/bencheval/data/mteb/leaderboard.tsv` & `bencheval-1.3.3/bencheval/data/mteb/leaderboard.tsv`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.2/bencheval/data/mteb/vanilla.txt` & `bencheval-1.3.3/bencheval/data/mteb/vanilla.txt`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.2/bencheval/data/openllm/leaderboard.tsv` & `bencheval-1.3.3/bencheval/data/openllm/leaderboard.tsv`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.2/bencheval/data/openllm/vanilla.txt` & `bencheval-1.3.3/bencheval/data/openllm/vanilla.txt`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.2/bencheval/data/superglue/__init__.py` & `bencheval-1.3.3/bencheval/data/superglue/__init__.py`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.2/bencheval/data/superglue/leaderboard.tsv` & `bencheval-1.3.3/bencheval/data/superglue/leaderboard.tsv`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.2/bencheval/data/vtab/leaderboard.tsv` & `bencheval-1.3.3/bencheval/data/vtab/leaderboard.tsv`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.2/bencheval/measures/cardinal.py` & `bencheval-1.3.3/bencheval/measures/cardinal.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,51 +27,50 @@
                     loss = loss + (old_rank[i] - old_rank[j]) * max(score[j] - score[i], 0.0)
                 else:
                     loss = loss + max(score[j] - score[i], 0.0)
     return loss
 
 
 def get_sensitivity(data, cols, min_value=0.01, lr=1.0, num_steps=1000, stop_threshold=1e-5,
-                    normalize_data=True, use_weighted_loss=None, return_weight=False, verbose=False):
+                    normalize_epsilon=True, use_weighted_loss=None, return_weight=False, verbose=False):
     """
     Calculate the sensitivity for a given benchmark.
 
     Args:
         data(pd.DataFrame): Each row represents a model, each column represents a task.
         cols(list): The column names of the tasks.
         min_value(float): Min values for epsilon.
         lr(float): Learning rate for optimization.
         num_steps(int): Number of steps for optimization.
         stop_threshold(float): Stop if the loss change is smaller than this value.
-        normalize_data(bool): Whether normalize the data before optimization.
+        normalize_epsilon(bool): Whether normalize epsilon by std.
         use_weighted_loss(bool): Whether use weighted approximation loss, if None, use both and return the better one.
         return_weight(bool): Whether return alpha.
         verbose(bool): Whether output logs.
 
     Returns:
         tuple: If return_weight is True, return ((tau, MRC), alpha); else return (tau, MRC).
     """
     if use_weighted_loss is None:
-        a = get_sensitivity(data, cols, min_value, lr, num_steps, stop_threshold, normalize_data,
+        a = get_sensitivity(data, cols, min_value, lr, num_steps, stop_threshold, normalize_epsilon,
                             use_weighted_loss=True, return_weight=True, verbose=verbose)
-        b = get_sensitivity(data, cols, min_value, lr, num_steps, stop_threshold, normalize_data,
+        b = get_sensitivity(data, cols, min_value, lr, num_steps, stop_threshold, normalize_epsilon,
                             use_weighted_loss=False, return_weight=True, verbose=verbose)
         if return_weight:
             return a if a[0] > b[0] else b
         else:
             return max(a[0], b[0])
 
     data = data[cols].values
     data = torch.tensor(data)
     data_std = data.std(0)
     data = data[:, [i for i, _std in enumerate(data_std) if _std > 1e-8]]
     orig_data = data.clone()
-    if normalize_data:
-        data = data - data.mean(0)
-        data = data / data.std(0)
+    data = data - data.mean(0)
+    data = data / data.std(0)
 
     old_score = orig_data.mean(1).detach().numpy()
     old_rank = rankdata(-old_score, method="average")
 
     weight = torch.ones(data.shape[1], requires_grad=True)
 
     def normalize_func(w):
@@ -96,16 +95,16 @@
         if np.fabs(loss.item() - last_loss) < stop_threshold:
             break
         last_loss = loss.item()
         if verbose:
             print("Step %d, Loss = %.2lf" % (step, loss.item()))
 
     norm_weight = normalize_func(weight).detach().numpy()
-    # if normalize_data:
-    #     norm_weight = norm_weight / orig_data.std(0).numpy()
+    if normalize_epsilon:
+        norm_weight = norm_weight / orig_data.std(0).numpy()
     norm_weight = norm_weight / norm_weight.max()
     new_score = (orig_data * norm_weight).mean(1).detach().numpy()
     new_rank = rankdata(-new_score, method="average")
     rank_diff = get_rank_diff(new_rank, old_rank)
     if return_weight:
         return rank_diff, norm_weight
     else:
```

### Comparing `bencheval-1.3.2/bencheval/measures/ordinal.py` & `bencheval-1.3.3/bencheval/measures/ordinal.py`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.2/bencheval/utils/base.py` & `bencheval-1.3.3/bencheval/utils/base.py`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.2/bencheval/utils/metric.py` & `bencheval-1.3.3/bencheval/utils/metric.py`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.2/bencheval/utils/win_rate.py` & `bencheval-1.3.3/bencheval/utils/win_rate.py`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.2/bencheval.egg-info/PKG-INFO` & `bencheval-1.3.3/bencheval.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bencheval
-Version: 1.3.2
+Version: 1.3.3
 Summary: Tools for measuring sensitivity and diversity of multi-task benchmarks.
 Author: Guanhua Zhang
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `bencheval-1.3.2/bencheval.egg-info/SOURCES.txt` & `bencheval-1.3.3/bencheval.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bencheval-1.3.2/pyproject.toml` & `bencheval-1.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "bencheval"
 authors = [
     {name = "Guanhua Zhang"},
 ]
 description = "Tools for measuring sensitivity and diversity of multi-task benchmarks."
-version = "1.3.2"
+version = "1.3.3"
 requires-python = ">=3.7"
 readme = "README.md"
 license = {text = "MIT"}
 classifiers=[
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: MIT License",
     "Intended Audience :: Science/Research",
```

