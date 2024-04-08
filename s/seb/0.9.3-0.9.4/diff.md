# Comparing `tmp/seb-0.9.3.tar.gz` & `tmp/seb-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seb-0.9.3.tar", last modified: Sun Jan 28 10:06:38 2024, max compression
+gzip compressed data, was "seb-0.9.4.tar", last modified: Sun Jan 28 21:19:02 2024, max compression
```

## Comparing `seb-0.9.3.tar` & `seb-0.9.4.tar`

### file list

```diff
@@ -1,633 +1,633 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 10:06:38.520315 seb-0.9.3/
--rw-r--r--   0 root         (0) root         (0)      456 2024-01-28 10:06:30.000000 seb-0.9.3/.cookiecutter.json
--rw-r--r--   0 root         (0) root         (0)      703 2024-01-28 10:06:30.000000 seb-0.9.3/.cruft.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 10:06:38.400313 seb-0.9.3/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 10:06:38.408314 seb-0.9.3/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)      558 2024-01-28 10:06:30.000000 seb-0.9.3/.github/workflows/check_benchmark_is_up_to_date.yml
--rw-r--r--   0 root         (0) root         (0)      992 2024-01-28 10:06:30.000000 seb-0.9.3/.github/workflows/documentation.yml
--rw-r--r--   0 root         (0) root         (0)      456 2024-01-28 10:06:30.000000 seb-0.9.3/.github/workflows/lint.yml
--rw-r--r--   0 root         (0) root         (0)     2053 2024-01-28 10:06:30.000000 seb-0.9.3/.github/workflows/release.yml
--rw-r--r--   0 root         (0) root         (0)     1165 2024-01-28 10:06:30.000000 seb-0.9.3/.github/workflows/stalebot.yml
--rw-r--r--   0 root         (0) root         (0)      668 2024-01-28 10:06:30.000000 seb-0.9.3/.github/workflows/static_type_checks.yml
--rw-r--r--   0 root         (0) root         (0)     1033 2024-01-28 10:06:30.000000 seb-0.9.3/.github/workflows/tests.yml
--rw-r--r--   0 root         (0) root         (0)      499 2024-01-28 10:06:30.000000 seb-0.9.3/.gitignore
--rw-r--r--   0 root         (0) root         (0)    80324 2024-01-28 10:06:30.000000 seb-0.9.3/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     5532 2024-01-28 10:06:30.000000 seb-0.9.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 root         (0) root         (0)     2347 2024-01-28 10:06:30.000000 seb-0.9.3/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)     1074 2024-01-28 10:06:30.000000 seb-0.9.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6241 2024-01-28 10:06:38.520315 seb-0.9.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2996 2024-01-28 10:06:30.000000 seb-0.9.3/README.md
--rw-r--r--   0 root         (0) root         (0)      720 2024-01-28 10:06:30.000000 seb-0.9.3/citation.cff
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 10:06:38.412314 seb-0.9.3/docs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 10:06:38.412314 seb-0.9.3/docs/_static/
--rw-r--r--   0 root         (0) root         (0)   417053 2024-01-28 10:06:30.000000 seb-0.9.3/docs/_static/logo.png
--rw-r--r--   0 root         (0) root         (0)  1221950 2024-01-28 10:06:30.000000 seb-0.9.3/docs/_static/social.png
--rw-r--r--   0 root         (0) root         (0)      647 2024-01-28 10:06:30.000000 seb-0.9.3/docs/api.md
--rw-r--r--   0 root         (0) root         (0)     3328 2024-01-28 10:06:30.000000 seb-0.9.3/docs/cli.md
--rw-r--r--   0 root         (0) root         (0)      544 2024-01-28 10:06:30.000000 seb-0.9.3/docs/create_cli_docs.py
--rw-r--r--   0 root         (0) root         (0)     2071 2024-01-28 10:06:30.000000 seb-0.9.3/docs/create_desc_stats.py
--rw-r--r--   0 root         (0) root         (0)    15541 2024-01-28 10:06:30.000000 seb-0.9.3/docs/datasets.md
--rw-r--r--   0 root         (0) root         (0)    25049 2024-01-28 10:06:30.000000 seb-0.9.3/docs/getting_started.ipynb
--rw-r--r--   0 root         (0) root         (0)     4207 2024-01-28 10:06:30.000000 seb-0.9.3/docs/index.md
--rw-r--r--   0 root         (0) root         (0)      401 2024-01-28 10:06:30.000000 seb-0.9.3/docs/installation.md
--rw-r--r--   0 root         (0) root         (0)      801 2024-01-28 10:06:30.000000 seb-0.9.3/docs/paper.md
--rw-r--r--   0 root         (0) root         (0)     4251 2024-01-28 10:06:30.000000 seb-0.9.3/docs/run_benchmark.py
--rw-r--r--   0 root         (0) root         (0)     1704 2024-01-28 10:06:30.000000 seb-0.9.3/makefile
--rw-r--r--   0 root         (0) root         (0)     1769 2024-01-28 10:06:30.000000 seb-0.9.3/mkdocs.yml
--rw-r--r--   0 root         (0) root         (0)     3365 2024-01-28 10:06:32.000000 seb-0.9.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-01-28 10:06:38.520315 seb-0.9.3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 10:06:38.400313 seb-0.9.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 10:06:38.416314 seb-0.9.3/src/scripts/
--rw-r--r--   0 root         (0) root         (0)      155 2024-01-28 10:06:30.000000 seb-0.9.3/src/scripts/check_benchmark_is_up_to_date.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 10:06:38.416314 seb-0.9.3/src/seb/
--rw-r--r--   0 root         (0) root         (0)      480 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/__init__.py
--rw-r--r--   0 root         (0) root         (0)       78 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/__main__.py
--rw-r--r--   0 root         (0) root         (0)     7044 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/benchmark.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 10:06:38.404313 seb-0.9.3/src/seb/cache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 10:06:38.420314 seb-0.9.3/src/seb/cache/KBLab__sentence-bert-swedish-cased/
--rw-r--r--   0 root         (0) root         (0)      401 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KBLab__sentence-bert-swedish-cased/Angry_Tweets.json
--rw-r--r--   0 root         (0) root         (0)      620 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KBLab__sentence-bert-swedish-cased/Bornholm_Parallel.json
--rw-r--r--   0 root         (0) root         (0)      440 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KBLab__sentence-bert-swedish-cased/DKHate.json
--rw-r--r--   0 root         (0) root         (0)      452 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KBLab__sentence-bert-swedish-cased/DaLAJ.json
--rw-r--r--   0 root         (0) root         (0)      389 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KBLab__sentence-bert-swedish-cased/Da_Political_Comments.json
--rw-r--r--   0 root         (0) root         (0)      366 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KBLab__sentence-bert-swedish-cased/LCC.json
--rw-r--r--   0 root         (0) root         (0)     1202 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KBLab__sentence-bert-swedish-cased/Language_Identification.json
--rw-r--r--   0 root         (0) root         (0)      771 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KBLab__sentence-bert-swedish-cased/Massive_Intent.json
--rw-r--r--   0 root         (0) root         (0)      768 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KBLab__sentence-bert-swedish-cased/Massive_Scenario.json
--rw-r--r--   0 root         (0) root         (0)      360 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KBLab__sentence-bert-swedish-cased/NoReC.json
--rw-r--r--   0 root         (0) root         (0)      438 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KBLab__sentence-bert-swedish-cased/Norwegian_parliament.json
--rw-r--r--   0 root         (0) root         (0)     1085 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KBLab__sentence-bert-swedish-cased/ScaLA.json
--rw-r--r--   0 root         (0) root         (0)      844 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KBLab__sentence-bert-swedish-cased/SweFAQ.json
--rw-r--r--   0 root         (0) root         (0)      351 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KBLab__sentence-bert-swedish-cased/SweReC.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 10:06:38.424314 seb-0.9.3/src/seb/cache/KB__bert-base-swedish-cased/
--rw-r--r--   0 root         (0) root         (0)      401 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KB__bert-base-swedish-cased/Angry_Tweets.json
--rw-r--r--   0 root         (0) root         (0)      622 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KB__bert-base-swedish-cased/Bornholm_Parallel.json
--rw-r--r--   0 root         (0) root         (0)      441 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KB__bert-base-swedish-cased/DKHate.json
--rw-r--r--   0 root         (0) root         (0)      450 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KB__bert-base-swedish-cased/DaLAJ.json
--rw-r--r--   0 root         (0) root         (0)      389 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KB__bert-base-swedish-cased/Da_Political_Comments.json
--rw-r--r--   0 root         (0) root         (0)      367 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KB__bert-base-swedish-cased/LCC.json
--rw-r--r--   0 root         (0) root         (0)     1046 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KB__bert-base-swedish-cased/Language_Identification.json
--rw-r--r--   0 root         (0) root         (0)      766 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KB__bert-base-swedish-cased/Massive_Intent.json
--rw-r--r--   0 root         (0) root         (0)      765 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KB__bert-base-swedish-cased/Massive_Scenario.json
--rw-r--r--   0 root         (0) root         (0)      354 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KB__bert-base-swedish-cased/NoReC.json
--rw-r--r--   0 root         (0) root         (0)      436 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KB__bert-base-swedish-cased/Norwegian_parliament.json
--rw-r--r--   0 root         (0) root         (0)     1601 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KB__bert-base-swedish-cased/ScaLA.json
--rw-r--r--   0 root         (0) root         (0)      844 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KB__bert-base-swedish-cased/SweFAQ.json
--rw-r--r--   0 root         (0) root         (0)      353 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KB__bert-base-swedish-cased/SweReC.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 10:06:38.424314 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-1/
--rw-r--r--   0 root         (0) root         (0)      399 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-1/Angry_Tweets.json
--rw-r--r--   0 root         (0) root         (0)      620 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-1/Bornholm_Parallel.json
--rw-r--r--   0 root         (0) root         (0)      440 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-1/DKHate.json
--rw-r--r--   0 root         (0) root         (0)      450 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-1/DaLAJ.json
--rw-r--r--   0 root         (0) root         (0)      389 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-1/Da_Political_Comments.json
--rw-r--r--   0 root         (0) root         (0)      365 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-1/LCC.json
--rw-r--r--   0 root         (0) root         (0)     1202 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-1/Language_Identification.json
--rw-r--r--   0 root         (0) root         (0)      765 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-1/Massive_Intent.json
--rw-r--r--   0 root         (0) root         (0)      764 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-1/Massive_Scenario.json
--rw-r--r--   0 root         (0) root         (0)      362 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-1/NoReC.json
--rw-r--r--   0 root         (0) root         (0)      437 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-1/Norwegian_parliament.json
--rw-r--r--   0 root         (0) root         (0)     1081 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-1/ScaLA.json
--rw-r--r--   0 root         (0) root         (0)      837 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-1/SweFAQ.json
--rw-r--r--   0 root         (0) root         (0)      362 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-1/SweReC.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 10:06:38.428314 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp1/
--rw-r--r--   0 root         (0) root         (0)      401 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp1/Angry_Tweets.json
--rw-r--r--   0 root         (0) root         (0)      544 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp1/Bornholm_Parallel.json
--rw-r--r--   0 root         (0) root         (0)      438 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp1/DKHate.json
--rw-r--r--   0 root         (0) root         (0)      453 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp1/DaLAJ.json
--rw-r--r--   0 root         (0) root         (0)      389 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp1/Da_Political_Comments.json
--rw-r--r--   0 root         (0) root         (0)      366 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp1/LCC.json
--rw-r--r--   0 root         (0) root         (0)     1196 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp1/Language_Identification.json
--rw-r--r--   0 root         (0) root         (0)      762 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp1/Massive_Intent.json
--rw-r--r--   0 root         (0) root         (0)      764 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp1/Massive_Scenario.json
--rw-r--r--   0 root         (0) root         (0)      364 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp1/NoReC.json
--rw-r--r--   0 root         (0) root         (0)      437 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp1/Norwegian_parliament.json
--rw-r--r--   0 root         (0) root         (0)     1088 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp1/ScaLA.json
--rw-r--r--   0 root         (0) root         (0)      838 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp1/SweFAQ.json
--rw-r--r--   0 root         (0) root         (0)      356 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp1/SweReC.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 10:06:38.432314 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp2-no-lang-align/
--rw-r--r--   0 root         (0) root         (0)      400 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp2-no-lang-align/Angry_Tweets.json
--rw-r--r--   0 root         (0) root         (0)      544 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp2-no-lang-align/Bornholm_Parallel.json
--rw-r--r--   0 root         (0) root         (0)      439 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp2-no-lang-align/DKHate.json
--rw-r--r--   0 root         (0) root         (0)      451 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp2-no-lang-align/DaLAJ.json
--rw-r--r--   0 root         (0) root         (0)      387 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp2-no-lang-align/Da_Political_Comments.json
--rw-r--r--   0 root         (0) root         (0)      366 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp2-no-lang-align/LCC.json
--rw-r--r--   0 root         (0) root         (0)     1202 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp2-no-lang-align/Language_Identification.json
--rw-r--r--   0 root         (0) root         (0)      765 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp2-no-lang-align/Massive_Intent.json
--rw-r--r--   0 root         (0) root         (0)      766 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp2-no-lang-align/Massive_Scenario.json
--rw-r--r--   0 root         (0) root         (0)      364 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp2-no-lang-align/NoReC.json
--rw-r--r--   0 root         (0) root         (0)      412 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp2-no-lang-align/Norwegian_parliament.json
--rw-r--r--   0 root         (0) root         (0)     1086 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp2-no-lang-align/ScaLA.json
--rw-r--r--   0 root         (0) root         (0)      844 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp2-no-lang-align/SweFAQ.json
--rw-r--r--   0 root         (0) root         (0)      361 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp2-no-lang-align/SweReC.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 10:06:38.432314 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-medium-v1/
--rw-r--r--   0 root         (0) root         (0)      400 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-medium-v1/Angry_Tweets.json
--rw-r--r--   0 root         (0) root         (0)      617 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-medium-v1/Bornholm_Parallel.json
--rw-r--r--   0 root         (0) root         (0)      441 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-medium-v1/DKHate.json
--rw-r--r--   0 root         (0) root         (0)      453 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-medium-v1/DaLAJ.json
--rw-r--r--   0 root         (0) root         (0)      388 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-medium-v1/Da_Political_Comments.json
--rw-r--r--   0 root         (0) root         (0)      365 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-medium-v1/LCC.json
--rw-r--r--   0 root         (0) root         (0)     1190 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-medium-v1/Language_Identification.json
--rw-r--r--   0 root         (0) root         (0)      762 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-medium-v1/Massive_Intent.json
--rw-r--r--   0 root         (0) root         (0)      766 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-medium-v1/Massive_Scenario.json
--rw-r--r--   0 root         (0) root         (0)      357 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-medium-v1/NoReC.json
--rw-r--r--   0 root         (0) root         (0)      438 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-medium-v1/Norwegian_parliament.json
--rw-r--r--   0 root         (0) root         (0)     1081 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-medium-v1/ScaLA.json
--rw-r--r--   0 root         (0) root         (0)      840 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-medium-v1/SweFAQ.json
--rw-r--r--   0 root         (0) root         (0)      362 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-medium-v1/SweReC.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 10:06:38.436314 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-small-v1/
--rw-r--r--   0 root         (0) root         (0)      400 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-small-v1/Angry_Tweets.json
--rw-r--r--   0 root         (0) root         (0)      620 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-small-v1/Bornholm_Parallel.json
--rw-r--r--   0 root         (0) root         (0)      409 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-small-v1/DKHate.json
--rw-r--r--   0 root         (0) root         (0)      451 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-small-v1/DaLAJ.json
--rw-r--r--   0 root         (0) root         (0)      388 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-small-v1/Da_Political_Comments.json
--rw-r--r--   0 root         (0) root         (0)      366 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-small-v1/LCC.json
--rw-r--r--   0 root         (0) root         (0)     1034 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-small-v1/Language_Identification.json
--rw-r--r--   0 root         (0) root         (0)      766 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-small-v1/Massive_Intent.json
--rw-r--r--   0 root         (0) root         (0)      768 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-small-v1/Massive_Scenario.json
--rw-r--r--   0 root         (0) root         (0)      360 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-small-v1/NoReC.json
--rw-r--r--   0 root         (0) root         (0)      411 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-small-v1/Norwegian_parliament.json
--rw-r--r--   0 root         (0) root         (0)     1077 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-small-v1/ScaLA.json
--rw-r--r--   0 root         (0) root         (0)      845 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-small-v1/SweFAQ.json
--rw-r--r--   0 root         (0) root         (0)      358 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-small-v1/SweReC.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 10:06:38.440314 seb-0.9.3/src/seb/cache/NbAiLab__nb-bert-base/
--rw-r--r--   0 root         (0) root         (0)      400 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/NbAiLab__nb-bert-base/Angry_Tweets.json
--rw-r--r--   0 root         (0) root         (0)      624 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/NbAiLab__nb-bert-base/Bornholm_Parallel.json
--rw-r--r--   0 root         (0) root         (0)      437 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/NbAiLab__nb-bert-base/DKHate.json
--rw-r--r--   0 root         (0) root         (0)      450 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/NbAiLab__nb-bert-base/DaLAJ.json
--rw-r--r--   0 root         (0) root         (0)      387 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/NbAiLab__nb-bert-base/Da_Political_Comments.json
--rw-r--r--   0 root         (0) root         (0)      338 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/NbAiLab__nb-bert-base/LCC.json
--rw-r--r--   0 root         (0) root         (0)     1190 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/NbAiLab__nb-bert-base/Language_Identification.json
--rw-r--r--   0 root         (0) root         (0)      765 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/NbAiLab__nb-bert-base/Massive_Intent.json
--rw-r--r--   0 root         (0) root         (0)      766 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/NbAiLab__nb-bert-base/Massive_Scenario.json
--rw-r--r--   0 root         (0) root         (0)      363 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/NbAiLab__nb-bert-base/NoReC.json
--rw-r--r--   0 root         (0) root         (0)      435 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/NbAiLab__nb-bert-base/Norwegian_parliament.json
--rw-r--r--   0 root         (0) root         (0)     1088 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/NbAiLab__nb-bert-base/ScaLA.json
--rw-r--r--   0 root         (0) root         (0)      845 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/NbAiLab__nb-bert-base/SweFAQ.json
--rw-r--r--   0 root         (0) root         (0)      362 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/NbAiLab__nb-bert-base/SweReC.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 10:06:38.440314 seb-0.9.3/src/seb/cache/NbAiLab__nb-bert-large/
--rw-r--r--   0 root         (0) root         (0)      401 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/NbAiLab__nb-bert-large/Angry_Tweets.json
--rw-r--r--   0 root         (0) root         (0)      625 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/NbAiLab__nb-bert-large/Bornholm_Parallel.json
--rw-r--r--   0 root         (0) root         (0)      439 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/NbAiLab__nb-bert-large/DKHate.json
--rw-r--r--   0 root         (0) root         (0)      447 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/NbAiLab__nb-bert-large/DaLAJ.json
--rw-r--r--   0 root         (0) root         (0)      388 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/NbAiLab__nb-bert-large/Da_Political_Comments.json
--rw-r--r--   0 root         (0) root         (0)      365 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/NbAiLab__nb-bert-large/LCC.json
--rw-r--r--   0 root         (0) root         (0)     1201 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/NbAiLab__nb-bert-large/Language_Identification.json
--rw-r--r--   0 root         (0) root         (0)      765 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/NbAiLab__nb-bert-large/Massive_Intent.json
--rw-r--r--   0 root         (0) root         (0)      768 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/NbAiLab__nb-bert-large/Massive_Scenario.json
--rw-r--r--   0 root         (0) root         (0)      361 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/NbAiLab__nb-bert-large/NoReC.json
--rw-r--r--   0 root         (0) root         (0)      437 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/NbAiLab__nb-bert-large/Norwegian_parliament.json
--rw-r--r--   0 root         (0) root         (0)     1598 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/NbAiLab__nb-bert-large/ScaLA.json
--rw-r--r--   0 root         (0) root         (0)      842 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/NbAiLab__nb-bert-large/SweFAQ.json
--rw-r--r--   0 root         (0) root         (0)      363 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/NbAiLab__nb-bert-large/SweReC.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 10:06:38.444314 seb-0.9.3/src/seb/cache/chcaa__dfm-encoder-large-v1/
--rw-r--r--   0 root         (0) root         (0)      401 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/chcaa__dfm-encoder-large-v1/Angry_Tweets.json
--rw-r--r--   0 root         (0) root         (0)      622 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/chcaa__dfm-encoder-large-v1/Bornholm_Parallel.json
--rw-r--r--   0 root         (0) root         (0)      438 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/chcaa__dfm-encoder-large-v1/DKHate.json
--rw-r--r--   0 root         (0) root         (0)      448 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/chcaa__dfm-encoder-large-v1/DaLAJ.json
--rw-r--r--   0 root         (0) root         (0)      389 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/chcaa__dfm-encoder-large-v1/Da_Political_Comments.json
--rw-r--r--   0 root         (0) root         (0)      367 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/chcaa__dfm-encoder-large-v1/LCC.json
--rw-r--r--   0 root         (0) root         (0)     1196 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/chcaa__dfm-encoder-large-v1/Language_Identification.json
--rw-r--r--   0 root         (0) root         (0)      766 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/chcaa__dfm-encoder-large-v1/Massive_Intent.json
--rw-r--r--   0 root         (0) root         (0)      767 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/chcaa__dfm-encoder-large-v1/Massive_Scenario.json
--rw-r--r--   0 root         (0) root         (0)      359 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/chcaa__dfm-encoder-large-v1/NoReC.json
--rw-r--r--   0 root         (0) root         (0)      414 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/chcaa__dfm-encoder-large-v1/Norwegian_parliament.json
--rw-r--r--   0 root         (0) root         (0)     1080 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/chcaa__dfm-encoder-large-v1/ScaLA.json
--rw-r--r--   0 root         (0) root         (0)      845 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/chcaa__dfm-encoder-large-v1/SweFAQ.json
--rw-r--r--   0 root         (0) root         (0)      359 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/chcaa__dfm-encoder-large-v1/SweReC.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 10:06:38.448314 seb-0.9.3/src/seb/cache/embed-multilingual-v3.0/
--rw-r--r--   0 root         (0) root         (0)      396 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/embed-multilingual-v3.0/Angry_Tweets.json
--rw-r--r--   0 root         (0) root         (0)      620 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/embed-multilingual-v3.0/Bornholm_Parallel.json
--rw-r--r--   0 root         (0) root         (0)      440 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/embed-multilingual-v3.0/DKHate.json
--rw-r--r--   0 root         (0) root         (0)      452 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/embed-multilingual-v3.0/DaLAJ.json
--rw-r--r--   0 root         (0) root         (0)      388 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/embed-multilingual-v3.0/Da_Political_Comments.json
--rw-r--r--   0 root         (0) root         (0)      340 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/embed-multilingual-v3.0/LCC.json
--rw-r--r--   0 root         (0) root         (0)     1208 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/embed-multilingual-v3.0/Language_Identification.json
--rw-r--r--   0 root         (0) root         (0)      765 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/embed-multilingual-v3.0/Massive_Intent.json
--rw-r--r--   0 root         (0) root         (0)      767 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/embed-multilingual-v3.0/Massive_Scenario.json
--rw-r--r--   0 root         (0) root         (0)      362 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/embed-multilingual-v3.0/NoReC.json
--rw-r--r--   0 root         (0) root         (0)      439 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/embed-multilingual-v3.0/Norwegian_parliament.json
--rw-r--r--   0 root         (0) root         (0)     1083 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/embed-multilingual-v3.0/ScaLA.json
--rw-r--r--   0 root         (0) root         (0)      838 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/embed-multilingual-v3.0/SweFAQ.json
--rw-r--r--   0 root         (0) root         (0)      357 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/embed-multilingual-v3.0/SweReC.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 10:06:38.448314 seb-0.9.3/src/seb/cache/fasttext-cc-da-300/
--rw-r--r--   0 root         (0) root         (0)      399 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/fasttext-cc-da-300/Angry_Tweets.json
--rw-r--r--   0 root         (0) root         (0)      613 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/fasttext-cc-da-300/Bornholm_Parallel.json
--rw-r--r--   0 root         (0) root         (0)      435 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/fasttext-cc-da-300/DKHate.json
--rw-r--r--   0 root         (0) root         (0)      449 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/fasttext-cc-da-300/DaLAJ.json
--rw-r--r--   0 root         (0) root         (0)      385 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/fasttext-cc-da-300/Da_Political_Comments.json
--rw-r--r--   0 root         (0) root         (0)      361 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/fasttext-cc-da-300/LCC.json
--rw-r--r--   0 root         (0) root         (0)     1197 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/fasttext-cc-da-300/Language_Identification.json
--rw-r--r--   0 root         (0) root         (0)      764 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/fasttext-cc-da-300/Massive_Intent.json
--rw-r--r--   0 root         (0) root         (0)      769 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/fasttext-cc-da-300/Massive_Scenario.json
--rw-r--r--   0 root         (0) root         (0)      357 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/fasttext-cc-da-300/NoReC.json
--rw-r--r--   0 root         (0) root         (0)      501 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/fasttext-cc-da-300/Norwegian_parliament.json
--rw-r--r--   0 root         (0) root         (0)     1087 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/fasttext-cc-da-300/ScaLA.json
--rw-r--r--   0 root         (0) root         (0)      844 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/fasttext-cc-da-300/SweFAQ.json
--rw-r--r--   0 root         (0) root         (0)      356 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/fasttext-cc-da-300/SweReC.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 10:06:38.452314 seb-0.9.3/src/seb/cache/fasttext-cc-nb-300/
--rw-r--r--   0 root         (0) root         (0)      393 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/fasttext-cc-nb-300/Angry_Tweets.json
--rw-r--r--   0 root         (0) root         (0)      619 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/fasttext-cc-nb-300/Bornholm_Parallel.json
--rw-r--r--   0 root         (0) root         (0)      435 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/fasttext-cc-nb-300/DKHate.json
--rw-r--r--   0 root         (0) root         (0)      442 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/fasttext-cc-nb-300/DaLAJ.json
--rw-r--r--   0 root         (0) root         (0)      381 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/fasttext-cc-nb-300/Da_Political_Comments.json
--rw-r--r--   0 root         (0) root         (0)      359 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/fasttext-cc-nb-300/LCC.json
--rw-r--r--   0 root         (0) root         (0)     1197 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/fasttext-cc-nb-300/Language_Identification.json
--rw-r--r--   0 root         (0) root         (0)      765 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/fasttext-cc-nb-300/Massive_Intent.json
--rw-r--r--   0 root         (0) root         (0)      768 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/fasttext-cc-nb-300/Massive_Scenario.json
--rw-r--r--   0 root         (0) root         (0)      357 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/fasttext-cc-nb-300/NoReC.json
--rw-r--r--   0 root         (0) root         (0)      479 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/fasttext-cc-nb-300/Norwegian_parliament.json
--rw-r--r--   0 root         (0) root         (0)     1090 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/fasttext-cc-nb-300/ScaLA.json
--rw-r--r--   0 root         (0) root         (0)      843 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/fasttext-cc-nb-300/SweFAQ.json
--rw-r--r--   0 root         (0) root         (0)      356 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/fasttext-cc-nb-300/SweReC.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 10:06:38.456314 seb-0.9.3/src/seb/cache/fasttext-cc-nn-300/
--rw-r--r--   0 root         (0) root         (0)      395 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/fasttext-cc-nn-300/Angry_Tweets.json
--rw-r--r--   0 root         (0) root         (0)      619 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/fasttext-cc-nn-300/Bornholm_Parallel.json
--rw-r--r--   0 root         (0) root         (0)      434 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/fasttext-cc-nn-300/DKHate.json
--rw-r--r--   0 root         (0) root         (0)      448 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/fasttext-cc-nn-300/DaLAJ.json
--rw-r--r--   0 root         (0) root         (0)      384 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/fasttext-cc-nn-300/Da_Political_Comments.json
--rw-r--r--   0 root         (0) root         (0)      336 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/fasttext-cc-nn-300/LCC.json
--rw-r--r--   0 root         (0) root         (0)     1197 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/fasttext-cc-nn-300/Language_Identification.json
--rw-r--r--   0 root         (0) root         (0)      766 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/fasttext-cc-nn-300/Massive_Intent.json
--rw-r--r--   0 root         (0) root         (0)      769 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/fasttext-cc-nn-300/Massive_Scenario.json
--rw-r--r--   0 root         (0) root         (0)      356 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/fasttext-cc-nn-300/NoReC.json
--rw-r--r--   0 root         (0) root         (0)      502 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/fasttext-cc-nn-300/Norwegian_parliament.json
--rw-r--r--   0 root         (0) root         (0)     1074 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/fasttext-cc-nn-300/ScaLA.json
--rw-r--r--   0 root         (0) root         (0)      838 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/fasttext-cc-nn-300/SweFAQ.json
--rw-r--r--   0 root         (0) root         (0)      357 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/fasttext-cc-nn-300/SweReC.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 10:06:38.456314 seb-0.9.3/src/seb/cache/fasttext-cc-sv-300/
--rw-r--r--   0 root         (0) root         (0)      393 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/fasttext-cc-sv-300/Angry_Tweets.json
--rw-r--r--   0 root         (0) root         (0)      619 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/fasttext-cc-sv-300/Bornholm_Parallel.json
--rw-r--r--   0 root         (0) root         (0)      434 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/fasttext-cc-sv-300/DKHate.json
--rw-r--r--   0 root         (0) root         (0)      448 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/fasttext-cc-sv-300/DaLAJ.json
--rw-r--r--   0 root         (0) root         (0)      382 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/fasttext-cc-sv-300/Da_Political_Comments.json
--rw-r--r--   0 root         (0) root         (0)      364 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/fasttext-cc-sv-300/LCC.json
--rw-r--r--   0 root         (0) root         (0)     1185 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/fasttext-cc-sv-300/Language_Identification.json
--rw-r--r--   0 root         (0) root         (0)      762 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/fasttext-cc-sv-300/Massive_Intent.json
--rw-r--r--   0 root         (0) root         (0)      761 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/fasttext-cc-sv-300/Massive_Scenario.json
--rw-r--r--   0 root         (0) root         (0)      357 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/fasttext-cc-sv-300/NoReC.json
--rw-r--r--   0 root         (0) root         (0)      503 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/fasttext-cc-sv-300/Norwegian_parliament.json
--rw-r--r--   0 root         (0) root         (0)     1080 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/fasttext-cc-sv-300/ScaLA.json
--rw-r--r--   0 root         (0) root         (0)      843 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/fasttext-cc-sv-300/SweFAQ.json
--rw-r--r--   0 root         (0) root         (0)      357 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/fasttext-cc-sv-300/SweReC.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 10:06:38.460314 seb-0.9.3/src/seb/cache/intfloat__e5-base/
--rw-r--r--   0 root         (0) root         (0)      401 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__e5-base/Angry_Tweets.json
--rw-r--r--   0 root         (0) root         (0)      621 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__e5-base/Bornholm_Parallel.json
--rw-r--r--   0 root         (0) root         (0)      439 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__e5-base/DKHate.json
--rw-r--r--   0 root         (0) root         (0)      450 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__e5-base/DaLAJ.json
--rw-r--r--   0 root         (0) root         (0)      390 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__e5-base/Da_Political_Comments.json
--rw-r--r--   0 root         (0) root         (0)      366 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__e5-base/LCC.json
--rw-r--r--   0 root         (0) root         (0)     1196 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__e5-base/Language_Identification.json
--rw-r--r--   0 root         (0) root         (0)      767 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__e5-base/Massive_Intent.json
--rw-r--r--   0 root         (0) root         (0)      763 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__e5-base/Massive_Scenario.json
--rw-r--r--   0 root         (0) root         (0)      363 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__e5-base/NoReC.json
--rw-r--r--   0 root         (0) root         (0)      437 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__e5-base/Norwegian_parliament.json
--rw-r--r--   0 root         (0) root         (0)     1093 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__e5-base/ScaLA.json
--rw-r--r--   0 root         (0) root         (0)      841 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__e5-base/SweFAQ.json
--rw-r--r--   0 root         (0) root         (0)      360 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__e5-base/SweReC.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 10:06:38.464314 seb-0.9.3/src/seb/cache/intfloat__e5-large/
--rw-r--r--   0 root         (0) root         (0)      400 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__e5-large/Angry_Tweets.json
--rw-r--r--   0 root         (0) root         (0)      614 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__e5-large/Bornholm_Parallel.json
--rw-r--r--   0 root         (0) root         (0)      440 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__e5-large/DKHate.json
--rw-r--r--   0 root         (0) root         (0)      451 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__e5-large/DaLAJ.json
--rw-r--r--   0 root         (0) root         (0)      386 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__e5-large/Da_Political_Comments.json
--rw-r--r--   0 root         (0) root         (0)      367 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__e5-large/LCC.json
--rw-r--r--   0 root         (0) root         (0)     1190 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__e5-large/Language_Identification.json
--rw-r--r--   0 root         (0) root         (0)      768 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__e5-large/Massive_Intent.json
--rw-r--r--   0 root         (0) root         (0)      763 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__e5-large/Massive_Scenario.json
--rw-r--r--   0 root         (0) root         (0)      364 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__e5-large/NoReC.json
--rw-r--r--   0 root         (0) root         (0)      439 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__e5-large/Norwegian_parliament.json
--rw-r--r--   0 root         (0) root         (0)     1101 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__e5-large/ScaLA.json
--rw-r--r--   0 root         (0) root         (0)      845 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__e5-large/SweFAQ.json
--rw-r--r--   0 root         (0) root         (0)      361 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__e5-large/SweReC.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 10:06:38.464314 seb-0.9.3/src/seb/cache/intfloat__e5-mistral-7b-instruct/
--rw-r--r--   0 root         (0) root         (0)      396 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__e5-mistral-7b-instruct/Angry_Tweets.json
--rw-r--r--   0 root         (0) root         (0)      619 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__e5-mistral-7b-instruct/Bornholm_Parallel.json
--rw-r--r--   0 root         (0) root         (0)      434 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__e5-mistral-7b-instruct/DKHate.json
--rw-r--r--   0 root         (0) root         (0)      448 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__e5-mistral-7b-instruct/DaLAJ.json
--rw-r--r--   0 root         (0) root         (0)      386 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__e5-mistral-7b-instruct/Da_Political_Comments.json
--rw-r--r--   0 root         (0) root         (0)      334 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__e5-mistral-7b-instruct/LCC.json
--rw-r--r--   0 root         (0) root         (0)     1197 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__e5-mistral-7b-instruct/Language_Identification.json
--rw-r--r--   0 root         (0) root         (0)      758 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__e5-mistral-7b-instruct/Massive_Intent.json
--rw-r--r--   0 root         (0) root         (0)      761 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__e5-mistral-7b-instruct/Massive_Scenario.json
--rw-r--r--   0 root         (0) root         (0)      357 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__e5-mistral-7b-instruct/NoReC.json
--rw-r--r--   0 root         (0) root         (0)      502 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__e5-mistral-7b-instruct/Norwegian_parliament.json
--rw-r--r--   0 root         (0) root         (0)     1069 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__e5-mistral-7b-instruct/ScaLA.json
--rw-r--r--   0 root         (0) root         (0)      840 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__e5-mistral-7b-instruct/SweFAQ.json
--rw-r--r--   0 root         (0) root         (0)      356 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__e5-mistral-7b-instruct/SweReC.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 10:06:38.468314 seb-0.9.3/src/seb/cache/intfloat__e5-small/
--rw-r--r--   0 root         (0) root         (0)      400 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__e5-small/Angry_Tweets.json
--rw-r--r--   0 root         (0) root         (0)      616 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__e5-small/Bornholm_Parallel.json
--rw-r--r--   0 root         (0) root         (0)      439 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__e5-small/DKHate.json
--rw-r--r--   0 root         (0) root         (0)      453 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__e5-small/DaLAJ.json
--rw-r--r--   0 root         (0) root         (0)      390 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__e5-small/Da_Political_Comments.json
--rw-r--r--   0 root         (0) root         (0)      366 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__e5-small/LCC.json
--rw-r--r--   0 root         (0) root         (0)     1202 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__e5-small/Language_Identification.json
--rw-r--r--   0 root         (0) root         (0)      769 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__e5-small/Massive_Intent.json
--rw-r--r--   0 root         (0) root         (0)      770 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__e5-small/Massive_Scenario.json
--rw-r--r--   0 root         (0) root         (0)      357 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__e5-small/NoReC.json
--rw-r--r--   0 root         (0) root         (0)      438 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__e5-small/Norwegian_parliament.json
--rw-r--r--   0 root         (0) root         (0)     1104 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__e5-small/ScaLA.json
--rw-r--r--   0 root         (0) root         (0)      841 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__e5-small/SweFAQ.json
--rw-r--r--   0 root         (0) root         (0)      362 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__e5-small/SweReC.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 10:06:38.472314 seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-base/
--rw-r--r--   0 root         (0) root         (0)      401 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-base/Angry_Tweets.json
--rw-r--r--   0 root         (0) root         (0)      617 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-base/Bornholm_Parallel.json
--rw-r--r--   0 root         (0) root         (0)      437 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-base/DKHate.json
--rw-r--r--   0 root         (0) root         (0)      450 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-base/DaLAJ.json
--rw-r--r--   0 root         (0) root         (0)      388 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-base/Da_Political_Comments.json
--rw-r--r--   0 root         (0) root         (0)      366 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-base/LCC.json
--rw-r--r--   0 root         (0) root         (0)     1190 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-base/Language_Identification.json
--rw-r--r--   0 root         (0) root         (0)      765 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-base/Massive_Intent.json
--rw-r--r--   0 root         (0) root         (0)      766 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-base/Massive_Scenario.json
--rw-r--r--   0 root         (0) root         (0)      363 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-base/NoReC.json
--rw-r--r--   0 root         (0) root         (0)      438 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-base/Norwegian_parliament.json
--rw-r--r--   0 root         (0) root         (0)     1096 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-base/ScaLA.json
--rw-r--r--   0 root         (0) root         (0)      842 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-base/SweFAQ.json
--rw-r--r--   0 root         (0) root         (0)      360 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-base/SweReC.json
--rw-r--r--   0 root         (0) root         (0)      864 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-base/SwednRetrieval.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 10:06:38.472314 seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-large/
--rw-r--r--   0 root         (0) root         (0)      399 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-large/Angry_Tweets.json
--rw-r--r--   0 root         (0) root         (0)      621 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-large/Bornholm_Parallel.json
--rw-r--r--   0 root         (0) root         (0)      439 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-large/DKHate.json
--rw-r--r--   0 root         (0) root         (0)      455 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-large/DaLAJ.json
--rw-r--r--   0 root         (0) root         (0)      390 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-large/Da_Political_Comments.json
--rw-r--r--   0 root         (0) root         (0)      365 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-large/LCC.json
--rw-r--r--   0 root         (0) root         (0)     1196 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-large/Language_Identification.json
--rw-r--r--   0 root         (0) root         (0)      758 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-large/Massive_Intent.json
--rw-r--r--   0 root         (0) root         (0)      765 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-large/Massive_Scenario.json
--rw-r--r--   0 root         (0) root         (0)      363 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-large/NoReC.json
--rw-r--r--   0 root         (0) root         (0)      439 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-large/Norwegian_parliament.json
--rw-r--r--   0 root         (0) root         (0)     1081 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-large/ScaLA.json
--rw-r--r--   0 root         (0) root         (0)      842 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-large/SweFAQ.json
--rw-r--r--   0 root         (0) root         (0)      359 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-large/SweReC.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 10:06:38.476314 seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-small/
--rw-r--r--   0 root         (0) root         (0)      397 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-small/Angry_Tweets.json
--rw-r--r--   0 root         (0) root         (0)      622 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-small/Bornholm_Parallel.json
--rw-r--r--   0 root         (0) root         (0)      439 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-small/DKHate.json
--rw-r--r--   0 root         (0) root         (0)      452 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-small/DaLAJ.json
--rw-r--r--   0 root         (0) root         (0)      386 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-small/Da_Political_Comments.json
--rw-r--r--   0 root         (0) root         (0)      922 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-small/DanFEVER.json
--rw-r--r--   0 root         (0) root         (0)      366 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-small/LCC.json
--rw-r--r--   0 root         (0) root         (0)     1202 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-small/Language_Identification.json
--rw-r--r--   0 root         (0) root         (0)      764 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-small/Massive_Intent.json
--rw-r--r--   0 root         (0) root         (0)      767 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-small/Massive_Scenario.json
--rw-r--r--   0 root         (0) root         (0)      362 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-small/NoReC.json
--rw-r--r--   0 root         (0) root         (0)      437 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-small/Norwegian_parliament.json
--rw-r--r--   0 root         (0) root         (0)     1095 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-small/ScaLA.json
--rw-r--r--   0 root         (0) root         (0)      841 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-small/SweFAQ.json
--rw-r--r--   0 root         (0) root         (0)      359 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-small/SweReC.json
--rw-r--r--   0 root         (0) root         (0)      507 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-small/SwednClustering.json
--rw-r--r--   0 root         (0) root         (0)      869 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-small/SwednRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      444 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-small/SwednSTS.json
--rw-r--r--   0 root         (0) root         (0)      353 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-small/VGSummarizationClustering.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 10:06:38.480314 seb-0.9.3/src/seb/cache/jonfd__electra-small-nordic/
--rw-r--r--   0 root         (0) root         (0)      401 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/jonfd__electra-small-nordic/Angry_Tweets.json
--rw-r--r--   0 root         (0) root         (0)      624 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/jonfd__electra-small-nordic/Bornholm_Parallel.json
--rw-r--r--   0 root         (0) root         (0)      439 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/jonfd__electra-small-nordic/DKHate.json
--rw-r--r--   0 root         (0) root         (0)      444 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/jonfd__electra-small-nordic/DaLAJ.json
--rw-r--r--   0 root         (0) root         (0)      389 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/jonfd__electra-small-nordic/Da_Political_Comments.json
--rw-r--r--   0 root         (0) root         (0)      365 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/jonfd__electra-small-nordic/LCC.json
--rw-r--r--   0 root         (0) root         (0)     1196 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/jonfd__electra-small-nordic/Language_Identification.json
--rw-r--r--   0 root         (0) root         (0)      773 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/jonfd__electra-small-nordic/Massive_Intent.json
--rw-r--r--   0 root         (0) root         (0)      771 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/jonfd__electra-small-nordic/Massive_Scenario.json
--rw-r--r--   0 root         (0) root         (0)      362 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/jonfd__electra-small-nordic/NoReC.json
--rw-r--r--   0 root         (0) root         (0)      414 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/jonfd__electra-small-nordic/Norwegian_parliament.json
--rw-r--r--   0 root         (0) root         (0)     1596 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/jonfd__electra-small-nordic/ScaLA.json
--rw-r--r--   0 root         (0) root         (0)      843 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/jonfd__electra-small-nordic/SweFAQ.json
--rw-r--r--   0 root         (0) root         (0)      363 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/jonfd__electra-small-nordic/SweReC.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 10:06:38.480314 seb-0.9.3/src/seb/cache/kb__electra-small-swedish-cased-discriminator/
--rw-r--r--   0 root         (0) root         (0)      401 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/kb__electra-small-swedish-cased-discriminator/Angry_Tweets.json
--rw-r--r--   0 root         (0) root         (0)      630 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/kb__electra-small-swedish-cased-discriminator/Bornholm_Parallel.json
--rw-r--r--   0 root         (0) root         (0)      439 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/kb__electra-small-swedish-cased-discriminator/DKHate.json
--rw-r--r--   0 root         (0) root         (0)      446 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/kb__electra-small-swedish-cased-discriminator/DaLAJ.json
--rw-r--r--   0 root         (0) root         (0)      389 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/kb__electra-small-swedish-cased-discriminator/Da_Political_Comments.json
--rw-r--r--   0 root         (0) root         (0)      367 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/kb__electra-small-swedish-cased-discriminator/LCC.json
--rw-r--r--   0 root         (0) root         (0)     1196 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/kb__electra-small-swedish-cased-discriminator/Language_Identification.json
--rw-r--r--   0 root         (0) root         (0)      775 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/kb__electra-small-swedish-cased-discriminator/Massive_Intent.json
--rw-r--r--   0 root         (0) root         (0)      776 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/kb__electra-small-swedish-cased-discriminator/Massive_Scenario.json
--rw-r--r--   0 root         (0) root         (0)      362 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/kb__electra-small-swedish-cased-discriminator/NoReC.json
--rw-r--r--   0 root         (0) root         (0)      436 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/kb__electra-small-swedish-cased-discriminator/Norwegian_parliament.json
--rw-r--r--   0 root         (0) root         (0)     1090 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/kb__electra-small-swedish-cased-discriminator/ScaLA.json
--rw-r--r--   0 root         (0) root         (0)      843 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/kb__electra-small-swedish-cased-discriminator/SweFAQ.json
--rw-r--r--   0 root         (0) root         (0)      363 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/kb__electra-small-swedish-cased-discriminator/SweReC.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 10:06:38.484314 seb-0.9.3/src/seb/cache/sentence-transformers__all-MiniLM-L6-v2/
--rw-r--r--   0 root         (0) root         (0)      403 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sentence-transformers__all-MiniLM-L6-v2/Angry_Tweets.json
--rw-r--r--   0 root         (0) root         (0)      616 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sentence-transformers__all-MiniLM-L6-v2/Bornholm_Parallel.json
--rw-r--r--   0 root         (0) root         (0)      434 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sentence-transformers__all-MiniLM-L6-v2/DKHate.json
--rw-r--r--   0 root         (0) root         (0)      450 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sentence-transformers__all-MiniLM-L6-v2/DaLAJ.json
--rw-r--r--   0 root         (0) root         (0)      391 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sentence-transformers__all-MiniLM-L6-v2/Da_Political_Comments.json
--rw-r--r--   0 root         (0) root         (0)      925 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sentence-transformers__all-MiniLM-L6-v2/DanFEVER.json
--rw-r--r--   0 root         (0) root         (0)      365 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sentence-transformers__all-MiniLM-L6-v2/LCC.json
--rw-r--r--   0 root         (0) root         (0)     1058 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sentence-transformers__all-MiniLM-L6-v2/Language_Identification.json
--rw-r--r--   0 root         (0) root         (0)      769 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sentence-transformers__all-MiniLM-L6-v2/Massive_Intent.json
--rw-r--r--   0 root         (0) root         (0)      773 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sentence-transformers__all-MiniLM-L6-v2/Massive_Scenario.json
--rw-r--r--   0 root         (0) root         (0)      359 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sentence-transformers__all-MiniLM-L6-v2/NoReC.json
--rw-r--r--   0 root         (0) root         (0)      413 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sentence-transformers__all-MiniLM-L6-v2/Norwegian_parliament.json
--rw-r--r--   0 root         (0) root         (0)     1095 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sentence-transformers__all-MiniLM-L6-v2/ScaLA.json
--rw-r--r--   0 root         (0) root         (0)      838 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sentence-transformers__all-MiniLM-L6-v2/SweFAQ.json
--rw-r--r--   0 root         (0) root         (0)      356 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sentence-transformers__all-MiniLM-L6-v2/SweReC.json
--rw-r--r--   0 root         (0) root         (0)      508 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sentence-transformers__all-MiniLM-L6-v2/SwednClustering.json
--rw-r--r--   0 root         (0) root         (0)      872 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sentence-transformers__all-MiniLM-L6-v2/SwednRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      443 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sentence-transformers__all-MiniLM-L6-v2/SwednSTS.json
--rw-r--r--   0 root         (0) root         (0)      352 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sentence-transformers__all-MiniLM-L6-v2/VGSummarizationClustering.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 10:06:38.488314 seb-0.9.3/src/seb/cache/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/
--rw-r--r--   0 root         (0) root         (0)      401 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/Angry_Tweets.json
--rw-r--r--   0 root         (0) root         (0)      624 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/Bornholm_Parallel.json
--rw-r--r--   0 root         (0) root         (0)      439 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DKHate.json
--rw-r--r--   0 root         (0) root         (0)      448 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DaLAJ.json
--rw-r--r--   0 root         (0) root         (0)      386 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/Da_Political_Comments.json
--rw-r--r--   0 root         (0) root         (0)      364 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LCC.json
--rw-r--r--   0 root         (0) root         (0)     1208 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/Language_Identification.json
--rw-r--r--   0 root         (0) root         (0)      762 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/Massive_Intent.json
--rw-r--r--   0 root         (0) root         (0)      767 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/Massive_Scenario.json
--rw-r--r--   0 root         (0) root         (0)      364 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NoReC.json
--rw-r--r--   0 root         (0) root         (0)      439 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/Norwegian_parliament.json
--rw-r--r--   0 root         (0) root         (0)     1605 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ScaLA.json
--rw-r--r--   0 root         (0) root         (0)      845 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SweFAQ.json
--rw-r--r--   0 root         (0) root         (0)      363 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SweReC.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 10:06:38.492314 seb-0.9.3/src/seb/cache/sentence-transformers__paraphrase-multilingual-mpnet-base-v2/
--rw-r--r--   0 root         (0) root         (0)      400 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sentence-transformers__paraphrase-multilingual-mpnet-base-v2/Angry_Tweets.json
--rw-r--r--   0 root         (0) root         (0)      624 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sentence-transformers__paraphrase-multilingual-mpnet-base-v2/Bornholm_Parallel.json
--rw-r--r--   0 root         (0) root         (0)      437 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sentence-transformers__paraphrase-multilingual-mpnet-base-v2/DKHate.json
--rw-r--r--   0 root         (0) root         (0)      452 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sentence-transformers__paraphrase-multilingual-mpnet-base-v2/DaLAJ.json
--rw-r--r--   0 root         (0) root         (0)      387 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sentence-transformers__paraphrase-multilingual-mpnet-base-v2/Da_Political_Comments.json
--rw-r--r--   0 root         (0) root         (0)      340 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sentence-transformers__paraphrase-multilingual-mpnet-base-v2/LCC.json
--rw-r--r--   0 root         (0) root         (0)     1208 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sentence-transformers__paraphrase-multilingual-mpnet-base-v2/Language_Identification.json
--rw-r--r--   0 root         (0) root         (0)      766 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sentence-transformers__paraphrase-multilingual-mpnet-base-v2/Massive_Intent.json
--rw-r--r--   0 root         (0) root         (0)      766 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sentence-transformers__paraphrase-multilingual-mpnet-base-v2/Massive_Scenario.json
--rw-r--r--   0 root         (0) root         (0)      360 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sentence-transformers__paraphrase-multilingual-mpnet-base-v2/NoReC.json
--rw-r--r--   0 root         (0) root         (0)      412 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sentence-transformers__paraphrase-multilingual-mpnet-base-v2/Norwegian_parliament.json
--rw-r--r--   0 root         (0) root         (0)     1100 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sentence-transformers__paraphrase-multilingual-mpnet-base-v2/ScaLA.json
--rw-r--r--   0 root         (0) root         (0)      845 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sentence-transformers__paraphrase-multilingual-mpnet-base-v2/SweFAQ.json
--rw-r--r--   0 root         (0) root         (0)      363 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sentence-transformers__paraphrase-multilingual-mpnet-base-v2/SweReC.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 10:06:38.492314 seb-0.9.3/src/seb/cache/sonar-dan/
--rw-r--r--   0 root         (0) root         (0)      395 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sonar-dan/Angry_Tweets.json
--rw-r--r--   0 root         (0) root         (0)      617 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sonar-dan/Bornholm_Parallel.json
--rw-r--r--   0 root         (0) root         (0)      435 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sonar-dan/DKHate.json
--rw-r--r--   0 root         (0) root         (0)      448 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sonar-dan/DaLAJ.json
--rw-r--r--   0 root         (0) root         (0)      386 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sonar-dan/Da_Political_Comments.json
--rw-r--r--   0 root         (0) root         (0)      361 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sonar-dan/LCC.json
--rw-r--r--   0 root         (0) root         (0)     1215 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sonar-dan/Language_Identification.json
--rw-r--r--   0 root         (0) root         (0)      759 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sonar-dan/Massive_Intent.json
--rw-r--r--   0 root         (0) root         (0)      761 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sonar-dan/Massive_Scenario.json
--rw-r--r--   0 root         (0) root         (0)      360 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sonar-dan/NoReC.json
--rw-r--r--   0 root         (0) root         (0)      433 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sonar-dan/Norwegian_parliament.json
--rw-r--r--   0 root         (0) root         (0)     1592 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sonar-dan/ScaLA.json
--rw-r--r--   0 root         (0) root         (0)      845 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sonar-dan/SweFAQ.json
--rw-r--r--   0 root         (0) root         (0)      358 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sonar-dan/SweReC.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 10:06:38.496314 seb-0.9.3/src/seb/cache/sonar-nno/
--rw-r--r--   0 root         (0) root         (0)      395 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sonar-nno/Angry_Tweets.json
--rw-r--r--   0 root         (0) root         (0)      619 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sonar-nno/Bornholm_Parallel.json
--rw-r--r--   0 root         (0) root         (0)      432 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sonar-nno/DKHate.json
--rw-r--r--   0 root         (0) root         (0)      448 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sonar-nno/DaLAJ.json
--rw-r--r--   0 root         (0) root         (0)      383 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sonar-nno/Da_Political_Comments.json
--rw-r--r--   0 root         (0) root         (0)      361 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sonar-nno/LCC.json
--rw-r--r--   0 root         (0) root         (0)     1053 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sonar-nno/Language_Identification.json
--rw-r--r--   0 root         (0) root         (0)      759 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sonar-nno/Massive_Intent.json
--rw-r--r--   0 root         (0) root         (0)      756 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sonar-nno/Massive_Scenario.json
--rw-r--r--   0 root         (0) root         (0)      349 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sonar-nno/NoReC.json
--rw-r--r--   0 root         (0) root         (0)      431 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sonar-nno/Norwegian_parliament.json
--rw-r--r--   0 root         (0) root         (0)     1090 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sonar-nno/ScaLA.json
--rw-r--r--   0 root         (0) root         (0)      837 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sonar-nno/SweFAQ.json
--rw-r--r--   0 root         (0) root         (0)      356 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sonar-nno/SweReC.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 10:06:38.500314 seb-0.9.3/src/seb/cache/sonar-nob/
--rw-r--r--   0 root         (0) root         (0)      395 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sonar-nob/Angry_Tweets.json
--rw-r--r--   0 root         (0) root         (0)      617 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sonar-nob/Bornholm_Parallel.json
--rw-r--r--   0 root         (0) root         (0)      433 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sonar-nob/DKHate.json
--rw-r--r--   0 root         (0) root         (0)      448 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sonar-nob/DaLAJ.json
--rw-r--r--   0 root         (0) root         (0)      382 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sonar-nob/Da_Political_Comments.json
--rw-r--r--   0 root         (0) root         (0)      361 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sonar-nob/LCC.json
--rw-r--r--   0 root         (0) root         (0)     1191 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sonar-nob/Language_Identification.json
--rw-r--r--   0 root         (0) root         (0)      761 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sonar-nob/Massive_Intent.json
--rw-r--r--   0 root         (0) root         (0)      761 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sonar-nob/Massive_Scenario.json
--rw-r--r--   0 root         (0) root         (0)      358 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sonar-nob/NoReC.json
--rw-r--r--   0 root         (0) root         (0)      432 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sonar-nob/Norwegian_parliament.json
--rw-r--r--   0 root         (0) root         (0)     1598 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sonar-nob/ScaLA.json
--rw-r--r--   0 root         (0) root         (0)      841 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sonar-nob/SweFAQ.json
--rw-r--r--   0 root         (0) root         (0)      357 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sonar-nob/SweReC.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 10:06:38.500314 seb-0.9.3/src/seb/cache/sonar-swe/
--rw-r--r--   0 root         (0) root         (0)      396 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sonar-swe/Angry_Tweets.json
--rw-r--r--   0 root         (0) root         (0)      615 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sonar-swe/Bornholm_Parallel.json
--rw-r--r--   0 root         (0) root         (0)      435 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sonar-swe/DKHate.json
--rw-r--r--   0 root         (0) root         (0)      446 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sonar-swe/DaLAJ.json
--rw-r--r--   0 root         (0) root         (0)      383 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sonar-swe/Da_Political_Comments.json
--rw-r--r--   0 root         (0) root         (0)      360 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sonar-swe/LCC.json
--rw-r--r--   0 root         (0) root         (0)     1197 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sonar-swe/Language_Identification.json
--rw-r--r--   0 root         (0) root         (0)      759 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sonar-swe/Massive_Intent.json
--rw-r--r--   0 root         (0) root         (0)      759 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sonar-swe/Massive_Scenario.json
--rw-r--r--   0 root         (0) root         (0)      358 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sonar-swe/NoReC.json
--rw-r--r--   0 root         (0) root         (0)      433 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sonar-swe/Norwegian_parliament.json
--rw-r--r--   0 root         (0) root         (0)     1588 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sonar-swe/ScaLA.json
--rw-r--r--   0 root         (0) root         (0)      842 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sonar-swe/SweFAQ.json
--rw-r--r--   0 root         (0) root         (0)      355 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/sonar-swe/SweReC.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 10:06:38.500314 seb-0.9.3/src/seb/cache/text-embedding-3-large/
--rw-r--r--   0 root         (0) root         (0)      434 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/text-embedding-3-large/DKHate.json
--rw-r--r--   0 root         (0) root         (0)      842 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/text-embedding-3-large/SweFAQ.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 10:06:38.504315 seb-0.9.3/src/seb/cache/text-embedding-3-small/
--rw-r--r--   0 root         (0) root         (0)      433 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/text-embedding-3-small/DKHate.json
--rw-r--r--   0 root         (0) root         (0)      841 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/text-embedding-3-small/SweFAQ.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 10:06:38.504315 seb-0.9.3/src/seb/cache/text-embedding-ada-002/
--rw-r--r--   0 root         (0) root         (0)      399 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/text-embedding-ada-002/Angry_Tweets.json
--rw-r--r--   0 root         (0) root         (0)      620 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/text-embedding-ada-002/Bornholm_Parallel.json
--rw-r--r--   0 root         (0) root         (0)      441 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/text-embedding-ada-002/DKHate.json
--rw-r--r--   0 root         (0) root         (0)      452 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/text-embedding-ada-002/DaLAJ.json
--rw-r--r--   0 root         (0) root         (0)      387 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/text-embedding-ada-002/Da_Political_Comments.json
--rw-r--r--   0 root         (0) root         (0)      366 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/text-embedding-ada-002/LCC.json
--rw-r--r--   0 root         (0) root         (0)     1196 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/text-embedding-ada-002/Language_Identification.json
--rw-r--r--   0 root         (0) root         (0)      764 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/text-embedding-ada-002/Massive_Intent.json
--rw-r--r--   0 root         (0) root         (0)      767 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/text-embedding-ada-002/Massive_Scenario.json
--rw-r--r--   0 root         (0) root         (0)      363 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/text-embedding-ada-002/NoReC.json
--rw-r--r--   0 root         (0) root         (0)      438 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/text-embedding-ada-002/Norwegian_parliament.json
--rw-r--r--   0 root         (0) root         (0)     1092 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/text-embedding-ada-002/ScaLA.json
--rw-r--r--   0 root         (0) root         (0)      839 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/text-embedding-ada-002/SweFAQ.json
--rw-r--r--   0 root         (0) root         (0)      358 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/text-embedding-ada-002/SweReC.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 10:06:38.508314 seb-0.9.3/src/seb/cache/vesteinn__DanskBERT/
--rw-r--r--   0 root         (0) root         (0)      400 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/vesteinn__DanskBERT/Angry_Tweets.json
--rw-r--r--   0 root         (0) root         (0)      622 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/vesteinn__DanskBERT/Bornholm_Parallel.json
--rw-r--r--   0 root         (0) root         (0)      440 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/vesteinn__DanskBERT/DKHate.json
--rw-r--r--   0 root         (0) root         (0)      450 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/vesteinn__DanskBERT/DaLAJ.json
--rw-r--r--   0 root         (0) root         (0)      388 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/vesteinn__DanskBERT/Da_Political_Comments.json
--rw-r--r--   0 root         (0) root         (0)      338 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/vesteinn__DanskBERT/LCC.json
--rw-r--r--   0 root         (0) root         (0)     1202 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/vesteinn__DanskBERT/Language_Identification.json
--rw-r--r--   0 root         (0) root         (0)      769 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/vesteinn__DanskBERT/Massive_Intent.json
--rw-r--r--   0 root         (0) root         (0)      769 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/vesteinn__DanskBERT/Massive_Scenario.json
--rw-r--r--   0 root         (0) root         (0)      364 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/vesteinn__DanskBERT/NoReC.json
--rw-r--r--   0 root         (0) root         (0)      435 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/vesteinn__DanskBERT/Norwegian_parliament.json
--rw-r--r--   0 root         (0) root         (0)     1598 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/vesteinn__DanskBERT/ScaLA.json
--rw-r--r--   0 root         (0) root         (0)      844 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/vesteinn__DanskBERT/SweFAQ.json
--rw-r--r--   0 root         (0) root         (0)      363 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/vesteinn__DanskBERT/SweReC.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 10:06:38.508314 seb-0.9.3/src/seb/cache/xlm-roberta-base/
--rw-r--r--   0 root         (0) root         (0)      399 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/xlm-roberta-base/Angry_Tweets.json
--rw-r--r--   0 root         (0) root         (0)      624 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/xlm-roberta-base/Bornholm_Parallel.json
--rw-r--r--   0 root         (0) root         (0)      439 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/xlm-roberta-base/DKHate.json
--rw-r--r--   0 root         (0) root         (0)      450 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/xlm-roberta-base/DaLAJ.json
--rw-r--r--   0 root         (0) root         (0)      389 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/xlm-roberta-base/Da_Political_Comments.json
--rw-r--r--   0 root         (0) root         (0)      366 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/xlm-roberta-base/LCC.json
--rw-r--r--   0 root         (0) root         (0)     1195 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/xlm-roberta-base/Language_Identification.json
--rw-r--r--   0 root         (0) root         (0)      766 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/xlm-roberta-base/Massive_Intent.json
--rw-r--r--   0 root         (0) root         (0)      769 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/xlm-roberta-base/Massive_Scenario.json
--rw-r--r--   0 root         (0) root         (0)      359 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/xlm-roberta-base/NoReC.json
--rw-r--r--   0 root         (0) root         (0)      436 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/xlm-roberta-base/Norwegian_parliament.json
--rw-r--r--   0 root         (0) root         (0)     1087 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/xlm-roberta-base/ScaLA.json
--rw-r--r--   0 root         (0) root         (0)      836 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/xlm-roberta-base/SweFAQ.json
--rw-r--r--   0 root         (0) root         (0)      360 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cache/xlm-roberta-base/SweReC.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 10:06:38.512314 seb-0.9.3/src/seb/cli/
--rw-r--r--   0 root         (0) root         (0)       66 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)      118 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cli/cli.py
--rw-r--r--   0 root         (0) root         (0)     1087 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cli/import_code.py
--rw-r--r--   0 root         (0) root         (0)     5668 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cli/run.py
--rw-r--r--   0 root         (0) root         (0)     4492 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/cli/table.py
--rw-r--r--   0 root         (0) root         (0)     2210 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/full_benchmark.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 10:06:38.512314 seb-0.9.3/src/seb/interfaces/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/interfaces/__init__.py
--rw-r--r--   0 root         (0) root         (0)      191 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/interfaces/language.py
--rw-r--r--   0 root         (0) root         (0)     5115 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/interfaces/model.py
--rw-r--r--   0 root         (0) root         (0)     4616 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/interfaces/mteb_task.py
--rw-r--r--   0 root         (0) root         (0)     1906 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/interfaces/task.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 10:06:38.512314 seb-0.9.3/src/seb/registered_models/
--rw-r--r--   0 root         (0) root         (0)      223 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/registered_models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2721 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/registered_models/cohere_models.py
--rw-r--r--   0 root         (0) root         (0)     3935 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/registered_models/e5_mistral.py
--rw-r--r--   0 root         (0) root         (0)     5140 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/registered_models/e5_models.py
--rw-r--r--   0 root         (0) root         (0)     5343 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/registered_models/fairseq_models.py
--rw-r--r--   0 root         (0) root         (0)     3181 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/registered_models/fasttext.py
--rw-r--r--   0 root         (0) root         (0)    13457 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/registered_models/hf_models.py
--rw-r--r--   0 root         (0) root         (0)     4338 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/registered_models/openai_models.py
--rw-r--r--   0 root         (0) root         (0)     3129 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/registered_models/translate_e5_models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 10:06:38.516315 seb-0.9.3/src/seb/registered_tasks/
--rw-r--r--   0 root         (0) root         (0)       98 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/registered_tasks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1931 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/registered_tasks/danish.py
--rw-r--r--   0 root         (0) root         (0)     2907 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/registered_tasks/mteb_retrieval.py
--rw-r--r--   0 root         (0) root         (0)    11126 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/registered_tasks/mteb_tasks.py
--rw-r--r--   0 root         (0) root         (0)     6651 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/registered_tasks/mteb_tasks_clustering.py
--rw-r--r--   0 root         (0) root         (0)     4552 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/registered_tasks/multilingual.py
--rw-r--r--   0 root         (0) root         (0)     1233 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/registered_tasks/norwegian.py
--rw-r--r--   0 root         (0) root         (0)     3771 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/registered_tasks/speed.py
--rw-r--r--   0 root         (0) root         (0)     1884 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/registered_tasks/swedish.py
--rw-r--r--   0 root         (0) root         (0)    18988 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/registered_tasks/the_ugly_duckling.txt
--rw-r--r--   0 root         (0) root         (0)     1025 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/registries.py
--rw-r--r--   0 root         (0) root         (0)     5425 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/result_dataclasses.py
--rw-r--r--   0 root         (0) root         (0)     1338 2024-01-28 10:06:30.000000 seb-0.9.3/src/seb/warning_ignore_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 10:06:38.516315 seb-0.9.3/src/seb.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6241 2024-01-28 10:06:38.000000 seb-0.9.3/src/seb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    32552 2024-01-28 10:06:38.000000 seb-0.9.3/src/seb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-28 10:06:38.000000 seb-0.9.3/src/seb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2024-01-28 10:06:38.000000 seb-0.9.3/src/seb.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      445 2024-01-28 10:06:38.000000 seb-0.9.3/src/seb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-01-28 10:06:38.000000 seb-0.9.3/src/seb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       99 2024-01-28 10:06:30.000000 seb-0.9.3/test.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 10:06:38.516315 seb-0.9.3/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-28 10:06:30.000000 seb-0.9.3/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 10:06:38.516315 seb-0.9.3/tests/cli/
--rw-r--r--   0 root         (0) root         (0)     1745 2024-01-28 10:06:30.000000 seb-0.9.3/tests/cli/benchmark_cli_code_inject.py
--rw-r--r--   0 root         (0) root         (0)     2852 2024-01-28 10:06:30.000000 seb-0.9.3/tests/cli/test_cli.py
--rw-r--r--   0 root         (0) root         (0)      695 2024-01-28 10:06:30.000000 seb-0.9.3/tests/dummy_model.py
--rw-r--r--   0 root         (0) root         (0)     1789 2024-01-28 10:06:30.000000 seb-0.9.3/tests/dummy_task.py
--rw-r--r--   0 root         (0) root         (0)     1475 2024-01-28 10:06:30.000000 seb-0.9.3/tests/test_all_models.py
--rw-r--r--   0 root         (0) root         (0)     4985 2024-01-28 10:06:30.000000 seb-0.9.3/tests/test_benchmark.py
--rw-r--r--   0 root         (0) root         (0)     1780 2024-01-28 10:06:30.000000 seb-0.9.3/tests/test_integration.py
--rw-r--r--   0 root         (0) root         (0)      379 2024-01-28 10:06:30.000000 seb-0.9.3/tests/test_seb_models.py
--rw-r--r--   0 root         (0) root         (0)      872 2024-01-28 10:06:30.000000 seb-0.9.3/tests/test_speed_task.py
--rw-r--r--   0 root         (0) root         (0)     2562 2024-01-28 10:06:30.000000 seb-0.9.3/tests/test_task_dependent_encode.py
--rw-r--r--   0 root         (0) root         (0)     2426 2024-01-28 10:06:30.000000 seb-0.9.3/tests/test_tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 21:19:02.588946 seb-0.9.4/
+-rw-r--r--   0 root         (0) root         (0)      456 2024-01-28 21:18:55.000000 seb-0.9.4/.cookiecutter.json
+-rw-r--r--   0 root         (0) root         (0)      703 2024-01-28 21:18:55.000000 seb-0.9.4/.cruft.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 21:19:02.468945 seb-0.9.4/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 21:19:02.476945 seb-0.9.4/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)      558 2024-01-28 21:18:55.000000 seb-0.9.4/.github/workflows/check_benchmark_is_up_to_date.yml
+-rw-r--r--   0 root         (0) root         (0)      992 2024-01-28 21:18:55.000000 seb-0.9.4/.github/workflows/documentation.yml
+-rw-r--r--   0 root         (0) root         (0)      456 2024-01-28 21:18:55.000000 seb-0.9.4/.github/workflows/lint.yml
+-rw-r--r--   0 root         (0) root         (0)     2053 2024-01-28 21:18:55.000000 seb-0.9.4/.github/workflows/release.yml
+-rw-r--r--   0 root         (0) root         (0)     1165 2024-01-28 21:18:55.000000 seb-0.9.4/.github/workflows/stalebot.yml
+-rw-r--r--   0 root         (0) root         (0)      668 2024-01-28 21:18:55.000000 seb-0.9.4/.github/workflows/static_type_checks.yml
+-rw-r--r--   0 root         (0) root         (0)     1033 2024-01-28 21:18:55.000000 seb-0.9.4/.github/workflows/tests.yml
+-rw-r--r--   0 root         (0) root         (0)      499 2024-01-28 21:18:55.000000 seb-0.9.4/.gitignore
+-rw-r--r--   0 root         (0) root         (0)    80523 2024-01-28 21:18:55.000000 seb-0.9.4/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     5532 2024-01-28 21:18:55.000000 seb-0.9.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 root         (0) root         (0)     2347 2024-01-28 21:18:55.000000 seb-0.9.4/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)     1074 2024-01-28 21:18:55.000000 seb-0.9.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6241 2024-01-28 21:19:02.588946 seb-0.9.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2996 2024-01-28 21:18:55.000000 seb-0.9.4/README.md
+-rw-r--r--   0 root         (0) root         (0)      720 2024-01-28 21:18:55.000000 seb-0.9.4/citation.cff
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 21:19:02.480945 seb-0.9.4/docs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 21:19:02.480945 seb-0.9.4/docs/_static/
+-rw-r--r--   0 root         (0) root         (0)   417053 2024-01-28 21:18:55.000000 seb-0.9.4/docs/_static/logo.png
+-rw-r--r--   0 root         (0) root         (0)  1221950 2024-01-28 21:18:55.000000 seb-0.9.4/docs/_static/social.png
+-rw-r--r--   0 root         (0) root         (0)      647 2024-01-28 21:18:55.000000 seb-0.9.4/docs/api.md
+-rw-r--r--   0 root         (0) root         (0)     3328 2024-01-28 21:18:55.000000 seb-0.9.4/docs/cli.md
+-rw-r--r--   0 root         (0) root         (0)      544 2024-01-28 21:18:55.000000 seb-0.9.4/docs/create_cli_docs.py
+-rw-r--r--   0 root         (0) root         (0)     2071 2024-01-28 21:18:55.000000 seb-0.9.4/docs/create_desc_stats.py
+-rw-r--r--   0 root         (0) root         (0)    15541 2024-01-28 21:18:55.000000 seb-0.9.4/docs/datasets.md
+-rw-r--r--   0 root         (0) root         (0)    25049 2024-01-28 21:18:55.000000 seb-0.9.4/docs/getting_started.ipynb
+-rw-r--r--   0 root         (0) root         (0)     4207 2024-01-28 21:18:55.000000 seb-0.9.4/docs/index.md
+-rw-r--r--   0 root         (0) root         (0)      401 2024-01-28 21:18:55.000000 seb-0.9.4/docs/installation.md
+-rw-r--r--   0 root         (0) root         (0)      801 2024-01-28 21:18:55.000000 seb-0.9.4/docs/paper.md
+-rw-r--r--   0 root         (0) root         (0)     4251 2024-01-28 21:18:55.000000 seb-0.9.4/docs/run_benchmark.py
+-rw-r--r--   0 root         (0) root         (0)     1704 2024-01-28 21:18:55.000000 seb-0.9.4/makefile
+-rw-r--r--   0 root         (0) root         (0)     1769 2024-01-28 21:18:55.000000 seb-0.9.4/mkdocs.yml
+-rw-r--r--   0 root         (0) root         (0)     3365 2024-01-28 21:18:56.000000 seb-0.9.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-01-28 21:19:02.588946 seb-0.9.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 21:19:02.468945 seb-0.9.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 21:19:02.484946 seb-0.9.4/src/scripts/
+-rw-r--r--   0 root         (0) root         (0)      155 2024-01-28 21:18:55.000000 seb-0.9.4/src/scripts/check_benchmark_is_up_to_date.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 21:19:02.484946 seb-0.9.4/src/seb/
+-rw-r--r--   0 root         (0) root         (0)      480 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       78 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     7044 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/benchmark.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 21:19:02.472946 seb-0.9.4/src/seb/cache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 21:19:02.488946 seb-0.9.4/src/seb/cache/KBLab__sentence-bert-swedish-cased/
+-rw-r--r--   0 root         (0) root         (0)      401 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KBLab__sentence-bert-swedish-cased/Angry_Tweets.json
+-rw-r--r--   0 root         (0) root         (0)      620 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KBLab__sentence-bert-swedish-cased/Bornholm_Parallel.json
+-rw-r--r--   0 root         (0) root         (0)      440 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KBLab__sentence-bert-swedish-cased/DKHate.json
+-rw-r--r--   0 root         (0) root         (0)      452 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KBLab__sentence-bert-swedish-cased/DaLAJ.json
+-rw-r--r--   0 root         (0) root         (0)      389 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KBLab__sentence-bert-swedish-cased/Da_Political_Comments.json
+-rw-r--r--   0 root         (0) root         (0)      366 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KBLab__sentence-bert-swedish-cased/LCC.json
+-rw-r--r--   0 root         (0) root         (0)     1202 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KBLab__sentence-bert-swedish-cased/Language_Identification.json
+-rw-r--r--   0 root         (0) root         (0)      771 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KBLab__sentence-bert-swedish-cased/Massive_Intent.json
+-rw-r--r--   0 root         (0) root         (0)      768 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KBLab__sentence-bert-swedish-cased/Massive_Scenario.json
+-rw-r--r--   0 root         (0) root         (0)      360 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KBLab__sentence-bert-swedish-cased/NoReC.json
+-rw-r--r--   0 root         (0) root         (0)      438 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KBLab__sentence-bert-swedish-cased/Norwegian_parliament.json
+-rw-r--r--   0 root         (0) root         (0)     1085 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KBLab__sentence-bert-swedish-cased/ScaLA.json
+-rw-r--r--   0 root         (0) root         (0)      844 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KBLab__sentence-bert-swedish-cased/SweFAQ.json
+-rw-r--r--   0 root         (0) root         (0)      351 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KBLab__sentence-bert-swedish-cased/SweReC.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 21:19:02.492946 seb-0.9.4/src/seb/cache/KB__bert-base-swedish-cased/
+-rw-r--r--   0 root         (0) root         (0)      401 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KB__bert-base-swedish-cased/Angry_Tweets.json
+-rw-r--r--   0 root         (0) root         (0)      622 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KB__bert-base-swedish-cased/Bornholm_Parallel.json
+-rw-r--r--   0 root         (0) root         (0)      441 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KB__bert-base-swedish-cased/DKHate.json
+-rw-r--r--   0 root         (0) root         (0)      450 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KB__bert-base-swedish-cased/DaLAJ.json
+-rw-r--r--   0 root         (0) root         (0)      389 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KB__bert-base-swedish-cased/Da_Political_Comments.json
+-rw-r--r--   0 root         (0) root         (0)      367 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KB__bert-base-swedish-cased/LCC.json
+-rw-r--r--   0 root         (0) root         (0)     1046 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KB__bert-base-swedish-cased/Language_Identification.json
+-rw-r--r--   0 root         (0) root         (0)      766 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KB__bert-base-swedish-cased/Massive_Intent.json
+-rw-r--r--   0 root         (0) root         (0)      765 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KB__bert-base-swedish-cased/Massive_Scenario.json
+-rw-r--r--   0 root         (0) root         (0)      354 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KB__bert-base-swedish-cased/NoReC.json
+-rw-r--r--   0 root         (0) root         (0)      436 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KB__bert-base-swedish-cased/Norwegian_parliament.json
+-rw-r--r--   0 root         (0) root         (0)     1601 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KB__bert-base-swedish-cased/ScaLA.json
+-rw-r--r--   0 root         (0) root         (0)      844 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KB__bert-base-swedish-cased/SweFAQ.json
+-rw-r--r--   0 root         (0) root         (0)      353 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KB__bert-base-swedish-cased/SweReC.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 21:19:02.492946 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-1/
+-rw-r--r--   0 root         (0) root         (0)      399 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-1/Angry_Tweets.json
+-rw-r--r--   0 root         (0) root         (0)      620 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-1/Bornholm_Parallel.json
+-rw-r--r--   0 root         (0) root         (0)      440 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-1/DKHate.json
+-rw-r--r--   0 root         (0) root         (0)      450 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-1/DaLAJ.json
+-rw-r--r--   0 root         (0) root         (0)      389 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-1/Da_Political_Comments.json
+-rw-r--r--   0 root         (0) root         (0)      365 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-1/LCC.json
+-rw-r--r--   0 root         (0) root         (0)     1202 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-1/Language_Identification.json
+-rw-r--r--   0 root         (0) root         (0)      765 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-1/Massive_Intent.json
+-rw-r--r--   0 root         (0) root         (0)      764 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-1/Massive_Scenario.json
+-rw-r--r--   0 root         (0) root         (0)      362 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-1/NoReC.json
+-rw-r--r--   0 root         (0) root         (0)      437 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-1/Norwegian_parliament.json
+-rw-r--r--   0 root         (0) root         (0)     1081 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-1/ScaLA.json
+-rw-r--r--   0 root         (0) root         (0)      837 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-1/SweFAQ.json
+-rw-r--r--   0 root         (0) root         (0)      362 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-1/SweReC.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 21:19:02.496946 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp1/
+-rw-r--r--   0 root         (0) root         (0)      401 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp1/Angry_Tweets.json
+-rw-r--r--   0 root         (0) root         (0)      544 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp1/Bornholm_Parallel.json
+-rw-r--r--   0 root         (0) root         (0)      438 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp1/DKHate.json
+-rw-r--r--   0 root         (0) root         (0)      453 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp1/DaLAJ.json
+-rw-r--r--   0 root         (0) root         (0)      389 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp1/Da_Political_Comments.json
+-rw-r--r--   0 root         (0) root         (0)      366 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp1/LCC.json
+-rw-r--r--   0 root         (0) root         (0)     1196 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp1/Language_Identification.json
+-rw-r--r--   0 root         (0) root         (0)      762 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp1/Massive_Intent.json
+-rw-r--r--   0 root         (0) root         (0)      764 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp1/Massive_Scenario.json
+-rw-r--r--   0 root         (0) root         (0)      364 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp1/NoReC.json
+-rw-r--r--   0 root         (0) root         (0)      437 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp1/Norwegian_parliament.json
+-rw-r--r--   0 root         (0) root         (0)     1088 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp1/ScaLA.json
+-rw-r--r--   0 root         (0) root         (0)      838 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp1/SweFAQ.json
+-rw-r--r--   0 root         (0) root         (0)      356 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp1/SweReC.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 21:19:02.500946 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp2-no-lang-align/
+-rw-r--r--   0 root         (0) root         (0)      400 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp2-no-lang-align/Angry_Tweets.json
+-rw-r--r--   0 root         (0) root         (0)      544 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp2-no-lang-align/Bornholm_Parallel.json
+-rw-r--r--   0 root         (0) root         (0)      439 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp2-no-lang-align/DKHate.json
+-rw-r--r--   0 root         (0) root         (0)      451 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp2-no-lang-align/DaLAJ.json
+-rw-r--r--   0 root         (0) root         (0)      387 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp2-no-lang-align/Da_Political_Comments.json
+-rw-r--r--   0 root         (0) root         (0)      366 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp2-no-lang-align/LCC.json
+-rw-r--r--   0 root         (0) root         (0)     1202 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp2-no-lang-align/Language_Identification.json
+-rw-r--r--   0 root         (0) root         (0)      765 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp2-no-lang-align/Massive_Intent.json
+-rw-r--r--   0 root         (0) root         (0)      766 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp2-no-lang-align/Massive_Scenario.json
+-rw-r--r--   0 root         (0) root         (0)      364 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp2-no-lang-align/NoReC.json
+-rw-r--r--   0 root         (0) root         (0)      412 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp2-no-lang-align/Norwegian_parliament.json
+-rw-r--r--   0 root         (0) root         (0)     1086 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp2-no-lang-align/ScaLA.json
+-rw-r--r--   0 root         (0) root         (0)      844 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp2-no-lang-align/SweFAQ.json
+-rw-r--r--   0 root         (0) root         (0)      361 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp2-no-lang-align/SweReC.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 21:19:02.500946 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-medium-v1/
+-rw-r--r--   0 root         (0) root         (0)      400 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-medium-v1/Angry_Tweets.json
+-rw-r--r--   0 root         (0) root         (0)      617 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-medium-v1/Bornholm_Parallel.json
+-rw-r--r--   0 root         (0) root         (0)      441 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-medium-v1/DKHate.json
+-rw-r--r--   0 root         (0) root         (0)      453 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-medium-v1/DaLAJ.json
+-rw-r--r--   0 root         (0) root         (0)      388 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-medium-v1/Da_Political_Comments.json
+-rw-r--r--   0 root         (0) root         (0)      365 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-medium-v1/LCC.json
+-rw-r--r--   0 root         (0) root         (0)     1190 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-medium-v1/Language_Identification.json
+-rw-r--r--   0 root         (0) root         (0)      762 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-medium-v1/Massive_Intent.json
+-rw-r--r--   0 root         (0) root         (0)      766 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-medium-v1/Massive_Scenario.json
+-rw-r--r--   0 root         (0) root         (0)      357 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-medium-v1/NoReC.json
+-rw-r--r--   0 root         (0) root         (0)      438 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-medium-v1/Norwegian_parliament.json
+-rw-r--r--   0 root         (0) root         (0)     1081 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-medium-v1/ScaLA.json
+-rw-r--r--   0 root         (0) root         (0)      840 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-medium-v1/SweFAQ.json
+-rw-r--r--   0 root         (0) root         (0)      362 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-medium-v1/SweReC.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 21:19:02.504946 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-small-v1/
+-rw-r--r--   0 root         (0) root         (0)      400 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-small-v1/Angry_Tweets.json
+-rw-r--r--   0 root         (0) root         (0)      620 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-small-v1/Bornholm_Parallel.json
+-rw-r--r--   0 root         (0) root         (0)      409 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-small-v1/DKHate.json
+-rw-r--r--   0 root         (0) root         (0)      451 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-small-v1/DaLAJ.json
+-rw-r--r--   0 root         (0) root         (0)      388 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-small-v1/Da_Political_Comments.json
+-rw-r--r--   0 root         (0) root         (0)      366 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-small-v1/LCC.json
+-rw-r--r--   0 root         (0) root         (0)     1034 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-small-v1/Language_Identification.json
+-rw-r--r--   0 root         (0) root         (0)      766 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-small-v1/Massive_Intent.json
+-rw-r--r--   0 root         (0) root         (0)      768 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-small-v1/Massive_Scenario.json
+-rw-r--r--   0 root         (0) root         (0)      360 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-small-v1/NoReC.json
+-rw-r--r--   0 root         (0) root         (0)      411 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-small-v1/Norwegian_parliament.json
+-rw-r--r--   0 root         (0) root         (0)     1077 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-small-v1/ScaLA.json
+-rw-r--r--   0 root         (0) root         (0)      845 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-small-v1/SweFAQ.json
+-rw-r--r--   0 root         (0) root         (0)      358 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-small-v1/SweReC.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 21:19:02.508946 seb-0.9.4/src/seb/cache/NbAiLab__nb-bert-base/
+-rw-r--r--   0 root         (0) root         (0)      400 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/NbAiLab__nb-bert-base/Angry_Tweets.json
+-rw-r--r--   0 root         (0) root         (0)      624 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/NbAiLab__nb-bert-base/Bornholm_Parallel.json
+-rw-r--r--   0 root         (0) root         (0)      437 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/NbAiLab__nb-bert-base/DKHate.json
+-rw-r--r--   0 root         (0) root         (0)      450 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/NbAiLab__nb-bert-base/DaLAJ.json
+-rw-r--r--   0 root         (0) root         (0)      387 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/NbAiLab__nb-bert-base/Da_Political_Comments.json
+-rw-r--r--   0 root         (0) root         (0)      338 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/NbAiLab__nb-bert-base/LCC.json
+-rw-r--r--   0 root         (0) root         (0)     1190 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/NbAiLab__nb-bert-base/Language_Identification.json
+-rw-r--r--   0 root         (0) root         (0)      765 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/NbAiLab__nb-bert-base/Massive_Intent.json
+-rw-r--r--   0 root         (0) root         (0)      766 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/NbAiLab__nb-bert-base/Massive_Scenario.json
+-rw-r--r--   0 root         (0) root         (0)      363 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/NbAiLab__nb-bert-base/NoReC.json
+-rw-r--r--   0 root         (0) root         (0)      435 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/NbAiLab__nb-bert-base/Norwegian_parliament.json
+-rw-r--r--   0 root         (0) root         (0)     1088 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/NbAiLab__nb-bert-base/ScaLA.json
+-rw-r--r--   0 root         (0) root         (0)      845 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/NbAiLab__nb-bert-base/SweFAQ.json
+-rw-r--r--   0 root         (0) root         (0)      362 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/NbAiLab__nb-bert-base/SweReC.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 21:19:02.508946 seb-0.9.4/src/seb/cache/NbAiLab__nb-bert-large/
+-rw-r--r--   0 root         (0) root         (0)      401 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/NbAiLab__nb-bert-large/Angry_Tweets.json
+-rw-r--r--   0 root         (0) root         (0)      625 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/NbAiLab__nb-bert-large/Bornholm_Parallel.json
+-rw-r--r--   0 root         (0) root         (0)      439 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/NbAiLab__nb-bert-large/DKHate.json
+-rw-r--r--   0 root         (0) root         (0)      447 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/NbAiLab__nb-bert-large/DaLAJ.json
+-rw-r--r--   0 root         (0) root         (0)      388 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/NbAiLab__nb-bert-large/Da_Political_Comments.json
+-rw-r--r--   0 root         (0) root         (0)      365 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/NbAiLab__nb-bert-large/LCC.json
+-rw-r--r--   0 root         (0) root         (0)     1201 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/NbAiLab__nb-bert-large/Language_Identification.json
+-rw-r--r--   0 root         (0) root         (0)      765 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/NbAiLab__nb-bert-large/Massive_Intent.json
+-rw-r--r--   0 root         (0) root         (0)      768 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/NbAiLab__nb-bert-large/Massive_Scenario.json
+-rw-r--r--   0 root         (0) root         (0)      361 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/NbAiLab__nb-bert-large/NoReC.json
+-rw-r--r--   0 root         (0) root         (0)      437 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/NbAiLab__nb-bert-large/Norwegian_parliament.json
+-rw-r--r--   0 root         (0) root         (0)     1598 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/NbAiLab__nb-bert-large/ScaLA.json
+-rw-r--r--   0 root         (0) root         (0)      842 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/NbAiLab__nb-bert-large/SweFAQ.json
+-rw-r--r--   0 root         (0) root         (0)      363 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/NbAiLab__nb-bert-large/SweReC.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 21:19:02.512946 seb-0.9.4/src/seb/cache/chcaa__dfm-encoder-large-v1/
+-rw-r--r--   0 root         (0) root         (0)      401 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/chcaa__dfm-encoder-large-v1/Angry_Tweets.json
+-rw-r--r--   0 root         (0) root         (0)      622 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/chcaa__dfm-encoder-large-v1/Bornholm_Parallel.json
+-rw-r--r--   0 root         (0) root         (0)      438 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/chcaa__dfm-encoder-large-v1/DKHate.json
+-rw-r--r--   0 root         (0) root         (0)      448 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/chcaa__dfm-encoder-large-v1/DaLAJ.json
+-rw-r--r--   0 root         (0) root         (0)      389 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/chcaa__dfm-encoder-large-v1/Da_Political_Comments.json
+-rw-r--r--   0 root         (0) root         (0)      367 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/chcaa__dfm-encoder-large-v1/LCC.json
+-rw-r--r--   0 root         (0) root         (0)     1196 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/chcaa__dfm-encoder-large-v1/Language_Identification.json
+-rw-r--r--   0 root         (0) root         (0)      766 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/chcaa__dfm-encoder-large-v1/Massive_Intent.json
+-rw-r--r--   0 root         (0) root         (0)      767 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/chcaa__dfm-encoder-large-v1/Massive_Scenario.json
+-rw-r--r--   0 root         (0) root         (0)      359 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/chcaa__dfm-encoder-large-v1/NoReC.json
+-rw-r--r--   0 root         (0) root         (0)      414 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/chcaa__dfm-encoder-large-v1/Norwegian_parliament.json
+-rw-r--r--   0 root         (0) root         (0)     1080 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/chcaa__dfm-encoder-large-v1/ScaLA.json
+-rw-r--r--   0 root         (0) root         (0)      845 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/chcaa__dfm-encoder-large-v1/SweFAQ.json
+-rw-r--r--   0 root         (0) root         (0)      359 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/chcaa__dfm-encoder-large-v1/SweReC.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 21:19:02.516946 seb-0.9.4/src/seb/cache/embed-multilingual-v3.0/
+-rw-r--r--   0 root         (0) root         (0)      396 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/embed-multilingual-v3.0/Angry_Tweets.json
+-rw-r--r--   0 root         (0) root         (0)      620 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/embed-multilingual-v3.0/Bornholm_Parallel.json
+-rw-r--r--   0 root         (0) root         (0)      440 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/embed-multilingual-v3.0/DKHate.json
+-rw-r--r--   0 root         (0) root         (0)      452 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/embed-multilingual-v3.0/DaLAJ.json
+-rw-r--r--   0 root         (0) root         (0)      388 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/embed-multilingual-v3.0/Da_Political_Comments.json
+-rw-r--r--   0 root         (0) root         (0)      340 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/embed-multilingual-v3.0/LCC.json
+-rw-r--r--   0 root         (0) root         (0)     1208 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/embed-multilingual-v3.0/Language_Identification.json
+-rw-r--r--   0 root         (0) root         (0)      765 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/embed-multilingual-v3.0/Massive_Intent.json
+-rw-r--r--   0 root         (0) root         (0)      767 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/embed-multilingual-v3.0/Massive_Scenario.json
+-rw-r--r--   0 root         (0) root         (0)      362 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/embed-multilingual-v3.0/NoReC.json
+-rw-r--r--   0 root         (0) root         (0)      439 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/embed-multilingual-v3.0/Norwegian_parliament.json
+-rw-r--r--   0 root         (0) root         (0)     1083 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/embed-multilingual-v3.0/ScaLA.json
+-rw-r--r--   0 root         (0) root         (0)      838 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/embed-multilingual-v3.0/SweFAQ.json
+-rw-r--r--   0 root         (0) root         (0)      357 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/embed-multilingual-v3.0/SweReC.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 21:19:02.516946 seb-0.9.4/src/seb/cache/fasttext-cc-da-300/
+-rw-r--r--   0 root         (0) root         (0)      399 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/fasttext-cc-da-300/Angry_Tweets.json
+-rw-r--r--   0 root         (0) root         (0)      613 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/fasttext-cc-da-300/Bornholm_Parallel.json
+-rw-r--r--   0 root         (0) root         (0)      435 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/fasttext-cc-da-300/DKHate.json
+-rw-r--r--   0 root         (0) root         (0)      449 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/fasttext-cc-da-300/DaLAJ.json
+-rw-r--r--   0 root         (0) root         (0)      385 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/fasttext-cc-da-300/Da_Political_Comments.json
+-rw-r--r--   0 root         (0) root         (0)      361 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/fasttext-cc-da-300/LCC.json
+-rw-r--r--   0 root         (0) root         (0)     1197 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/fasttext-cc-da-300/Language_Identification.json
+-rw-r--r--   0 root         (0) root         (0)      764 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/fasttext-cc-da-300/Massive_Intent.json
+-rw-r--r--   0 root         (0) root         (0)      769 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/fasttext-cc-da-300/Massive_Scenario.json
+-rw-r--r--   0 root         (0) root         (0)      357 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/fasttext-cc-da-300/NoReC.json
+-rw-r--r--   0 root         (0) root         (0)      501 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/fasttext-cc-da-300/Norwegian_parliament.json
+-rw-r--r--   0 root         (0) root         (0)     1087 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/fasttext-cc-da-300/ScaLA.json
+-rw-r--r--   0 root         (0) root         (0)      844 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/fasttext-cc-da-300/SweFAQ.json
+-rw-r--r--   0 root         (0) root         (0)      356 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/fasttext-cc-da-300/SweReC.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 21:19:02.520946 seb-0.9.4/src/seb/cache/fasttext-cc-nb-300/
+-rw-r--r--   0 root         (0) root         (0)      393 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/fasttext-cc-nb-300/Angry_Tweets.json
+-rw-r--r--   0 root         (0) root         (0)      619 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/fasttext-cc-nb-300/Bornholm_Parallel.json
+-rw-r--r--   0 root         (0) root         (0)      435 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/fasttext-cc-nb-300/DKHate.json
+-rw-r--r--   0 root         (0) root         (0)      442 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/fasttext-cc-nb-300/DaLAJ.json
+-rw-r--r--   0 root         (0) root         (0)      381 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/fasttext-cc-nb-300/Da_Political_Comments.json
+-rw-r--r--   0 root         (0) root         (0)      359 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/fasttext-cc-nb-300/LCC.json
+-rw-r--r--   0 root         (0) root         (0)     1197 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/fasttext-cc-nb-300/Language_Identification.json
+-rw-r--r--   0 root         (0) root         (0)      765 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/fasttext-cc-nb-300/Massive_Intent.json
+-rw-r--r--   0 root         (0) root         (0)      768 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/fasttext-cc-nb-300/Massive_Scenario.json
+-rw-r--r--   0 root         (0) root         (0)      357 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/fasttext-cc-nb-300/NoReC.json
+-rw-r--r--   0 root         (0) root         (0)      479 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/fasttext-cc-nb-300/Norwegian_parliament.json
+-rw-r--r--   0 root         (0) root         (0)     1090 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/fasttext-cc-nb-300/ScaLA.json
+-rw-r--r--   0 root         (0) root         (0)      843 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/fasttext-cc-nb-300/SweFAQ.json
+-rw-r--r--   0 root         (0) root         (0)      356 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/fasttext-cc-nb-300/SweReC.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 21:19:02.524946 seb-0.9.4/src/seb/cache/fasttext-cc-nn-300/
+-rw-r--r--   0 root         (0) root         (0)      395 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/fasttext-cc-nn-300/Angry_Tweets.json
+-rw-r--r--   0 root         (0) root         (0)      619 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/fasttext-cc-nn-300/Bornholm_Parallel.json
+-rw-r--r--   0 root         (0) root         (0)      434 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/fasttext-cc-nn-300/DKHate.json
+-rw-r--r--   0 root         (0) root         (0)      448 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/fasttext-cc-nn-300/DaLAJ.json
+-rw-r--r--   0 root         (0) root         (0)      384 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/fasttext-cc-nn-300/Da_Political_Comments.json
+-rw-r--r--   0 root         (0) root         (0)      336 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/fasttext-cc-nn-300/LCC.json
+-rw-r--r--   0 root         (0) root         (0)     1197 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/fasttext-cc-nn-300/Language_Identification.json
+-rw-r--r--   0 root         (0) root         (0)      766 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/fasttext-cc-nn-300/Massive_Intent.json
+-rw-r--r--   0 root         (0) root         (0)      769 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/fasttext-cc-nn-300/Massive_Scenario.json
+-rw-r--r--   0 root         (0) root         (0)      356 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/fasttext-cc-nn-300/NoReC.json
+-rw-r--r--   0 root         (0) root         (0)      502 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/fasttext-cc-nn-300/Norwegian_parliament.json
+-rw-r--r--   0 root         (0) root         (0)     1074 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/fasttext-cc-nn-300/ScaLA.json
+-rw-r--r--   0 root         (0) root         (0)      838 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/fasttext-cc-nn-300/SweFAQ.json
+-rw-r--r--   0 root         (0) root         (0)      357 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/fasttext-cc-nn-300/SweReC.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 21:19:02.524946 seb-0.9.4/src/seb/cache/fasttext-cc-sv-300/
+-rw-r--r--   0 root         (0) root         (0)      393 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/fasttext-cc-sv-300/Angry_Tweets.json
+-rw-r--r--   0 root         (0) root         (0)      619 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/fasttext-cc-sv-300/Bornholm_Parallel.json
+-rw-r--r--   0 root         (0) root         (0)      434 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/fasttext-cc-sv-300/DKHate.json
+-rw-r--r--   0 root         (0) root         (0)      448 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/fasttext-cc-sv-300/DaLAJ.json
+-rw-r--r--   0 root         (0) root         (0)      382 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/fasttext-cc-sv-300/Da_Political_Comments.json
+-rw-r--r--   0 root         (0) root         (0)      364 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/fasttext-cc-sv-300/LCC.json
+-rw-r--r--   0 root         (0) root         (0)     1185 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/fasttext-cc-sv-300/Language_Identification.json
+-rw-r--r--   0 root         (0) root         (0)      762 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/fasttext-cc-sv-300/Massive_Intent.json
+-rw-r--r--   0 root         (0) root         (0)      761 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/fasttext-cc-sv-300/Massive_Scenario.json
+-rw-r--r--   0 root         (0) root         (0)      357 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/fasttext-cc-sv-300/NoReC.json
+-rw-r--r--   0 root         (0) root         (0)      503 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/fasttext-cc-sv-300/Norwegian_parliament.json
+-rw-r--r--   0 root         (0) root         (0)     1080 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/fasttext-cc-sv-300/ScaLA.json
+-rw-r--r--   0 root         (0) root         (0)      843 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/fasttext-cc-sv-300/SweFAQ.json
+-rw-r--r--   0 root         (0) root         (0)      357 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/fasttext-cc-sv-300/SweReC.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 21:19:02.528946 seb-0.9.4/src/seb/cache/intfloat__e5-base/
+-rw-r--r--   0 root         (0) root         (0)      401 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__e5-base/Angry_Tweets.json
+-rw-r--r--   0 root         (0) root         (0)      621 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__e5-base/Bornholm_Parallel.json
+-rw-r--r--   0 root         (0) root         (0)      439 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__e5-base/DKHate.json
+-rw-r--r--   0 root         (0) root         (0)      450 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__e5-base/DaLAJ.json
+-rw-r--r--   0 root         (0) root         (0)      390 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__e5-base/Da_Political_Comments.json
+-rw-r--r--   0 root         (0) root         (0)      366 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__e5-base/LCC.json
+-rw-r--r--   0 root         (0) root         (0)     1196 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__e5-base/Language_Identification.json
+-rw-r--r--   0 root         (0) root         (0)      767 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__e5-base/Massive_Intent.json
+-rw-r--r--   0 root         (0) root         (0)      763 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__e5-base/Massive_Scenario.json
+-rw-r--r--   0 root         (0) root         (0)      363 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__e5-base/NoReC.json
+-rw-r--r--   0 root         (0) root         (0)      437 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__e5-base/Norwegian_parliament.json
+-rw-r--r--   0 root         (0) root         (0)     1093 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__e5-base/ScaLA.json
+-rw-r--r--   0 root         (0) root         (0)      841 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__e5-base/SweFAQ.json
+-rw-r--r--   0 root         (0) root         (0)      360 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__e5-base/SweReC.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 21:19:02.532946 seb-0.9.4/src/seb/cache/intfloat__e5-large/
+-rw-r--r--   0 root         (0) root         (0)      400 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__e5-large/Angry_Tweets.json
+-rw-r--r--   0 root         (0) root         (0)      614 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__e5-large/Bornholm_Parallel.json
+-rw-r--r--   0 root         (0) root         (0)      440 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__e5-large/DKHate.json
+-rw-r--r--   0 root         (0) root         (0)      451 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__e5-large/DaLAJ.json
+-rw-r--r--   0 root         (0) root         (0)      386 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__e5-large/Da_Political_Comments.json
+-rw-r--r--   0 root         (0) root         (0)      367 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__e5-large/LCC.json
+-rw-r--r--   0 root         (0) root         (0)     1190 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__e5-large/Language_Identification.json
+-rw-r--r--   0 root         (0) root         (0)      768 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__e5-large/Massive_Intent.json
+-rw-r--r--   0 root         (0) root         (0)      763 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__e5-large/Massive_Scenario.json
+-rw-r--r--   0 root         (0) root         (0)      364 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__e5-large/NoReC.json
+-rw-r--r--   0 root         (0) root         (0)      439 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__e5-large/Norwegian_parliament.json
+-rw-r--r--   0 root         (0) root         (0)     1101 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__e5-large/ScaLA.json
+-rw-r--r--   0 root         (0) root         (0)      845 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__e5-large/SweFAQ.json
+-rw-r--r--   0 root         (0) root         (0)      361 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__e5-large/SweReC.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 21:19:02.532946 seb-0.9.4/src/seb/cache/intfloat__e5-mistral-7b-instruct/
+-rw-r--r--   0 root         (0) root         (0)      396 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__e5-mistral-7b-instruct/Angry_Tweets.json
+-rw-r--r--   0 root         (0) root         (0)      619 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__e5-mistral-7b-instruct/Bornholm_Parallel.json
+-rw-r--r--   0 root         (0) root         (0)      434 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__e5-mistral-7b-instruct/DKHate.json
+-rw-r--r--   0 root         (0) root         (0)      448 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__e5-mistral-7b-instruct/DaLAJ.json
+-rw-r--r--   0 root         (0) root         (0)      386 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__e5-mistral-7b-instruct/Da_Political_Comments.json
+-rw-r--r--   0 root         (0) root         (0)      334 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__e5-mistral-7b-instruct/LCC.json
+-rw-r--r--   0 root         (0) root         (0)     1197 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__e5-mistral-7b-instruct/Language_Identification.json
+-rw-r--r--   0 root         (0) root         (0)      758 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__e5-mistral-7b-instruct/Massive_Intent.json
+-rw-r--r--   0 root         (0) root         (0)      761 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__e5-mistral-7b-instruct/Massive_Scenario.json
+-rw-r--r--   0 root         (0) root         (0)      357 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__e5-mistral-7b-instruct/NoReC.json
+-rw-r--r--   0 root         (0) root         (0)      502 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__e5-mistral-7b-instruct/Norwegian_parliament.json
+-rw-r--r--   0 root         (0) root         (0)     1069 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__e5-mistral-7b-instruct/ScaLA.json
+-rw-r--r--   0 root         (0) root         (0)      840 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__e5-mistral-7b-instruct/SweFAQ.json
+-rw-r--r--   0 root         (0) root         (0)      356 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__e5-mistral-7b-instruct/SweReC.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 21:19:02.536946 seb-0.9.4/src/seb/cache/intfloat__e5-small/
+-rw-r--r--   0 root         (0) root         (0)      400 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__e5-small/Angry_Tweets.json
+-rw-r--r--   0 root         (0) root         (0)      616 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__e5-small/Bornholm_Parallel.json
+-rw-r--r--   0 root         (0) root         (0)      439 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__e5-small/DKHate.json
+-rw-r--r--   0 root         (0) root         (0)      453 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__e5-small/DaLAJ.json
+-rw-r--r--   0 root         (0) root         (0)      390 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__e5-small/Da_Political_Comments.json
+-rw-r--r--   0 root         (0) root         (0)      366 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__e5-small/LCC.json
+-rw-r--r--   0 root         (0) root         (0)     1202 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__e5-small/Language_Identification.json
+-rw-r--r--   0 root         (0) root         (0)      769 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__e5-small/Massive_Intent.json
+-rw-r--r--   0 root         (0) root         (0)      770 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__e5-small/Massive_Scenario.json
+-rw-r--r--   0 root         (0) root         (0)      357 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__e5-small/NoReC.json
+-rw-r--r--   0 root         (0) root         (0)      438 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__e5-small/Norwegian_parliament.json
+-rw-r--r--   0 root         (0) root         (0)     1104 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__e5-small/ScaLA.json
+-rw-r--r--   0 root         (0) root         (0)      841 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__e5-small/SweFAQ.json
+-rw-r--r--   0 root         (0) root         (0)      362 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__e5-small/SweReC.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 21:19:02.540946 seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-base/
+-rw-r--r--   0 root         (0) root         (0)      401 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-base/Angry_Tweets.json
+-rw-r--r--   0 root         (0) root         (0)      617 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-base/Bornholm_Parallel.json
+-rw-r--r--   0 root         (0) root         (0)      437 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-base/DKHate.json
+-rw-r--r--   0 root         (0) root         (0)      450 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-base/DaLAJ.json
+-rw-r--r--   0 root         (0) root         (0)      388 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-base/Da_Political_Comments.json
+-rw-r--r--   0 root         (0) root         (0)      366 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-base/LCC.json
+-rw-r--r--   0 root         (0) root         (0)     1190 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-base/Language_Identification.json
+-rw-r--r--   0 root         (0) root         (0)      765 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-base/Massive_Intent.json
+-rw-r--r--   0 root         (0) root         (0)      766 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-base/Massive_Scenario.json
+-rw-r--r--   0 root         (0) root         (0)      363 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-base/NoReC.json
+-rw-r--r--   0 root         (0) root         (0)      438 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-base/Norwegian_parliament.json
+-rw-r--r--   0 root         (0) root         (0)     1096 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-base/ScaLA.json
+-rw-r--r--   0 root         (0) root         (0)      842 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-base/SweFAQ.json
+-rw-r--r--   0 root         (0) root         (0)      360 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-base/SweReC.json
+-rw-r--r--   0 root         (0) root         (0)      864 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-base/SwednRetrieval.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 21:19:02.540946 seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-large/
+-rw-r--r--   0 root         (0) root         (0)      399 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-large/Angry_Tweets.json
+-rw-r--r--   0 root         (0) root         (0)      621 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-large/Bornholm_Parallel.json
+-rw-r--r--   0 root         (0) root         (0)      439 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-large/DKHate.json
+-rw-r--r--   0 root         (0) root         (0)      455 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-large/DaLAJ.json
+-rw-r--r--   0 root         (0) root         (0)      390 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-large/Da_Political_Comments.json
+-rw-r--r--   0 root         (0) root         (0)      365 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-large/LCC.json
+-rw-r--r--   0 root         (0) root         (0)     1196 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-large/Language_Identification.json
+-rw-r--r--   0 root         (0) root         (0)      758 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-large/Massive_Intent.json
+-rw-r--r--   0 root         (0) root         (0)      765 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-large/Massive_Scenario.json
+-rw-r--r--   0 root         (0) root         (0)      363 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-large/NoReC.json
+-rw-r--r--   0 root         (0) root         (0)      439 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-large/Norwegian_parliament.json
+-rw-r--r--   0 root         (0) root         (0)     1081 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-large/ScaLA.json
+-rw-r--r--   0 root         (0) root         (0)      842 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-large/SweFAQ.json
+-rw-r--r--   0 root         (0) root         (0)      359 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-large/SweReC.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 21:19:02.544946 seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-small/
+-rw-r--r--   0 root         (0) root         (0)      397 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-small/Angry_Tweets.json
+-rw-r--r--   0 root         (0) root         (0)      622 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-small/Bornholm_Parallel.json
+-rw-r--r--   0 root         (0) root         (0)      439 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-small/DKHate.json
+-rw-r--r--   0 root         (0) root         (0)      452 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-small/DaLAJ.json
+-rw-r--r--   0 root         (0) root         (0)      386 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-small/Da_Political_Comments.json
+-rw-r--r--   0 root         (0) root         (0)      922 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-small/DanFEVER.json
+-rw-r--r--   0 root         (0) root         (0)      366 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-small/LCC.json
+-rw-r--r--   0 root         (0) root         (0)     1202 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-small/Language_Identification.json
+-rw-r--r--   0 root         (0) root         (0)      764 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-small/Massive_Intent.json
+-rw-r--r--   0 root         (0) root         (0)      767 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-small/Massive_Scenario.json
+-rw-r--r--   0 root         (0) root         (0)      362 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-small/NoReC.json
+-rw-r--r--   0 root         (0) root         (0)      437 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-small/Norwegian_parliament.json
+-rw-r--r--   0 root         (0) root         (0)     1095 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-small/ScaLA.json
+-rw-r--r--   0 root         (0) root         (0)      841 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-small/SweFAQ.json
+-rw-r--r--   0 root         (0) root         (0)      359 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-small/SweReC.json
+-rw-r--r--   0 root         (0) root         (0)      507 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-small/SwednClustering.json
+-rw-r--r--   0 root         (0) root         (0)      869 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-small/SwednRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      444 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-small/SwednSTS.json
+-rw-r--r--   0 root         (0) root         (0)      353 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-small/VGSummarizationClustering.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 21:19:02.548946 seb-0.9.4/src/seb/cache/jonfd__electra-small-nordic/
+-rw-r--r--   0 root         (0) root         (0)      401 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/jonfd__electra-small-nordic/Angry_Tweets.json
+-rw-r--r--   0 root         (0) root         (0)      624 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/jonfd__electra-small-nordic/Bornholm_Parallel.json
+-rw-r--r--   0 root         (0) root         (0)      439 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/jonfd__electra-small-nordic/DKHate.json
+-rw-r--r--   0 root         (0) root         (0)      444 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/jonfd__electra-small-nordic/DaLAJ.json
+-rw-r--r--   0 root         (0) root         (0)      389 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/jonfd__electra-small-nordic/Da_Political_Comments.json
+-rw-r--r--   0 root         (0) root         (0)      365 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/jonfd__electra-small-nordic/LCC.json
+-rw-r--r--   0 root         (0) root         (0)     1196 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/jonfd__electra-small-nordic/Language_Identification.json
+-rw-r--r--   0 root         (0) root         (0)      773 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/jonfd__electra-small-nordic/Massive_Intent.json
+-rw-r--r--   0 root         (0) root         (0)      771 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/jonfd__electra-small-nordic/Massive_Scenario.json
+-rw-r--r--   0 root         (0) root         (0)      362 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/jonfd__electra-small-nordic/NoReC.json
+-rw-r--r--   0 root         (0) root         (0)      414 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/jonfd__electra-small-nordic/Norwegian_parliament.json
+-rw-r--r--   0 root         (0) root         (0)     1596 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/jonfd__electra-small-nordic/ScaLA.json
+-rw-r--r--   0 root         (0) root         (0)      843 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/jonfd__electra-small-nordic/SweFAQ.json
+-rw-r--r--   0 root         (0) root         (0)      363 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/jonfd__electra-small-nordic/SweReC.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 21:19:02.552946 seb-0.9.4/src/seb/cache/kb__electra-small-swedish-cased-discriminator/
+-rw-r--r--   0 root         (0) root         (0)      401 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/kb__electra-small-swedish-cased-discriminator/Angry_Tweets.json
+-rw-r--r--   0 root         (0) root         (0)      630 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/kb__electra-small-swedish-cased-discriminator/Bornholm_Parallel.json
+-rw-r--r--   0 root         (0) root         (0)      439 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/kb__electra-small-swedish-cased-discriminator/DKHate.json
+-rw-r--r--   0 root         (0) root         (0)      446 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/kb__electra-small-swedish-cased-discriminator/DaLAJ.json
+-rw-r--r--   0 root         (0) root         (0)      389 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/kb__electra-small-swedish-cased-discriminator/Da_Political_Comments.json
+-rw-r--r--   0 root         (0) root         (0)      367 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/kb__electra-small-swedish-cased-discriminator/LCC.json
+-rw-r--r--   0 root         (0) root         (0)     1196 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/kb__electra-small-swedish-cased-discriminator/Language_Identification.json
+-rw-r--r--   0 root         (0) root         (0)      775 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/kb__electra-small-swedish-cased-discriminator/Massive_Intent.json
+-rw-r--r--   0 root         (0) root         (0)      776 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/kb__electra-small-swedish-cased-discriminator/Massive_Scenario.json
+-rw-r--r--   0 root         (0) root         (0)      362 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/kb__electra-small-swedish-cased-discriminator/NoReC.json
+-rw-r--r--   0 root         (0) root         (0)      436 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/kb__electra-small-swedish-cased-discriminator/Norwegian_parliament.json
+-rw-r--r--   0 root         (0) root         (0)     1090 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/kb__electra-small-swedish-cased-discriminator/ScaLA.json
+-rw-r--r--   0 root         (0) root         (0)      843 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/kb__electra-small-swedish-cased-discriminator/SweFAQ.json
+-rw-r--r--   0 root         (0) root         (0)      363 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/kb__electra-small-swedish-cased-discriminator/SweReC.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 21:19:02.556946 seb-0.9.4/src/seb/cache/sentence-transformers__all-MiniLM-L6-v2/
+-rw-r--r--   0 root         (0) root         (0)      403 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sentence-transformers__all-MiniLM-L6-v2/Angry_Tweets.json
+-rw-r--r--   0 root         (0) root         (0)      616 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sentence-transformers__all-MiniLM-L6-v2/Bornholm_Parallel.json
+-rw-r--r--   0 root         (0) root         (0)      434 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sentence-transformers__all-MiniLM-L6-v2/DKHate.json
+-rw-r--r--   0 root         (0) root         (0)      450 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sentence-transformers__all-MiniLM-L6-v2/DaLAJ.json
+-rw-r--r--   0 root         (0) root         (0)      391 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sentence-transformers__all-MiniLM-L6-v2/Da_Political_Comments.json
+-rw-r--r--   0 root         (0) root         (0)      925 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sentence-transformers__all-MiniLM-L6-v2/DanFEVER.json
+-rw-r--r--   0 root         (0) root         (0)      365 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sentence-transformers__all-MiniLM-L6-v2/LCC.json
+-rw-r--r--   0 root         (0) root         (0)     1058 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sentence-transformers__all-MiniLM-L6-v2/Language_Identification.json
+-rw-r--r--   0 root         (0) root         (0)      769 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sentence-transformers__all-MiniLM-L6-v2/Massive_Intent.json
+-rw-r--r--   0 root         (0) root         (0)      773 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sentence-transformers__all-MiniLM-L6-v2/Massive_Scenario.json
+-rw-r--r--   0 root         (0) root         (0)      359 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sentence-transformers__all-MiniLM-L6-v2/NoReC.json
+-rw-r--r--   0 root         (0) root         (0)      413 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sentence-transformers__all-MiniLM-L6-v2/Norwegian_parliament.json
+-rw-r--r--   0 root         (0) root         (0)     1095 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sentence-transformers__all-MiniLM-L6-v2/ScaLA.json
+-rw-r--r--   0 root         (0) root         (0)      838 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sentence-transformers__all-MiniLM-L6-v2/SweFAQ.json
+-rw-r--r--   0 root         (0) root         (0)      356 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sentence-transformers__all-MiniLM-L6-v2/SweReC.json
+-rw-r--r--   0 root         (0) root         (0)      508 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sentence-transformers__all-MiniLM-L6-v2/SwednClustering.json
+-rw-r--r--   0 root         (0) root         (0)      872 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sentence-transformers__all-MiniLM-L6-v2/SwednRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      443 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sentence-transformers__all-MiniLM-L6-v2/SwednSTS.json
+-rw-r--r--   0 root         (0) root         (0)      352 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sentence-transformers__all-MiniLM-L6-v2/VGSummarizationClustering.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 21:19:02.556946 seb-0.9.4/src/seb/cache/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/
+-rw-r--r--   0 root         (0) root         (0)      401 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/Angry_Tweets.json
+-rw-r--r--   0 root         (0) root         (0)      624 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/Bornholm_Parallel.json
+-rw-r--r--   0 root         (0) root         (0)      439 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DKHate.json
+-rw-r--r--   0 root         (0) root         (0)      448 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DaLAJ.json
+-rw-r--r--   0 root         (0) root         (0)      386 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/Da_Political_Comments.json
+-rw-r--r--   0 root         (0) root         (0)      364 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LCC.json
+-rw-r--r--   0 root         (0) root         (0)     1208 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/Language_Identification.json
+-rw-r--r--   0 root         (0) root         (0)      762 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/Massive_Intent.json
+-rw-r--r--   0 root         (0) root         (0)      767 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/Massive_Scenario.json
+-rw-r--r--   0 root         (0) root         (0)      364 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NoReC.json
+-rw-r--r--   0 root         (0) root         (0)      439 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/Norwegian_parliament.json
+-rw-r--r--   0 root         (0) root         (0)     1605 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ScaLA.json
+-rw-r--r--   0 root         (0) root         (0)      845 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SweFAQ.json
+-rw-r--r--   0 root         (0) root         (0)      363 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SweReC.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 21:19:02.560946 seb-0.9.4/src/seb/cache/sentence-transformers__paraphrase-multilingual-mpnet-base-v2/
+-rw-r--r--   0 root         (0) root         (0)      400 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sentence-transformers__paraphrase-multilingual-mpnet-base-v2/Angry_Tweets.json
+-rw-r--r--   0 root         (0) root         (0)      624 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sentence-transformers__paraphrase-multilingual-mpnet-base-v2/Bornholm_Parallel.json
+-rw-r--r--   0 root         (0) root         (0)      437 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sentence-transformers__paraphrase-multilingual-mpnet-base-v2/DKHate.json
+-rw-r--r--   0 root         (0) root         (0)      452 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sentence-transformers__paraphrase-multilingual-mpnet-base-v2/DaLAJ.json
+-rw-r--r--   0 root         (0) root         (0)      387 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sentence-transformers__paraphrase-multilingual-mpnet-base-v2/Da_Political_Comments.json
+-rw-r--r--   0 root         (0) root         (0)      340 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sentence-transformers__paraphrase-multilingual-mpnet-base-v2/LCC.json
+-rw-r--r--   0 root         (0) root         (0)     1208 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sentence-transformers__paraphrase-multilingual-mpnet-base-v2/Language_Identification.json
+-rw-r--r--   0 root         (0) root         (0)      766 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sentence-transformers__paraphrase-multilingual-mpnet-base-v2/Massive_Intent.json
+-rw-r--r--   0 root         (0) root         (0)      766 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sentence-transformers__paraphrase-multilingual-mpnet-base-v2/Massive_Scenario.json
+-rw-r--r--   0 root         (0) root         (0)      360 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sentence-transformers__paraphrase-multilingual-mpnet-base-v2/NoReC.json
+-rw-r--r--   0 root         (0) root         (0)      412 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sentence-transformers__paraphrase-multilingual-mpnet-base-v2/Norwegian_parliament.json
+-rw-r--r--   0 root         (0) root         (0)     1100 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sentence-transformers__paraphrase-multilingual-mpnet-base-v2/ScaLA.json
+-rw-r--r--   0 root         (0) root         (0)      845 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sentence-transformers__paraphrase-multilingual-mpnet-base-v2/SweFAQ.json
+-rw-r--r--   0 root         (0) root         (0)      363 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sentence-transformers__paraphrase-multilingual-mpnet-base-v2/SweReC.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 21:19:02.560946 seb-0.9.4/src/seb/cache/sonar-dan/
+-rw-r--r--   0 root         (0) root         (0)      395 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sonar-dan/Angry_Tweets.json
+-rw-r--r--   0 root         (0) root         (0)      617 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sonar-dan/Bornholm_Parallel.json
+-rw-r--r--   0 root         (0) root         (0)      435 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sonar-dan/DKHate.json
+-rw-r--r--   0 root         (0) root         (0)      448 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sonar-dan/DaLAJ.json
+-rw-r--r--   0 root         (0) root         (0)      386 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sonar-dan/Da_Political_Comments.json
+-rw-r--r--   0 root         (0) root         (0)      361 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sonar-dan/LCC.json
+-rw-r--r--   0 root         (0) root         (0)     1215 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sonar-dan/Language_Identification.json
+-rw-r--r--   0 root         (0) root         (0)      759 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sonar-dan/Massive_Intent.json
+-rw-r--r--   0 root         (0) root         (0)      761 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sonar-dan/Massive_Scenario.json
+-rw-r--r--   0 root         (0) root         (0)      360 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sonar-dan/NoReC.json
+-rw-r--r--   0 root         (0) root         (0)      433 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sonar-dan/Norwegian_parliament.json
+-rw-r--r--   0 root         (0) root         (0)     1592 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sonar-dan/ScaLA.json
+-rw-r--r--   0 root         (0) root         (0)      845 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sonar-dan/SweFAQ.json
+-rw-r--r--   0 root         (0) root         (0)      358 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sonar-dan/SweReC.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 21:19:02.564946 seb-0.9.4/src/seb/cache/sonar-nno/
+-rw-r--r--   0 root         (0) root         (0)      395 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sonar-nno/Angry_Tweets.json
+-rw-r--r--   0 root         (0) root         (0)      619 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sonar-nno/Bornholm_Parallel.json
+-rw-r--r--   0 root         (0) root         (0)      432 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sonar-nno/DKHate.json
+-rw-r--r--   0 root         (0) root         (0)      448 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sonar-nno/DaLAJ.json
+-rw-r--r--   0 root         (0) root         (0)      383 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sonar-nno/Da_Political_Comments.json
+-rw-r--r--   0 root         (0) root         (0)      361 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sonar-nno/LCC.json
+-rw-r--r--   0 root         (0) root         (0)     1053 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sonar-nno/Language_Identification.json
+-rw-r--r--   0 root         (0) root         (0)      759 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sonar-nno/Massive_Intent.json
+-rw-r--r--   0 root         (0) root         (0)      756 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sonar-nno/Massive_Scenario.json
+-rw-r--r--   0 root         (0) root         (0)      349 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sonar-nno/NoReC.json
+-rw-r--r--   0 root         (0) root         (0)      431 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sonar-nno/Norwegian_parliament.json
+-rw-r--r--   0 root         (0) root         (0)     1090 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sonar-nno/ScaLA.json
+-rw-r--r--   0 root         (0) root         (0)      837 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sonar-nno/SweFAQ.json
+-rw-r--r--   0 root         (0) root         (0)      356 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sonar-nno/SweReC.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 21:19:02.568946 seb-0.9.4/src/seb/cache/sonar-nob/
+-rw-r--r--   0 root         (0) root         (0)      395 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sonar-nob/Angry_Tweets.json
+-rw-r--r--   0 root         (0) root         (0)      617 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sonar-nob/Bornholm_Parallel.json
+-rw-r--r--   0 root         (0) root         (0)      433 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sonar-nob/DKHate.json
+-rw-r--r--   0 root         (0) root         (0)      448 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sonar-nob/DaLAJ.json
+-rw-r--r--   0 root         (0) root         (0)      382 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sonar-nob/Da_Political_Comments.json
+-rw-r--r--   0 root         (0) root         (0)      361 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sonar-nob/LCC.json
+-rw-r--r--   0 root         (0) root         (0)     1191 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sonar-nob/Language_Identification.json
+-rw-r--r--   0 root         (0) root         (0)      761 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sonar-nob/Massive_Intent.json
+-rw-r--r--   0 root         (0) root         (0)      761 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sonar-nob/Massive_Scenario.json
+-rw-r--r--   0 root         (0) root         (0)      358 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sonar-nob/NoReC.json
+-rw-r--r--   0 root         (0) root         (0)      432 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sonar-nob/Norwegian_parliament.json
+-rw-r--r--   0 root         (0) root         (0)     1598 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sonar-nob/ScaLA.json
+-rw-r--r--   0 root         (0) root         (0)      841 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sonar-nob/SweFAQ.json
+-rw-r--r--   0 root         (0) root         (0)      357 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sonar-nob/SweReC.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 21:19:02.568946 seb-0.9.4/src/seb/cache/sonar-swe/
+-rw-r--r--   0 root         (0) root         (0)      396 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sonar-swe/Angry_Tweets.json
+-rw-r--r--   0 root         (0) root         (0)      615 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sonar-swe/Bornholm_Parallel.json
+-rw-r--r--   0 root         (0) root         (0)      435 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sonar-swe/DKHate.json
+-rw-r--r--   0 root         (0) root         (0)      446 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sonar-swe/DaLAJ.json
+-rw-r--r--   0 root         (0) root         (0)      383 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sonar-swe/Da_Political_Comments.json
+-rw-r--r--   0 root         (0) root         (0)      360 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sonar-swe/LCC.json
+-rw-r--r--   0 root         (0) root         (0)     1197 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sonar-swe/Language_Identification.json
+-rw-r--r--   0 root         (0) root         (0)      759 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sonar-swe/Massive_Intent.json
+-rw-r--r--   0 root         (0) root         (0)      759 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sonar-swe/Massive_Scenario.json
+-rw-r--r--   0 root         (0) root         (0)      358 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sonar-swe/NoReC.json
+-rw-r--r--   0 root         (0) root         (0)      433 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sonar-swe/Norwegian_parliament.json
+-rw-r--r--   0 root         (0) root         (0)     1588 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sonar-swe/ScaLA.json
+-rw-r--r--   0 root         (0) root         (0)      842 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sonar-swe/SweFAQ.json
+-rw-r--r--   0 root         (0) root         (0)      355 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/sonar-swe/SweReC.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 21:19:02.568946 seb-0.9.4/src/seb/cache/text-embedding-3-large/
+-rw-r--r--   0 root         (0) root         (0)      434 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/text-embedding-3-large/DKHate.json
+-rw-r--r--   0 root         (0) root         (0)      842 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/text-embedding-3-large/SweFAQ.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 21:19:02.572946 seb-0.9.4/src/seb/cache/text-embedding-3-small/
+-rw-r--r--   0 root         (0) root         (0)      433 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/text-embedding-3-small/DKHate.json
+-rw-r--r--   0 root         (0) root         (0)      841 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/text-embedding-3-small/SweFAQ.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 21:19:02.572946 seb-0.9.4/src/seb/cache/text-embedding-ada-002/
+-rw-r--r--   0 root         (0) root         (0)      399 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/text-embedding-ada-002/Angry_Tweets.json
+-rw-r--r--   0 root         (0) root         (0)      620 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/text-embedding-ada-002/Bornholm_Parallel.json
+-rw-r--r--   0 root         (0) root         (0)      441 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/text-embedding-ada-002/DKHate.json
+-rw-r--r--   0 root         (0) root         (0)      452 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/text-embedding-ada-002/DaLAJ.json
+-rw-r--r--   0 root         (0) root         (0)      387 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/text-embedding-ada-002/Da_Political_Comments.json
+-rw-r--r--   0 root         (0) root         (0)      366 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/text-embedding-ada-002/LCC.json
+-rw-r--r--   0 root         (0) root         (0)     1196 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/text-embedding-ada-002/Language_Identification.json
+-rw-r--r--   0 root         (0) root         (0)      764 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/text-embedding-ada-002/Massive_Intent.json
+-rw-r--r--   0 root         (0) root         (0)      767 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/text-embedding-ada-002/Massive_Scenario.json
+-rw-r--r--   0 root         (0) root         (0)      363 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/text-embedding-ada-002/NoReC.json
+-rw-r--r--   0 root         (0) root         (0)      438 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/text-embedding-ada-002/Norwegian_parliament.json
+-rw-r--r--   0 root         (0) root         (0)     1092 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/text-embedding-ada-002/ScaLA.json
+-rw-r--r--   0 root         (0) root         (0)      839 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/text-embedding-ada-002/SweFAQ.json
+-rw-r--r--   0 root         (0) root         (0)      358 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/text-embedding-ada-002/SweReC.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 21:19:02.576946 seb-0.9.4/src/seb/cache/vesteinn__DanskBERT/
+-rw-r--r--   0 root         (0) root         (0)      400 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/vesteinn__DanskBERT/Angry_Tweets.json
+-rw-r--r--   0 root         (0) root         (0)      622 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/vesteinn__DanskBERT/Bornholm_Parallel.json
+-rw-r--r--   0 root         (0) root         (0)      440 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/vesteinn__DanskBERT/DKHate.json
+-rw-r--r--   0 root         (0) root         (0)      450 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/vesteinn__DanskBERT/DaLAJ.json
+-rw-r--r--   0 root         (0) root         (0)      388 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/vesteinn__DanskBERT/Da_Political_Comments.json
+-rw-r--r--   0 root         (0) root         (0)      338 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/vesteinn__DanskBERT/LCC.json
+-rw-r--r--   0 root         (0) root         (0)     1202 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/vesteinn__DanskBERT/Language_Identification.json
+-rw-r--r--   0 root         (0) root         (0)      769 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/vesteinn__DanskBERT/Massive_Intent.json
+-rw-r--r--   0 root         (0) root         (0)      769 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/vesteinn__DanskBERT/Massive_Scenario.json
+-rw-r--r--   0 root         (0) root         (0)      364 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/vesteinn__DanskBERT/NoReC.json
+-rw-r--r--   0 root         (0) root         (0)      435 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/vesteinn__DanskBERT/Norwegian_parliament.json
+-rw-r--r--   0 root         (0) root         (0)     1598 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/vesteinn__DanskBERT/ScaLA.json
+-rw-r--r--   0 root         (0) root         (0)      844 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/vesteinn__DanskBERT/SweFAQ.json
+-rw-r--r--   0 root         (0) root         (0)      363 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/vesteinn__DanskBERT/SweReC.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 21:19:02.580947 seb-0.9.4/src/seb/cache/xlm-roberta-base/
+-rw-r--r--   0 root         (0) root         (0)      399 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/xlm-roberta-base/Angry_Tweets.json
+-rw-r--r--   0 root         (0) root         (0)      624 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/xlm-roberta-base/Bornholm_Parallel.json
+-rw-r--r--   0 root         (0) root         (0)      439 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/xlm-roberta-base/DKHate.json
+-rw-r--r--   0 root         (0) root         (0)      450 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/xlm-roberta-base/DaLAJ.json
+-rw-r--r--   0 root         (0) root         (0)      389 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/xlm-roberta-base/Da_Political_Comments.json
+-rw-r--r--   0 root         (0) root         (0)      366 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/xlm-roberta-base/LCC.json
+-rw-r--r--   0 root         (0) root         (0)     1195 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/xlm-roberta-base/Language_Identification.json
+-rw-r--r--   0 root         (0) root         (0)      766 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/xlm-roberta-base/Massive_Intent.json
+-rw-r--r--   0 root         (0) root         (0)      769 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/xlm-roberta-base/Massive_Scenario.json
+-rw-r--r--   0 root         (0) root         (0)      359 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/xlm-roberta-base/NoReC.json
+-rw-r--r--   0 root         (0) root         (0)      436 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/xlm-roberta-base/Norwegian_parliament.json
+-rw-r--r--   0 root         (0) root         (0)     1087 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/xlm-roberta-base/ScaLA.json
+-rw-r--r--   0 root         (0) root         (0)      836 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/xlm-roberta-base/SweFAQ.json
+-rw-r--r--   0 root         (0) root         (0)      360 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cache/xlm-roberta-base/SweReC.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 21:19:02.580947 seb-0.9.4/src/seb/cli/
+-rw-r--r--   0 root         (0) root         (0)       66 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      118 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cli/cli.py
+-rw-r--r--   0 root         (0) root         (0)     1087 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cli/import_code.py
+-rw-r--r--   0 root         (0) root         (0)     5668 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cli/run.py
+-rw-r--r--   0 root         (0) root         (0)     4492 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/cli/table.py
+-rw-r--r--   0 root         (0) root         (0)     2223 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/full_benchmark.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 21:19:02.580947 seb-0.9.4/src/seb/interfaces/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/interfaces/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      191 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/interfaces/language.py
+-rw-r--r--   0 root         (0) root         (0)     5115 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/interfaces/model.py
+-rw-r--r--   0 root         (0) root         (0)     4616 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/interfaces/mteb_task.py
+-rw-r--r--   0 root         (0) root         (0)     1906 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/interfaces/task.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 21:19:02.580947 seb-0.9.4/src/seb/registered_models/
+-rw-r--r--   0 root         (0) root         (0)      223 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/registered_models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2721 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/registered_models/cohere_models.py
+-rw-r--r--   0 root         (0) root         (0)     3935 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/registered_models/e5_mistral.py
+-rw-r--r--   0 root         (0) root         (0)     5140 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/registered_models/e5_models.py
+-rw-r--r--   0 root         (0) root         (0)     5343 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/registered_models/fairseq_models.py
+-rw-r--r--   0 root         (0) root         (0)     3181 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/registered_models/fasttext.py
+-rw-r--r--   0 root         (0) root         (0)    13457 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/registered_models/hf_models.py
+-rw-r--r--   0 root         (0) root         (0)     4338 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/registered_models/openai_models.py
+-rw-r--r--   0 root         (0) root         (0)     3129 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/registered_models/translate_e5_models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 21:19:02.584946 seb-0.9.4/src/seb/registered_tasks/
+-rw-r--r--   0 root         (0) root         (0)       98 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/registered_tasks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1931 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/registered_tasks/danish.py
+-rw-r--r--   0 root         (0) root         (0)     2907 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/registered_tasks/mteb_retrieval.py
+-rw-r--r--   0 root         (0) root         (0)    11126 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/registered_tasks/mteb_tasks.py
+-rw-r--r--   0 root         (0) root         (0)     6651 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/registered_tasks/mteb_tasks_clustering.py
+-rw-r--r--   0 root         (0) root         (0)     4552 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/registered_tasks/multilingual.py
+-rw-r--r--   0 root         (0) root         (0)     1233 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/registered_tasks/norwegian.py
+-rw-r--r--   0 root         (0) root         (0)     3771 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/registered_tasks/speed.py
+-rw-r--r--   0 root         (0) root         (0)     1884 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/registered_tasks/swedish.py
+-rw-r--r--   0 root         (0) root         (0)    18988 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/registered_tasks/the_ugly_duckling.txt
+-rw-r--r--   0 root         (0) root         (0)     1025 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/registries.py
+-rw-r--r--   0 root         (0) root         (0)     5425 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/result_dataclasses.py
+-rw-r--r--   0 root         (0) root         (0)     1338 2024-01-28 21:18:55.000000 seb-0.9.4/src/seb/warning_ignore_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 21:19:02.588946 seb-0.9.4/src/seb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6241 2024-01-28 21:19:02.000000 seb-0.9.4/src/seb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    32552 2024-01-28 21:19:02.000000 seb-0.9.4/src/seb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-01-28 21:19:02.000000 seb-0.9.4/src/seb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2024-01-28 21:19:02.000000 seb-0.9.4/src/seb.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2024-01-28 21:19:02.000000 seb-0.9.4/src/seb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-01-28 21:19:02.000000 seb-0.9.4/src/seb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       99 2024-01-28 21:18:55.000000 seb-0.9.4/test.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 21:19:02.584946 seb-0.9.4/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-28 21:18:55.000000 seb-0.9.4/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 21:19:02.584946 seb-0.9.4/tests/cli/
+-rw-r--r--   0 root         (0) root         (0)     1745 2024-01-28 21:18:55.000000 seb-0.9.4/tests/cli/benchmark_cli_code_inject.py
+-rw-r--r--   0 root         (0) root         (0)     2852 2024-01-28 21:18:55.000000 seb-0.9.4/tests/cli/test_cli.py
+-rw-r--r--   0 root         (0) root         (0)      695 2024-01-28 21:18:55.000000 seb-0.9.4/tests/dummy_model.py
+-rw-r--r--   0 root         (0) root         (0)     1789 2024-01-28 21:18:55.000000 seb-0.9.4/tests/dummy_task.py
+-rw-r--r--   0 root         (0) root         (0)     1475 2024-01-28 21:18:55.000000 seb-0.9.4/tests/test_all_models.py
+-rw-r--r--   0 root         (0) root         (0)     4985 2024-01-28 21:18:55.000000 seb-0.9.4/tests/test_benchmark.py
+-rw-r--r--   0 root         (0) root         (0)     1780 2024-01-28 21:18:55.000000 seb-0.9.4/tests/test_integration.py
+-rw-r--r--   0 root         (0) root         (0)      379 2024-01-28 21:18:55.000000 seb-0.9.4/tests/test_seb_models.py
+-rw-r--r--   0 root         (0) root         (0)      872 2024-01-28 21:18:55.000000 seb-0.9.4/tests/test_speed_task.py
+-rw-r--r--   0 root         (0) root         (0)     2562 2024-01-28 21:18:55.000000 seb-0.9.4/tests/test_task_dependent_encode.py
+-rw-r--r--   0 root         (0) root         (0)     2426 2024-01-28 21:18:55.000000 seb-0.9.4/tests/test_tasks.py
```

### Comparing `seb-0.9.3/.cruft.json` & `seb-0.9.4/.cruft.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/.github/workflows/check_benchmark_is_up_to_date.yml` & `seb-0.9.4/.github/workflows/check_benchmark_is_up_to_date.yml`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/.github/workflows/documentation.yml` & `seb-0.9.4/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/.github/workflows/release.yml` & `seb-0.9.4/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/.github/workflows/stalebot.yml` & `seb-0.9.4/.github/workflows/stalebot.yml`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/.github/workflows/static_type_checks.yml` & `seb-0.9.4/.github/workflows/static_type_checks.yml`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/.github/workflows/tests.yml` & `seb-0.9.4/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/CHANGELOG.md` & `seb-0.9.4/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # CHANGELOG
 
 
 
+## v0.9.3 (2024-01-28)
+
+### Fix
+
+* fix: Added new OpenAI Models ([`e096ef5`](https://github.com/KennethEnevoldsen/scandinavian-embedding-benchmark/commit/e096ef5efe351087207e49a254e3ffc6dcf30916))
+
+
 ## v0.9.2 (2024-01-26)
 
 ### Ci
 
 * ci: Updated lint workflow to actually fail when not linted ([`d1c177c`](https://github.com/KennethEnevoldsen/scandinavian-embedding-benchmark/commit/d1c177cfe8c4f976ab7d8d8701b0df9fa80496c9))
 
 ### Fix
```

### Comparing `seb-0.9.3/CODE_OF_CONDUCT.md` & `seb-0.9.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/CONTRIBUTING.md` & `seb-0.9.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/LICENSE` & `seb-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/PKG-INFO` & `seb-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seb
-Version: 0.9.3
+Version: 0.9.4
 Summary: Scandinavian Embedding Benchmark
 Author-email: Kenneth Enevoldsen <Kennethcenevoldsen@gmail.com>
 License: MIT License
         
         Copyright © 2023 Kenneth Enevoldsen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: seb Version: 0.9.3 Summary: Scandinavian Embedding
+Metadata-Version: 2.1 Name: seb Version: 0.9.4 Summary: Scandinavian Embedding
 Benchmark Author-email: Kenneth Enevoldsen
 gmail.com> License: MIT License Copyright Â© 2023 Kenneth Enevoldsen Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `seb-0.9.3/README.md` & `seb-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/citation.cff` & `seb-0.9.4/citation.cff`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/docs/_static/logo.png` & `seb-0.9.4/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/docs/_static/social.png` & `seb-0.9.4/docs/_static/social.png`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/docs/api.md` & `seb-0.9.4/docs/api.md`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/docs/cli.md` & `seb-0.9.4/docs/cli.md`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/docs/create_cli_docs.py` & `seb-0.9.4/docs/create_cli_docs.py`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/docs/create_desc_stats.py` & `seb-0.9.4/docs/create_desc_stats.py`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/docs/datasets.md` & `seb-0.9.4/docs/datasets.md`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/docs/getting_started.ipynb` & `seb-0.9.4/docs/getting_started.ipynb`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/docs/index.md` & `seb-0.9.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/docs/paper.md` & `seb-0.9.4/docs/paper.md`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/docs/run_benchmark.py` & `seb-0.9.4/docs/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/makefile` & `seb-0.9.4/makefile`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/mkdocs.yml` & `seb-0.9.4/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/pyproject.toml` & `seb-0.9.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "seb"
-version = "0.9.3"
+version = "0.9.4"
 authors = [
   { name = "Kenneth Enevoldsen", email = "Kennethcenevoldsen@gmail.com" },
 ]
 description = "Scandinavian Embedding Benchmark"
 classifiers = [
   "Operating System :: POSIX :: Linux",
   "Operating System :: MacOS :: MacOS X",
```

### Comparing `seb-0.9.3/src/seb/benchmark.py` & `seb-0.9.4/src/seb/benchmark.py`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/KBLab__sentence-bert-swedish-cased/Bornholm_Parallel.json` & `seb-0.9.4/src/seb/cache/KBLab__sentence-bert-swedish-cased/Bornholm_Parallel.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/KBLab__sentence-bert-swedish-cased/Language_Identification.json` & `seb-0.9.4/src/seb/cache/KBLab__sentence-bert-swedish-cased/Language_Identification.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/KBLab__sentence-bert-swedish-cased/Massive_Intent.json` & `seb-0.9.4/src/seb/cache/KBLab__sentence-bert-swedish-cased/Massive_Intent.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/KBLab__sentence-bert-swedish-cased/Massive_Scenario.json` & `seb-0.9.4/src/seb/cache/KBLab__sentence-bert-swedish-cased/Massive_Scenario.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/KBLab__sentence-bert-swedish-cased/ScaLA.json` & `seb-0.9.4/src/seb/cache/KBLab__sentence-bert-swedish-cased/ScaLA.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/KBLab__sentence-bert-swedish-cased/SweFAQ.json` & `seb-0.9.4/src/seb/cache/KBLab__sentence-bert-swedish-cased/SweFAQ.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/KB__bert-base-swedish-cased/Bornholm_Parallel.json` & `seb-0.9.4/src/seb/cache/KB__bert-base-swedish-cased/Bornholm_Parallel.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/KB__bert-base-swedish-cased/Language_Identification.json` & `seb-0.9.4/src/seb/cache/KB__bert-base-swedish-cased/Language_Identification.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/KB__bert-base-swedish-cased/Massive_Intent.json` & `seb-0.9.4/src/seb/cache/KB__bert-base-swedish-cased/Massive_Intent.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/KB__bert-base-swedish-cased/Massive_Scenario.json` & `seb-0.9.4/src/seb/cache/KB__bert-base-swedish-cased/Massive_Scenario.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/KB__bert-base-swedish-cased/ScaLA.json` & `seb-0.9.4/src/seb/cache/KB__bert-base-swedish-cased/ScaLA.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/KB__bert-base-swedish-cased/SweFAQ.json` & `seb-0.9.4/src/seb/cache/KB__bert-base-swedish-cased/SweFAQ.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-1/Bornholm_Parallel.json` & `seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-1/Bornholm_Parallel.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-1/Language_Identification.json` & `seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-1/Language_Identification.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-1/Massive_Intent.json` & `seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-1/Massive_Intent.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-1/Massive_Scenario.json` & `seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-1/Massive_Scenario.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-1/ScaLA.json` & `seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-1/ScaLA.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-1/SweFAQ.json` & `seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-1/SweFAQ.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp1/Bornholm_Parallel.json` & `seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp1/Bornholm_Parallel.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp1/Language_Identification.json` & `seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp1/Language_Identification.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp1/Massive_Intent.json` & `seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp1/Massive_Intent.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp1/Massive_Scenario.json` & `seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp1/Massive_Scenario.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp1/ScaLA.json` & `seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp1/ScaLA.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp1/SweFAQ.json` & `seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp1/SweFAQ.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp2-no-lang-align/Bornholm_Parallel.json` & `seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp2-no-lang-align/Bornholm_Parallel.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp2-no-lang-align/Language_Identification.json` & `seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp2-no-lang-align/Language_Identification.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp2-no-lang-align/Massive_Intent.json` & `seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp2-no-lang-align/Massive_Intent.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp2-no-lang-align/Massive_Scenario.json` & `seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp2-no-lang-align/Massive_Scenario.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp2-no-lang-align/ScaLA.json` & `seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp2-no-lang-align/ScaLA.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp2-no-lang-align/SweFAQ.json` & `seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-large-exp2-no-lang-align/SweFAQ.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-medium-v1/Bornholm_Parallel.json` & `seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-medium-v1/Bornholm_Parallel.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-medium-v1/Language_Identification.json` & `seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-medium-v1/Language_Identification.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-medium-v1/Massive_Intent.json` & `seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-medium-v1/Massive_Intent.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-medium-v1/Massive_Scenario.json` & `seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-medium-v1/Massive_Scenario.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-medium-v1/ScaLA.json` & `seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-medium-v1/ScaLA.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-medium-v1/SweFAQ.json` & `seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-medium-v1/SweFAQ.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-small-v1/Bornholm_Parallel.json` & `seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-small-v1/Bornholm_Parallel.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-small-v1/Language_Identification.json` & `seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-small-v1/Language_Identification.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-small-v1/Massive_Intent.json` & `seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-small-v1/Massive_Intent.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-small-v1/Massive_Scenario.json` & `seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-small-v1/Massive_Scenario.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-small-v1/ScaLA.json` & `seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-small-v1/ScaLA.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-small-v1/SweFAQ.json` & `seb-0.9.4/src/seb/cache/KennethEnevoldsen__dfm-sentence-encoder-small-v1/SweFAQ.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/NbAiLab__nb-bert-base/Bornholm_Parallel.json` & `seb-0.9.4/src/seb/cache/NbAiLab__nb-bert-base/Bornholm_Parallel.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/NbAiLab__nb-bert-base/Language_Identification.json` & `seb-0.9.4/src/seb/cache/NbAiLab__nb-bert-base/Language_Identification.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/NbAiLab__nb-bert-base/Massive_Intent.json` & `seb-0.9.4/src/seb/cache/NbAiLab__nb-bert-base/Massive_Intent.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/NbAiLab__nb-bert-base/Massive_Scenario.json` & `seb-0.9.4/src/seb/cache/NbAiLab__nb-bert-base/Massive_Scenario.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/NbAiLab__nb-bert-base/ScaLA.json` & `seb-0.9.4/src/seb/cache/NbAiLab__nb-bert-base/ScaLA.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/NbAiLab__nb-bert-base/SweFAQ.json` & `seb-0.9.4/src/seb/cache/NbAiLab__nb-bert-base/SweFAQ.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/NbAiLab__nb-bert-large/Bornholm_Parallel.json` & `seb-0.9.4/src/seb/cache/NbAiLab__nb-bert-large/Bornholm_Parallel.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/NbAiLab__nb-bert-large/Language_Identification.json` & `seb-0.9.4/src/seb/cache/NbAiLab__nb-bert-large/Language_Identification.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/NbAiLab__nb-bert-large/Massive_Intent.json` & `seb-0.9.4/src/seb/cache/NbAiLab__nb-bert-large/Massive_Intent.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/NbAiLab__nb-bert-large/Massive_Scenario.json` & `seb-0.9.4/src/seb/cache/NbAiLab__nb-bert-large/Massive_Scenario.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/NbAiLab__nb-bert-large/ScaLA.json` & `seb-0.9.4/src/seb/cache/NbAiLab__nb-bert-large/ScaLA.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/NbAiLab__nb-bert-large/SweFAQ.json` & `seb-0.9.4/src/seb/cache/NbAiLab__nb-bert-large/SweFAQ.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/chcaa__dfm-encoder-large-v1/Bornholm_Parallel.json` & `seb-0.9.4/src/seb/cache/chcaa__dfm-encoder-large-v1/Bornholm_Parallel.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/chcaa__dfm-encoder-large-v1/Language_Identification.json` & `seb-0.9.4/src/seb/cache/chcaa__dfm-encoder-large-v1/Language_Identification.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/chcaa__dfm-encoder-large-v1/Massive_Intent.json` & `seb-0.9.4/src/seb/cache/chcaa__dfm-encoder-large-v1/Massive_Intent.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/chcaa__dfm-encoder-large-v1/Massive_Scenario.json` & `seb-0.9.4/src/seb/cache/chcaa__dfm-encoder-large-v1/Massive_Scenario.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/chcaa__dfm-encoder-large-v1/ScaLA.json` & `seb-0.9.4/src/seb/cache/chcaa__dfm-encoder-large-v1/ScaLA.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/chcaa__dfm-encoder-large-v1/SweFAQ.json` & `seb-0.9.4/src/seb/cache/chcaa__dfm-encoder-large-v1/SweFAQ.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/embed-multilingual-v3.0/Bornholm_Parallel.json` & `seb-0.9.4/src/seb/cache/embed-multilingual-v3.0/Bornholm_Parallel.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/embed-multilingual-v3.0/Language_Identification.json` & `seb-0.9.4/src/seb/cache/embed-multilingual-v3.0/Language_Identification.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/embed-multilingual-v3.0/Massive_Intent.json` & `seb-0.9.4/src/seb/cache/embed-multilingual-v3.0/Massive_Intent.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/embed-multilingual-v3.0/Massive_Scenario.json` & `seb-0.9.4/src/seb/cache/embed-multilingual-v3.0/Massive_Scenario.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/embed-multilingual-v3.0/ScaLA.json` & `seb-0.9.4/src/seb/cache/embed-multilingual-v3.0/ScaLA.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/embed-multilingual-v3.0/SweFAQ.json` & `seb-0.9.4/src/seb/cache/embed-multilingual-v3.0/SweFAQ.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/fasttext-cc-da-300/Bornholm_Parallel.json` & `seb-0.9.4/src/seb/cache/fasttext-cc-da-300/Bornholm_Parallel.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/fasttext-cc-da-300/Language_Identification.json` & `seb-0.9.4/src/seb/cache/fasttext-cc-da-300/Language_Identification.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/fasttext-cc-da-300/Massive_Intent.json` & `seb-0.9.4/src/seb/cache/fasttext-cc-da-300/Massive_Intent.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/fasttext-cc-da-300/Massive_Scenario.json` & `seb-0.9.4/src/seb/cache/fasttext-cc-da-300/Massive_Scenario.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/fasttext-cc-da-300/ScaLA.json` & `seb-0.9.4/src/seb/cache/fasttext-cc-da-300/ScaLA.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/fasttext-cc-da-300/SweFAQ.json` & `seb-0.9.4/src/seb/cache/fasttext-cc-da-300/SweFAQ.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/fasttext-cc-nb-300/Bornholm_Parallel.json` & `seb-0.9.4/src/seb/cache/fasttext-cc-nb-300/Bornholm_Parallel.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/fasttext-cc-nb-300/Language_Identification.json` & `seb-0.9.4/src/seb/cache/fasttext-cc-nb-300/Language_Identification.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/fasttext-cc-nb-300/Massive_Intent.json` & `seb-0.9.4/src/seb/cache/fasttext-cc-nb-300/Massive_Intent.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/fasttext-cc-nb-300/Massive_Scenario.json` & `seb-0.9.4/src/seb/cache/fasttext-cc-nb-300/Massive_Scenario.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/fasttext-cc-nb-300/ScaLA.json` & `seb-0.9.4/src/seb/cache/fasttext-cc-nb-300/ScaLA.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/fasttext-cc-nb-300/SweFAQ.json` & `seb-0.9.4/src/seb/cache/fasttext-cc-nb-300/SweFAQ.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/fasttext-cc-nn-300/Bornholm_Parallel.json` & `seb-0.9.4/src/seb/cache/fasttext-cc-nn-300/Bornholm_Parallel.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/fasttext-cc-nn-300/Language_Identification.json` & `seb-0.9.4/src/seb/cache/fasttext-cc-nn-300/Language_Identification.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/fasttext-cc-nn-300/Massive_Intent.json` & `seb-0.9.4/src/seb/cache/fasttext-cc-nn-300/Massive_Intent.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/fasttext-cc-nn-300/Massive_Scenario.json` & `seb-0.9.4/src/seb/cache/fasttext-cc-nn-300/Massive_Scenario.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/fasttext-cc-nn-300/ScaLA.json` & `seb-0.9.4/src/seb/cache/fasttext-cc-nn-300/ScaLA.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/fasttext-cc-nn-300/SweFAQ.json` & `seb-0.9.4/src/seb/cache/fasttext-cc-nn-300/SweFAQ.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/fasttext-cc-sv-300/Bornholm_Parallel.json` & `seb-0.9.4/src/seb/cache/fasttext-cc-sv-300/Bornholm_Parallel.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/fasttext-cc-sv-300/Language_Identification.json` & `seb-0.9.4/src/seb/cache/fasttext-cc-sv-300/Language_Identification.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/fasttext-cc-sv-300/Massive_Intent.json` & `seb-0.9.4/src/seb/cache/fasttext-cc-sv-300/Massive_Intent.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/fasttext-cc-sv-300/Massive_Scenario.json` & `seb-0.9.4/src/seb/cache/fasttext-cc-sv-300/Massive_Scenario.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/fasttext-cc-sv-300/ScaLA.json` & `seb-0.9.4/src/seb/cache/fasttext-cc-sv-300/ScaLA.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/fasttext-cc-sv-300/SweFAQ.json` & `seb-0.9.4/src/seb/cache/fasttext-cc-sv-300/SweFAQ.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/intfloat__e5-base/Bornholm_Parallel.json` & `seb-0.9.4/src/seb/cache/intfloat__e5-base/Bornholm_Parallel.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/intfloat__e5-base/Language_Identification.json` & `seb-0.9.4/src/seb/cache/intfloat__e5-base/Language_Identification.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/intfloat__e5-base/Massive_Intent.json` & `seb-0.9.4/src/seb/cache/intfloat__e5-base/Massive_Intent.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/intfloat__e5-base/Massive_Scenario.json` & `seb-0.9.4/src/seb/cache/intfloat__e5-base/Massive_Scenario.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/intfloat__e5-base/ScaLA.json` & `seb-0.9.4/src/seb/cache/intfloat__e5-base/ScaLA.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/intfloat__e5-base/SweFAQ.json` & `seb-0.9.4/src/seb/cache/intfloat__e5-base/SweFAQ.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/intfloat__e5-large/Bornholm_Parallel.json` & `seb-0.9.4/src/seb/cache/intfloat__e5-large/Bornholm_Parallel.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/intfloat__e5-large/Language_Identification.json` & `seb-0.9.4/src/seb/cache/intfloat__e5-large/Language_Identification.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/intfloat__e5-large/Massive_Intent.json` & `seb-0.9.4/src/seb/cache/intfloat__e5-large/Massive_Intent.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/intfloat__e5-large/Massive_Scenario.json` & `seb-0.9.4/src/seb/cache/intfloat__e5-large/Massive_Scenario.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/intfloat__e5-large/ScaLA.json` & `seb-0.9.4/src/seb/cache/intfloat__e5-large/ScaLA.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/intfloat__e5-large/SweFAQ.json` & `seb-0.9.4/src/seb/cache/intfloat__e5-large/SweFAQ.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/intfloat__e5-mistral-7b-instruct/Bornholm_Parallel.json` & `seb-0.9.4/src/seb/cache/intfloat__e5-mistral-7b-instruct/Bornholm_Parallel.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/intfloat__e5-mistral-7b-instruct/Language_Identification.json` & `seb-0.9.4/src/seb/cache/intfloat__e5-mistral-7b-instruct/Language_Identification.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/intfloat__e5-mistral-7b-instruct/Massive_Intent.json` & `seb-0.9.4/src/seb/cache/intfloat__e5-mistral-7b-instruct/Massive_Intent.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/intfloat__e5-mistral-7b-instruct/Massive_Scenario.json` & `seb-0.9.4/src/seb/cache/intfloat__e5-mistral-7b-instruct/Massive_Scenario.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/intfloat__e5-mistral-7b-instruct/ScaLA.json` & `seb-0.9.4/src/seb/cache/intfloat__e5-mistral-7b-instruct/ScaLA.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/intfloat__e5-mistral-7b-instruct/SweFAQ.json` & `seb-0.9.4/src/seb/cache/intfloat__e5-mistral-7b-instruct/SweFAQ.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/intfloat__e5-small/Bornholm_Parallel.json` & `seb-0.9.4/src/seb/cache/intfloat__e5-small/Bornholm_Parallel.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/intfloat__e5-small/Language_Identification.json` & `seb-0.9.4/src/seb/cache/intfloat__e5-small/Language_Identification.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/intfloat__e5-small/Massive_Intent.json` & `seb-0.9.4/src/seb/cache/intfloat__e5-small/Massive_Intent.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/intfloat__e5-small/Massive_Scenario.json` & `seb-0.9.4/src/seb/cache/intfloat__e5-small/Massive_Scenario.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/intfloat__e5-small/ScaLA.json` & `seb-0.9.4/src/seb/cache/intfloat__e5-small/ScaLA.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/intfloat__e5-small/SweFAQ.json` & `seb-0.9.4/src/seb/cache/intfloat__e5-small/SweFAQ.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-base/Bornholm_Parallel.json` & `seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-base/Bornholm_Parallel.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-base/Language_Identification.json` & `seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-base/Language_Identification.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-base/Massive_Intent.json` & `seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-base/Massive_Intent.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-base/Massive_Scenario.json` & `seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-base/Massive_Scenario.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-base/ScaLA.json` & `seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-base/ScaLA.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-base/SweFAQ.json` & `seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-base/SweFAQ.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-base/SwednRetrieval.json` & `seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-base/SwednRetrieval.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-large/Bornholm_Parallel.json` & `seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-large/Bornholm_Parallel.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-large/Language_Identification.json` & `seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-large/Language_Identification.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-large/Massive_Intent.json` & `seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-large/Massive_Intent.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-large/Massive_Scenario.json` & `seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-large/Massive_Scenario.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-large/ScaLA.json` & `seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-large/ScaLA.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-large/SweFAQ.json` & `seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-large/SweFAQ.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-small/Bornholm_Parallel.json` & `seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-small/Bornholm_Parallel.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-small/DanFEVER.json` & `seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-small/DanFEVER.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-small/Language_Identification.json` & `seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-small/Language_Identification.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-small/Massive_Intent.json` & `seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-small/Massive_Intent.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-small/Massive_Scenario.json` & `seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-small/Massive_Scenario.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-small/ScaLA.json` & `seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-small/ScaLA.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-small/SweFAQ.json` & `seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-small/SweFAQ.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/intfloat__multilingual-e5-small/SwednRetrieval.json` & `seb-0.9.4/src/seb/cache/intfloat__multilingual-e5-small/SwednRetrieval.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/jonfd__electra-small-nordic/Bornholm_Parallel.json` & `seb-0.9.4/src/seb/cache/jonfd__electra-small-nordic/Bornholm_Parallel.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/jonfd__electra-small-nordic/Language_Identification.json` & `seb-0.9.4/src/seb/cache/jonfd__electra-small-nordic/Language_Identification.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/jonfd__electra-small-nordic/Massive_Intent.json` & `seb-0.9.4/src/seb/cache/jonfd__electra-small-nordic/Massive_Intent.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/jonfd__electra-small-nordic/Massive_Scenario.json` & `seb-0.9.4/src/seb/cache/jonfd__electra-small-nordic/Massive_Scenario.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/jonfd__electra-small-nordic/ScaLA.json` & `seb-0.9.4/src/seb/cache/jonfd__electra-small-nordic/ScaLA.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/jonfd__electra-small-nordic/SweFAQ.json` & `seb-0.9.4/src/seb/cache/jonfd__electra-small-nordic/SweFAQ.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/kb__electra-small-swedish-cased-discriminator/Bornholm_Parallel.json` & `seb-0.9.4/src/seb/cache/kb__electra-small-swedish-cased-discriminator/Bornholm_Parallel.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/kb__electra-small-swedish-cased-discriminator/Language_Identification.json` & `seb-0.9.4/src/seb/cache/kb__electra-small-swedish-cased-discriminator/Language_Identification.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/kb__electra-small-swedish-cased-discriminator/Massive_Intent.json` & `seb-0.9.4/src/seb/cache/kb__electra-small-swedish-cased-discriminator/Massive_Intent.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/kb__electra-small-swedish-cased-discriminator/Massive_Scenario.json` & `seb-0.9.4/src/seb/cache/kb__electra-small-swedish-cased-discriminator/Massive_Scenario.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/kb__electra-small-swedish-cased-discriminator/ScaLA.json` & `seb-0.9.4/src/seb/cache/kb__electra-small-swedish-cased-discriminator/ScaLA.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/kb__electra-small-swedish-cased-discriminator/SweFAQ.json` & `seb-0.9.4/src/seb/cache/kb__electra-small-swedish-cased-discriminator/SweFAQ.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/sentence-transformers__all-MiniLM-L6-v2/Bornholm_Parallel.json` & `seb-0.9.4/src/seb/cache/sentence-transformers__all-MiniLM-L6-v2/Bornholm_Parallel.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/sentence-transformers__all-MiniLM-L6-v2/DanFEVER.json` & `seb-0.9.4/src/seb/cache/sentence-transformers__all-MiniLM-L6-v2/DanFEVER.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/sentence-transformers__all-MiniLM-L6-v2/Language_Identification.json` & `seb-0.9.4/src/seb/cache/sentence-transformers__all-MiniLM-L6-v2/Language_Identification.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/sentence-transformers__all-MiniLM-L6-v2/Massive_Intent.json` & `seb-0.9.4/src/seb/cache/sentence-transformers__all-MiniLM-L6-v2/Massive_Intent.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/sentence-transformers__all-MiniLM-L6-v2/Massive_Scenario.json` & `seb-0.9.4/src/seb/cache/sentence-transformers__all-MiniLM-L6-v2/Massive_Scenario.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/sentence-transformers__all-MiniLM-L6-v2/ScaLA.json` & `seb-0.9.4/src/seb/cache/sentence-transformers__all-MiniLM-L6-v2/ScaLA.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/sentence-transformers__all-MiniLM-L6-v2/SweFAQ.json` & `seb-0.9.4/src/seb/cache/sentence-transformers__all-MiniLM-L6-v2/SweFAQ.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/sentence-transformers__all-MiniLM-L6-v2/SwednRetrieval.json` & `seb-0.9.4/src/seb/cache/sentence-transformers__all-MiniLM-L6-v2/SwednRetrieval.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/Bornholm_Parallel.json` & `seb-0.9.4/src/seb/cache/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/Bornholm_Parallel.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/Language_Identification.json` & `seb-0.9.4/src/seb/cache/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/Language_Identification.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/Massive_Intent.json` & `seb-0.9.4/src/seb/cache/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/Massive_Intent.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/Massive_Scenario.json` & `seb-0.9.4/src/seb/cache/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/Massive_Scenario.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ScaLA.json` & `seb-0.9.4/src/seb/cache/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ScaLA.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SweFAQ.json` & `seb-0.9.4/src/seb/cache/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SweFAQ.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/sentence-transformers__paraphrase-multilingual-mpnet-base-v2/Bornholm_Parallel.json` & `seb-0.9.4/src/seb/cache/sentence-transformers__paraphrase-multilingual-mpnet-base-v2/Bornholm_Parallel.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/sentence-transformers__paraphrase-multilingual-mpnet-base-v2/Language_Identification.json` & `seb-0.9.4/src/seb/cache/sentence-transformers__paraphrase-multilingual-mpnet-base-v2/Language_Identification.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/sentence-transformers__paraphrase-multilingual-mpnet-base-v2/Massive_Intent.json` & `seb-0.9.4/src/seb/cache/sentence-transformers__paraphrase-multilingual-mpnet-base-v2/Massive_Intent.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/sentence-transformers__paraphrase-multilingual-mpnet-base-v2/Massive_Scenario.json` & `seb-0.9.4/src/seb/cache/sentence-transformers__paraphrase-multilingual-mpnet-base-v2/Massive_Scenario.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/sentence-transformers__paraphrase-multilingual-mpnet-base-v2/ScaLA.json` & `seb-0.9.4/src/seb/cache/sentence-transformers__paraphrase-multilingual-mpnet-base-v2/ScaLA.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/sentence-transformers__paraphrase-multilingual-mpnet-base-v2/SweFAQ.json` & `seb-0.9.4/src/seb/cache/sentence-transformers__paraphrase-multilingual-mpnet-base-v2/SweFAQ.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/sonar-dan/Bornholm_Parallel.json` & `seb-0.9.4/src/seb/cache/sonar-dan/Bornholm_Parallel.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/sonar-dan/Language_Identification.json` & `seb-0.9.4/src/seb/cache/sonar-dan/Language_Identification.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/sonar-dan/Massive_Intent.json` & `seb-0.9.4/src/seb/cache/sonar-dan/Massive_Intent.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/sonar-dan/Massive_Scenario.json` & `seb-0.9.4/src/seb/cache/sonar-dan/Massive_Scenario.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/sonar-dan/ScaLA.json` & `seb-0.9.4/src/seb/cache/sonar-dan/ScaLA.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/sonar-dan/SweFAQ.json` & `seb-0.9.4/src/seb/cache/sonar-dan/SweFAQ.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/sonar-nno/Bornholm_Parallel.json` & `seb-0.9.4/src/seb/cache/sonar-nno/Bornholm_Parallel.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/sonar-nno/Language_Identification.json` & `seb-0.9.4/src/seb/cache/sonar-nno/Language_Identification.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/sonar-nno/Massive_Intent.json` & `seb-0.9.4/src/seb/cache/sonar-nno/Massive_Intent.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/sonar-nno/Massive_Scenario.json` & `seb-0.9.4/src/seb/cache/sonar-nno/Massive_Scenario.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/sonar-nno/ScaLA.json` & `seb-0.9.4/src/seb/cache/sonar-nno/ScaLA.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/sonar-nno/SweFAQ.json` & `seb-0.9.4/src/seb/cache/sonar-nno/SweFAQ.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/sonar-nob/Bornholm_Parallel.json` & `seb-0.9.4/src/seb/cache/sonar-nob/Bornholm_Parallel.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/sonar-nob/Language_Identification.json` & `seb-0.9.4/src/seb/cache/sonar-nob/Language_Identification.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/sonar-nob/Massive_Intent.json` & `seb-0.9.4/src/seb/cache/sonar-nob/Massive_Intent.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/sonar-nob/Massive_Scenario.json` & `seb-0.9.4/src/seb/cache/sonar-nob/Massive_Scenario.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/sonar-nob/ScaLA.json` & `seb-0.9.4/src/seb/cache/sonar-nob/ScaLA.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/sonar-nob/SweFAQ.json` & `seb-0.9.4/src/seb/cache/sonar-nob/SweFAQ.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/sonar-swe/Bornholm_Parallel.json` & `seb-0.9.4/src/seb/cache/sonar-swe/Bornholm_Parallel.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/sonar-swe/Language_Identification.json` & `seb-0.9.4/src/seb/cache/sonar-swe/Language_Identification.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/sonar-swe/Massive_Intent.json` & `seb-0.9.4/src/seb/cache/sonar-swe/Massive_Intent.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/sonar-swe/Massive_Scenario.json` & `seb-0.9.4/src/seb/cache/sonar-swe/Massive_Scenario.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/sonar-swe/ScaLA.json` & `seb-0.9.4/src/seb/cache/sonar-swe/ScaLA.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/sonar-swe/SweFAQ.json` & `seb-0.9.4/src/seb/cache/sonar-swe/SweFAQ.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/text-embedding-3-large/SweFAQ.json` & `seb-0.9.4/src/seb/cache/text-embedding-3-large/SweFAQ.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/text-embedding-3-small/SweFAQ.json` & `seb-0.9.4/src/seb/cache/text-embedding-3-small/SweFAQ.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/text-embedding-ada-002/Bornholm_Parallel.json` & `seb-0.9.4/src/seb/cache/text-embedding-ada-002/Bornholm_Parallel.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/text-embedding-ada-002/Language_Identification.json` & `seb-0.9.4/src/seb/cache/text-embedding-ada-002/Language_Identification.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/text-embedding-ada-002/Massive_Intent.json` & `seb-0.9.4/src/seb/cache/text-embedding-ada-002/Massive_Intent.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/text-embedding-ada-002/Massive_Scenario.json` & `seb-0.9.4/src/seb/cache/text-embedding-ada-002/Massive_Scenario.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/text-embedding-ada-002/ScaLA.json` & `seb-0.9.4/src/seb/cache/text-embedding-ada-002/ScaLA.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/text-embedding-ada-002/SweFAQ.json` & `seb-0.9.4/src/seb/cache/text-embedding-ada-002/SweFAQ.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/vesteinn__DanskBERT/Bornholm_Parallel.json` & `seb-0.9.4/src/seb/cache/vesteinn__DanskBERT/Bornholm_Parallel.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/vesteinn__DanskBERT/Language_Identification.json` & `seb-0.9.4/src/seb/cache/vesteinn__DanskBERT/Language_Identification.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/vesteinn__DanskBERT/Massive_Intent.json` & `seb-0.9.4/src/seb/cache/vesteinn__DanskBERT/Massive_Intent.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/vesteinn__DanskBERT/Massive_Scenario.json` & `seb-0.9.4/src/seb/cache/vesteinn__DanskBERT/Massive_Scenario.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/vesteinn__DanskBERT/ScaLA.json` & `seb-0.9.4/src/seb/cache/vesteinn__DanskBERT/ScaLA.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/vesteinn__DanskBERT/SweFAQ.json` & `seb-0.9.4/src/seb/cache/vesteinn__DanskBERT/SweFAQ.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/xlm-roberta-base/Bornholm_Parallel.json` & `seb-0.9.4/src/seb/cache/xlm-roberta-base/Bornholm_Parallel.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/xlm-roberta-base/Language_Identification.json` & `seb-0.9.4/src/seb/cache/xlm-roberta-base/Language_Identification.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/xlm-roberta-base/Massive_Intent.json` & `seb-0.9.4/src/seb/cache/xlm-roberta-base/Massive_Intent.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/xlm-roberta-base/Massive_Scenario.json` & `seb-0.9.4/src/seb/cache/xlm-roberta-base/Massive_Scenario.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/xlm-roberta-base/ScaLA.json` & `seb-0.9.4/src/seb/cache/xlm-roberta-base/ScaLA.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cache/xlm-roberta-base/SweFAQ.json` & `seb-0.9.4/src/seb/cache/xlm-roberta-base/SweFAQ.json`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cli/import_code.py` & `seb-0.9.4/src/seb/cli/import_code.py`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cli/run.py` & `seb-0.9.4/src/seb/cli/run.py`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/cli/table.py` & `seb-0.9.4/src/seb/cli/table.py`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/full_benchmark.py` & `seb-0.9.4/src/seb/full_benchmark.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     if use_cache:
         logger.warn(
             "Running the speed benchmark with use_cache=True will load speed results from the cache, this might lead to incomparable results."
         )
 
     results = {}
     for subset, langs in BENCHMARKS.items():
-        benchmark = Benchmark(languages=langs)
+        benchmark = Benchmark(languages=langs, tasks=tasks)
         bm_results = benchmark.evaluate_models(
             models=models,
             use_cache=use_cache,
             run_model=run_models,
             raise_errors=raise_errors,
             cache_dir=cache_dir,
         )
```

### Comparing `seb-0.9.3/src/seb/interfaces/model.py` & `seb-0.9.4/src/seb/interfaces/model.py`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/interfaces/mteb_task.py` & `seb-0.9.4/src/seb/interfaces/mteb_task.py`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/interfaces/task.py` & `seb-0.9.4/src/seb/interfaces/task.py`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/registered_models/cohere_models.py` & `seb-0.9.4/src/seb/registered_models/cohere_models.py`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/registered_models/e5_mistral.py` & `seb-0.9.4/src/seb/registered_models/e5_mistral.py`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/registered_models/e5_models.py` & `seb-0.9.4/src/seb/registered_models/e5_models.py`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/registered_models/fairseq_models.py` & `seb-0.9.4/src/seb/registered_models/fairseq_models.py`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/registered_models/fasttext.py` & `seb-0.9.4/src/seb/registered_models/fasttext.py`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/registered_models/hf_models.py` & `seb-0.9.4/src/seb/registered_models/hf_models.py`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/registered_models/openai_models.py` & `seb-0.9.4/src/seb/registered_models/openai_models.py`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/registered_models/translate_e5_models.py` & `seb-0.9.4/src/seb/registered_models/translate_e5_models.py`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/registered_tasks/danish.py` & `seb-0.9.4/src/seb/registered_tasks/danish.py`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/registered_tasks/mteb_retrieval.py` & `seb-0.9.4/src/seb/registered_tasks/mteb_retrieval.py`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/registered_tasks/mteb_tasks.py` & `seb-0.9.4/src/seb/registered_tasks/mteb_tasks.py`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/registered_tasks/mteb_tasks_clustering.py` & `seb-0.9.4/src/seb/registered_tasks/mteb_tasks_clustering.py`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/registered_tasks/multilingual.py` & `seb-0.9.4/src/seb/registered_tasks/multilingual.py`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/registered_tasks/norwegian.py` & `seb-0.9.4/src/seb/registered_tasks/norwegian.py`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/registered_tasks/speed.py` & `seb-0.9.4/src/seb/registered_tasks/speed.py`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/registered_tasks/swedish.py` & `seb-0.9.4/src/seb/registered_tasks/swedish.py`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/registered_tasks/the_ugly_duckling.txt` & `seb-0.9.4/src/seb/registered_tasks/the_ugly_duckling.txt`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/registries.py` & `seb-0.9.4/src/seb/registries.py`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/result_dataclasses.py` & `seb-0.9.4/src/seb/result_dataclasses.py`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb/warning_ignore_manager.py` & `seb-0.9.4/src/seb/warning_ignore_manager.py`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/src/seb.egg-info/PKG-INFO` & `seb-0.9.4/src/seb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seb
-Version: 0.9.3
+Version: 0.9.4
 Summary: Scandinavian Embedding Benchmark
 Author-email: Kenneth Enevoldsen <Kennethcenevoldsen@gmail.com>
 License: MIT License
         
         Copyright © 2023 Kenneth Enevoldsen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: seb Version: 0.9.3 Summary: Scandinavian Embedding
+Metadata-Version: 2.1 Name: seb Version: 0.9.4 Summary: Scandinavian Embedding
 Benchmark Author-email: Kenneth Enevoldsen
 gmail.com> License: MIT License Copyright Â© 2023 Kenneth Enevoldsen Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `seb-0.9.3/src/seb.egg-info/SOURCES.txt` & `seb-0.9.4/src/seb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/tests/cli/benchmark_cli_code_inject.py` & `seb-0.9.4/tests/cli/benchmark_cli_code_inject.py`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/tests/cli/test_cli.py` & `seb-0.9.4/tests/cli/test_cli.py`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/tests/dummy_model.py` & `seb-0.9.4/tests/dummy_model.py`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/tests/dummy_task.py` & `seb-0.9.4/tests/dummy_task.py`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/tests/test_all_models.py` & `seb-0.9.4/tests/test_all_models.py`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/tests/test_benchmark.py` & `seb-0.9.4/tests/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/tests/test_integration.py` & `seb-0.9.4/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/tests/test_speed_task.py` & `seb-0.9.4/tests/test_speed_task.py`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/tests/test_task_dependent_encode.py` & `seb-0.9.4/tests/test_task_dependent_encode.py`

 * *Files identical despite different names*

### Comparing `seb-0.9.3/tests/test_tasks.py` & `seb-0.9.4/tests/test_tasks.py`

 * *Files identical despite different names*

