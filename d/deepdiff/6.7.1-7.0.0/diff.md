# Comparing `tmp/deepdiff-6.7.1.tar.gz` & `tmp/deepdiff-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepdiff-6.7.1.tar", last modified: Tue Nov 14 07:19:40 2023, max compression
+gzip compressed data, was "deepdiff-7.0.0.tar", last modified: Mon Apr  8 08:47:43 2024, max compression
```

## Comparing `deepdiff-6.7.1.tar` & `deepdiff-7.0.0.tar`

### file list

```diff
@@ -1,131 +1,130 @@
-drwxrwxr-x   0 erasmose  (1000) erasmose  (1000)        0 2023-11-14 07:19:40.424622 deepdiff-6.7.1/
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     5344 2023-10-04 22:33:53.000000 deepdiff-6.7.1/AUTHORS.md
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     1131 2021-04-28 22:25:20.000000 deepdiff-6.7.1/LICENSE
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      442 2023-01-06 05:04:29.000000 deepdiff-6.7.1/MANIFEST.in
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     5958 2023-11-14 07:19:40.424622 deepdiff-6.7.1/PKG-INFO
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     4895 2023-11-14 07:16:24.000000 deepdiff-6.7.1/README.md
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     3571 2022-08-28 02:43:58.000000 deepdiff-6.7.1/conftest.py
-drwxrwxr-x   0 erasmose  (1000) erasmose  (1000)        0 2023-11-14 07:19:40.416622 deepdiff-6.7.1/deepdiff/
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      398 2023-11-14 07:16:24.000000 deepdiff-6.7.1/deepdiff/__init__.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     2002 2021-02-01 00:46:22.000000 deepdiff-6.7.1/deepdiff/anyset.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     2057 2021-02-01 00:46:22.000000 deepdiff-6.7.1/deepdiff/base.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    10041 2023-03-17 18:15:49.000000 deepdiff-6.7.1/deepdiff/commands.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    20902 2023-09-01 00:27:49.000000 deepdiff-6.7.1/deepdiff/deephash.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    46277 2023-11-14 07:16:24.000000 deepdiff-6.7.1/deepdiff/delta.py
--rwxrwxr-x   0 erasmose  (1000) erasmose  (1000)    80854 2023-11-14 07:16:24.000000 deepdiff-6.7.1/deepdiff/diff.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    10699 2021-12-17 19:31:57.000000 deepdiff-6.7.1/deepdiff/distance.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    20357 2023-10-17 22:51:06.000000 deepdiff-6.7.1/deepdiff/helper.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     6848 2021-02-01 00:46:22.000000 deepdiff-6.7.1/deepdiff/lfucache.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    39364 2023-11-08 00:27:54.000000 deepdiff-6.7.1/deepdiff/model.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     1264 2023-03-17 18:15:49.000000 deepdiff-6.7.1/deepdiff/operator.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    10360 2023-11-14 07:16:24.000000 deepdiff-6.7.1/deepdiff/path.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    12408 2021-04-29 06:21:17.000000 deepdiff-6.7.1/deepdiff/search.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    21467 2023-11-14 07:16:24.000000 deepdiff-6.7.1/deepdiff/serialization.py
-drwxrwxr-x   0 erasmose  (1000) erasmose  (1000)        0 2023-11-14 07:19:40.420622 deepdiff-6.7.1/deepdiff.egg-info/
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     5958 2023-11-14 07:19:40.000000 deepdiff-6.7.1/deepdiff.egg-info/PKG-INFO
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     3859 2023-11-14 07:19:40.000000 deepdiff-6.7.1/deepdiff.egg-info/SOURCES.txt
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)        1 2023-11-14 07:19:40.000000 deepdiff-6.7.1/deepdiff.egg-info/dependency_links.txt
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       47 2023-11-14 07:19:40.000000 deepdiff-6.7.1/deepdiff.egg-info/entry_points.txt
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       79 2023-11-14 07:19:40.000000 deepdiff-6.7.1/deepdiff.egg-info/requires.txt
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)        9 2023-11-14 07:19:40.000000 deepdiff-6.7.1/deepdiff.egg-info/top_level.txt
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)        1 2023-01-06 05:03:23.000000 deepdiff-6.7.1/deepdiff.egg-info/zip-safe
-drwxrwxr-x   0 erasmose  (1000) erasmose  (1000)        0 2023-11-14 07:19:40.420622 deepdiff-6.7.1/docs/
-drwxrwxr-x   0 erasmose  (1000) erasmose  (1000)        0 2023-11-14 07:19:40.420622 deepdiff-6.7.1/docs/_static/
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    33163 2021-02-01 00:46:22.000000 deepdiff-6.7.1/docs/_static/benchmark_array_no_numpy__3.8__ignore_order=True__cache_size=0__cache_tuning_sample_size=0__cutoff_intersection_for_pairs=1.png
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    33204 2021-02-01 00:46:22.000000 deepdiff-6.7.1/docs/_static/benchmark_array_no_numpy__3.8__ignore_order=True__cache_size=10000__cache_tuning_sample_size=0__cutoff_intersection_for_pairs=1.png
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    27892 2021-02-01 00:46:22.000000 deepdiff-6.7.1/docs/_static/benchmark_big_jsons__3.8__ignore_order=True__cache_size=0__cache_tuning_sample_size=0__max_diffs=300000__max_passes=40000__cutoff_intersection_for_pairs=1.png
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    30167 2021-02-01 00:46:22.000000 deepdiff-6.7.1/docs/_static/benchmark_big_jsons__pypy3.6__ignore_order=True__cache_size=0__cache_tuning_sample_size=0__max_diffs=300000__max_passes=40000__cutoff_intersection_for_pairs=1.png
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    22641 2021-02-01 00:46:22.000000 deepdiff-6.7.1/docs/_static/benchmark_deeply_nested_a__3.8__ignore_order=True__cache_size=0__cache_tuning_sample_size=0__cutoff_intersection_for_pairs=1.png
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    21556 2021-02-01 00:46:22.000000 deepdiff-6.7.1/docs/_static/benchmark_deeply_nested_a__3.8__ignore_order=True__cache_size=5000__cache_tuning_sample_size=0__cutoff_intersection_for_pairs=1.png
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    20752 2021-02-01 00:46:22.000000 deepdiff-6.7.1/docs/_static/benchmark_deeply_nested_a__3.8__ignore_order=True__cache_size=500__cache_tuning_sample_size=0__cutoff_intersection_for_pairs=1.png
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    19635 2021-02-01 00:46:22.000000 deepdiff-6.7.1/docs/_static/benchmark_deeply_nested_a__3.8__ignore_order=True__cache_size=500__cache_tuning_sample_size=500__cutoff_intersection_for_pairs=1.png
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    32429 2021-02-01 00:46:22.000000 deepdiff-6.7.1/docs/_static/benchmark_numpy_array__3.8__ignore_order=True__cache_size=0__cache_tuning_sample_size=0__cutoff_intersection_for_pairs=1.png
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     6136 2023-10-04 22:33:53.000000 deepdiff-6.7.1/docs/authors.rst
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    10667 2023-10-18 05:21:38.000000 deepdiff-6.7.1/docs/basics.rst
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     9543 2023-11-14 07:16:24.000000 deepdiff-6.7.1/docs/changelog.rst
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     8030 2021-02-01 00:46:22.000000 deepdiff-6.7.1/docs/commandline.rst
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    12063 2023-11-08 00:27:54.000000 deepdiff-6.7.1/docs/custom.rst
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     6444 2021-02-01 00:46:22.000000 deepdiff-6.7.1/docs/deep_distance.rst
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      160 2021-02-01 00:46:22.000000 deepdiff-6.7.1/docs/deephash.rst
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    17898 2023-09-01 00:27:49.000000 deepdiff-6.7.1/docs/deephash_doc.rst
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    21595 2023-11-14 07:16:24.000000 deepdiff-6.7.1/docs/delta.rst
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      361 2022-04-11 00:27:20.000000 deepdiff-6.7.1/docs/diff.rst
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    14904 2023-10-17 22:51:06.000000 deepdiff-6.7.1/docs/diff_doc.rst
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      222 2021-02-01 00:46:22.000000 deepdiff-6.7.1/docs/dsearch.rst
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     3595 2022-08-28 02:43:58.000000 deepdiff-6.7.1/docs/exclude_paths.rst
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      133 2021-02-01 00:46:22.000000 deepdiff-6.7.1/docs/extract.rst
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     4731 2023-10-04 22:33:53.000000 deepdiff-6.7.1/docs/faq.rst
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    14344 2021-10-13 18:10:55.000000 deepdiff-6.7.1/docs/ignore_order.rst
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    14455 2023-03-17 18:15:49.000000 deepdiff-6.7.1/docs/ignore_types_or_values.rst
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     4494 2023-11-14 07:16:24.000000 deepdiff-6.7.1/docs/index.rst
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     7224 2021-02-01 00:46:22.000000 deepdiff-6.7.1/docs/numbers.rst
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    13229 2023-09-01 00:27:49.000000 deepdiff-6.7.1/docs/optimizations.rst
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     3215 2022-04-11 00:27:20.000000 deepdiff-6.7.1/docs/other.rst
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     2648 2021-04-29 06:21:17.000000 deepdiff-6.7.1/docs/search_doc.rst
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     5996 2023-11-08 00:27:54.000000 deepdiff-6.7.1/docs/serialization.rst
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     2982 2021-02-01 00:46:22.000000 deepdiff-6.7.1/docs/stats.rst
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     1158 2023-10-04 22:33:53.000000 deepdiff-6.7.1/docs/support.rst
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      616 2021-02-01 00:46:22.000000 deepdiff-6.7.1/docs/troubleshoot.rst
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    13411 2021-04-29 06:21:17.000000 deepdiff-6.7.1/docs/view.rst
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       58 2021-02-01 00:46:22.000000 deepdiff-6.7.1/pytest.ini
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       27 2023-09-01 00:27:49.000000 deepdiff-6.7.1/requirements-cli.txt
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      265 2023-07-06 14:07:33.000000 deepdiff-6.7.1/requirements-dev-3.7.txt
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      428 2023-10-04 22:33:53.000000 deepdiff-6.7.1/requirements-dev.txt
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)        7 2023-03-17 18:15:49.000000 deepdiff-6.7.1/requirements-optimize.txt
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       26 2023-03-17 18:15:49.000000 deepdiff-6.7.1/requirements.txt
--rwxrwxr-x   0 erasmose  (1000) erasmose  (1000)       48 2021-02-01 00:46:22.000000 deepdiff-6.7.1/run_tests.sh
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      433 2023-11-14 07:19:40.428622 deepdiff-6.7.1/setup.cfg
--rwxrwxr-x   0 erasmose  (1000) erasmose  (1000)     2254 2023-11-14 07:16:24.000000 deepdiff-6.7.1/setup.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      447 2022-09-02 18:37:29.000000 deepdiff-6.7.1/temp.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      678 2023-09-14 07:10:30.000000 deepdiff-6.7.1/temp1.py
-drwxrwxr-x   0 erasmose  (1000) erasmose  (1000)        0 2023-11-14 07:19:40.424622 deepdiff-6.7.1/tests/
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     2090 2022-09-04 22:40:39.000000 deepdiff-6.7.1/tests/__init__.py
-drwxrwxr-x   0 erasmose  (1000) erasmose  (1000)        0 2023-11-14 07:19:40.424622 deepdiff-6.7.1/tests/fixtures/
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      182 2021-02-01 00:46:22.000000 deepdiff-6.7.1/tests/fixtures/another.yaml
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       57 2021-02-01 00:46:22.000000 deepdiff-6.7.1/tests/fixtures/c_t1.csv
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       59 2021-02-01 00:46:22.000000 deepdiff-6.7.1/tests/fixtures/c_t2.csv
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      964 2022-09-04 22:40:39.000000 deepdiff-6.7.1/tests/fixtures/compare_func_result1.json
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      861 2021-04-29 06:21:17.000000 deepdiff-6.7.1/tests/fixtures/compare_func_t1.json
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      834 2021-04-29 06:21:17.000000 deepdiff-6.7.1/tests/fixtures/compare_func_t2.json
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       84 2021-02-01 00:46:22.000000 deepdiff-6.7.1/tests/fixtures/d_t1.yaml
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       84 2021-02-01 00:46:22.000000 deepdiff-6.7.1/tests/fixtures/d_t2.yaml
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       18 2021-02-01 00:46:22.000000 deepdiff-6.7.1/tests/fixtures/invalid_yaml.yaml
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     5391 2021-02-01 00:46:22.000000 deepdiff-6.7.1/tests/fixtures/nested_a_result.json
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     1772 2021-02-01 00:46:22.000000 deepdiff-6.7.1/tests/fixtures/nested_a_t1.json
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     1839 2021-02-01 00:46:22.000000 deepdiff-6.7.1/tests/fixtures/nested_a_t2.json
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      487 2021-02-01 00:46:22.000000 deepdiff-6.7.1/tests/fixtures/nested_b_result.json
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      165 2021-02-01 00:46:22.000000 deepdiff-6.7.1/tests/fixtures/nested_b_t1.json
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      167 2021-02-01 00:46:22.000000 deepdiff-6.7.1/tests/fixtures/nested_b_t2.json
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       72 2021-02-01 00:46:22.000000 deepdiff-6.7.1/tests/fixtures/patch1.pickle
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       80 2021-02-01 00:46:22.000000 deepdiff-6.7.1/tests/fixtures/t1.csv
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       49 2021-02-01 00:46:22.000000 deepdiff-6.7.1/tests/fixtures/t1.json
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       28 2021-02-01 00:46:22.000000 deepdiff-6.7.1/tests/fixtures/t1.pickle
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      510 2021-02-01 00:46:22.000000 deepdiff-6.7.1/tests/fixtures/t1.toml
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       84 2021-02-01 00:46:22.000000 deepdiff-6.7.1/tests/fixtures/t1.yaml
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       50 2021-02-01 00:46:22.000000 deepdiff-6.7.1/tests/fixtures/t1_corrupt.json
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       80 2021-02-01 00:46:22.000000 deepdiff-6.7.1/tests/fixtures/t2.csv
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       71 2021-02-01 00:46:22.000000 deepdiff-6.7.1/tests/fixtures/t2.json
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       28 2021-02-01 00:46:22.000000 deepdiff-6.7.1/tests/fixtures/t2.pickle
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      496 2021-02-01 00:46:22.000000 deepdiff-6.7.1/tests/fixtures/t2.toml
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       84 2021-02-01 00:46:22.000000 deepdiff-6.7.1/tests/fixtures/t2.yaml
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       24 2021-02-01 00:46:22.000000 deepdiff-6.7.1/tests/fixtures/t2_json.csv
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     1297 2022-04-10 05:44:35.000000 deepdiff-6.7.1/tests/test_anyset.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     7425 2022-08-28 02:43:58.000000 deepdiff-6.7.1/tests/test_cache.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     5110 2023-03-17 18:15:49.000000 deepdiff-6.7.1/tests/test_command.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    76956 2023-11-14 07:16:24.000000 deepdiff-6.7.1/tests/test_delta.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     2307 2023-07-06 14:07:33.000000 deepdiff-6.7.1/tests/test_diff_datetime.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     4067 2021-02-01 00:46:22.000000 deepdiff-6.7.1/tests/test_diff_math.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     5961 2023-03-17 18:15:49.000000 deepdiff-6.7.1/tests/test_diff_numpy.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     7027 2023-10-04 22:33:53.000000 deepdiff-6.7.1/tests/test_diff_other.py
--rwxrwxr-x   0 erasmose  (1000) erasmose  (1000)    66902 2023-11-14 07:16:24.000000 deepdiff-6.7.1/tests/test_diff_text.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     6266 2023-03-17 18:15:49.000000 deepdiff-6.7.1/tests/test_diff_tree.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     9166 2022-04-10 05:44:35.000000 deepdiff-6.7.1/tests/test_distance.py
--rwxrwxr-x   0 erasmose  (1000) erasmose  (1000)    32066 2023-09-01 00:27:49.000000 deepdiff-6.7.1/tests/test_hash.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    17011 2023-09-01 00:27:49.000000 deepdiff-6.7.1/tests/test_helper.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    40789 2023-11-14 07:16:24.000000 deepdiff-6.7.1/tests/test_ignore_order.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     1766 2021-02-01 00:46:22.000000 deepdiff-6.7.1/tests/test_lfucache.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     7746 2021-10-13 18:10:55.000000 deepdiff-6.7.1/tests/test_model.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     9730 2023-09-01 00:27:49.000000 deepdiff-6.7.1/tests/test_operators.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     2471 2023-11-14 06:32:35.000000 deepdiff-6.7.1/tests/test_path.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    17641 2021-04-29 06:21:17.000000 deepdiff-6.7.1/tests/test_search.py
--rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    15997 2023-11-08 00:27:54.000000 deepdiff-6.7.1/tests/test_serialization.py
+drwxrwxr-x   0 erasmose  (1000) erasmose  (1000)        0 2024-04-08 08:47:43.916459 deepdiff-7.0.0/
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     5576 2024-04-08 08:46:34.000000 deepdiff-7.0.0/AUTHORS.md
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     1131 2021-04-28 22:25:20.000000 deepdiff-7.0.0/LICENSE
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      442 2023-11-21 06:18:29.000000 deepdiff-7.0.0/MANIFEST.in
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     6554 2024-04-08 08:47:43.916459 deepdiff-7.0.0/PKG-INFO
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     5470 2024-04-08 08:44:34.000000 deepdiff-7.0.0/README.md
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     3571 2024-04-08 07:55:01.000000 deepdiff-7.0.0/conftest.py
+drwxrwxr-x   0 erasmose  (1000) erasmose  (1000)        0 2024-04-08 08:47:43.908459 deepdiff-7.0.0/deepdiff/
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      398 2024-04-08 08:12:17.000000 deepdiff-7.0.0/deepdiff/__init__.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     2002 2021-02-01 00:46:22.000000 deepdiff-7.0.0/deepdiff/anyset.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     2163 2024-04-08 08:12:17.000000 deepdiff-7.0.0/deepdiff/base.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    10041 2023-11-21 06:18:29.000000 deepdiff-7.0.0/deepdiff/commands.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    21284 2024-04-08 08:12:17.000000 deepdiff-7.0.0/deepdiff/deephash.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    52507 2024-04-08 08:12:17.000000 deepdiff-7.0.0/deepdiff/delta.py
+-rwxrwxr-x   0 erasmose  (1000) erasmose  (1000)    84982 2024-04-08 08:12:17.000000 deepdiff-7.0.0/deepdiff/diff.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    10720 2024-04-08 08:12:17.000000 deepdiff-7.0.0/deepdiff/distance.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    22577 2024-04-08 08:12:17.000000 deepdiff-7.0.0/deepdiff/helper.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     6848 2021-02-01 00:46:22.000000 deepdiff-7.0.0/deepdiff/lfucache.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    40952 2024-04-08 08:12:17.000000 deepdiff-7.0.0/deepdiff/model.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     1264 2023-11-21 06:18:29.000000 deepdiff-7.0.0/deepdiff/operator.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    10360 2023-11-21 06:18:29.000000 deepdiff-7.0.0/deepdiff/path.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    12408 2021-04-29 06:21:17.000000 deepdiff-7.0.0/deepdiff/search.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    22615 2024-04-08 08:12:17.000000 deepdiff-7.0.0/deepdiff/serialization.py
+drwxrwxr-x   0 erasmose  (1000) erasmose  (1000)        0 2024-04-08 08:47:43.908459 deepdiff-7.0.0/deepdiff.egg-info/
+-rw-r--r--   0 erasmose  (1000) erasmose  (1000)     6554 2024-04-08 08:47:43.000000 deepdiff-7.0.0/deepdiff.egg-info/PKG-INFO
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     3834 2024-04-08 08:47:43.000000 deepdiff-7.0.0/deepdiff.egg-info/SOURCES.txt
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)        1 2024-04-08 08:47:43.000000 deepdiff-7.0.0/deepdiff.egg-info/dependency_links.txt
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       48 2024-04-08 08:47:43.000000 deepdiff-7.0.0/deepdiff.egg-info/entry_points.txt
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       79 2024-04-08 08:47:43.000000 deepdiff-7.0.0/deepdiff.egg-info/requires.txt
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)        9 2024-04-08 08:47:43.000000 deepdiff-7.0.0/deepdiff.egg-info/top_level.txt
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)        1 2023-01-06 05:03:23.000000 deepdiff-7.0.0/deepdiff.egg-info/zip-safe
+drwxrwxr-x   0 erasmose  (1000) erasmose  (1000)        0 2024-04-08 08:47:43.908459 deepdiff-7.0.0/docs/
+drwxrwxr-x   0 erasmose  (1000) erasmose  (1000)        0 2024-04-08 08:47:43.912459 deepdiff-7.0.0/docs/_static/
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    33163 2021-02-01 00:46:22.000000 deepdiff-7.0.0/docs/_static/benchmark_array_no_numpy__3.8__ignore_order=True__cache_size=0__cache_tuning_sample_size=0__cutoff_intersection_for_pairs=1.png
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    33204 2021-02-01 00:46:22.000000 deepdiff-7.0.0/docs/_static/benchmark_array_no_numpy__3.8__ignore_order=True__cache_size=10000__cache_tuning_sample_size=0__cutoff_intersection_for_pairs=1.png
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    27892 2021-02-01 00:46:22.000000 deepdiff-7.0.0/docs/_static/benchmark_big_jsons__3.8__ignore_order=True__cache_size=0__cache_tuning_sample_size=0__max_diffs=300000__max_passes=40000__cutoff_intersection_for_pairs=1.png
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    30167 2021-02-01 00:46:22.000000 deepdiff-7.0.0/docs/_static/benchmark_big_jsons__pypy3.6__ignore_order=True__cache_size=0__cache_tuning_sample_size=0__max_diffs=300000__max_passes=40000__cutoff_intersection_for_pairs=1.png
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    22641 2021-02-01 00:46:22.000000 deepdiff-7.0.0/docs/_static/benchmark_deeply_nested_a__3.8__ignore_order=True__cache_size=0__cache_tuning_sample_size=0__cutoff_intersection_for_pairs=1.png
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    21556 2021-02-01 00:46:22.000000 deepdiff-7.0.0/docs/_static/benchmark_deeply_nested_a__3.8__ignore_order=True__cache_size=5000__cache_tuning_sample_size=0__cutoff_intersection_for_pairs=1.png
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    20752 2021-02-01 00:46:22.000000 deepdiff-7.0.0/docs/_static/benchmark_deeply_nested_a__3.8__ignore_order=True__cache_size=500__cache_tuning_sample_size=0__cutoff_intersection_for_pairs=1.png
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    19635 2021-02-01 00:46:22.000000 deepdiff-7.0.0/docs/_static/benchmark_deeply_nested_a__3.8__ignore_order=True__cache_size=500__cache_tuning_sample_size=500__cutoff_intersection_for_pairs=1.png
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    32429 2021-02-01 00:46:22.000000 deepdiff-7.0.0/docs/_static/benchmark_numpy_array__3.8__ignore_order=True__cache_size=0__cache_tuning_sample_size=0__cutoff_intersection_for_pairs=1.png
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     6389 2024-04-08 08:46:59.000000 deepdiff-7.0.0/docs/authors.rst
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    11077 2024-04-08 08:41:32.000000 deepdiff-7.0.0/docs/basics.rst
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    10663 2024-04-08 08:16:43.000000 deepdiff-7.0.0/docs/changelog.rst
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     8030 2021-02-01 00:46:22.000000 deepdiff-7.0.0/docs/commandline.rst
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    12063 2023-11-21 06:18:29.000000 deepdiff-7.0.0/docs/custom.rst
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     6444 2021-02-01 00:46:22.000000 deepdiff-7.0.0/docs/deep_distance.rst
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      160 2021-02-01 00:46:22.000000 deepdiff-7.0.0/docs/deephash.rst
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    17898 2023-11-21 06:18:29.000000 deepdiff-7.0.0/docs/deephash_doc.rst
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    21816 2024-04-08 08:12:17.000000 deepdiff-7.0.0/docs/delta.rst
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      361 2022-04-11 00:27:20.000000 deepdiff-7.0.0/docs/diff.rst
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    15116 2024-04-08 08:12:17.000000 deepdiff-7.0.0/docs/diff_doc.rst
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      222 2021-02-01 00:46:22.000000 deepdiff-7.0.0/docs/dsearch.rst
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     3595 2023-11-21 06:18:29.000000 deepdiff-7.0.0/docs/exclude_paths.rst
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      133 2021-02-01 00:46:22.000000 deepdiff-7.0.0/docs/extract.rst
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     4731 2023-11-21 06:18:29.000000 deepdiff-7.0.0/docs/faq.rst
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    14344 2021-10-13 18:10:55.000000 deepdiff-7.0.0/docs/ignore_order.rst
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    15138 2024-04-08 08:12:17.000000 deepdiff-7.0.0/docs/ignore_types_or_values.rst
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     5394 2024-04-08 08:45:38.000000 deepdiff-7.0.0/docs/index.rst
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     7224 2021-02-01 00:46:22.000000 deepdiff-7.0.0/docs/numbers.rst
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    13229 2023-11-21 06:18:29.000000 deepdiff-7.0.0/docs/optimizations.rst
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     3215 2022-04-11 00:27:20.000000 deepdiff-7.0.0/docs/other.rst
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     2648 2021-04-29 06:21:17.000000 deepdiff-7.0.0/docs/search_doc.rst
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    10997 2024-04-08 08:12:17.000000 deepdiff-7.0.0/docs/serialization.rst
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     2982 2021-02-01 00:46:22.000000 deepdiff-7.0.0/docs/stats.rst
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     1158 2023-11-21 06:18:29.000000 deepdiff-7.0.0/docs/support.rst
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      616 2021-02-01 00:46:22.000000 deepdiff-7.0.0/docs/troubleshoot.rst
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    13455 2024-04-08 08:42:44.000000 deepdiff-7.0.0/docs/view.rst
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       58 2021-02-01 00:46:22.000000 deepdiff-7.0.0/pytest.ini
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       27 2024-04-08 08:12:17.000000 deepdiff-7.0.0/requirements-cli.txt
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      441 2024-04-08 08:12:17.000000 deepdiff-7.0.0/requirements-dev.txt
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)        7 2023-11-21 06:18:29.000000 deepdiff-7.0.0/requirements-optimize.txt
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       26 2024-04-08 08:12:17.000000 deepdiff-7.0.0/requirements.txt
+-rwxrwxr-x   0 erasmose  (1000) erasmose  (1000)       48 2021-02-01 00:46:22.000000 deepdiff-7.0.0/run_tests.sh
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      466 2024-04-08 08:47:43.916459 deepdiff-7.0.0/setup.cfg
+-rwxrwxr-x   0 erasmose  (1000) erasmose  (1000)     2255 2024-04-08 08:12:17.000000 deepdiff-7.0.0/setup.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      447 2022-09-02 18:37:29.000000 deepdiff-7.0.0/temp.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      678 2023-09-14 07:10:30.000000 deepdiff-7.0.0/temp1.py
+drwxrwxr-x   0 erasmose  (1000) erasmose  (1000)        0 2024-04-08 08:47:43.916459 deepdiff-7.0.0/tests/
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     2090 2023-11-21 06:18:29.000000 deepdiff-7.0.0/tests/__init__.py
+drwxrwxr-x   0 erasmose  (1000) erasmose  (1000)        0 2024-04-08 08:47:43.916459 deepdiff-7.0.0/tests/fixtures/
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      182 2021-02-01 00:46:22.000000 deepdiff-7.0.0/tests/fixtures/another.yaml
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       57 2021-02-01 00:46:22.000000 deepdiff-7.0.0/tests/fixtures/c_t1.csv
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       59 2021-02-01 00:46:22.000000 deepdiff-7.0.0/tests/fixtures/c_t2.csv
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      964 2023-11-21 06:18:29.000000 deepdiff-7.0.0/tests/fixtures/compare_func_result1.json
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      861 2021-04-29 06:21:17.000000 deepdiff-7.0.0/tests/fixtures/compare_func_t1.json
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      834 2021-04-29 06:21:17.000000 deepdiff-7.0.0/tests/fixtures/compare_func_t2.json
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       84 2021-02-01 00:46:22.000000 deepdiff-7.0.0/tests/fixtures/d_t1.yaml
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       84 2021-02-01 00:46:22.000000 deepdiff-7.0.0/tests/fixtures/d_t2.yaml
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       18 2021-02-01 00:46:22.000000 deepdiff-7.0.0/tests/fixtures/invalid_yaml.yaml
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     5391 2024-04-08 07:54:55.000000 deepdiff-7.0.0/tests/fixtures/nested_a_result.json
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     1772 2021-02-01 00:46:22.000000 deepdiff-7.0.0/tests/fixtures/nested_a_t1.json
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     1839 2021-02-01 00:46:22.000000 deepdiff-7.0.0/tests/fixtures/nested_a_t2.json
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      487 2021-02-01 00:46:22.000000 deepdiff-7.0.0/tests/fixtures/nested_b_result.json
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      165 2021-02-01 00:46:22.000000 deepdiff-7.0.0/tests/fixtures/nested_b_t1.json
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      167 2021-02-01 00:46:22.000000 deepdiff-7.0.0/tests/fixtures/nested_b_t2.json
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       72 2021-02-01 00:46:22.000000 deepdiff-7.0.0/tests/fixtures/patch1.pickle
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       80 2021-02-01 00:46:22.000000 deepdiff-7.0.0/tests/fixtures/t1.csv
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       49 2021-02-01 00:46:22.000000 deepdiff-7.0.0/tests/fixtures/t1.json
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       28 2021-02-01 00:46:22.000000 deepdiff-7.0.0/tests/fixtures/t1.pickle
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      510 2021-02-01 00:46:22.000000 deepdiff-7.0.0/tests/fixtures/t1.toml
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       84 2021-02-01 00:46:22.000000 deepdiff-7.0.0/tests/fixtures/t1.yaml
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       50 2021-02-01 00:46:22.000000 deepdiff-7.0.0/tests/fixtures/t1_corrupt.json
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       80 2021-02-01 00:46:22.000000 deepdiff-7.0.0/tests/fixtures/t2.csv
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       71 2021-02-01 00:46:22.000000 deepdiff-7.0.0/tests/fixtures/t2.json
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       28 2021-02-01 00:46:22.000000 deepdiff-7.0.0/tests/fixtures/t2.pickle
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)      496 2021-02-01 00:46:22.000000 deepdiff-7.0.0/tests/fixtures/t2.toml
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       84 2021-02-01 00:46:22.000000 deepdiff-7.0.0/tests/fixtures/t2.yaml
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)       24 2021-02-01 00:46:22.000000 deepdiff-7.0.0/tests/fixtures/t2_json.csv
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     1297 2022-04-10 05:44:35.000000 deepdiff-7.0.0/tests/test_anyset.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     7425 2024-04-08 07:55:27.000000 deepdiff-7.0.0/tests/test_cache.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     5110 2023-11-21 06:18:29.000000 deepdiff-7.0.0/tests/test_command.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    93024 2024-04-08 08:12:17.000000 deepdiff-7.0.0/tests/test_delta.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     2307 2023-11-21 06:18:29.000000 deepdiff-7.0.0/tests/test_diff_datetime.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     4067 2021-02-01 00:46:22.000000 deepdiff-7.0.0/tests/test_diff_math.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     6182 2024-04-08 08:12:17.000000 deepdiff-7.0.0/tests/test_diff_numpy.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     7027 2024-04-08 07:06:53.000000 deepdiff-7.0.0/tests/test_diff_other.py
+-rwxrwxr-x   0 erasmose  (1000) erasmose  (1000)    68573 2024-04-08 08:12:17.000000 deepdiff-7.0.0/tests/test_diff_text.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     6266 2023-11-21 06:18:29.000000 deepdiff-7.0.0/tests/test_diff_tree.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     9166 2024-04-08 07:52:54.000000 deepdiff-7.0.0/tests/test_distance.py
+-rwxrwxr-x   0 erasmose  (1000) erasmose  (1000)    33020 2024-04-08 08:12:17.000000 deepdiff-7.0.0/tests/test_hash.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    17011 2023-11-21 06:18:29.000000 deepdiff-7.0.0/tests/test_helper.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    48800 2024-04-08 08:12:17.000000 deepdiff-7.0.0/tests/test_ignore_order.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     1766 2021-02-01 00:46:22.000000 deepdiff-7.0.0/tests/test_lfucache.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    10440 2024-04-08 08:12:17.000000 deepdiff-7.0.0/tests/test_model.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     9730 2023-11-21 06:18:29.000000 deepdiff-7.0.0/tests/test_operators.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)     2471 2023-11-21 06:18:29.000000 deepdiff-7.0.0/tests/test_path.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    17641 2021-04-29 06:21:17.000000 deepdiff-7.0.0/tests/test_search.py
+-rw-rw-r--   0 erasmose  (1000) erasmose  (1000)    17234 2024-04-08 08:12:17.000000 deepdiff-7.0.0/tests/test_serialization.py
```

### Comparing `deepdiff-6.7.1/AUTHORS.md` & `deepdiff-7.0.0/AUTHORS.md`

 * *Files 3% similar despite different names*

```diff
@@ -55,7 +55,9 @@
 - [maggelus](https://github.com/maggelus) for the bugfix deephash for paths.
 - [maggelus](https://github.com/maggelus) for the bugfix deephash compiled regex.
 - [martin-kokos](https://github.com/martin-kokos) for fixing the tests dependent on toml.
 - [kor4ik](https://github.com/kor4ik) for the bugfix for `include_paths` for nested dictionaries.
 - [martin-kokos](https://github.com/martin-kokos) for using tomli and tomli-w for dealing with tomli files.
 - [Alex Sauer-Budge](https://github.com/amsb) for the bugfix for `datetime.date`.
 - [William Jamieson](https://github.com/WilliamJamieson) for [NumPy 2.0 compatibility](https://github.com/seperman/deepdiff/pull/422)
+- [Leo Sin](https://github.com/leoslf) for Supporting Python 3.12 in the build process
+- [sf-tcalhoun](https://github.com/sf-tcalhoun) for fixing "Instantiating a Delta with a flat_dict_list unexpectedly mutates the flat_dict_list"
```

### Comparing `deepdiff-6.7.1/LICENSE` & `deepdiff-7.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deepdiff-6.7.1/PKG-INFO` & `deepdiff-7.0.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 Metadata-Version: 2.1
 Name: deepdiff
-Version: 6.7.1
+Version: 7.0.0
 Summary: Deep Difference and Search of any Python object/data. Recreate objects by adding adding deltas to each other.
 Home-page: https://github.com/seperman/deepdiff
-Download-URL: https://github.com/seperman/deepdiff/tarball/master
 Author: Seperman
 Author-email: sep@zepworks.com
 License: MIT
+Download-URL: https://github.com/seperman/deepdiff/tarball/master
+Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: cli
 Provides-Extra: optimize
 License-File: LICENSE
 License-File: AUTHORS.md
 
-# DeepDiff v 6.7.1
+# DeepDiff v 7.0.0
 
 ![Downloads](https://img.shields.io/pypi/dm/deepdiff.svg?style=flat)
 ![Python Versions](https://img.shields.io/pypi/pyversions/deepdiff.svg?style=flat)
 ![License](https://img.shields.io/pypi/l/deepdiff.svg?version=latest)
 [![Build Status](https://github.com/seperman/deepdiff/workflows/Unit%20Tests/badge.svg)](https://github.com/seperman/deepdiff/actions)
 [![codecov](https://codecov.io/gh/seperman/deepdiff/branch/master/graph/badge.svg?token=KkHZ3siA3m)](https://codecov.io/gh/seperman/deepdiff)
 
@@ -38,22 +39,31 @@
 - [DeepDiff](https://zepworks.com/deepdiff/current/diff.html): Deep Difference of dictionaries, iterables, strings, and ANY other object.
 - [DeepSearch](https://zepworks.com/deepdiff/current/dsearch.html): Search for objects within other objects.
 - [DeepHash](https://zepworks.com/deepdiff/current/deephash.html): Hash any object based on their content.
 - [Delta](https://zepworks.com/deepdiff/current/delta.html): Store the difference of objects and apply them to other objects.
 - [Extract](https://zepworks.com/deepdiff/current/extract.html): Extract an item from a nested Python object using its path.
 - [commandline](https://zepworks.com/deepdiff/current/commandline.html): Use DeepDiff from commandline.
 
-Tested on Python 3.7+ and PyPy3.
+Tested on Python 3.8+ and PyPy3.
 
-- **[Documentation](https://zepworks.com/deepdiff/6.7.1/)**
+- **[Documentation](https://zepworks.com/deepdiff/7.0.0/)**
 
 ## What is new?
 
 Please check the [ChangeLog](CHANGELOG.md) file for the detailed information.
 
+DeepDiff 7-0-0
+
+- DeepDiff 7 comes with an improved delta object. [Delta to flat dictionaries](https://zepworks.com/deepdiff/current/serialization.html#delta-serialize-to-flat-dictionaries) have undergone a major change. We have also introduced [Delta serialize to flat rows](https://zepworks.com/deepdiff/current/serialization.html#delta-serialize-to-flat-rows).
+- Subtracting delta objects have dramatically improved at the cost of holding more metadata about the original objects.
+- When `verbose=2`, and the "path" of an item has changed in a report between t1 and t2, we include it as `new_path`.
+- `path(use_t2=True)` returns the correct path to t2 in any reported change in the [`tree view`](https://zepworks.com/deepdiff/current/view.html#tree-view)
+- Python 3.7 support is dropped and Python 3.12 is officially supported.
+
+
 DeepDiff 6-7-1
 
 - Support for subtracting delta objects when iterable_compare_func is used.
 - Better handling of force adding a delta to an object. 
 - Fix for [`Can't compare dicts with both single and double quotes in keys`](https://github.com/seperman/deepdiff/issues/430)
 - Updated docs for Inconsistent Behavior with math_epsilon and ignore_order = True
 
@@ -124,20 +134,12 @@
 
 Please run `pytest --cov=deepdiff --runslow` to see the coverage report. Note that the `--runslow` flag will run some slow tests too. In most cases you only want to run the fast tests which so you wont add the `--runslow` flag.
 
 Or to see a more user friendly version, please run: `pytest --cov=deepdiff --cov-report term-missing --runslow`.
 
 Thank you!
 
-# Citing
-
-How to cite this library (APA style):
-
-    Dehpour, S. (2023). DeepDiff (Version 6.7.1) [Software]. Available from https://github.com/seperman/deepdiff.
-
-How to cite this library (Chicago style):
-
-    Dehpour, Sep. 2023. DeepDiff (version 6.7.1).
-
 # Authors
 
 Please take a look at the [AUTHORS](AUTHORS.md) file.
+
+
```

### Comparing `deepdiff-6.7.1/README.md` & `deepdiff-7.0.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# DeepDiff v 6.7.1
+# DeepDiff v 7.0.0
 
 ![Downloads](https://img.shields.io/pypi/dm/deepdiff.svg?style=flat)
 ![Python Versions](https://img.shields.io/pypi/pyversions/deepdiff.svg?style=flat)
 ![License](https://img.shields.io/pypi/l/deepdiff.svg?version=latest)
 [![Build Status](https://github.com/seperman/deepdiff/workflows/Unit%20Tests/badge.svg)](https://github.com/seperman/deepdiff/actions)
 [![codecov](https://codecov.io/gh/seperman/deepdiff/branch/master/graph/badge.svg?token=KkHZ3siA3m)](https://codecov.io/gh/seperman/deepdiff)
 
@@ -11,22 +11,31 @@
 - [DeepDiff](https://zepworks.com/deepdiff/current/diff.html): Deep Difference of dictionaries, iterables, strings, and ANY other object.
 - [DeepSearch](https://zepworks.com/deepdiff/current/dsearch.html): Search for objects within other objects.
 - [DeepHash](https://zepworks.com/deepdiff/current/deephash.html): Hash any object based on their content.
 - [Delta](https://zepworks.com/deepdiff/current/delta.html): Store the difference of objects and apply them to other objects.
 - [Extract](https://zepworks.com/deepdiff/current/extract.html): Extract an item from a nested Python object using its path.
 - [commandline](https://zepworks.com/deepdiff/current/commandline.html): Use DeepDiff from commandline.
 
-Tested on Python 3.7+ and PyPy3.
+Tested on Python 3.8+ and PyPy3.
 
-- **[Documentation](https://zepworks.com/deepdiff/6.7.1/)**
+- **[Documentation](https://zepworks.com/deepdiff/7.0.0/)**
 
 ## What is new?
 
 Please check the [ChangeLog](CHANGELOG.md) file for the detailed information.
 
+DeepDiff 7-0-0
+
+- DeepDiff 7 comes with an improved delta object. [Delta to flat dictionaries](https://zepworks.com/deepdiff/current/serialization.html#delta-serialize-to-flat-dictionaries) have undergone a major change. We have also introduced [Delta serialize to flat rows](https://zepworks.com/deepdiff/current/serialization.html#delta-serialize-to-flat-rows).
+- Subtracting delta objects have dramatically improved at the cost of holding more metadata about the original objects.
+- When `verbose=2`, and the "path" of an item has changed in a report between t1 and t2, we include it as `new_path`.
+- `path(use_t2=True)` returns the correct path to t2 in any reported change in the [`tree view`](https://zepworks.com/deepdiff/current/view.html#tree-view)
+- Python 3.7 support is dropped and Python 3.12 is officially supported.
+
+
 DeepDiff 6-7-1
 
 - Support for subtracting delta objects when iterable_compare_func is used.
 - Better handling of force adding a delta to an object. 
 - Fix for [`Can't compare dicts with both single and double quotes in keys`](https://github.com/seperman/deepdiff/issues/430)
 - Updated docs for Inconsistent Behavior with math_epsilon and ignore_order = True
 
@@ -97,20 +106,10 @@
 
 Please run `pytest --cov=deepdiff --runslow` to see the coverage report. Note that the `--runslow` flag will run some slow tests too. In most cases you only want to run the fast tests which so you wont add the `--runslow` flag.
 
 Or to see a more user friendly version, please run: `pytest --cov=deepdiff --cov-report term-missing --runslow`.
 
 Thank you!
 
-# Citing
-
-How to cite this library (APA style):
-
-    Dehpour, S. (2023). DeepDiff (Version 6.7.1) [Software]. Available from https://github.com/seperman/deepdiff.
-
-How to cite this library (Chicago style):
-
-    Dehpour, Sep. 2023. DeepDiff (version 6.7.1).
-
 # Authors
 
 Please take a look at the [AUTHORS](AUTHORS.md) file.
```

### Comparing `deepdiff-6.7.1/conftest.py` & `deepdiff-7.0.0/conftest.py`

 * *Files identical despite different names*

### Comparing `deepdiff-6.7.1/deepdiff/anyset.py` & `deepdiff-7.0.0/deepdiff/anyset.py`

 * *Files identical despite different names*

### Comparing `deepdiff-6.7.1/deepdiff/base.py` & `deepdiff-7.0.0/deepdiff/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,11 +40,12 @@
 
         if ignore_string_type_changes and self.strings not in ignore_type_in_groups:
             ignore_type_in_groups.append(OrderedSet(self.strings))
 
         if ignore_numeric_type_changes and self.numbers not in ignore_type_in_groups:
             ignore_type_in_groups.append(OrderedSet(self.numbers))
 
-        if ignore_type_subclasses:
+        if not ignore_type_subclasses:
+            # is_instance method needs tuples. When we look for subclasses, we need them to be tuples
             ignore_type_in_groups = list(map(tuple, ignore_type_in_groups))
 
         return ignore_type_in_groups
```

### Comparing `deepdiff-6.7.1/deepdiff/commands.py` & `deepdiff-7.0.0/deepdiff/commands.py`

 * *Files identical despite different names*

### Comparing `deepdiff-6.7.1/deepdiff/deephash.py` & `deepdiff-7.0.0/deepdiff/deephash.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/env python
 import inspect
 import logging
+import datetime
 from collections.abc import Iterable, MutableMapping
 from collections import defaultdict
 from hashlib import sha1, sha256
 from pathlib import Path
 from enum import Enum
 from deepdiff.helper import (strings, numbers, times, unprocessed, not_hashed, add_to_frozen_set,
                              convert_item_or_items_into_set_else_none, get_doc,
@@ -182,15 +183,16 @@
         self.ignore_numeric_type_changes = ignore_numeric_type_changes
         self.ignore_string_case = ignore_string_case
         self.exclude_obj_callback = exclude_obj_callback
         # makes the hash return constant size result if true
         # the only time it should be set to False is when
         # testing the individual hash functions for different types of objects.
         self.apply_hash = apply_hash
-        self.type_check_func = type_is_subclass_of_type_group if ignore_type_subclasses else type_in_type_group
+        self.type_check_func = type_in_type_group if ignore_type_subclasses else type_is_subclass_of_type_group
+        # self.type_check_func = type_is_subclass_of_type_group if ignore_type_subclasses else type_in_type_group
         self.number_to_string = number_to_string_func or number_to_string
         self.ignore_private_variables = ignore_private_variables
         self.encodings = encodings
         self.ignore_encoding_errors = ignore_encoding_errors
         self.ignore_iterable_order = ignore_iterable_order
 
         self._hash(obj, parent=parent, parents_ids=frozenset({get_id(obj)}))
@@ -451,14 +453,18 @@
         return KEY_TO_VAL_STR.format(type_, obj)
 
     def _prep_datetime(self, obj):
         type_ = 'datetime'
         obj = datetime_normalize(self.truncate_datetime, obj)
         return KEY_TO_VAL_STR.format(type_, obj)
 
+    def _prep_date(self, obj):
+        type_ = 'datetime'  # yes still datetime but it doesn't need normalization
+        return KEY_TO_VAL_STR.format(type_, obj)
+
     def _prep_tuple(self, obj, parent, parents_ids):
         # Checking to see if it has _fields. Which probably means it is a named
         # tuple.
         try:
             obj._asdict
         # It must be a normal tuple
         except AttributeError:
@@ -501,14 +507,17 @@
 
         elif isinstance(obj, Path):
             result = self._prep_path(obj)
 
         elif isinstance(obj, times):
             result = self._prep_datetime(obj)
 
+        elif isinstance(obj, datetime.date):
+            result = self._prep_date(obj)
+
         elif isinstance(obj, numbers):
             result = self._prep_number(obj)
 
         elif isinstance(obj, MutableMapping):
             result, counts = self._prep_dict(obj=obj, parent=parent, parents_ids=parents_ids)
 
         elif isinstance(obj, tuple):
```

### Comparing `deepdiff-6.7.1/deepdiff/delta.py` & `deepdiff-7.0.0/deepdiff/delta.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,33 @@
+import copy
 import logging
-from functools import partial
+from typing import List, Dict, IO, Callable, Set, Union, Optional
+from functools import partial, cmp_to_key
 from collections.abc import Mapping
 from copy import deepcopy
 from ordered_set import OrderedSet
 from deepdiff import DeepDiff
 from deepdiff.serialization import pickle_load, pickle_dump
 from deepdiff.helper import (
     strings, short_repr, numbers,
     np_ndarray, np_array_factory, numpy_dtypes, get_doc,
     not_found, numpy_dtype_string_to_type, dict_,
+    Opcode, FlatDeltaRow, UnkownValueCode,
 )
 from deepdiff.path import (
     _path_to_elements, _get_nested_obj, _get_nested_obj_and_force,
-    GET, GETATTR, parse_path, stringify_path, DEFAULT_FIRST_ELEMENT
+    GET, GETATTR, parse_path, stringify_path,
 )
 from deepdiff.anyset import AnySet
 
 
 logger = logging.getLogger(__name__)
 
 
-VERIFICATION_MSG = 'Expected the old value for {} to be {} but it is {}. Error found on: {}'
+VERIFICATION_MSG = 'Expected the old value for {} to be {} but it is {}. Error found on: {}. You may want to set force=True, especially if this delta is created by passing flat_rows_list or flat_dict_list'
 ELEM_NOT_FOUND_TO_ADD_MSG = 'Key or index of {} is not found for {} for setting operation.'
 TYPE_CHANGE_FAIL_MSG = 'Unable to do the type change for {} from to type {} due to {}'
 VERIFY_BIDIRECTIONAL_MSG = ('You have applied the delta to an object that has '
                             'different values than the original object the delta was made from.')
 FAIL_TO_REMOVE_ITEM_IGNORE_ORDER_MSG = 'Failed to remove index[{}] on {}. It was expected to be {} but got {}'
 DELTA_NUMPY_OPERATOR_OVERRIDE_MSG = (
     'A numpy ndarray is most likely being added to a delta. '
@@ -54,46 +57,57 @@
 class DeltaNumpyOperatorOverrideError(ValueError):
     """
     Delta Numpy Operator Override Error
     """
     pass
 
 
-class _ObjDoesNotExist:
-    pass
-
-
 class Delta:
 
     __doc__ = doc
 
     def __init__(
         self,
-        diff=None,
-        delta_path=None,
-        delta_file=None,
-        delta_diff=None,
-        flat_dict_list=None,
-        deserializer=pickle_load,
-        log_errors=True,
-        mutate=False,
-        raise_errors=False,
-        safe_to_import=None,
-        serializer=pickle_dump,
-        verify_symmetry=None,
-        bidirectional=False,
-        always_include_values=False,
-        iterable_compare_func_was_used=None,
-        force=False,
+        diff: Union[DeepDiff, Mapping, str, bytes, None]=None,
+        delta_path: Optional[str]=None,
+        delta_file: Optional[IO]=None,
+        delta_diff: Optional[dict]=None,
+        flat_dict_list: Optional[List[Dict]]=None,
+        flat_rows_list: Optional[List[FlatDeltaRow]]=None,
+        deserializer: Callable=pickle_load,
+        log_errors: bool=True,
+        mutate: bool=False,
+        raise_errors: bool=False,
+        safe_to_import: Optional[Set[str]]=None,
+        serializer: Callable=pickle_dump,
+        verify_symmetry: Optional[bool]=None,
+        bidirectional: bool=False,
+        always_include_values: bool=False,
+        iterable_compare_func_was_used: Optional[bool]=None,
+        force: bool=False,
     ):
+        # for pickle deserializer:
         if hasattr(deserializer, '__code__') and 'safe_to_import' in set(deserializer.__code__.co_varnames):
             _deserializer = deserializer
         else:
             def _deserializer(obj, safe_to_import=None):
-                return deserializer(obj)
+                result = deserializer(obj)
+                if result.get('_iterable_opcodes'):
+                    _iterable_opcodes = {}
+                    for path, op_codes in result['_iterable_opcodes'].items():
+                        _iterable_opcodes[path] = []
+                        for op_code in op_codes:
+                            _iterable_opcodes[path].append(
+                                Opcode(
+                                    **op_code
+                                )
+                            )
+                    result['_iterable_opcodes'] = _iterable_opcodes
+                return result
+
 
         self._reversed_diff = None
 
         if verify_symmetry is not None:
             logger.warning(
                 "DeepDiff Deprecation: use bidirectional instead of verify_symmetry parameter."
             )
@@ -121,15 +135,18 @@
         elif delta_file:
             try:
                 content = delta_file.read()
             except UnicodeDecodeError as e:
                 raise ValueError(BINIARY_MODE_NEEDED_MSG.format(e)) from None
             self.diff = _deserializer(content, safe_to_import=safe_to_import)
         elif flat_dict_list:
-            self.diff = self._from_flat_dicts(flat_dict_list)
+            # Use copy to preserve original value of flat_dict_list in calling module
+            self.diff = self._from_flat_dicts(copy.deepcopy(flat_dict_list))
+        elif flat_rows_list:
+            self.diff = self._from_flat_rows(copy.deepcopy(flat_rows_list))
         else:
             raise ValueError(DELTA_AT_LEAST_ONE_ARG_NEEDED)
 
         self.mutate = mutate
         self.raise_errors = raise_errors
         self.log_errors = log_errors
         self._numpy_paths = self.diff.get('_numpy_paths', False)
@@ -161,14 +178,15 @@
         self._do_pre_process()
         self._do_values_changed()
         self._do_set_item_added()
         self._do_set_item_removed()
         self._do_type_changes()
         # NOTE: the remove iterable action needs to happen BEFORE
         # all the other iterables to match the reverse of order of operations in DeepDiff
+        self._do_iterable_opcodes()
         self._do_iterable_item_removed()
         self._do_iterable_item_added()
         self._do_ignore_order()
         self._do_dictionary_item_added()
         self._do_dictionary_item_removed()
         self._do_attribute_added()
         self._do_attribute_removed()
@@ -377,20 +395,59 @@
     @staticmethod
     def _sort_key_for_item_added(path_and_value):
         elements = _path_to_elements(path_and_value[0])
         # Example elements: [(4.3, 'GET'), ('b', 'GETATTR'), ('a3', 'GET')]
         # We only care about the values in the elements not how to get the values.
         return [i[0] for i in elements] 
 
+    @staticmethod
+    def _sort_comparison(left, right):
+        """
+        We use sort comparison instead of _sort_key_for_item_added when we run into comparing element types that can not
+        be compared with each other, such as None to None. Or integer to string.
+        """
+        # Example elements: [(4.3, 'GET'), ('b', 'GETATTR'), ('a3', 'GET')]
+        # We only care about the values in the elements not how to get the values.
+        left_path = [i[0] for i in _path_to_elements(left[0], root_element=None)]
+        right_path = [i[0] for i in _path_to_elements(right[0], root_element=None)]
+        try:
+            if left_path < right_path:
+                return -1
+            elif left_path > right_path:
+                return 1
+            else:
+                return 0
+        except TypeError:
+            if len(left_path) > len(right_path):
+                left_path = left_path[:len(right_path)]
+            elif len(right_path) > len(left_path):
+                right_path = right_path[:len(left_path)]
+            for l_elem, r_elem in zip(left_path, right_path):
+                if type(l_elem) != type(r_elem) or type(l_elem) in None:
+                    l_elem = str(l_elem)
+                    r_elem = str(r_elem)
+                try:
+                    if l_elem < r_elem:
+                        return -1
+                    elif l_elem > r_elem:
+                        return 1
+                except TypeError:
+                    continue
+        return 0
+
+
     def _do_item_added(self, items, sort=True, insert=False):
         if sort:
             # sorting items by their path so that the items with smaller index
             # are applied first (unless `sort` is `False` so that order of
             # added items is retained, e.g. for dicts).
-            items = sorted(items.items(), key=self._sort_key_for_item_added)
+            try:
+                items = sorted(items.items(), key=self._sort_key_for_item_added)
+            except TypeError:
+                items = sorted(items.items(), key=cmp_to_key(self._sort_comparison))
         else:
             items = items.items()
 
         for path, new_value in items:
             elem_and_details = self._get_elements_and_details(path)
             if elem_and_details:
                 elements, parent, parent_to_obj_elem, parent_to_obj_action, obj, elem, action = elem_and_details
@@ -446,14 +503,18 @@
                     next_element = None
                 parent = self.get_nested_obj(obj=self, elements=elements_subset, next_element=next_element)
                 parent_to_obj_elem, parent_to_obj_action = elements[-2]
                 obj = self._get_elem_and_compare_to_old_value(
                     obj=parent, path_for_err_reporting=path, expected_old_value=None,
                     elem=parent_to_obj_elem, action=parent_to_obj_action, next_element=next2_element)
             else:
+                # parent = self
+                # obj = self.root
+                # parent_to_obj_elem = 'root'
+                # parent_to_obj_action = GETATTR
                 parent = parent_to_obj_elem = parent_to_obj_action = None
                 obj = self
                 # obj = self.get_nested_obj(obj=self, elements=elements[:-1])
             elem, action = elements[-1]
         except Exception as e:
             self._raise_or_log(UNABLE_TO_GET_ITEM_MSG.format(path, e))
             return None
@@ -500,30 +561,33 @@
 
     def _do_item_removed(self, items):
         """
         Handle removing items.
         """
         # Sorting the iterable_item_removed in reverse order based on the paths.
         # So that we delete a bigger index before a smaller index
-        for path, expected_old_value in sorted(items.items(), key=self._sort_key_for_item_added, reverse=True):
+        try:
+            sorted_item = sorted(items.items(), key=self._sort_key_for_item_added, reverse=True)
+        except TypeError:
+            sorted_item = sorted(items.items(), key=cmp_to_key(self._sort_comparison), reverse=True)
+        for path, expected_old_value in sorted_item:
             elem_and_details = self._get_elements_and_details(path)
             if elem_and_details:
                 elements, parent, parent_to_obj_elem, parent_to_obj_action, obj, elem, action = elem_and_details
             else:
                 continue  # pragma: no cover. Due to cPython peephole optimizer, this line doesn't get covered. https://github.com/nedbat/coveragepy/issues/198
 
             look_for_expected_old_value = False
             current_old_value = not_found
             try:
                 if action == GET:
                     current_old_value = obj[elem]
-                    look_for_expected_old_value = current_old_value != expected_old_value
                 elif action == GETATTR:
                     current_old_value = getattr(obj, elem)
-                    look_for_expected_old_value = current_old_value != expected_old_value
+                look_for_expected_old_value = current_old_value != expected_old_value
             except (KeyError, IndexError, AttributeError, TypeError):
                 look_for_expected_old_value = True
 
             if look_for_expected_old_value and isinstance(obj, list) and not self._iterable_compare_func_was_used:
                 # It may return None if it doesn't find it
                 elem = self._find_closest_iterable_element_for_index(obj, elem, expected_old_value)
                 if elem is not None:
@@ -543,33 +607,60 @@
             if dist > closest_distance:
                 break
             if value == expected_old_value and dist < closest_distance:
                 closest_elem = index
                 closest_distance = dist
         return closest_elem
 
-    def _do_item_removedOLD(self, items):
-        """
-        Handle removing items.
-        """
-        # Sorting the iterable_item_removed in reverse order based on the paths.
-        # So that we delete a bigger index before a smaller index
-        for path, expected_old_value in sorted(items.items(), key=self._sort_key_for_item_added, reverse=True):
-            elem_and_details = self._get_elements_and_details(path)
-            if elem_and_details:
-                elements, parent, parent_to_obj_elem, parent_to_obj_action, obj, elem, action = elem_and_details
-            else:
-                continue  # pragma: no cover. Due to cPython peephole optimizer, this line doesn't get covered. https://github.com/nedbat/coveragepy/issues/198
-            current_old_value = self._get_elem_and_compare_to_old_value(
-                obj=obj, elem=elem, path_for_err_reporting=path, expected_old_value=expected_old_value, action=action)
-            if current_old_value is not_found:
-                continue
-            self._del_elem(parent, parent_to_obj_elem, parent_to_obj_action,
-                           obj, elements, path, elem, action)
-            self._do_verify_changes(path, expected_old_value, current_old_value)
+    def _do_iterable_opcodes(self):
+        _iterable_opcodes = self.diff.get('_iterable_opcodes', {})
+        if _iterable_opcodes:
+            for path, opcodes in _iterable_opcodes.items():
+                transformed = []
+                # elements = _path_to_elements(path)
+                elem_and_details = self._get_elements_and_details(path)
+                if elem_and_details:
+                    elements, parent, parent_to_obj_elem, parent_to_obj_action, obj, elem, action = elem_and_details
+                    if parent is None:
+                        parent = self
+                        obj = self.root
+                        parent_to_obj_elem = 'root'
+                        parent_to_obj_action = GETATTR
+                else:
+                    continue  # pragma: no cover. Due to cPython peephole optimizer, this line doesn't get covered. https://github.com/nedbat/coveragepy/issues/198
+                # import pytest; pytest.set_trace()
+                obj = self.get_nested_obj(obj=self, elements=elements)
+                is_obj_tuple = isinstance(obj, tuple)
+                for opcode in opcodes:    
+                    if opcode.tag == 'replace':
+                        # Replace items in list a[i1:i2] with b[j1:j2]
+                        transformed.extend(opcode.new_values)
+                    elif opcode.tag == 'delete':
+                        # Delete items from list a[i1:i2], so we do nothing here
+                        continue
+                    elif opcode.tag == 'insert':
+                        # Insert items from list b[j1:j2] into the new list
+                        transformed.extend(opcode.new_values)
+                    elif opcode.tag == 'equal':
+                        # Items are the same in both lists, so we add them to the result
+                        transformed.extend(obj[opcode.t1_from_index:opcode.t1_to_index])
+                if is_obj_tuple:
+                    obj = tuple(obj)
+                    # Making sure that the object is re-instated inside the parent especially if it was immutable
+                    # and we had to turn it into a mutable one. In such cases the object has a new id.
+                    self._simple_set_elem_value(obj=parent, path_for_err_reporting=path, elem=parent_to_obj_elem,
+                                                value=obj, action=parent_to_obj_action)
+                else:
+                    obj[:] = transformed
+
+
+
+                # obj = self.get_nested_obj(obj=self, elements=elements)
+                # for
+
 
     def _do_iterable_item_removed(self):
         iterable_item_removed = self.diff.get('iterable_item_removed', {})
 
         iterable_item_moved = self.diff.get('iterable_item_moved')
         if iterable_item_moved:
             # These will get added back during items_added
@@ -717,34 +808,53 @@
         for action, info in self.diff.items():
             reverse_action = SIMPLE_ACTION_TO_REVERSE.get(action)
             if reverse_action:
                 r_diff[reverse_action] = info
             elif action == 'values_changed':
                 r_diff[action] = {}
                 for path, path_info in info.items():
-                    r_diff[action][path] = {
+                    reverse_path = path_info['new_path'] if path_info.get('new_path') else path
+                    r_diff[action][reverse_path] = {
                         'new_value': path_info['old_value'], 'old_value': path_info['new_value']
                     } 
             elif action == 'type_changes':
                 r_diff[action] = {}
                 for path, path_info in info.items():
-                    r_diff[action][path] = {
+                    reverse_path = path_info['new_path'] if path_info.get('new_path') else path
+                    r_diff[action][reverse_path] = {
                         'old_type': path_info['new_type'], 'new_type': path_info['old_type'],
                     }
                     if 'new_value' in path_info:
-                        r_diff[action][path]['old_value'] = path_info['new_value']
+                        r_diff[action][reverse_path]['old_value'] = path_info['new_value']
                     if 'old_value' in path_info:
-                        r_diff[action][path]['new_value'] = path_info['old_value']
+                        r_diff[action][reverse_path]['new_value'] = path_info['old_value']
             elif action == 'iterable_item_moved':
                 r_diff[action] = {}
                 for path, path_info in info.items():
                     old_path = path_info['new_path']
                     r_diff[action][old_path] = {
                         'new_path': path, 'value': path_info['value'],
                     }
+            elif action == '_iterable_opcodes':
+                r_diff[action] = {}
+                for path, op_codes in info.items():
+                    r_diff[action][path] = []
+                    for op_code in op_codes:
+                        tag = op_code.tag
+                        tag = {'delete': 'insert', 'insert': 'delete'}.get(tag, tag)
+                        new_op_code = Opcode(
+                            tag=tag,
+                            t1_from_index=op_code.t2_from_index,
+                            t1_to_index=op_code.t2_to_index,
+                            t2_from_index=op_code.t1_from_index,
+                            t2_to_index=op_code.t1_to_index,
+                            new_values=op_code.old_values,
+                            old_values=op_code.new_values,
+                        )
+                        r_diff[action][path].append(new_op_code)
         return r_diff
 
     def dump(self, file):
         """
         Dump into file object
         """
         # Small optimization: Our internal pickle serializer can just take a file object
@@ -773,15 +883,20 @@
             row = {'path': _parse_path(path), 'action': action}
             for key, new_key, func in keys_and_funcs:
                 if key in details:
                     if func:
                         row[new_key] = func(details[key])
                     else:
                         row[new_key] = details[key]
-            yield row
+            yield FlatDeltaRow(**row)
+
+    @staticmethod
+    def _from_flat_rows(flat_rows_list: List[FlatDeltaRow]):
+        flat_dict_list = (i._asdict() for i in flat_rows_list)
+        return Delta._from_flat_dicts(flat_dict_list)
 
     @staticmethod
     def _from_flat_dicts(flat_dict_list):
         """
         Create the delta's diff object from the flat_dict_list
         """
         result = {}
@@ -790,27 +905,32 @@
             'unordered_iterable_item_removed': 'iterable_items_removed_at_indexes',
         }
         for flat_dict in flat_dict_list:
             index = None
             action = flat_dict.get("action")
             path = flat_dict.get("path")
             value = flat_dict.get('value')
-            old_value = flat_dict.get('old_value', _ObjDoesNotExist)
+            new_path = flat_dict.get('new_path')
+            old_value = flat_dict.get('old_value', UnkownValueCode)
             if not action:
                 raise ValueError("Flat dict need to include the 'action'.")
             if path is None:
                 raise ValueError("Flat dict need to include the 'path'.")
             if action in FLATTENING_NEW_ACTION_MAP:
                 action = FLATTENING_NEW_ACTION_MAP[action]
                 index = path.pop()
             if action in {'attribute_added', 'attribute_removed'}:
                 root_element = ('root', GETATTR)
             else:
                 root_element = ('root', GET)
             path_str = stringify_path(path, root_element=root_element)  # We need the string path
+            if new_path and new_path != path:
+                new_path = stringify_path(new_path, root_element=root_element)
+            else:
+                new_path = None
             if action not in result:
                 result[action] = {}
             if action in {'iterable_items_added_at_indexes', 'iterable_items_removed_at_indexes'}:
                 if path_str not in result[action]:
                     result[action][path_str] = {}
                 result[action][path_str][index] = value
             elif action in {'set_item_added', 'set_item_removed'}:
@@ -819,42 +939,38 @@
                 result[action][path_str].add(value)
             elif action in {
                 'dictionary_item_added', 'dictionary_item_removed',
                 'attribute_removed', 'attribute_added', 'iterable_item_added', 'iterable_item_removed',
             }:
                 result[action][path_str] = value
             elif action == 'values_changed':
-                if old_value is _ObjDoesNotExist:
+                if old_value == UnkownValueCode:
                     result[action][path_str] = {'new_value': value}
                 else:
                     result[action][path_str] = {'new_value': value, 'old_value': old_value}
             elif action == 'type_changes':
-                type_ = flat_dict.get('type', _ObjDoesNotExist)
-                old_type = flat_dict.get('old_type', _ObjDoesNotExist)
+                type_ = flat_dict.get('type', UnkownValueCode)
+                old_type = flat_dict.get('old_type', UnkownValueCode)
 
                 result[action][path_str] = {'new_value': value}
                 for elem, elem_value in [
                     ('new_type', type_),
                     ('old_type', old_type),
                     ('old_value', old_value),
                 ]:
-                    if elem_value is not _ObjDoesNotExist:
+                    if elem_value != UnkownValueCode:
                         result[action][path_str][elem] = elem_value
             elif action == 'iterable_item_moved':
-                result[action][path_str] = {
-                    'new_path': stringify_path(
-                        flat_dict.get('new_path', ''),
-                        root_element=('root', GET)
-                    ),
-                    'value': value,
-                }
+                result[action][path_str] = {'value': value}
+            if new_path:
+                result[action][path_str]['new_path'] = new_path
 
         return result
 
-    def to_flat_dicts(self, include_action_in_path=False, report_type_changes=True):
+    def to_flat_dicts(self, include_action_in_path=False, report_type_changes=True) -> List[FlatDeltaRow]:
         """
         Returns a flat list of actions that is easily machine readable.
 
         For example:
             {'iterable_item_added': {'root[3]': 5, 'root[2]': 3}}
 
         Becomes:
@@ -900,14 +1016,22 @@
             set_item_added
             set_item_removed
             dictionary_item_added
             dictionary_item_removed
             attribute_added
             attribute_removed
         """
+        return [
+            i._asdict() for i in self.to_flat_rows(include_action_in_path=False, report_type_changes=True)
+        ]
+
+    def to_flat_rows(self, include_action_in_path=False, report_type_changes=True) -> List[FlatDeltaRow]:
+        """
+        Just like to_flat_dicts but returns FlatDeltaRow Named Tuples
+        """
         result = []
         if include_action_in_path:
             _parse_path = partial(parse_path, include_actions=True)
         else:
             _parse_path = parse_path
         if report_type_changes:
             keys_and_funcs = [
@@ -944,61 +1068,55 @@
                     path = _parse_path(path)
                     for index, value in index_to_value.items():
                         path2 = path.copy()
                         if include_action_in_path:
                             path2.append((index, 'GET'))
                         else:
                             path2.append(index)
-                        result.append(
-                            {'path': path2, 'value': value, 'action': new_action}
-                        )
+                        result.append(FlatDeltaRow(path=path2, value=value, action=new_action))
             elif action in {'set_item_added', 'set_item_removed'}:
                 for path, values in info.items():
                     path = _parse_path(path)
                     for value in values:
-                        result.append(
-                            {'path': path, 'value': value, 'action': action}
-                        )
+                        result.append(FlatDeltaRow(path=path, value=value, action=action))
             elif action == 'dictionary_item_added':
                 for path, value in info.items():
                     path = _parse_path(path)
                     if isinstance(value, dict) and len(value) == 1:
                         new_key = next(iter(value))
                         path.append(new_key)
                         value = value[new_key]
                     elif isinstance(value, (list, tuple)) and len(value) == 1:
                         value = value[0]
                         path.append(0)
                         action = 'iterable_item_added'
                     elif isinstance(value, set) and len(value) == 1:
                         value = value.pop()
                         action = 'set_item_added'
-                    result.append(
-                        {'path': path, 'value': value, 'action': action}
-                    )
+                    result.append(FlatDeltaRow(path=path, value=value, action=action))
             elif action in {
                 'dictionary_item_removed', 'iterable_item_added',
                 'iterable_item_removed', 'attribute_removed', 'attribute_added'
             }:
                 for path, value in info.items():
                     path = _parse_path(path)
-                    result.append(
-                        {'path': path, 'value': value, 'action': action}
-                    )
+                    result.append(FlatDeltaRow(path=path, value=value, action=action))
             elif action == 'type_changes':
                 if not report_type_changes:
                     action = 'values_changed'
 
                 for row in self._get_flat_row(
                     action=action,
                     info=info,
                     _parse_path=_parse_path,
                     keys_and_funcs=keys_and_funcs,
                 ):
                     result.append(row)
+            elif action == '_iterable_opcodes':
+                result.extend(self._flatten_iterable_opcodes())
             else:
                 for row in self._get_flat_row(
                     action=action,
                     info=info,
                     _parse_path=_parse_path,
                     keys_and_funcs=keys_and_funcs,
                 ):
```

### Comparing `deepdiff-6.7.1/deepdiff/diff.py` & `deepdiff-7.0.0/deepdiff/diff.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,36 +7,39 @@
 # However the docstring expects it in a specific order in order to pass!
 import difflib
 import logging
 import types
 from enum import Enum
 from copy import deepcopy
 from math import isclose as is_close
+from typing import List, Dict, IO, Callable, Set, Union, Any, Pattern, Tuple, Optional
 from collections.abc import Mapping, Iterable, Sequence
 from collections import defaultdict
 from inspect import getmembers
 from itertools import zip_longest
 from ordered_set import OrderedSet
 from deepdiff.helper import (strings, bytes_type, numbers, uuids, datetimes, ListItemRemovedOrAdded, notpresent,
                              IndexedHash, unprocessed, add_to_frozen_set, basic_types,
                              convert_item_or_items_into_set_else_none, get_type,
                              convert_item_or_items_into_compiled_regexes_else_none,
                              type_is_subclass_of_type_group, type_in_type_group, get_doc,
                              number_to_string, datetime_normalize, KEY_TO_VAL_STR, booleans,
                              np_ndarray, np_floating, get_numpy_ndarray_rows, OrderedSetPlus, RepeatedTimer,
                              TEXT_VIEW, TREE_VIEW, DELTA_VIEW, detailed__dict__, add_root_to_paths,
                              np, get_truncate_datetime, dict_, CannotCompare, ENUM_INCLUDE_KEYS,
-                             PydanticBaseModel, )
+                             PydanticBaseModel, Opcode,)
 from deepdiff.serialization import SerializationMixin
 from deepdiff.distance import DistanceMixin
 from deepdiff.model import (
     RemapDict, ResultDict, TextResult, TreeResult, DiffLevel,
     DictRelationship, AttributeRelationship, REPORT_KEYS,
     SubscriptableIterableRelationship, NonSubscriptableIterableRelationship,
-    SetRelationship, NumpyArrayRelationship, CUSTOM_FIELD, PrettyOrderedSet, )
+    SetRelationship, NumpyArrayRelationship, CUSTOM_FIELD, PrettyOrderedSet,
+    FORCE_DEFAULT,
+)
 from deepdiff.deephash import DeepHash, combine_hashes_lists
 from deepdiff.base import Base
 from deepdiff.lfucache import LFUCache, DummyLFU
 
 logger = logging.getLogger(__name__)
 
 MAX_PASSES_REACHED_MSG = (
@@ -107,60 +110,60 @@
 
 class DeepDiff(ResultDict, SerializationMixin, DistanceMixin, Base):
     __doc__ = doc
 
     CACHE_AUTO_ADJUST_THRESHOLD = 0.25
 
     def __init__(self,
-                 t1,
-                 t2,
-                 cache_purge_level=1,
-                 cache_size=0,
-                 cache_tuning_sample_size=0,
-                 custom_operators=None,
-                 cutoff_distance_for_pairs=CUTOFF_DISTANCE_FOR_PAIRS_DEFAULT,
-                 cutoff_intersection_for_pairs=CUTOFF_INTERSECTION_FOR_PAIRS_DEFAULT,
-                 encodings=None,
-                 exclude_obj_callback=None,
-                 exclude_obj_callback_strict=None,
-                 exclude_paths=None,
-                 include_obj_callback=None,
-                 include_obj_callback_strict=None,
-                 include_paths=None,
-                 exclude_regex_paths=None,
-                 exclude_types=None,
-                 get_deep_distance=False,
-                 group_by=None,
-                 group_by_sort_key=None,
-                 hasher=None,
-                 hashes=None,
-                 ignore_encoding_errors=False,
-                 ignore_nan_inequality=False,
-                 ignore_numeric_type_changes=False,
-                 ignore_order=False,
-                 ignore_order_func=None,
-                 ignore_private_variables=True,
-                 ignore_string_case=False,
-                 ignore_string_type_changes=False,
-                 ignore_type_in_groups=None,
-                 ignore_type_subclasses=False,
-                 iterable_compare_func=None,
-                 zip_ordered_iterables=False,
-                 log_frequency_in_sec=0,
-                 math_epsilon=None,
-                 max_diffs=None,
-                 max_passes=10000000,
-                 number_format_notation="f",
-                 number_to_string_func=None,
-                 progress_logger=logger.info,
-                 report_repetition=False,
-                 significant_digits=None,
-                 truncate_datetime=None,
-                 verbose_level=1,
-                 view=TEXT_VIEW,
+                 t1: Any,
+                 t2: Any,
+                 cache_purge_level: int=1,
+                 cache_size: int=0,
+                 cache_tuning_sample_size: int=0,
+                 custom_operators: Optional[List[Any]] =None,
+                 cutoff_distance_for_pairs: float=CUTOFF_DISTANCE_FOR_PAIRS_DEFAULT,
+                 cutoff_intersection_for_pairs: float=CUTOFF_INTERSECTION_FOR_PAIRS_DEFAULT,
+                 encodings: Optional[List[str]]=None,
+                 exclude_obj_callback: Optional[Callable]=None,
+                 exclude_obj_callback_strict: Optional[Callable]=None,
+                 exclude_paths: Union[str, List[str]]=None,
+                 include_obj_callback: Optional[Callable]=None,
+                 include_obj_callback_strict: Optional[Callable]=None,
+                 include_paths: Union[str, List[str]]=None,
+                 exclude_regex_paths: Union[str, List[str], Pattern[str], List[Pattern[str]], None]=None,
+                 exclude_types: Optional[List[Any]]=None,
+                 get_deep_distance: bool=False,
+                 group_by: Union[str, Tuple[str, str], None]=None,
+                 group_by_sort_key: Union[str, Callable, None]=None,
+                 hasher: Optional[Callable]=None,
+                 hashes: Optional[Dict]=None,
+                 ignore_encoding_errors: bool=False,
+                 ignore_nan_inequality: bool=False,
+                 ignore_numeric_type_changes: bool=False,
+                 ignore_order: bool=False,
+                 ignore_order_func: Optional[Callable]=None,
+                 ignore_private_variables: bool=True,
+                 ignore_string_case: bool=False,
+                 ignore_string_type_changes: bool=False,
+                 ignore_type_in_groups: Optional[List[Tuple]]=None,
+                 ignore_type_subclasses: bool=False,
+                 iterable_compare_func: Optional[Callable]=None,
+                 zip_ordered_iterables: bool=False,
+                 log_frequency_in_sec: int=0,
+                 math_epsilon: Optional[float]=None,
+                 max_diffs: Optional[int]=None,
+                 max_passes: int=10000000,
+                 number_format_notation: str="f",
+                 number_to_string_func: Optional[Callable]=None,
+                 progress_logger: Callable=logger.info,
+                 report_repetition: bool=False,
+                 significant_digits: Optional[int]=None,
+                 truncate_datetime: Optional[str]=None,
+                 verbose_level: int=1,
+                 view: str=TEXT_VIEW,
                  _original_type=None,
                  _parameters=None,
                  _shared_parameters=None,
                  **kwargs):
         super().__init__()
         if kwargs:
             raise ValueError((
@@ -199,15 +202,15 @@
             self.report_repetition = report_repetition
             self.exclude_paths = add_root_to_paths(convert_item_or_items_into_set_else_none(exclude_paths))
             self.include_paths = add_root_to_paths(convert_item_or_items_into_set_else_none(include_paths))
             self.exclude_regex_paths = convert_item_or_items_into_compiled_regexes_else_none(exclude_regex_paths)
             self.exclude_types = set(exclude_types) if exclude_types else None
             self.exclude_types_tuple = tuple(exclude_types) if exclude_types else None  # we need tuple for checking isinstance
             self.ignore_type_subclasses = ignore_type_subclasses
-            self.type_check_func = type_is_subclass_of_type_group if ignore_type_subclasses else type_in_type_group
+            self.type_check_func = type_in_type_group if ignore_type_subclasses else type_is_subclass_of_type_group
             self.ignore_string_case = ignore_string_case
             self.exclude_obj_callback = exclude_obj_callback
             self.exclude_obj_callback_strict = exclude_obj_callback_strict
             self.include_obj_callback = include_obj_callback
             self.include_obj_callback_strict = include_obj_callback_strict
             self.number_to_string = number_to_string_func or number_to_string
             self.iterable_compare_func = iterable_compare_func
@@ -293,14 +296,15 @@
                 progress_timer = RepeatedTimer(log_frequency_in_sec, _report_progress, self._stats, progress_logger)
             else:
                 progress_timer = None
 
         self._parameters = _parameters
         self.deephash_parameters = self._get_deephash_params()
         self.tree = TreeResult()
+        self._iterable_opcodes = {}
         if group_by and self.is_root:
             try:
                 original_t1 = t1
                 t1 = self._group_iterable_to_dict(t1, group_by, item_name='t1')
             except (KeyError, ValueError):
                 pass
             else:
@@ -344,31 +348,31 @@
 
     def _get_deephash_params(self):
         result = {key: self._parameters[key] for key in DEEPHASH_PARAM_KEYS}
         result['ignore_repetition'] = not self.report_repetition
         result['number_to_string_func'] = self.number_to_string
         return result
 
-    def _report_result(self, report_type, level, local_tree=None):
+    def _report_result(self, report_type, change_level, local_tree=None):
         """
         Add a detected change to the reference-style result dictionary.
         report_type will be added to level.
         (We'll create the text-style report from there later.)
         :param report_type: A well defined string key describing the type of change.
                             Examples: "set_item_added", "values_changed"
-        :param parent: A DiffLevel object describing the objects in question in their
+        :param change_level: A DiffLevel object describing the objects in question in their
                        before-change and after-change object structure.
 
-        :rtype: None
+        :local_tree: None
         """
 
-        if not self._skip_this(level):
-            level.report_type = report_type
+        if not self._skip_this(change_level):
+            change_level.report_type = report_type
             tree = self.tree if local_tree is None else local_tree
-            tree[report_type].add(level)
+            tree[report_type].add(change_level)
 
     def custom_report_result(self, report_type, level, extra_info=None):
         """
         Add a detected change to the reference-style result dictionary.
         report_type will be added to level.
         (We'll create the text-style report from there later.)
         :param report_type: A well defined string key describing the type of change.
@@ -512,14 +516,16 @@
             elif isinstance(key, numbers):
                 type_ = "number" if self.ignore_numeric_type_changes else key.__class__.__name__
                 clean_key = self.number_to_string(key, significant_digits=self.significant_digits,
                                                   number_format_notation=self.number_format_notation)
                 clean_key = KEY_TO_VAL_STR.format(type_, clean_key)
             else:
                 clean_key = key
+            if self.ignore_string_case:
+                clean_key = clean_key.lower()
             if clean_key in result:
                 logger.warning(('{} and {} in {} become the same key when ignore_numeric_type_changes'
                                 'or ignore_numeric_type_changes are set to be true.').format(
                                     key, result[clean_key], level.path()))
             else:
                 result[clean_key] = key
         return result
@@ -555,15 +561,15 @@
 
         if self.ignore_private_variables:
             t1_keys = OrderedSet([key for key in t1 if not(isinstance(key, str) and key.startswith('__'))])
             t2_keys = OrderedSet([key for key in t2 if not(isinstance(key, str) and key.startswith('__'))])
         else:
             t1_keys = OrderedSet(t1.keys())
             t2_keys = OrderedSet(t2.keys())
-        if self.ignore_string_type_changes or self.ignore_numeric_type_changes:
+        if self.ignore_string_type_changes or self.ignore_numeric_type_changes or self.ignore_string_case:
             t1_clean_to_keys = self._get_clean_to_keys_mapping(keys=t1_keys, level=level)
             t2_clean_to_keys = self._get_clean_to_keys_mapping(keys=t2_keys, level=level)
             t1_keys = OrderedSet(t1_clean_to_keys.keys())
             t2_keys = OrderedSet(t2_clean_to_keys.keys())
         else:
             t1_clean_to_keys = t2_clean_to_keys = None
 
@@ -577,27 +583,31 @@
                 return
 
             key = t2_clean_to_keys[key] if t2_clean_to_keys else key
             change_level = level.branch_deeper(
                 notpresent,
                 t2[key],
                 child_relationship_class=rel_class,
-                child_relationship_param=key)
+                child_relationship_param=key,
+                child_relationship_param2=key,
+            )
             self._report_result(item_added_key, change_level, local_tree=local_tree)
 
         for key in t_keys_removed:
             if self._count_diff() is StopIteration:
                 return  # pragma: no cover. This is already covered for addition.
 
             key = t1_clean_to_keys[key] if t1_clean_to_keys else key
             change_level = level.branch_deeper(
                 t1[key],
                 notpresent,
                 child_relationship_class=rel_class,
-                child_relationship_param=key)
+                child_relationship_param=key,
+                child_relationship_param2=key,
+            )
             self._report_result(item_removed_key, change_level, local_tree=local_tree)
 
         for key in t_keys_intersect:  # key present in both dicts - need to compare values
             if self._count_diff() is StopIteration:
                 return  # pragma: no cover. This is already covered for addition.
 
             key1 = t1_clean_to_keys[key] if t1_clean_to_keys else key
@@ -608,15 +618,17 @@
             parents_ids_added = add_to_frozen_set(parents_ids, item_id)
 
             # Go one level deeper
             next_level = level.branch_deeper(
                 t1[key1],
                 t2[key2],
                 child_relationship_class=rel_class,
-                child_relationship_param=key)
+                child_relationship_param=key,
+                child_relationship_param2=key,
+                )
             self._diff(next_level, parents_ids_added, local_tree=local_tree)
 
     def _diff_set(self, level, local_tree=None):
         """Difference of sets"""
         t1_hashtable = self._create_hashtable(level, 't1')
         t2_hashtable = self._create_hashtable(level, 't2')
 
@@ -762,15 +774,15 @@
             and isinstance(level.t1, Sequence)
             and isinstance(level.t2, Sequence)
             and self._all_values_basic_hashable(level.t1)
             and self._all_values_basic_hashable(level.t2)
             and self.iterable_compare_func is None
         ):
             local_tree_pass = TreeResult()
-            self._diff_ordered_iterable_by_difflib(
+            opcodes_with_values = self._diff_ordered_iterable_by_difflib(
                 level,
                 parents_ids=parents_ids,
                 _original_type=_original_type,
                 child_relationship_class=child_relationship_class,
                 local_tree=local_tree_pass,
             )
             # Sometimes DeepDiff's old iterable diff does a better job than DeepDiff
@@ -781,14 +793,16 @@
                     parents_ids=parents_ids,
                     _original_type=_original_type,
                     child_relationship_class=child_relationship_class,
                     local_tree=local_tree_pass2,
                 )
                 if len(local_tree_pass) >= len(local_tree_pass2):
                     local_tree_pass = local_tree_pass2
+                else:
+                    self._iterable_opcodes[level.path(force=FORCE_DEFAULT)] = opcodes_with_values
             for report_type, levels in local_tree_pass.items():
                 if levels:
                     self.tree[report_type] |= levels
         else:
             self._diff_by_forming_pairs_and_comparing_one_by_one(
                 level,
                 parents_ids=parents_ids,
@@ -827,23 +841,27 @@
                 return  # pragma: no cover. This is already covered for addition.
 
             if y is ListItemRemovedOrAdded:  # item removed completely
                 change_level = level.branch_deeper(
                     x,
                     notpresent,
                     child_relationship_class=child_relationship_class,
-                    child_relationship_param=i)
+                    child_relationship_param=i,
+                    child_relationship_param2=j,
+                    )
                 self._report_result('iterable_item_removed', change_level, local_tree=local_tree)
 
             elif x is ListItemRemovedOrAdded:  # new item added
                 change_level = level.branch_deeper(
                     notpresent,
                     y,
                     child_relationship_class=child_relationship_class,
-                    child_relationship_param=j)
+                    child_relationship_param=i,
+                    child_relationship_param2=j,
+                    )
                 self._report_result('iterable_item_added', change_level, local_tree=local_tree)
 
             else:  # check if item value has changed
 
                 # if (i != j):
                 #     # Item moved
                 #     change_level = level.branch_deeper(
@@ -886,53 +904,71 @@
                 parents_ids_added = add_to_frozen_set(parents_ids, item_id)
 
                 # Go one level deeper
                 next_level = level.branch_deeper(
                     x,
                     y,
                     child_relationship_class=child_relationship_class,
-                    child_relationship_param=j
+                    child_relationship_param=i,
+                    child_relationship_param2=j,
                 )
                 self._diff(next_level, parents_ids_added, local_tree=local_tree)
 
     def _diff_ordered_iterable_by_difflib(
         self, level, local_tree, parents_ids=frozenset(), _original_type=None, child_relationship_class=None,
     ):
 
         seq = difflib.SequenceMatcher(isjunk=None, a=level.t1, b=level.t2, autojunk=False)
 
-        opcode = seq.get_opcodes()
-        for tag, t1_from_index, t1_to_index, t2_from_index, t2_to_index in opcode:
+        opcodes = seq.get_opcodes()
+        opcodes_with_values = []
+        for tag, t1_from_index, t1_to_index, t2_from_index, t2_to_index in opcodes:
             if tag == 'equal':
+                opcodes_with_values.append(Opcode(
+                    tag, t1_from_index, t1_to_index, t2_from_index, t2_to_index,
+                ))
                 continue
             # print('{:7}   t1[{}:{}] --> t2[{}:{}] {!r:>8} --> {!r}'.format(
             #     tag, t1_from_index, t1_to_index, t2_from_index, t2_to_index, level.t1[t1_from_index:t1_to_index], level.t2[t2_from_index:t2_to_index]))
+
+            opcodes_with_values.append(Opcode(
+                tag, t1_from_index, t1_to_index, t2_from_index, t2_to_index,
+                old_values = level.t1[t1_from_index: t1_to_index],
+                new_values = level.t2[t2_from_index: t2_to_index],
+            ))
+
             if tag == 'replace':
                 self._diff_by_forming_pairs_and_comparing_one_by_one(
                     level, local_tree=local_tree, parents_ids=parents_ids,
                     _original_type=_original_type, child_relationship_class=child_relationship_class,
                     t1_from_index=t1_from_index, t1_to_index=t1_to_index,
                     t2_from_index=t2_from_index, t2_to_index=t2_to_index,
                 )
             elif tag == 'delete':
                 for index, x in enumerate(level.t1[t1_from_index:t1_to_index]):
                     change_level = level.branch_deeper(
                         x,
                         notpresent,
                         child_relationship_class=child_relationship_class,
-                        child_relationship_param=index + t1_from_index)
+                        child_relationship_param=index + t1_from_index,
+                        child_relationship_param2=index + t1_from_index,
+                    )
                     self._report_result('iterable_item_removed', change_level, local_tree=local_tree)
             elif tag == 'insert':
                 for index, y in enumerate(level.t2[t2_from_index:t2_to_index]):
                     change_level = level.branch_deeper(
                         notpresent,
                         y,
                         child_relationship_class=child_relationship_class,
-                        child_relationship_param=index + t2_from_index)
+                        child_relationship_param=index + t2_from_index,
+                        child_relationship_param2=index + t2_from_index,
+                    )
                     self._report_result('iterable_item_added', change_level, local_tree=local_tree)
+        return opcodes_with_values
+
 
     def _diff_str(self, level, local_tree=None):
         """Compare strings"""
         if self.ignore_string_case:
             level.t1 = level.t1.lower()
             level.t2 = level.t2.lower()
 
@@ -952,14 +988,20 @@
 
         if isinstance(level.t2, bytes_type):
             try:
                 t2_str = level.t2.decode('ascii')
             except UnicodeDecodeError:
                 do_diff = False
 
+        if isinstance(level.t1, Enum):
+            t1_str = level.t1.value
+
+        if isinstance(level.t2, Enum):
+            t2_str = level.t2.value
+
         if t1_str == t2_str:
             return
 
         if do_diff:
             if '\n' in t1_str or isinstance(t2_str, str) and '\n' in t2_str:
                 diff = difflib.unified_diff(
                     t1_str.splitlines(), t2_str.splitlines(), lineterm='')
@@ -1121,15 +1163,17 @@
         if hashes_added and hashes_removed and np and len(hashes_added) > 1 and len(hashes_removed) > 1:
             # pre-calculates distances ONLY for 1D arrays whether an _original_type
             # was explicitly passed or a homogeneous array is detected.
             # Numpy is needed for this optimization.
             pre_calced_distances = self._precalculate_numpy_arrays_distance(
                 hashes_added, hashes_removed, t1_hashtable, t2_hashtable, _original_type)
 
-        if hashes_added and hashes_removed and self.iterable_compare_func and len(hashes_added) > 1 and len(hashes_removed) > 1:
+        if hashes_added and hashes_removed \
+                and self.iterable_compare_func \
+                and len(hashes_added) > 0 and len(hashes_removed) > 0:
             pre_calced_distances = self._precalculate_distance_by_custom_compare_func(
                 hashes_added, hashes_removed, t1_hashtable, t2_hashtable, _original_type)
 
         for added_hash in hashes_added:
             for removed_hash in hashes_removed:
                 added_hash_obj = t2_hashtable[added_hash]
                 removed_hash_obj = t1_hashtable[removed_hash]
@@ -1242,37 +1286,54 @@
         if self.report_repetition:
             for hash_value in hashes_added:
                 if self._count_diff() is StopIteration:
                     return  # pragma: no cover. This is already covered for addition (when report_repetition=False).
                 other = get_other_pair(hash_value)
                 item_id = id(other.item)
                 indexes = t2_hashtable[hash_value].indexes if other.item is notpresent else other.indexes
+                # When we report repetitions, we want the child_relationship_param2 only if there is no repetition.
+                # Because when there is a repetition, we report it in a different way (iterable_items_added_at_indexes for example).
+                # When there is no repetition, we want child_relationship_param2 so that we report the "new_path" correctly.
+                if len(t2_hashtable[hash_value].indexes) == 1:
+                    index2 = t2_hashtable[hash_value].indexes[0]
+                else:
+                    index2 = None
                 for i in indexes:
                     change_level = level.branch_deeper(
                         other.item,
                         t2_hashtable[hash_value].item,
                         child_relationship_class=SubscriptableIterableRelationship,
-                        child_relationship_param=i
+                        child_relationship_param=i,
+                        child_relationship_param2=index2,
                     )
                     if other.item is notpresent:
                         self._report_result('iterable_item_added', change_level, local_tree=local_tree)
                     else:
                         parents_ids_added = add_to_frozen_set(parents_ids, item_id)
                         self._diff(change_level, parents_ids_added, local_tree=local_tree)
             for hash_value in hashes_removed:
                 if self._count_diff() is StopIteration:
                     return  # pragma: no cover. This is already covered for addition.
                 other = get_other_pair(hash_value, in_t1=False)
                 item_id = id(other.item)
+                # When we report repetitions, we want the child_relationship_param2 only if there is no repetition.
+                # Because when there is a repetition, we report it in a different way (iterable_items_added_at_indexes for example).
+                # When there is no repetition, we want child_relationship_param2 so that we report the "new_path" correctly.
+                if other.item is notpresent or len(other.indexes > 1):
+                    index2 = None
+                else:
+                    index2 = other.indexes[0]
                 for i in t1_hashtable[hash_value].indexes:
                     change_level = level.branch_deeper(
                         t1_hashtable[hash_value].item,
                         other.item,
                         child_relationship_class=SubscriptableIterableRelationship,
-                        child_relationship_param=i)
+                        child_relationship_param=i,
+                        child_relationship_param2=index2,
+                    )
                     if other.item is notpresent:
                         self._report_result('iterable_item_removed', change_level, local_tree=local_tree)
                     else:
                         # I was not able to make a test case for the following 2 lines since the cases end up
                         # getting resolved above in the hashes_added calcs. However I am leaving these 2 lines
                         # in case things change in future.
                         parents_ids_added = add_to_frozen_set(parents_ids, item_id)  # pragma: no cover.
@@ -1304,36 +1365,42 @@
         else:
             for hash_value in hashes_added:
                 if self._count_diff() is StopIteration:
                     return
                 other = get_other_pair(hash_value)
                 item_id = id(other.item)
                 index = t2_hashtable[hash_value].indexes[0] if other.item is notpresent else other.indexes[0]
+                index2 = t2_hashtable[hash_value].indexes[0]
                 change_level = level.branch_deeper(
                     other.item,
                     t2_hashtable[hash_value].item,
                     child_relationship_class=SubscriptableIterableRelationship,
-                    child_relationship_param=index)
+                    child_relationship_param=index,
+                    child_relationship_param2=index2,
+                )
                 if other.item is notpresent:
                     self._report_result('iterable_item_added', change_level, local_tree=local_tree)
                 else:
                     parents_ids_added = add_to_frozen_set(parents_ids, item_id)
                     self._diff(change_level, parents_ids_added, local_tree=local_tree)
 
             for hash_value in hashes_removed:
                 if self._count_diff() is StopIteration:
                     return  # pragma: no cover. This is already covered for addition.
                 other = get_other_pair(hash_value, in_t1=False)
                 item_id = id(other.item)
+                index = t1_hashtable[hash_value].indexes[0]
+                index2 = t1_hashtable[hash_value].indexes[0] if other.item is notpresent else other.indexes[0]
                 change_level = level.branch_deeper(
                     t1_hashtable[hash_value].item,
                     other.item,
                     child_relationship_class=SubscriptableIterableRelationship,
-                    child_relationship_param=t1_hashtable[hash_value].indexes[
-                        0])
+                    child_relationship_param=index,
+                    child_relationship_param2=index2,
+                )
                 if other.item is notpresent:
                     self._report_result('iterable_item_removed', change_level, local_tree=local_tree)
                 else:
                     # Just like the case when report_repetition = True, these lines never run currently.
                     # However they will stay here in case things change in future.
                     parents_ids_added = add_to_frozen_set(parents_ids, item_id)  # pragma: no cover.
                     self._diff(change_level, parents_ids_added, local_tree=local_tree)  # pragma: no cover.
@@ -1354,15 +1421,15 @@
             if not is_close(level.t1, level.t2, abs_tol=self.math_epsilon):
                 self._report_result('values_changed', level, local_tree=local_tree)
         elif self.significant_digits is None:
             if level.t1 != level.t2:
                 self._report_result('values_changed', level, local_tree=local_tree)
         else:
             # Bernhard10: I use string formatting for comparison, to be consistent with usecases where
-            # data is read from files that were previousely written from python and
+            # data is read from files that were previously written from python and
             # to be consistent with on-screen representation of numbers.
             # Other options would be abs(t1-t2)<10**-self.significant_digits
             # or math.is_close (python3.5+)
             # Note that abs(3.25-3.251) = 0.0009999999999998899 < 0.001
             # Note also that "{:.3f}".format(1.1135) = 1.113, but "{:.3f}".format(1.11351) = 1.114
             # For Decimals, format seems to round 2.5 to 2 and 3.5 to 4 (to closest even number)
             t1_s = self.number_to_string(level.t1,
@@ -1404,17 +1471,20 @@
             # fast checks
             if self.significant_digits is None:
                 if np.array_equal(level.t1, level.t2, equal_nan=self.ignore_nan_inequality):
                     return  # all good
             else:
                 try:
                     np.testing.assert_almost_equal(level.t1, level.t2, decimal=self.significant_digits)
-                    return  # all good
+                except TypeError:
+                    np.array_equal(level.t1, level.t2, equal_nan=self.ignore_nan_inequality)
                 except AssertionError:
                     pass    # do detailed checking below
+                else:
+                    return  # all good
 
         # compare array meta-data
         _original_type = level.t1.dtype
         if level.t1.shape != level.t2.shape:
             # arrays are converted to python lists so that certain features of DeepDiff can apply on them easier.
             # They will be converted back to Numpy at their final dimension.
             level.t1 = level.t1.tolist()
@@ -1437,15 +1507,17 @@
                         get_numpy_ndarray_rows(level.t1, shape),
                         get_numpy_ndarray_rows(level.t2, shape)):
 
                     new_level = level.branch_deeper(
                         t1_row,
                         t2_row,
                         child_relationship_class=NumpyArrayRelationship,
-                        child_relationship_param=t1_path)
+                        child_relationship_param=t1_path,
+                        child_relationship_param2=t2_path,
+                    )
 
                     self._diff_iterable_in_order(new_level, parents_ids, _original_type=_original_type, local_tree=local_tree)
 
     def _diff_types(self, level, local_tree=None):
         """Diff types"""
         level.report_type = 'type_changes'
         self._report_result('type_changes', level, local_tree=local_tree)
```

### Comparing `deepdiff-6.7.1/deepdiff/distance.py` & `deepdiff-7.0.0/deepdiff/distance.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,15 @@
                         if v_id not in used_value_ids:
                             used_value_ids.add(v_id)
                             new_indexes_to_items[k] = v
                     new_subitem[path_] = new_indexes_to_items
                 subitem = new_subitem
 
             # internal keys such as _numpy_paths should not count towards the distance
-            if isinstance(key, strings) and (key.startswith('_') or key == 'deep_distance'):
+            if isinstance(key, strings) and (key.startswith('_') or key == 'deep_distance' or key == 'new_path'):
                 continue
 
             item_id = id(subitem)
             if parents_ids and item_id in parents_ids:
                 continue
             parents_ids_added = add_to_frozen_set(parents_ids, item_id)
             length += _get_item_length(subitem, parents_ids_added)
```

### Comparing `deepdiff-6.7.1/deepdiff/helper.py` & `deepdiff-7.0.0/deepdiff/helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 import os
 import datetime
 import uuid
 import logging
 import warnings
 import string
 import time
+import enum
+from typing import NamedTuple, Any, List, Optional
 from ast import literal_eval
 from decimal import Decimal, localcontext, InvalidOperation as InvalidDecimalOperation
-from collections import namedtuple
 from itertools import repeat
 from ordered_set import OrderedSet
 from threading import Timer
 
 
 class np_type:
     pass
@@ -167,15 +168,17 @@
 uuids = (uuid.UUID, )
 times = (datetime.datetime, datetime.time)
 numbers = only_numbers + datetimes
 booleans = (bool, np_bool_)
 
 basic_types = strings + numbers + uuids + booleans + (type(None), )
 
-IndexedHash = namedtuple('IndexedHash', 'indexes item')
+class IndexedHash(NamedTuple):
+    indexes: List
+    item: Any
 
 current_dir = os.path.dirname(os.path.abspath(__file__))
 
 ID_PREFIX = '!>*id'
 
 KEY_TO_VAL_STR = "{}:{}"
 
@@ -414,14 +417,15 @@
                     number=number.imag,
                     significant_digits=significant_digits,
                     number_format_notation=number_format_notation
                 )
             )
         )
     else:
+        # import pytest; pytest.set_trace()
         number = round(number=number, ndigits=significant_digits)
 
         if significant_digits == 0:
             number = int(number)
 
     if number == 0.0:
         # Special case for 0: "-0.xx" should compare equal to "0.xx"
@@ -716,7 +720,71 @@
                         ignore_private_variables and not key.startswith('__') and not key.startswith(private_var_prefix)
                     )
             ):
                 value = getattr(obj, key)
                 if not callable(value):
                     result[key] = value
     return result
+
+
+def named_tuple_repr(self):
+    fields = []
+    for field, value in self._asdict().items():
+        # Only include fields that do not have their default value
+        if field in self._field_defaults:
+            if value != self._field_defaults[field]:
+                fields.append(f"{field}={value!r}")
+        else:
+            fields.append(f"{field}={value!r}")
+
+    return f"{self.__class__.__name__}({', '.join(fields)})"
+
+
+class Opcode(NamedTuple):
+    tag: str
+    t1_from_index: int
+    t1_to_index: int
+    t2_from_index: int
+    t2_to_index: int
+    old_values: Optional[List[Any]] = None
+    new_values: Optional[List[Any]] = None
+
+    __repr__ = __str__ = named_tuple_repr
+
+
+class FlatDataAction(str, enum.Enum):
+    values_changed = 'values_changed'
+    type_changes = 'type_changes'
+    set_item_added = 'set_item_added'
+    set_item_removed = 'set_item_removed'
+    dictionary_item_added = 'dictionary_item_added'
+    dictionary_item_removed = 'dictionary_item_removed'
+    iterable_item_added = 'iterable_item_added'
+    iterable_item_removed = 'iterable_item_removed'
+    iterable_item_moved = 'iterable_item_moved'
+    iterable_items_inserted = 'iterable_items_inserted'  # opcode
+    iterable_items_deleted = 'iterable_items_deleted'  # opcode
+    iterable_items_replaced = 'iterable_items_replaced'  # opcode
+    iterable_items_equal = 'iterable_items_equal'  # opcode
+    attribute_removed = 'attribute_removed'
+    attribute_added = 'attribute_added'
+    unordered_iterable_item_added = 'unordered_iterable_item_added'
+    unordered_iterable_item_removed = 'unordered_iterable_item_removed'
+
+
+UnkownValueCode = '*-UNKNOWN-*'
+
+
+class FlatDeltaRow(NamedTuple):
+    path: List
+    action: FlatDataAction
+    value: Optional[Any] = UnkownValueCode
+    old_value: Optional[Any] = UnkownValueCode
+    type: Optional[Any] = UnkownValueCode
+    old_type: Optional[Any] = UnkownValueCode
+    new_path: Optional[List] = None
+    t1_from_index: Optional[int] = None
+    t1_to_index: Optional[int] = None
+    t2_from_index: Optional[int] = None
+    t2_to_index: Optional[int] = None
+
+    __repr__ = __str__ = named_tuple_repr
```

### Comparing `deepdiff-6.7.1/deepdiff/lfucache.py` & `deepdiff-7.0.0/deepdiff/lfucache.py`

 * *Files identical despite different names*

### Comparing `deepdiff-6.7.1/deepdiff/model.py` & `deepdiff-7.0.0/deepdiff/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -148,17 +148,25 @@
         self._from_tree_default(tree, 'attribute_removed')
         self._from_tree_set_item_removed(tree)
         self._from_tree_set_item_added(tree)
         self._from_tree_repetition_change(tree)
         self._from_tree_deep_distance(tree)
         self._from_tree_custom_results(tree)
 
-    def _from_tree_default(self, tree, report_type):
+    def _from_tree_default(self, tree, report_type, ignore_if_in_iterable_opcodes=False):
         if report_type in tree:
+                
             for change in tree[report_type]:  # report each change
+                # When we convert from diff to delta result, we care more about opcodes than iterable_item_added or removed
+                if (
+                    ignore_if_in_iterable_opcodes
+                    and report_type in {"iterable_item_added", "iterable_item_removed"}
+                    and change.up.path(force=FORCE_DEFAULT) in self["_iterable_opcodes"]
+                ):
+                    continue
                 # determine change direction (added or removed)
                 # Report t2 (the new one) whenever possible.
                 # In cases where t2 doesn't exist (i.e. stuff removed), report t1.
                 if change.t2 is not notpresent:
                     item = change.t2
                 else:
                     item = change.t1
@@ -176,37 +184,45 @@
                     # should never happen
                     raise TypeError("Cannot handle {} report container type.".
                                     format(report))
 
     def _from_tree_type_changes(self, tree):
         if 'type_changes' in tree:
             for change in tree['type_changes']:
+                path = change.path(force=FORCE_DEFAULT)
                 if type(change.t1) is type:
                     include_values = False
                     old_type = change.t1
                     new_type = change.t2
                 else:
                     include_values = True
                     old_type = get_type(change.t1)
                     new_type = get_type(change.t2)
                 remap_dict = RemapDict({
                     'old_type': old_type,
-                    'new_type': new_type
+                    'new_type': new_type,
                 })
-                self['type_changes'][change.path(
-                    force=FORCE_DEFAULT)] = remap_dict
+                if self.verbose_level > 1:
+                    new_path = change.path(use_t2=True, force=FORCE_DEFAULT)
+                    if path != new_path:
+                        remap_dict['new_path'] = new_path
+                self['type_changes'][path] = remap_dict
                 if self.verbose_level and include_values:
                     remap_dict.update(old_value=change.t1, new_value=change.t2)
 
     def _from_tree_value_changed(self, tree):
         if 'values_changed' in tree and self.verbose_level > 0:
             for change in tree['values_changed']:
+                path = change.path(force=FORCE_DEFAULT)
                 the_changed = {'new_value': change.t2, 'old_value': change.t1}
-                self['values_changed'][change.path(
-                    force=FORCE_DEFAULT)] = the_changed
+                if self.verbose_level > 1:
+                    new_path = change.path(use_t2=True, force=FORCE_DEFAULT)
+                    if path != new_path:
+                        the_changed['new_path'] = new_path
+                self['values_changed'][path] = the_changed
                 if 'diff' in change.additional:
                     the_changed.update({'diff': change.additional['diff']})
 
     def _from_tree_iterable_item_moved(self, tree):
         if 'iterable_item_moved' in tree and self.verbose_level > 1:
             for change in tree['iterable_item_moved']:
                 the_changed = {'new_path': change.path(use_t2=True), 'value': change.t2}
@@ -275,15 +291,15 @@
                         force=FORCE_DEFAULT)] = _level.additional.get(CUSTOM_FIELD, {})
                 self[k] = _custom_dict
 
 
 class DeltaResult(TextResult):
     ADD_QUOTES_TO_STRINGS = False
 
-    def __init__(self, tree_results=None, ignore_order=None, always_include_values=False):
+    def __init__(self, tree_results=None, ignore_order=None, always_include_values=False, _iterable_opcodes=None):
         self.ignore_order = ignore_order
         self.always_include_values = always_include_values
 
         self.update({
             "type_changes": dict_(),
             "dictionary_item_added": dict_(),
             "dictionary_item_removed": dict_(),
@@ -293,14 +309,15 @@
             "iterable_item_moved": dict_(),
             "attribute_added": dict_(),
             "attribute_removed": dict_(),
             "set_item_removed": dict_(),
             "set_item_added": dict_(),
             "iterable_items_added_at_indexes": dict_(),
             "iterable_items_removed_at_indexes": dict_(),
+            "_iterable_opcodes": _iterable_opcodes or {},
         })
 
         if tree_results:
             self._from_tree_results(tree_results)
 
     def _from_tree_results(self, tree):
         """
@@ -314,16 +331,16 @@
         self._from_tree_value_changed(tree)
         if self.ignore_order:
             self._from_tree_iterable_item_added_or_removed(
                 tree, 'iterable_item_added', delta_report_key='iterable_items_added_at_indexes')
             self._from_tree_iterable_item_added_or_removed(
                 tree, 'iterable_item_removed', delta_report_key='iterable_items_removed_at_indexes')
         else:
-            self._from_tree_default(tree, 'iterable_item_added')
-            self._from_tree_default(tree, 'iterable_item_removed')
+            self._from_tree_default(tree, 'iterable_item_added', ignore_if_in_iterable_opcodes=True)
+            self._from_tree_default(tree, 'iterable_item_removed', ignore_if_in_iterable_opcodes=True)
             self._from_tree_iterable_item_moved(tree)
         self._from_tree_default(tree, 'attribute_added')
         self._from_tree_default(tree, 'attribute_removed')
         self._from_tree_set_item_removed(tree)
         self._from_tree_set_item_added(tree)
         self._from_tree_repetition_change(tree)
 
@@ -366,29 +383,35 @@
                             new_t1 = new_type(change.t1)
                             # If simply applying the type from one value converts it to the other value,
                             # there is no need to include the actual values in the delta.
                             include_values = new_t1 != change.t2
                     except Exception:
                         pass
 
+                path = change.path(force=FORCE_DEFAULT)
+                new_path = change.path(use_t2=True, force=FORCE_DEFAULT)
                 remap_dict = RemapDict({
                     'old_type': old_type,
-                    'new_type': new_type
+                    'new_type': new_type,
                 })
-                self['type_changes'][change.path(
-                    force=FORCE_DEFAULT)] = remap_dict
+                if path != new_path:
+                    remap_dict['new_path'] = new_path
+                self['type_changes'][path] = remap_dict
                 if include_values or self.always_include_values:
                     remap_dict.update(old_value=change.t1, new_value=change.t2)
 
     def _from_tree_value_changed(self, tree):
         if 'values_changed' in tree:
             for change in tree['values_changed']:
+                path = change.path(force=FORCE_DEFAULT)
+                new_path = change.path(use_t2=True, force=FORCE_DEFAULT)
                 the_changed = {'new_value': change.t2, 'old_value': change.t1}
-                self['values_changed'][change.path(
-                    force=FORCE_DEFAULT)] = the_changed
+                if path != new_path:
+                    the_changed['new_path'] = new_path
+                self['values_changed'][path] = the_changed
                 # If we ever want to store the difflib results instead of the new_value
                 # these lines need to be uncommented and the Delta object needs to be able
                 # to use them.
                 # if 'diff' in change.additional:
                 #     the_changed.update({'diff': change.additional['diff']})
 
     def _from_tree_repetition_change(self, tree):
@@ -403,17 +426,20 @@
                     iterable_items_added_at_indexes = self['iterable_items_added_at_indexes'][path] = dict_()
                 for index in repetition['new_indexes']:
                     iterable_items_added_at_indexes[index] = value
 
     def _from_tree_iterable_item_moved(self, tree):
         if 'iterable_item_moved' in tree:
             for change in tree['iterable_item_moved']:
-                the_changed = {'new_path': change.path(use_t2=True), 'value': change.t2}
-                self['iterable_item_moved'][change.path(
-                    force=FORCE_DEFAULT)] = the_changed
+                if (
+                    change.up.path(force=FORCE_DEFAULT) not in self["_iterable_opcodes"]
+                ):
+                    the_changed = {'new_path': change.path(use_t2=True), 'value': change.t2}
+                    self['iterable_item_moved'][change.path(
+                        force=FORCE_DEFAULT)] = the_changed
 
 
 class DiffLevel:
     """
     An object of this class represents a single object-tree-level in a reported change.
     A double-linked list of these object describes a single change on all of its levels.
     Looking at the tree of all changes, a list of those objects represents a single path through the tree
@@ -689,16 +715,16 @@
             result = []
 
         level = self.all_up  # start at the root
 
         # traverse all levels of this relationship
         while level and level is not self:
             # get this level's relationship object
-            if(use_t2):
-                next_rel = level.t2_child_rel
+            if use_t2:
+                next_rel = level.t2_child_rel or level.t1_child_rel
             else:
                 next_rel = level.t1_child_rel or level.t2_child_rel  # next relationship object to get a formatted param from
 
             # t1 and t2 both are empty
             if next_rel is None:
                 break
```

### Comparing `deepdiff-6.7.1/deepdiff/operator.py` & `deepdiff-7.0.0/deepdiff/operator.py`

 * *Files identical despite different names*

### Comparing `deepdiff-6.7.1/deepdiff/path.py` & `deepdiff-7.0.0/deepdiff/path.py`

 * *Files identical despite different names*

### Comparing `deepdiff-6.7.1/deepdiff/search.py` & `deepdiff-7.0.0/deepdiff/search.py`

 * *Files identical despite different names*

### Comparing `deepdiff-6.7.1/deepdiff/serialization.py` & `deepdiff-7.0.0/deepdiff/serialization.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 except ImportError:  # pragma: no cover.
     PydanticBaseModel = None
 
 from copy import deepcopy
 from functools import partial
 from collections.abc import Mapping
 from deepdiff.helper import (
-    strings, get_type, TEXT_VIEW, np_float32, np_float64, np_int32, np_int64
+    strings, get_type, TEXT_VIEW, np_float32, np_float64, np_int32, np_int64, np_ndarray, Opcode, py_current_version
 )
 from deepdiff.model import DeltaResult
 
 logger = logging.getLogger(__name__)
 
 try:
     import jsonpickle
@@ -92,14 +92,15 @@
     'datetime.timedelta',
     'decimal.Decimal',
     'uuid.UUID',
     'ordered_set.OrderedSet',
     'collections.namedtuple',
     'collections.OrderedDict',
     're.Pattern',
+    'deepdiff.helper.Opcode',
 }
 
 
 TYPE_STR_TO_TYPE = {
     'range': range,
     'complex': complex,
     'set': set,
@@ -237,15 +238,37 @@
         Note that it the items in t1 + delta might have slightly different order of items than t2 if ignore_order
         was set to be True in the diff object.
 
         """
         if self.group_by is not None:
             raise ValueError(DELTA_ERROR_WHEN_GROUP_BY)
 
-        result = DeltaResult(tree_results=self.tree, ignore_order=self.ignore_order, always_include_values=always_include_values)
+        if directed and not always_include_values:
+            _iterable_opcodes = {}
+            for path, op_codes in self._iterable_opcodes.items():
+                _iterable_opcodes[path] = []
+                for op_code in op_codes:
+                    new_op_code = Opcode(
+                        tag=op_code.tag,
+                        t1_from_index=op_code.t1_from_index,
+                        t1_to_index=op_code.t1_to_index,
+                        t2_from_index=op_code.t2_from_index,
+                        t2_to_index=op_code.t2_to_index,
+                        new_values=op_code.new_values,
+                    )
+                    _iterable_opcodes[path].append(new_op_code)
+        else:
+            _iterable_opcodes = self._iterable_opcodes
+
+        result = DeltaResult(
+            tree_results=self.tree,
+            ignore_order=self.ignore_order,
+            always_include_values=always_include_values,
+            _iterable_opcodes=_iterable_opcodes,
+        )
         result.remove_empty_keys()
         if report_repetition_required and self.ignore_order and not self.report_repetition:
             raise ValueError(DELTA_IGNORE_ORDER_NEEDS_REPETITION_REPORT)
         if directed:
             for report_key, report_value in result.items():
                 if isinstance(report_value, Mapping):
                     for path, value in report_value.items():
@@ -533,26 +556,35 @@
 def _serialize_decimal(value):
     if value.as_tuple().exponent == 0:
         return int(value)
     else:
         return float(value)
 
 
+def _serialize_tuple(value):
+    if hasattr(value, '_asdict'):  # namedtuple
+        return value._asdict()
+    return value
+
+
 JSON_CONVERTOR = {
     decimal.Decimal: _serialize_decimal,
     ordered_set.OrderedSet: list,
     set: list,
     type: lambda x: x.__name__,
     bytes: lambda x: x.decode('utf-8'),
     datetime.datetime: lambda x: x.isoformat(),
     uuid.UUID: lambda x: str(x),
     np_float32: float,
     np_float64: float,
     np_int32: int,
-    np_int64: int
+    np_int64: int,
+    np_ndarray: lambda x: x.tolist(),
+    tuple: _serialize_tuple,
+    Mapping: dict,
 }
 
 if PydanticBaseModel:
     JSON_CONVERTOR[PydanticBaseModel] = lambda x: x.dict()
 
 
 def json_convertor_default(default_mapping=None):
```

### Comparing `deepdiff-6.7.1/deepdiff.egg-info/PKG-INFO` & `deepdiff-7.0.0/deepdiff.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 Metadata-Version: 2.1
 Name: deepdiff
-Version: 6.7.1
+Version: 7.0.0
 Summary: Deep Difference and Search of any Python object/data. Recreate objects by adding adding deltas to each other.
 Home-page: https://github.com/seperman/deepdiff
-Download-URL: https://github.com/seperman/deepdiff/tarball/master
 Author: Seperman
 Author-email: sep@zepworks.com
 License: MIT
+Download-URL: https://github.com/seperman/deepdiff/tarball/master
+Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: cli
 Provides-Extra: optimize
 License-File: LICENSE
 License-File: AUTHORS.md
 
-# DeepDiff v 6.7.1
+# DeepDiff v 7.0.0
 
 ![Downloads](https://img.shields.io/pypi/dm/deepdiff.svg?style=flat)
 ![Python Versions](https://img.shields.io/pypi/pyversions/deepdiff.svg?style=flat)
 ![License](https://img.shields.io/pypi/l/deepdiff.svg?version=latest)
 [![Build Status](https://github.com/seperman/deepdiff/workflows/Unit%20Tests/badge.svg)](https://github.com/seperman/deepdiff/actions)
 [![codecov](https://codecov.io/gh/seperman/deepdiff/branch/master/graph/badge.svg?token=KkHZ3siA3m)](https://codecov.io/gh/seperman/deepdiff)
 
@@ -38,22 +39,31 @@
 - [DeepDiff](https://zepworks.com/deepdiff/current/diff.html): Deep Difference of dictionaries, iterables, strings, and ANY other object.
 - [DeepSearch](https://zepworks.com/deepdiff/current/dsearch.html): Search for objects within other objects.
 - [DeepHash](https://zepworks.com/deepdiff/current/deephash.html): Hash any object based on their content.
 - [Delta](https://zepworks.com/deepdiff/current/delta.html): Store the difference of objects and apply them to other objects.
 - [Extract](https://zepworks.com/deepdiff/current/extract.html): Extract an item from a nested Python object using its path.
 - [commandline](https://zepworks.com/deepdiff/current/commandline.html): Use DeepDiff from commandline.
 
-Tested on Python 3.7+ and PyPy3.
+Tested on Python 3.8+ and PyPy3.
 
-- **[Documentation](https://zepworks.com/deepdiff/6.7.1/)**
+- **[Documentation](https://zepworks.com/deepdiff/7.0.0/)**
 
 ## What is new?
 
 Please check the [ChangeLog](CHANGELOG.md) file for the detailed information.
 
+DeepDiff 7-0-0
+
+- DeepDiff 7 comes with an improved delta object. [Delta to flat dictionaries](https://zepworks.com/deepdiff/current/serialization.html#delta-serialize-to-flat-dictionaries) have undergone a major change. We have also introduced [Delta serialize to flat rows](https://zepworks.com/deepdiff/current/serialization.html#delta-serialize-to-flat-rows).
+- Subtracting delta objects have dramatically improved at the cost of holding more metadata about the original objects.
+- When `verbose=2`, and the "path" of an item has changed in a report between t1 and t2, we include it as `new_path`.
+- `path(use_t2=True)` returns the correct path to t2 in any reported change in the [`tree view`](https://zepworks.com/deepdiff/current/view.html#tree-view)
+- Python 3.7 support is dropped and Python 3.12 is officially supported.
+
+
 DeepDiff 6-7-1
 
 - Support for subtracting delta objects when iterable_compare_func is used.
 - Better handling of force adding a delta to an object. 
 - Fix for [`Can't compare dicts with both single and double quotes in keys`](https://github.com/seperman/deepdiff/issues/430)
 - Updated docs for Inconsistent Behavior with math_epsilon and ignore_order = True
 
@@ -124,20 +134,12 @@
 
 Please run `pytest --cov=deepdiff --runslow` to see the coverage report. Note that the `--runslow` flag will run some slow tests too. In most cases you only want to run the fast tests which so you wont add the `--runslow` flag.
 
 Or to see a more user friendly version, please run: `pytest --cov=deepdiff --cov-report term-missing --runslow`.
 
 Thank you!
 
-# Citing
-
-How to cite this library (APA style):
-
-    Dehpour, S. (2023). DeepDiff (Version 6.7.1) [Software]. Available from https://github.com/seperman/deepdiff.
-
-How to cite this library (Chicago style):
-
-    Dehpour, Sep. 2023. DeepDiff (version 6.7.1).
-
 # Authors
 
 Please take a look at the [AUTHORS](AUTHORS.md) file.
+
+
```

### Comparing `deepdiff-6.7.1/deepdiff.egg-info/SOURCES.txt` & `deepdiff-7.0.0/deepdiff.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 AUTHORS.md
 LICENSE
 MANIFEST.in
 README.md
 conftest.py
 pytest.ini
 requirements-cli.txt
-requirements-dev-3.7.txt
 requirements-dev.txt
 requirements-optimize.txt
 requirements.txt
 run_tests.sh
 setup.cfg
 setup.py
 temp.py
```

### Comparing `deepdiff-6.7.1/docs/_static/benchmark_array_no_numpy__3.8__ignore_order=True__cache_size=0__cache_tuning_sample_size=0__cutoff_intersection_for_pairs=1.png` & `deepdiff-7.0.0/docs/_static/benchmark_array_no_numpy__3.8__ignore_order=True__cache_size=0__cache_tuning_sample_size=0__cutoff_intersection_for_pairs=1.png`

 * *Files identical despite different names*

### Comparing `deepdiff-6.7.1/docs/_static/benchmark_array_no_numpy__3.8__ignore_order=True__cache_size=10000__cache_tuning_sample_size=0__cutoff_intersection_for_pairs=1.png` & `deepdiff-7.0.0/docs/_static/benchmark_array_no_numpy__3.8__ignore_order=True__cache_size=10000__cache_tuning_sample_size=0__cutoff_intersection_for_pairs=1.png`

 * *Files identical despite different names*

### Comparing `deepdiff-6.7.1/docs/_static/benchmark_big_jsons__3.8__ignore_order=True__cache_size=0__cache_tuning_sample_size=0__max_diffs=300000__max_passes=40000__cutoff_intersection_for_pairs=1.png` & `deepdiff-7.0.0/docs/_static/benchmark_big_jsons__3.8__ignore_order=True__cache_size=0__cache_tuning_sample_size=0__max_diffs=300000__max_passes=40000__cutoff_intersection_for_pairs=1.png`

 * *Files identical despite different names*

### Comparing `deepdiff-6.7.1/docs/_static/benchmark_big_jsons__pypy3.6__ignore_order=True__cache_size=0__cache_tuning_sample_size=0__max_diffs=300000__max_passes=40000__cutoff_intersection_for_pairs=1.png` & `deepdiff-7.0.0/docs/_static/benchmark_big_jsons__pypy3.6__ignore_order=True__cache_size=0__cache_tuning_sample_size=0__max_diffs=300000__max_passes=40000__cutoff_intersection_for_pairs=1.png`

 * *Files identical despite different names*

### Comparing `deepdiff-6.7.1/docs/_static/benchmark_deeply_nested_a__3.8__ignore_order=True__cache_size=0__cache_tuning_sample_size=0__cutoff_intersection_for_pairs=1.png` & `deepdiff-7.0.0/docs/_static/benchmark_deeply_nested_a__3.8__ignore_order=True__cache_size=0__cache_tuning_sample_size=0__cutoff_intersection_for_pairs=1.png`

 * *Files identical despite different names*

### Comparing `deepdiff-6.7.1/docs/_static/benchmark_deeply_nested_a__3.8__ignore_order=True__cache_size=5000__cache_tuning_sample_size=0__cutoff_intersection_for_pairs=1.png` & `deepdiff-7.0.0/docs/_static/benchmark_deeply_nested_a__3.8__ignore_order=True__cache_size=5000__cache_tuning_sample_size=0__cutoff_intersection_for_pairs=1.png`

 * *Files identical despite different names*

### Comparing `deepdiff-6.7.1/docs/_static/benchmark_deeply_nested_a__3.8__ignore_order=True__cache_size=500__cache_tuning_sample_size=0__cutoff_intersection_for_pairs=1.png` & `deepdiff-7.0.0/docs/_static/benchmark_deeply_nested_a__3.8__ignore_order=True__cache_size=500__cache_tuning_sample_size=0__cutoff_intersection_for_pairs=1.png`

 * *Files identical despite different names*

### Comparing `deepdiff-6.7.1/docs/_static/benchmark_deeply_nested_a__3.8__ignore_order=True__cache_size=500__cache_tuning_sample_size=500__cutoff_intersection_for_pairs=1.png` & `deepdiff-7.0.0/docs/_static/benchmark_deeply_nested_a__3.8__ignore_order=True__cache_size=500__cache_tuning_sample_size=500__cutoff_intersection_for_pairs=1.png`

 * *Files identical despite different names*

### Comparing `deepdiff-6.7.1/docs/_static/benchmark_numpy_array__3.8__ignore_order=True__cache_size=0__cache_tuning_sample_size=0__cutoff_intersection_for_pairs=1.png` & `deepdiff-7.0.0/docs/_static/benchmark_numpy_array__3.8__ignore_order=True__cache_size=0__cache_tuning_sample_size=0__cutoff_intersection_for_pairs=1.png`

 * *Files identical despite different names*

### Comparing `deepdiff-6.7.1/docs/authors.rst` & `deepdiff-7.0.0/docs/authors.rst`

 * *Files 4% similar despite different names*

```diff
@@ -80,14 +80,19 @@
 -  `kor4ik <https://github.com/kor4ik>`__ for the bugfix for
    ``include_paths`` for nested dictionaries.
 -  `martin-kokos <https://github.com/martin-kokos>`__ for using tomli
    and tomli-w for dealing with tomli files.
 -  `Alex Sauer-Budge <https://github.com/amsb>`__ for the bugfix for
    ``datetime.date``.
 - `William Jamieson <https://github.com/WilliamJamieson>`__ for `NumPy 2.0 compatibility <https://github.com/seperman/deepdiff/pull/422>`__
+-  `Leo Sin <https://github.com/leoslf>`__ for Supporting Python 3.12 in
+   the build process
+-  `sf-tcalhoun <https://github.com/sf-tcalhoun>`__ for fixing
+   “Instantiating a Delta with a flat_dict_list unexpectedly mutates the
+   flat_dict_list”
 
 .. _Sep Dehpour (Seperman): http://www.zepworks.com
 .. _Victor Hahn Castell: http://hahncastell.de
 .. _nfvs: https://github.com/nfvs
 .. _brbsix: https://github.com/brbsix
 .. _WangFenjin: https://github.com/WangFenjin
 .. _timoilya: https://github.com/timoilya
```

### Comparing `deepdiff-6.7.1/docs/basics.rst` & `deepdiff-7.0.0/docs/basics.rst`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,25 @@
     >>> t1 = {1:1, 3:3, 4:4}
     >>> t2 = {1:1, 3:3, 5:5, 6:6}
     >>> ddiff = DeepDiff(t1, t2, verbose_level=2)
     >>> pprint(ddiff, indent=2)
     { 'dictionary_item_added': {'root[5]': 5, 'root[6]': 6},
       'dictionary_item_removed': {'root[4]': 4}}
 
+Set verbose level to 2 includes new_path when the path has changed for a report between t1 and t2:
+    >>> t1 = [1, 3]
+    >>> t2 = [3, 2]
+    >>>
+    >>>
+    >>> diff = DeepDiff(t1, t2, ignore_order=True, verbose_level=2)
+    >>> pprint(diff)
+    {'values_changed': {'root[0]': {'new_path': 'root[1]',
+                                    'new_value': 2,
+                                    'old_value': 1}}}
+
 String difference
     >>> t1 = {1:1, 2:2, 3:3, 4:{"a":"hello", "b":"world"}}
     >>> t2 = {1:1, 2:4, 3:3, 4:{"a":"hello", "b":"world!"}}
     >>> ddiff = DeepDiff(t1, t2)
     >>> pprint (ddiff, indent = 2)
     { 'values_changed': { 'root[2]': {'new_value': 4, 'old_value': 2},
                           "root[4]['b']": { 'new_value': 'world!',
```

### Comparing `deepdiff-6.7.1/docs/changelog.rst` & `deepdiff-7.0.0/docs/changelog.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,38 @@
 :doc:`/index`
 
 Changelog
 =========
 
 DeepDiff Changelog
 
+-  v7-0-0
+
+   -  When verbose=2, return ``new_path`` when the ``path`` and
+      ``new_path`` are different (for example when ignore_order=True and
+      the index of items have changed).
+   -  Dropping support for Python 3.7
+   -  Introducing serialize to flat rows for delta objects.
+   -  fixes the issue with hashing ``datetime.date`` objects where it
+      treated them as numbers instead of dates (fixes #445).
+   -  upgrading orjson to the latest version
+   -  Fix for bug when diffing two lists with ignore_order and providing
+      compare_func
+   -  Fixes “Wrong diff on list of strings” #438
+   -  Supporting Python 3.12 in the build process by `Leo
+      Sin <https://github.com/leoslf>`__
+   -  Fixes “Instantiating a Delta with a flat_dict_list unexpectedly
+      mutates the flat_dict_list” #457 by
+      `sf-tcalhoun <https://github.com/sf-tcalhoun>`__
+   -  Fixes “Error on Delta With None Key and Removed Item from List”
+      #441
+   -  Fixes “Error when comparing two nested dicts with 2 added fields”
+      #450
+   -  Fixes “Error when subtracting Delta from a dictionary” #443
+
 -  v6-7-1
 
    -  Support for subtracting delta objects when iterable_compare_func
       is used.
    -  Better handling of force adding a delta to an object.
    -  Fix for
       ```Can't compare dicts with both single and double quotes in keys`` <https://github.com/seperman/deepdiff/issues/430>`__
```

### Comparing `deepdiff-6.7.1/docs/commandline.rst` & `deepdiff-7.0.0/docs/commandline.rst`

 * *Files identical despite different names*

### Comparing `deepdiff-6.7.1/docs/custom.rst` & `deepdiff-7.0.0/docs/custom.rst`

 * *Files identical despite different names*

### Comparing `deepdiff-6.7.1/docs/deep_distance.rst` & `deepdiff-7.0.0/docs/deep_distance.rst`

 * *Files identical despite different names*

### Comparing `deepdiff-6.7.1/docs/deephash_doc.rst` & `deepdiff-7.0.0/docs/deephash_doc.rst`

 * *Files identical despite different names*

### Comparing `deepdiff-6.7.1/docs/delta.rst` & `deepdiff-7.0.0/docs/delta.rst`

 * *Files 0% similar despite different names*

```diff
@@ -177,14 +177,21 @@
 .. _flat_dict_list_label:
 
 Flat Dict List
 --------------
 
 You can create a delta object from the list of flat dictionaries that are produced via :ref:`to_flat_dicts_label`. Read more on :ref:`delta_from_flat_dicts_label`.
 
+.. _flat_rows_list_label:
+
+Flat Rows List
+--------------
+
+You can create a delta object from the list of flat dictionaries that are produced via :ref:`to_flat_rows_label`. Read more on :ref:`delta_from_flat_rows_label`.
+
 
 .. _delta_deserializer_label:
 
 Delta Deserializer
 ------------------
 
 DeepDiff by default uses a restricted Python pickle function to deserialize the Delta dumps. Read more about :ref:`delta_dump_safety_label`.
```

### Comparing `deepdiff-6.7.1/docs/diff_doc.rst` & `deepdiff-7.0.0/docs/diff_doc.rst`

 * *Files 2% similar despite different names*

```diff
@@ -110,14 +110,18 @@
     :ref:`ignore_type_in_groups_label`
     ignores types when t1 and t2 are both within the same type group.
 
 ignore_type_subclasses: Boolean, default = False
     :ref:`ignore_type_subclasses_label`
     ignore type (class) changes when dealing with the subclasses of classes that were marked to be ignored.
 
+.. Note::
+    ignore_type_subclasses was incorrectly doing the reverse of its job up until DeepDiff 6.7.1
+    Please make sure to flip it in your use cases, when upgrading from older versions to 7.0.0 or above.
+
 ignore_string_case: Boolean, default = False
     :ref:`ignore_string_case_label`
     Whether to be case-sensitive or not when comparing strings. By settings ignore_string_case=False, strings will be compared case-insensitively.
 
 ignore_nan_inequality: Boolean, default = False
     :ref:`ignore_nan_inequality_label`
     Whether to ignore float('nan') inequality in Python.
```

### Comparing `deepdiff-6.7.1/docs/exclude_paths.rst` & `deepdiff-7.0.0/docs/exclude_paths.rst`

 * *Files identical despite different names*

### Comparing `deepdiff-6.7.1/docs/faq.rst` & `deepdiff-7.0.0/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `deepdiff-6.7.1/docs/ignore_order.rst` & `deepdiff-7.0.0/docs/ignore_order.rst`

 * *Files identical despite different names*

### Comparing `deepdiff-6.7.1/docs/ignore_types_or_values.rst` & `deepdiff-7.0.0/docs/ignore_types_or_values.rst`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,27 @@
 
     Now what if you want also typeA and typeB to be ignored when comparing against each other?
 
     1. ignore_type_in_groups=[DeepDiff.strings, (typeA, typeB)]
     2. or ignore_type_in_groups=[(str, bytes), (typeA, typeB)]
 
 
+Example: Ignore Enum to string comparison
+    >>> from deepdiff import DeepDiff
+    >>> from enum import Enum
+    >>> class MyEnum1(Enum):
+    ...     book = "book"
+    ...     cake = "cake"
+    ...
+    >>> DeepDiff("book", MyEnum1.book)
+    {'type_changes': {'root': {'old_type': <class 'str'>, 'new_type': <enum 'MyEnum1'>, 'old_value': 'book', 'new_value': <MyEnum1.book: 'book'>}}}
+    >>> DeepDiff("book", MyEnum1.book, ignore_type_in_groups=[(Enum, str)])
+    {}
+
+
 Example: Ignore Type Number - Dictionary that contains float and integer. Note that this is exactly the same as passing ignore_numeric_type_changes=True.
     >>> from deepdiff import DeepDiff
     >>> from pprint import pprint
     >>> t1 = {1: 1, 2: 2.22}
     >>> t2 = {1: 1.0, 2: 2.22}
     >>> ddiff = DeepDiff(t1, t2)
     >>> pprint(ddiff, indent=2)
@@ -197,14 +210,18 @@
 
 Ignore Type Subclasses
 ----------------------
 
 ignore_type_subclasses: Boolean, default = False
     Use ignore_type_subclasses=True so when ignoring type (class), the subclasses of that class are ignored too.
 
+.. Note::
+    ignore_type_subclasses was incorrectly doing the reverse of its job up until DeepDiff 6.7.1
+    Please make sure to flip it in your use cases, when upgrading from older versions to 7.0.0 or above.
+
     >>> from deepdiff import DeepDiff
     >>> class ClassA:
     ...     def __init__(self, x, y):
     ...         self.x = x
     ...         self.y = y
     ...
     >>> class ClassB:
@@ -213,18 +230,18 @@
     ...
     >>> class ClassC(ClassB):
     ...     pass
     ...
     >>> obj_a = ClassA(1, 2)
     >>> obj_c = ClassC(3)
     >>>
-    >>> DeepDiff(obj_a, obj_c, ignore_type_in_groups=[(ClassA, ClassB)], ignore_type_subclasses=False)
+    >>> DeepDiff(obj_a, obj_c, ignore_type_in_groups=[(ClassA, ClassB)], ignore_type_subclasses=True)
     {'type_changes': {'root': {'old_type': <class '__main__.ClassA'>, 'new_type': <class '__main__.ClassC'>, 'old_value': <__main__.ClassA object at 0x10076a2e8>, 'new_value': <__main__.ClassC object at 0x10082f630>}}}
     >>>
-    >>> DeepDiff(obj_a, obj_c, ignore_type_in_groups=[(ClassA, ClassB)], ignore_type_subclasses=True)
+    >>> DeepDiff(obj_a, obj_c, ignore_type_in_groups=[(ClassA, ClassB)], ignore_type_subclasses=False)
     {'values_changed': {'root.x': {'new_value': 3, 'old_value': 1}}, 'attribute_removed': [root.y]}
 
 
 
 .. _ignore_string_case_label:
 
 Ignore String Case
```

### Comparing `deepdiff-6.7.1/docs/index.rst` & `deepdiff-7.0.0/docs/index.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 .. DeepDiff documentation master file, created by
    sphinx-quickstart on Mon Jul 20 06:06:44 2015.
    You can adapt this file completely to your liking, but it should at least
    contain the root `toctree` directive.
 
 
-DeepDiff 6.7.1 documentation!
+DeepDiff 7.0.0 documentation!
 =============================
 
 *******
 Modules
 *******
 
 The DeepDiff library includes the following modules:
@@ -27,14 +27,32 @@
 
 - **Commandline** Most of the above functionality is also available via the commandline module  :doc:`/commandline`
 
 ***********
 What Is New
 ***********
 
+DeepDiff 7-0-0
+--------------
+
+-  DeepDiff 7 comes with an improved delta object. `Delta to flat
+   dictionaries <https://zepworks.com/deepdiff/current/serialization.html#delta-serialize-to-flat-dictionaries>`__
+   have undergone a major change. We have also introduced `Delta
+   serialize to flat
+   rows <https://zepworks.com/deepdiff/current/serialization.html#delta-serialize-to-flat-rows>`__.
+-  Subtracting delta objects have dramatically improved at the cost of
+   holding more metadata about the original objects.
+-  When ``verbose=2``, and the “path” of an item has changed in a report
+   between t1 and t2, we include it as ``new_path``.
+-  ``path(use_t2=True)`` returns the correct path to t2 in any reported
+   change in the
+   ```tree view`` <https://zepworks.com/deepdiff/current/view.html#tree-view>`__
+-  Python 3.7 support is dropped and Python 3.12 is officially
+   supported.
+
 
 DeepDiff 6-7-1
 --------------
 
    -  Support for subtracting delta objects when iterable_compare_func
       is used.
    -  Better handling of force adding a delta to an object.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `deepdiff-6.7.1/docs/numbers.rst` & `deepdiff-7.0.0/docs/numbers.rst`

 * *Files identical despite different names*

### Comparing `deepdiff-6.7.1/docs/optimizations.rst` & `deepdiff-7.0.0/docs/optimizations.rst`

 * *Files identical despite different names*

### Comparing `deepdiff-6.7.1/docs/other.rst` & `deepdiff-7.0.0/docs/other.rst`

 * *Files identical despite different names*

### Comparing `deepdiff-6.7.1/docs/search_doc.rst` & `deepdiff-7.0.0/docs/search_doc.rst`

 * *Files identical despite different names*

### Comparing `deepdiff-6.7.1/docs/stats.rst` & `deepdiff-7.0.0/docs/stats.rst`

 * *Files identical despite different names*

### Comparing `deepdiff-6.7.1/docs/support.rst` & `deepdiff-7.0.0/docs/support.rst`

 * *Files identical despite different names*

### Comparing `deepdiff-6.7.1/docs/troubleshoot.rst` & `deepdiff-7.0.0/docs/troubleshoot.rst`

 * *Files identical despite different names*

### Comparing `deepdiff-6.7.1/docs/view.rst` & `deepdiff-7.0.0/docs/view.rst`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     |    child(t1)              child node               child(t2)  |----level
     |                                                               |
     +---------------------------------------------------------------+
 
 
 :up: Move up to the parent node aka parent level
 :down: Move down to the child node aka child level
-:path(): Get the path to the current node in string representation, path(output_format='list') gives you the path in list representation.
+:path(): Get the path to the current node in string representation, path(output_format='list') gives you the path in list representation. path(use_t2=True) gives you the path to t2.
 :t1: The first item in the current node that is being diffed
 :t2: The second item in the current node that is being diffed
 :additional: Additional information about the node i.e. repetition
 :repetition: Shortcut to get the repetition report
 
 
 The tree view allows you to have more than mere textual representaion of the diffed objects.
```

### Comparing `deepdiff-6.7.1/setup.py` & `deepdiff-7.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     sys.exit('Python 2 is not supported anymore. The last version of DeepDiff that supported Py2 was 3.3.0')
 
 # if you are not using vagrant, just delete os.link directly,
 # The hard link only saves a little disk space, so you should not care
 if os.environ.get('USER', '') == 'vagrant':
     del os.link
 
-version = '6.7.1'
+version = '7.0.0'
 
 
 def get_reqs(filename):
     with open(filename, "r") as reqs_file:
         reqs = reqs_file.readlines()
     return reqs
 
@@ -39,28 +39,28 @@
       zip_safe=True,
       test_suite="tests",
       include_package_data=True,
       tests_require=['mock'],
       long_description=long_description,
       long_description_content_type='text/markdown',
       install_requires=reqs,
-      python_requires='>=3.7',
+      python_requires='>=3.8',
       extras_require={
           "cli": cli_reqs,
           "optimize": optimize_reqs,
       },
       classifiers=[
           "Intended Audience :: Developers",
           "Operating System :: OS Independent",
           "Topic :: Software Development",
-          "Programming Language :: Python :: 3.7",
           "Programming Language :: Python :: 3.8",
           "Programming Language :: Python :: 3.9",
           "Programming Language :: Python :: 3.10",
           "Programming Language :: Python :: 3.11",
+          "Programming Language :: Python :: 3.12",
           "Programming Language :: Python :: Implementation :: PyPy",
           "Development Status :: 5 - Production/Stable",
           "License :: OSI Approved :: MIT License"
       ],
       entry_points={
           'console_scripts': [
               'deep=deepdiff.commands:cli',
```

### Comparing `deepdiff-6.7.1/temp1.py` & `deepdiff-7.0.0/temp1.py`

 * *Files identical despite different names*

### Comparing `deepdiff-6.7.1/tests/__init__.py` & `deepdiff-7.0.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdiff-6.7.1/tests/fixtures/compare_func_result1.json` & `deepdiff-7.0.0/tests/fixtures/compare_func_result1.json`

 * *Files identical despite different names*

### Comparing `deepdiff-6.7.1/tests/fixtures/compare_func_t1.json` & `deepdiff-7.0.0/tests/fixtures/compare_func_t1.json`

 * *Files identical despite different names*

### Comparing `deepdiff-6.7.1/tests/fixtures/compare_func_t2.json` & `deepdiff-7.0.0/tests/fixtures/compare_func_t2.json`

 * *Files identical despite different names*

### Comparing `deepdiff-6.7.1/tests/fixtures/nested_a_result.json` & `deepdiff-7.0.0/tests/fixtures/nested_a_result.json`

 * *Files identical despite different names*

### Comparing `deepdiff-6.7.1/tests/fixtures/nested_a_t1.json` & `deepdiff-7.0.0/tests/fixtures/nested_a_t1.json`

 * *Files identical despite different names*

### Comparing `deepdiff-6.7.1/tests/fixtures/nested_a_t2.json` & `deepdiff-7.0.0/tests/fixtures/nested_a_t2.json`

 * *Files identical despite different names*

### Comparing `deepdiff-6.7.1/tests/test_anyset.py` & `deepdiff-7.0.0/tests/test_anyset.py`

 * *Files identical despite different names*

### Comparing `deepdiff-6.7.1/tests/test_cache.py` & `deepdiff-7.0.0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `deepdiff-6.7.1/tests/test_command.py` & `deepdiff-7.0.0/tests/test_command.py`

 * *Files identical despite different names*

### Comparing `deepdiff-6.7.1/tests/test_delta.py` & `deepdiff-7.0.0/tests/test_delta.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+import copy
+
 import pytest
 import os
 import io
 import json
 import sys
 from decimal import Decimal
 from unittest import mock
 from ordered_set import OrderedSet
 from deepdiff import Delta, DeepDiff
-from deepdiff.helper import np, number_to_string, TEXT_VIEW, DELTA_VIEW, CannotCompare
+from deepdiff.helper import np, number_to_string, TEXT_VIEW, DELTA_VIEW, CannotCompare, FlatDeltaRow
 from deepdiff.path import GETATTR, GET
 from deepdiff.delta import (
     ELEM_NOT_FOUND_TO_ADD_MSG,
     VERIFICATION_MSG, VERIFY_BIDIRECTIONAL_MSG, not_found, DeltaNumpyOperatorOverrideError,
     BINIARY_MODE_NEEDED_MSG, DELTA_AT_LEAST_ONE_ARG_NEEDED, DeltaError,
     INVALID_ACTION_WHEN_CALLING_GET_ELEM, INVALID_ACTION_WHEN_CALLING_SIMPLE_SET_ELEM,
     INVALID_ACTION_WHEN_CALLING_SIMPLE_DELETE_ELEM, INDEXES_NOT_FOUND_WHEN_IGNORE_ORDER,
@@ -65,18 +67,18 @@
         t2 = [1, 2, 3, 5]
         diff = {'iterable_item_added': {'root[3]': 5, 'root[2]': 3}}
         delta = Delta(diff)
 
         assert delta + t1 == t2
         assert t1 + delta == t2
 
-        flat_result1 = delta.to_flat_dicts()
+        flat_result1 = delta.to_flat_rows()
         flat_expected1 = [
-            {'path': [3], 'value': 5, 'action': 'iterable_item_added'},
-            {'path': [2], 'value': 3, 'action': 'iterable_item_added'},
+            FlatDeltaRow(path=[3], value=5, action='iterable_item_added'),
+            FlatDeltaRow(path=[2], value=3, action='iterable_item_added'),
         ]
 
         assert flat_expected1 == flat_result1
         delta2 = Delta(diff=diff, bidirectional=True)
         assert t1 == t2 - delta2
 
     def test_list_difference_dump_delta(self):
@@ -225,15 +227,15 @@
 
     def test_identical_delta(self):
         delta = Delta({})
 
         t1 = [1, 3]
         assert t1 + delta == t1
 
-        flat_result1 = delta.to_flat_dicts()
+        flat_result1 = delta.to_flat_rows()
         flat_expected1 = []
 
         assert flat_expected1 == flat_result1
 
     def test_delta_mutate(self):
         t1 = [1, 2]
         t2 = [1, 2, 3, 5]
@@ -283,19 +285,19 @@
             }
         }
         delta = Delta(diff)
 
         assert delta + t1 == t2
         assert t1 + delta == t2
 
-        flat_result1 = delta.to_flat_dicts()
+        flat_result1 = delta.to_flat_rows()
         flat_expected1 = [
-            {'path': [4, 'b', 2], 'action': 'values_changed', 'value': 2, 'old_value': 5},
-            {'path': [4, 'b', 1], 'action': 'values_changed', 'value': 3, 'old_value': 2},
-            {'path': [4, 'b', 3], 'value': 5, 'action': 'iterable_item_added'},
+            FlatDeltaRow(path=[4, 'b', 2], action='values_changed', value=2, old_value=5),
+            FlatDeltaRow(path=[4, 'b', 1], action='values_changed', value=3, old_value=2),
+            FlatDeltaRow(path=[4, 'b', 3], value=5, action='iterable_item_added'),
         ]
 
         assert flat_expected1 == flat_result1
 
         delta2 = Delta(diff=diff, bidirectional=True)
         assert t1 == t2 - delta2
 
@@ -324,19 +326,19 @@
         with pytest.raises(ValueError) as excinfo:
             delta + t1
         assert expected_msg == str(excinfo.value)
 
         delta2 = Delta(diff, bidirectional=False)
         assert delta2 + t1 == t2
 
-        flat_result2 = delta2.to_flat_dicts()
+        flat_result2 = delta2.to_flat_rows()
         flat_expected2 = [
-            {'path': [2], 'action': 'values_changed', 'value': 2, 'old_value': 5},
-            {'path': [1], 'action': 'values_changed', 'value': 3, 'old_value': 2},
-            {'path': [3], 'value': 5, 'action': 'iterable_item_added'},
+            FlatDeltaRow(path=[2], action='values_changed', value=2, old_value=5),
+            FlatDeltaRow(path=[1], action='values_changed', value=3, old_value=2),
+            FlatDeltaRow(path=[3], value=5, action='iterable_item_added'),
         ]
 
         assert flat_expected2 == flat_result2
 
     def test_list_difference_delta1(self):
         t1 = {
             1: 1,
@@ -355,18 +357,18 @@
                 "root[4]['b'][3]": 'to_be_removed2'
             }
         }
         delta = Delta(diff)
 
         assert delta + t1 == t2
 
-        flat_result = delta.to_flat_dicts()
+        flat_result = delta.to_flat_rows()
         flat_expected = [
-            {'path': [4, 'b', 2], 'value': 'to_be_removed', 'action': 'iterable_item_removed'},
-            {'path': [4, 'b', 3], 'value': 'to_be_removed2', 'action': 'iterable_item_removed'},
+            FlatDeltaRow(path=[4, 'b', 2], value='to_be_removed', action='iterable_item_removed'),
+            FlatDeltaRow(path=[4, 'b', 3], value='to_be_removed2', action='iterable_item_removed'),
         ]
 
         assert flat_expected == flat_result
 
         delta2 = Delta(diff=diff, bidirectional=True)
         assert t1 == t2 - delta2
 
@@ -457,14 +459,162 @@
 
         assert list(result.keys()) == [6, 7, 3, 5, 2, 4]
         assert list(result.keys()) == list(t2.keys())
 
         delta2 = Delta(diff=diff, bidirectional=True)
         assert t1 == t2 - delta2
 
+    def test_delta_constr_flat_dict_list_param_preserve(self):
+        """
+        Issue: https://github.com/seperman/deepdiff/issues/457
+
+        Scenario:
+        We found that when a flat_rows_list was provided as a constructor
+        parameter for instantiating a new delta, the provided flat_rows_list
+        is unexpectedly being mutated/changed, which can be troublesome for the
+        caller if they were expecting the flat_rows_list to be used BY COPY
+        rather than BY REFERENCE.
+
+        Intent:
+        Preserve the original value of the flat_rows_list variable within the
+        calling module/function after instantiating the new delta.
+        """
+
+        t1 = {
+            "individualNames": [
+                {
+                    "firstName": "Johnathan",
+                    "lastName": "Doe",
+                    "prefix": "COLONEL",
+                    "middleName": "A",
+                    "primaryIndicator": True,
+                    "professionalDesignation": "PHD",
+                    "suffix": "SR",
+                    "nameIdentifier": "00001"
+                },
+                {
+                    "firstName": "John",
+                    "lastName": "Doe",
+                    "prefix": "",
+                    "middleName": "",
+                    "primaryIndicator": False,
+                    "professionalDesignation": "",
+                    "suffix": "SR",
+                    "nameIdentifier": "00002"
+                }
+            ]
+        }
+
+        t2 = {
+            "individualNames": [
+                {
+                    "firstName": "Johnathan",
+                    "lastName": "Doe",
+                    "prefix": "COLONEL",
+                    "middleName": "A",
+                    "primaryIndicator": True,
+                    "professionalDesignation": "PHD",
+                    "suffix": "SR",
+                    "nameIdentifier": "00001"
+                },
+                {
+                    "firstName": "Johnny",
+                    "lastName": "Doe",
+                    "prefix": "",
+                    "middleName": "A",
+                    "primaryIndicator": False,
+                    "professionalDesignation": "",
+                    "suffix": "SR",
+                    "nameIdentifier": "00003"
+                }
+            ]
+        }
+
+        def compare_func(item1, item2, level=None):
+            print("*** inside compare ***")
+            it1_keys = item1.keys()
+
+            try:
+
+                # --- individualNames ---
+                if 'nameIdentifier' in it1_keys and 'lastName' in it1_keys:
+                    match_result = item1['nameIdentifier'] == item2['nameIdentifier']
+                    print("individualNames - matching result:", match_result)
+                    return match_result
+                else:
+                    print("Unknown list item...", "matching result:", item1 == item2)
+                    return item1 == item2
+            except Exception:
+                raise CannotCompare() from None
+        # ---------------------------- End of nested function
+
+        # This diff should show:
+        # 1 - list item (with an index on the path) being added
+        # 1 - list item (with an index on the path) being removed
+        diff = DeepDiff(t1, t2, report_repetition=True,
+                             ignore_order=True, iterable_compare_func=compare_func, cutoff_intersection_for_pairs=1)
+
+        # Now create a flat_rows_list from a delta instantiated from the diff...
+        temp_delta = Delta(diff, always_include_values=True, bidirectional=True, raise_errors=True)
+        flat_rows_list = temp_delta.to_flat_rows()
+
+        # Note: the list index is provided on the path value...
+        assert flat_rows_list == [FlatDeltaRow(path=['individualNames', 1],
+                                   value={'firstName': 'Johnny',
+                                             'lastName': 'Doe',
+                                             'prefix': '',
+                                             'middleName': 'A',
+                                             'primaryIndicator': False,
+                                             'professionalDesignation': '',
+                                             'suffix': 'SR',
+                                             'nameIdentifier': '00003'},
+                                   action='unordered_iterable_item_added'),
+                                  FlatDeltaRow(path=['individualNames', 1],
+                                   value={'firstName': 'John',
+                                             'lastName': 'Doe',
+                                             'prefix': '',
+                                             'middleName': '',
+                                             'primaryIndicator': False,
+                                             'professionalDesignation': '',
+                                             'suffix': 'SR',
+                                             'nameIdentifier': '00002'},
+                                   action='unordered_iterable_item_removed')]
+
+        preserved_flat_dict_list = copy.deepcopy(flat_rows_list)  # Use this later for assert comparison
+
+        # Now use the flat_rows_list to instantiate a new delta...
+        delta = Delta(flat_rows_list=flat_rows_list,
+                      always_include_values=True, bidirectional=True, raise_errors=True)
+
+        # if the flat_rows_list is (unexpectedly) mutated, it will be missing the list index number on the path value.
+        old_mutated_list_missing_indexes_on_path = [FlatDeltaRow(path=['individualNames'],
+                                         value={'firstName': 'Johnny',
+                                                   'lastName': 'Doe',
+                                                   'prefix': '',
+                                                   'middleName': 'A',
+                                                   'primaryIndicator': False,
+                                                   'professionalDesignation': '',
+                                                   'suffix': 'SR',
+                                                   'nameIdentifier': '00003'},
+                                         action='unordered_iterable_item_added'),
+                                        FlatDeltaRow(path=['individualNames'],
+                                         value={'firstName': 'John',
+                                                   'lastName': 'Doe',
+                                                   'prefix': '',
+                                                   'middleName': '',
+                                                   'primaryIndicator': False,
+                                                   'professionalDesignation': '',
+                                                   'suffix': 'SR',
+                                                   'nameIdentifier': '00002'},
+                                         action='unordered_iterable_item_removed')]
+
+        # Verify that our fix in the delta constructor worked...
+        assert flat_rows_list != old_mutated_list_missing_indexes_on_path
+        assert flat_rows_list == preserved_flat_dict_list
+
 
 picklalbe_obj_without_item = PicklableClass(11)
 del picklalbe_obj_without_item.item
 
 
 DELTA_CASES = {
     'delta_case0': {
@@ -757,16 +907,17 @@
             'ignore_order': True,
             'report_repetition': True
         },
         'to_delta_kwargs': {},
         'expected_delta_dict': {
             'values_changed': {
                 'root[6]': {
-                    'new_value': 5
-                }
+                    'new_value': 5,
+                    'new_path': 'root[3]',
+                },
             },
             'iterable_items_removed_at_indexes': {
                 'root': {
                     2: 'B',
                     4: 'B',
                     5: 'B'
                 }
@@ -781,16 +932,17 @@
             'ignore_order': True,
             'report_repetition': True
         },
         'to_delta_kwargs': {},
         'expected_delta_dict': {
             'values_changed': {
                 'root[3]': {
-                    'new_value': 4
-                }
+                    'new_value': 4,
+                    'new_path': 'root[6]',
+                },
             },
             'iterable_items_added_at_indexes': {
                 'root': {
                     2: 'B',
                     4: 'B',
                     5: 'B'
                 }
@@ -805,18 +957,20 @@
             'ignore_order': True,
             'report_repetition': True
         },
         'to_delta_kwargs': {},
         'expected_delta_dict': {
             'values_changed': {
                 'root[4]': {
-                    'new_value': 7
+                    'new_value': 7,
+                    'new_path': 'root[0]'
                 },
                 'root[0]': {
-                    'new_value': 8
+                    'new_value': 8,
+                    'new_path': 'root[4]'
                 }
             }
         },
         'expected_t1_plus_delta': [8, 1, 1, 1, 7],
     },
     'delta_ignore_order_case4': {
         't1': [5, 1, 3, 1, 4, 4, 6],
@@ -825,18 +979,20 @@
             'ignore_order': True,
             'report_repetition': True
         },
         'to_delta_kwargs': {},
         'expected_delta_dict': {
             'values_changed': {
                 'root[6]': {
-                    'new_value': 7
+                    'new_value': 7,
+                    'new_path': 'root[0]'
                 },
                 'root[0]': {
-                    'new_value': 8
+                    'new_value': 8,
+                    'new_path': 'root[6]'
                 }
             },
             'iterable_items_added_at_indexes': {
                 'root': {
                     1: 4,
                     2: 4,
                     5: 4,
@@ -860,18 +1016,20 @@
                     1: 4,
                     2: 4,
                     5: 4
                 }
             },
             'values_changed': {
                 'root[6]': {
-                    'new_value': 7
+                    'new_value': 7,
+                    'new_path': 'root[0]',
                 },
                 'root[0]': {
-                    'new_value': 8
+                    'new_value': 8,
+                    'new_path': 'root[6]',
                 }
             }
         },
         'expected_t1_plus_delta': (8, 4, 4, 1, 3, 4, 1, 7),
     },
     'delta_ignore_order_case6': {
         't1': [{1, 2, 3}, {4, 5}],
@@ -1162,14 +1320,23 @@
             },
             '_numpy_paths': {
                 'root': np.where((sys.maxsize > 2**32), 'int64', 'int32')
             }
         },
         'expected_result': 't2'
     },
+    'delta_with_null_as_key': {
+        't1': { None: [1, 2], 'foo': [1, 2] },
+        't2': { None: [1], 'foo': [1] },
+        'deepdiff_kwargs': {},
+        'to_delta_kwargs': {},
+        'expected_delta_dict': {
+        },
+        'expected_result': 't2'
+    },
 }
 
 
 DELTA_NUMPY_TEST_PARAMS = parameterize_cases(
     'test_name, t1, t2, deepdiff_kwargs, to_delta_kwargs, expected_delta_dict, expected_result', DELTA_NUMPY_TEST_CASES)
 
 
@@ -1232,41 +1399,43 @@
         delta1 = Delta(delta_dict1)
         t1_plus_delta1 = t1 + delta1
         assert t1_plus_delta1 == t2
         delta2 = Delta(delta_dict2)
         t1_plus_delta2 = t1 + delta2
         assert t1_plus_delta2 == (8, 4, 4, 1, 3, 4, 1, 7)
 
-        flat_result1 = delta1.to_flat_dicts()
+        flat_result1 = delta1.to_flat_rows()
         flat_expected1 = [
             {'path': [0], 'value': 7, 'action': 'unordered_iterable_item_added'},
             {'path': [6], 'value': 8, 'action': 'unordered_iterable_item_added'},
             {'path': [1], 'value': 4, 'action': 'unordered_iterable_item_added'},
             {'path': [2], 'value': 4, 'action': 'unordered_iterable_item_added'},
             {'path': [5], 'value': 4, 'action': 'unordered_iterable_item_added'},
             {'path': [6], 'value': 6, 'action': 'unordered_iterable_item_removed'},
             {'path': [0], 'value': 5, 'action': 'unordered_iterable_item_removed'},
         ]
+        flat_expected1 = [FlatDeltaRow(**i) for i in flat_expected1]
         assert flat_expected1 == flat_result1
 
-        delta1_again = Delta(flat_dict_list=flat_expected1)
+        delta1_again = Delta(flat_rows_list=flat_expected1)
         assert t1_plus_delta1 == t1 + delta1_again
         assert delta1.diff == delta1_again.diff
 
-        flat_result2 = delta2.to_flat_dicts()
+        flat_result2 = delta2.to_flat_rows()
         flat_expected2 = [
             {'path': [1], 'value': 4, 'action': 'unordered_iterable_item_added'},
             {'path': [2], 'value': 4, 'action': 'unordered_iterable_item_added'},
             {'path': [5], 'value': 4, 'action': 'unordered_iterable_item_added'},
             {'path': [6], 'action': 'values_changed', 'value': 7},
             {'path': [0], 'action': 'values_changed', 'value': 8},
         ]
+        flat_expected2 = [FlatDeltaRow(**i) for i in flat_expected2]
         assert flat_expected2 == flat_result2
 
-        delta2_again = Delta(flat_dict_list=flat_expected2)
+        delta2_again = Delta(flat_rows_list=flat_expected2)
         assert delta2.diff == delta2_again.diff
 
     def test_delta_view_and_to_delta_dict_are_equal_when_parameteres_passed(self):
         """
         This is a test that passes parameters in a dictionary instead of kwargs.
         Note that when parameters are passed as a dictionary, all of them even the ones that
         have default values need to be passed.
@@ -1391,27 +1560,31 @@
 
         diff = DeepDiff(t1, t2)
 
         delta2 = Delta(diff, raise_errors=False)
         t4 = delta2 + t3
         assert [] == t4
 
-        flat_result2 = delta2.to_flat_dicts()
+        flat_result2 = delta2.to_flat_rows()
         flat_expected2 = [{'path': [1, 2, 0], 'action': 'values_changed', 'value': 5}]
+        flat_expected2 = [FlatDeltaRow(**i) for i in flat_expected2]
+
         assert flat_expected2 == flat_result2
 
-        delta2_again = Delta(flat_dict_list=flat_expected2)
+        delta2_again = Delta(flat_rows_list=flat_expected2)
         assert delta2.diff == delta2_again.diff
 
         delta3 = Delta(diff, raise_errors=False, bidirectional=True)
-        flat_result3 = delta3.to_flat_dicts()
+        flat_result3 = delta3.to_flat_rows()
         flat_expected3 = [{'path': [1, 2, 0], 'action': 'values_changed', 'value': 5, 'old_value': 4}]
+        flat_expected3 = [FlatDeltaRow(**i) for i in flat_expected3]
+
         assert flat_expected3 == flat_result3
 
-        delta3_again = Delta(flat_dict_list=flat_expected3)
+        delta3_again = Delta(flat_rows_list=flat_expected3)
         assert delta3.diff == delta3_again.diff
 
     def test_apply_delta_to_incompatible_object7_type_change(self):
         t1 = ['1']
         t2 = [1]
         t3 = ['a']
 
@@ -1507,19 +1680,21 @@
         diff = DeepDiff(t1, t2, ignore_order=True, report_repetition=True)
         delta = Delta(diff, raise_errors=False, bidirectional=False)
 
         result = delta.to_dict()
         expected = {'iterable_items_removed_at_indexes': {'root': {2: 'B'}}}
         assert expected == result
 
-        flat_result = delta.to_flat_dicts()
+        flat_result = delta.to_flat_rows()
         flat_expected = [{'action': 'unordered_iterable_item_removed', 'path': [2], 'value': 'B'}]
+        flat_expected = [FlatDeltaRow(**i) for i in flat_expected]
+
         assert flat_expected == flat_result
 
-        delta_again = Delta(flat_dict_list=flat_expected)
+        delta_again = Delta(flat_rows_list=flat_expected)
         assert delta.diff == delta_again.diff
 
     def test_class_type_change(self):
         t1 = CustomClass
         t2 = CustomClass2
         diff = DeepDiff(t1, t2, view=DELTA_VIEW)
         expected = {'type_changes': {'root': {'new_type': CustomClass2,
@@ -1562,46 +1737,52 @@
         t1 = {"a": None}
         t2 = {"a": 1}
 
         dump = Delta(DeepDiff(t1, t2)).dumps()
         delta = Delta(dump)
         assert t2 == delta + t1
 
-        flat_result = delta.to_flat_dicts()
+        flat_result = delta.to_flat_rows()
         flat_expected = [{'path': ['a'], 'action': 'type_changes', 'value': 1, 'type': int, 'old_type': type(None)}]
+        flat_expected = [FlatDeltaRow(**i) for i in flat_expected]
+
         assert flat_expected == flat_result
 
-        delta_again = Delta(flat_dict_list=flat_expected)
+        delta_again = Delta(flat_rows_list=flat_expected)
         assert delta.diff == delta_again.diff
 
         with pytest.raises(ValueError) as exc_info:
-            delta.to_flat_dicts(report_type_changes=False)
+            delta.to_flat_rows(report_type_changes=False)
         assert str(exc_info.value).startswith("When converting to flat dictionaries, if report_type_changes=False and there are type")
         delta2 = Delta(dump, always_include_values=True)
-        flat_result2 = delta2.to_flat_dicts(report_type_changes=False)
+        flat_result2 = delta2.to_flat_rows(report_type_changes=False)
         flat_expected2 = [{'path': ['a'], 'action': 'values_changed', 'value': 1}]
+        flat_expected2 = [FlatDeltaRow(**i) for i in flat_expected2]
+
         assert flat_expected2 == flat_result2
 
     def test_delta_set_in_objects(self):
         t1 = [[1, OrderedSet(['A', 'B'])], {1}]
         t2 = [[2, OrderedSet([10, 'C', 'B'])], {1}]
         delta = Delta(DeepDiff(t1, t2))
-        flat_result = delta.to_flat_dicts()
+        flat_result = delta.to_flat_rows()
         flat_expected = [
             {'path': [0, 1], 'value': 10, 'action': 'set_item_added'},
             {'path': [0, 0], 'action': 'values_changed', 'value': 2},
             {'path': [0, 1], 'value': 'A', 'action': 'set_item_removed'},
             {'path': [0, 1], 'value': 'C', 'action': 'set_item_added'},
         ]
+        flat_expected = [FlatDeltaRow(**i) for i in flat_expected]
+
         # Sorting because otherwise the order is not deterministic for sets,
         # even though we are using OrderedSet here. It still is converted to set at some point and loses its order.
-        flat_result.sort(key=lambda x: str(x['value']))
+        flat_result.sort(key=lambda x: str(x.value))
         assert flat_expected == flat_result
 
-        delta_again = Delta(flat_dict_list=flat_expected)
+        delta_again = Delta(flat_rows_list=flat_expected)
         assert delta.diff == delta_again.diff
 
     def test_delta_with_json_serializer(self):
         t1 = {"a": 1}
         t2 = {"a": 2}
 
         diff = DeepDiff(t1, t2)
@@ -1698,26 +1879,28 @@
             }
         }
         assert expected == ddiff
         delta = Delta(ddiff)
         recreated_t2 = t1 + delta
         assert t2 == recreated_t2
 
-        flat_result = delta.to_flat_dicts()
+        flat_result = delta.to_flat_rows()
         flat_expected = [
             {'path': [2], 'value': {'id': 1, 'val': 3}, 'action': 'iterable_item_removed'},
             {'path': [0], 'value': {'id': 1, 'val': 3}, 'action': 'iterable_item_removed'},
             {'path': [3], 'value': {'id': 3, 'val': 3}, 'action': 'iterable_item_removed'},
-            {'path': [0], 'action': 'iterable_item_moved', 'value': {'id': 1, 'val': 3}, 'new_path': [2]},
+        {'path': [0], 'action': 'iterable_item_moved', 'value': {'id': 1, 'val': 3}, 'new_path': [2]},
             {'path': [3], 'action': 'iterable_item_moved', 'value': {'id': 3, 'val': 3}, 'new_path': [0]},
         ]
+        flat_expected = [FlatDeltaRow(**i) for i in flat_expected]
+
         assert flat_expected == flat_result
 
         # Delta.DEBUG = True
-        delta_again = Delta(flat_dict_list=flat_expected, iterable_compare_func_was_used=True)
+        delta_again = Delta(flat_rows_list=flat_expected, iterable_compare_func_was_used=True)
         expected_delta_dict = {
             'iterable_item_removed': {
                 'root[2]': {
                     'id': 1,
                     'val': 3
                 },
                 'root[0]': {
@@ -1899,175 +2082,195 @@
         assert expected == result
 
     def test_flatten_dict_with_one_key_added(self):
         t1 = {"field1": {"joe": "Joe"}}
         t2 = {"field1": {"joe": "Joe Nobody"}, "field2": {"jimmy": "Jimmy"}}
         diff = DeepDiff(t1, t2)
         delta = Delta(diff=diff, always_include_values=True)
-        flat_result = delta.to_flat_dicts(report_type_changes=False)
+        flat_result = delta.to_flat_rows(report_type_changes=False)
         flat_expected = [
             {'path': ['field2', 'jimmy'], 'value': 'Jimmy', 'action': 'dictionary_item_added'},
             {'path': ['field1', 'joe'], 'action': 'values_changed', 'value': 'Joe Nobody'},
         ]
+        flat_expected = [FlatDeltaRow(**i) for i in flat_expected]
         assert flat_expected == flat_result
 
-        delta_again = Delta(flat_dict_list=flat_expected, force=True)  # We need to enable force so it creates the dictionary when added to t1
+        delta_again = Delta(flat_rows_list=flat_expected, force=True)  # We need to enable force so it creates the dictionary when added to t1
         expected_data_again_diff = {'dictionary_item_added': {"root['field2']['jimmy']": 'Jimmy'}, 'values_changed': {"root['field1']['joe']": {'new_value': 'Joe Nobody'}}}
 
         assert delta.diff != delta_again.diff, "Since a dictionary containing a single field was created, the flat dict acted like one key was added."
         assert expected_data_again_diff == delta_again.diff, "Since a dictionary containing a single field was created, the flat dict acted like one key was added."
 
         assert t2 == t1 + delta_again
 
     def test_flatten_dict_with_multiple_keys_added(self):
         t1 = {"field1": {"joe": "Joe"}}
         t2 = {"field1": {"joe": "Joe Nobody"}, "field2": {"jimmy": "Jimmy", "sar": "Sarah"}}
         diff = DeepDiff(t1, t2)
         delta = Delta(diff=diff, always_include_values=True)
-        flat_result = delta.to_flat_dicts(report_type_changes=False)
+        flat_result = delta.to_flat_rows(report_type_changes=False)
         flat_expected = [
             {'path': ['field2'], 'value': {'jimmy': 'Jimmy', 'sar': 'Sarah'}, 'action': 'dictionary_item_added'},
             {'path': ['field1', 'joe'], 'action': 'values_changed', 'value': 'Joe Nobody'},
         ]
+        flat_expected = [FlatDeltaRow(**i) for i in flat_expected]
         assert flat_expected == flat_result
 
-        delta_again = Delta(flat_dict_list=flat_expected)
+        delta_again = Delta(flat_rows_list=flat_expected)
         assert delta.diff == delta_again.diff
 
     def test_flatten_list_with_one_item_added(self):
         t1 = {"field1": {"joe": "Joe"}}
         t2 = {"field1": {"joe": "Joe"}, "field2": ["James"]}
         t3 = {"field1": {"joe": "Joe"}, "field2": ["James", "Jack"]}
         diff = DeepDiff(t1, t2)
         delta = Delta(diff=diff, always_include_values=True)
-        flat_result = delta.to_flat_dicts(report_type_changes=False)
+        flat_result = delta.to_flat_rows(report_type_changes=False)
         flat_expected = [{'path': ['field2', 0], 'value': 'James', 'action': 'iterable_item_added'}]
+        flat_expected = [FlatDeltaRow(**i) for i in flat_expected]
         assert flat_expected == flat_result
 
-        delta_again = Delta(flat_dict_list=flat_expected, force=True)
+        delta_again = Delta(flat_rows_list=flat_expected, force=True)
         assert {'iterable_item_added': {"root['field2'][0]": 'James'}} == delta_again.diff
         # delta_again.DEBUG = True
         assert t2 == t1 + delta_again
 
         diff2 = DeepDiff(t2, t3)
         delta2 = Delta(diff=diff2, always_include_values=True)
-        flat_result2 = delta2.to_flat_dicts(report_type_changes=False)
+        flat_result2 = delta2.to_flat_rows(report_type_changes=False)
         flat_expected2 = [{'path': ['field2', 1], 'value': 'Jack', 'action': 'iterable_item_added'}]
+        flat_expected2 = [FlatDeltaRow(**i) for i in flat_expected2]
+
         assert flat_expected2 == flat_result2
 
-        delta_again2 = Delta(flat_dict_list=flat_expected2, force=True)
+        delta_again2 = Delta(flat_rows_list=flat_expected2, force=True)
 
         assert {'iterable_item_added': {"root['field2'][1]": 'Jack'}} == delta_again2.diff
         assert t3 == t2 + delta_again2
 
     def test_flatten_set_with_one_item_added(self):
         t1 = {"field1": {"joe": "Joe"}}
         t2 = {"field1": {"joe": "Joe"}, "field2": {"James"}}
         t3 = {"field1": {"joe": "Joe"}, "field2": {"James", "Jack"}}
         diff = DeepDiff(t1, t2)
         delta = Delta(diff=diff, always_include_values=True)
         assert t2 == t1 + delta
-        flat_result = delta.to_flat_dicts(report_type_changes=False)
+        flat_result = delta.to_flat_rows(report_type_changes=False)
         flat_expected = [{'path': ['field2'], 'value': 'James', 'action': 'set_item_added'}]
+        flat_expected = [FlatDeltaRow(**i) for i in flat_expected]
         assert flat_expected == flat_result
 
-        delta_again = Delta(flat_dict_list=flat_expected, force=True)
+        delta_again = Delta(flat_rows_list=flat_expected, force=True)
         assert {'set_item_added': {"root['field2']": {'James'}}} == delta_again.diff
         assert t2 == t1 + delta_again
 
         diff = DeepDiff(t2, t3)
         delta2 = Delta(diff=diff, always_include_values=True)
-        flat_result2 = delta2.to_flat_dicts(report_type_changes=False)
+        flat_result2 = delta2.to_flat_rows(report_type_changes=False)
         flat_expected2 = [{'path': ['field2'], 'value': 'Jack', 'action': 'set_item_added'}]
+        flat_expected2 = [FlatDeltaRow(**i) for i in flat_expected2]
+
         assert flat_expected2 == flat_result2
 
-        delta_again2 = Delta(flat_dict_list=flat_expected2, force=True)
+        delta_again2 = Delta(flat_rows_list=flat_expected2, force=True)
         assert {'set_item_added': {"root['field2']": {'Jack'}}} == delta_again2.diff
         assert t3 == t2 + delta_again2
 
     def test_flatten_tuple_with_one_item_added(self):
         t1 = {"field1": {"joe": "Joe"}}
         t2 = {"field1": {"joe": "Joe"}, "field2": ("James", )}
         t3 = {"field1": {"joe": "Joe"}, "field2": ("James", "Jack")}
         diff = DeepDiff(t1, t2)
         delta = Delta(diff=diff, always_include_values=True)
         assert t2 == t1 + delta
-        flat_expected = delta.to_flat_dicts(report_type_changes=False)
+        flat_expected = delta.to_flat_rows(report_type_changes=False)
         expected_result = [{'path': ['field2', 0], 'value': 'James', 'action': 'iterable_item_added'}]
+        expected_result = [FlatDeltaRow(**i) for i in expected_result]
+
         assert expected_result == flat_expected
 
-        delta_again = Delta(flat_dict_list=flat_expected, force=True)
+        delta_again = Delta(flat_rows_list=flat_expected, force=True)
         assert {'iterable_item_added': {"root['field2'][0]": 'James'}} == delta_again.diff
         assert {'field1': {'joe': 'Joe'}, 'field2': ['James']} == t1 + delta_again, "We lost the information about tuple when we convert to flat dict."
 
         diff = DeepDiff(t2, t3)
         delta2 = Delta(diff=diff, always_include_values=True, force=True)
-        flat_result2 = delta2.to_flat_dicts(report_type_changes=False)
+        flat_result2 = delta2.to_flat_rows(report_type_changes=False)
         expected_result2 = [{'path': ['field2', 1], 'value': 'Jack', 'action': 'iterable_item_added'}]
+        expected_result2 = [FlatDeltaRow(**i) for i in expected_result2]
+
         assert expected_result2 == flat_result2
         assert t3 == t2 + delta2
 
-        delta_again2 = Delta(flat_dict_list=flat_result2)
+        delta_again2 = Delta(flat_rows_list=flat_result2)
         assert {'iterable_item_added': {"root['field2'][1]": 'Jack'}} == delta_again2.diff
         assert t3 == t2 + delta_again2
 
     def test_flatten_list_with_multiple_item_added(self):
         t1 = {"field1": {"joe": "Joe"}}
         t2 = {"field1": {"joe": "Joe"}, "field2": ["James", "Jack"]}
         diff = DeepDiff(t1, t2)
         delta = Delta(diff=diff, always_include_values=True)
-        flat_result = delta.to_flat_dicts(report_type_changes=False)
+        flat_result = delta.to_flat_rows(report_type_changes=False)
         expected_result = [{'path': ['field2'], 'value': ['James', 'Jack'], 'action': 'dictionary_item_added'}]
+        expected_result = [FlatDeltaRow(**i) for i in expected_result]
+
         assert expected_result == flat_result
 
         delta2 = Delta(diff=diff, bidirectional=True, always_include_values=True)
-        flat_result2 = delta2.to_flat_dicts(report_type_changes=False)
+        flat_result2 = delta2.to_flat_rows(report_type_changes=False)
         assert expected_result == flat_result2
 
-        delta_again = Delta(flat_dict_list=flat_result)
+        delta_again = Delta(flat_rows_list=flat_result)
         assert delta.diff == delta_again.diff
 
     def test_flatten_attribute_added(self):
         t1 = picklalbe_obj_without_item
         t2 = PicklableClass(10)
         diff = DeepDiff(t1, t2)
         delta = Delta(diff=diff, always_include_values=True)
-        flat_result = delta.to_flat_dicts(report_type_changes=False)
+        flat_result = delta.to_flat_rows(report_type_changes=False)
         expected_result = [{'path': ['item'], 'value': 10, 'action': 'attribute_added'}]
+        expected_result = [FlatDeltaRow(**i) for i in expected_result]
+
         assert expected_result == flat_result
 
-        delta_again = Delta(flat_dict_list=flat_result)
+        delta_again = Delta(flat_rows_list=flat_result)
         assert delta.diff == delta_again.diff
 
     def test_flatten_when_simple_type_change(self):
         t1 = [1, 2, '3']
         t2 = [1, 2, 3]
 
         diff = DeepDiff(t1, t2)
         expected_diff = {
             'type_changes': {'root[2]': {'old_type': str, 'new_type': int, 'old_value': '3', 'new_value': 3}}
         }
 
         assert expected_diff == diff
         delta = Delta(diff=diff)
         with pytest.raises(ValueError) as exc_info:
-            delta.to_flat_dicts(report_type_changes=False)
+            delta.to_flat_rows(report_type_changes=False)
         assert str(exc_info.value).startswith("When converting to flat dictionaries")
 
         delta2 = Delta(diff=diff, always_include_values=True)
-        flat_result2 = delta2.to_flat_dicts(report_type_changes=False)
+        flat_result2 = delta2.to_flat_rows(report_type_changes=False)
         expected_result2 = [{'path': [2], 'action': 'values_changed', 'value': 3}]
+        expected_result2 = [FlatDeltaRow(**i) for i in expected_result2]
+
         assert expected_result2 == flat_result2
 
         delta3 = Delta(diff=diff, always_include_values=True, bidirectional=True)
-        flat_result3 = delta3.to_flat_dicts(report_type_changes=False)
+        flat_result3 = delta3.to_flat_rows(report_type_changes=False)
+
         expected_result3 = [{'path': [2], 'action': 'values_changed', 'value': 3, 'old_value': '3'}]
+        expected_result3 = [FlatDeltaRow(**i) for i in expected_result3]
         assert expected_result3 == flat_result3
 
-        delta_again = Delta(flat_dict_list=flat_result3)
+        delta_again = Delta(flat_rows_list=flat_result3)
         assert {'values_changed': {'root[2]': {'new_value': 3, 'old_value': '3'}}} == delta_again.diff
 
     def test_subtract_delta1(self):
         t1 = {'field_name1': ['yyy']}
         t2 = {'field_name1': ['xxx', 'yyy']}
         delta_diff = {'iterable_items_removed_at_indexes': {"root['field_name1']": {(0, 'GET'): 'xxx'}}}
         expected_reverse_diff = {'iterable_items_added_at_indexes': {"root['field_name1']": {(0, 'GET'): 'xxx'}}}
@@ -2078,57 +2281,225 @@
         assert t2 != {'field_name1': ['yyy', 'xxx']} == t1 - delta, "Since iterable_items_added_at_indexes is used when ignore_order=True, the order is not necessarily the original order."
 
     def test_subtract_delta_made_from_flat_dicts1(self):
         t1 = {'field_name1': ['xxx', 'yyy']}
         t2 = {'field_name1': []}
         diff = DeepDiff(t1, t2)
         delta = Delta(diff=diff, bidirectional=True)
-        flat_dict_list = delta.to_flat_dicts(include_action_in_path=False, report_type_changes=True)
+        flat_rows_list = delta.to_flat_rows(include_action_in_path=False, report_type_changes=True)
         expected_flat_dicts = [{
             'path': ['field_name1', 0],
             'value': 'xxx',
             'action': 'iterable_item_removed'
         }, {
             'path': ['field_name1', 1],
             'value': 'yyy',
             'action': 'iterable_item_removed'
         }]
-        assert expected_flat_dicts == flat_dict_list
+        expected_flat_dicts = [FlatDeltaRow(**i) for i in expected_flat_dicts]
 
-        delta1 = Delta(flat_dict_list=flat_dict_list, bidirectional=True, force=True)
+        assert expected_flat_dicts == flat_rows_list
+
+        delta1 = Delta(flat_rows_list=flat_rows_list, bidirectional=True, force=True)
         assert t1 == t2 - delta1
 
-        delta2 = Delta(flat_dict_list=[flat_dict_list[0]], bidirectional=True, force=True)
+        delta2 = Delta(flat_rows_list=[flat_rows_list[0]], bidirectional=True, force=True)
         middle_t = t2 - delta2
         assert {'field_name1': ['xxx']} == middle_t
 
-        delta3 = Delta(flat_dict_list=[flat_dict_list[1]], bidirectional=True, force=True)
+        delta3 = Delta(flat_rows_list=[flat_rows_list[1]], bidirectional=True, force=True)
         assert t1 == middle_t - delta3
 
     def test_subtract_delta_made_from_flat_dicts2(self):
         t1 = {'field_name1': []}
         t2 = {'field_name1': ['xxx', 'yyy']}
         diff = DeepDiff(t1, t2)
         delta = Delta(diff=diff, bidirectional=True)
-        flat_dict_list = delta.to_flat_dicts(include_action_in_path=False, report_type_changes=True)
+        flat_rows_list = delta.to_flat_rows(include_action_in_path=False, report_type_changes=True)
         expected_flat_dicts = [{
             'path': ['field_name1', 0],
             'value': 'xxx',
             'action': 'iterable_item_added'
         }, {
             'path': ['field_name1', 1],
             'value': 'yyy',
             'action': 'iterable_item_added'
         }]
-        assert expected_flat_dicts == flat_dict_list
+        expected_flat_dicts = [FlatDeltaRow(**i) for i in expected_flat_dicts]
+
+        assert expected_flat_dicts == flat_rows_list
 
-        delta1 = Delta(flat_dict_list=flat_dict_list, bidirectional=True, force=True)
+        delta1 = Delta(flat_rows_list=flat_rows_list, bidirectional=True, force=True)
         assert t1 == t2 - delta1
 
         # We need to subtract the changes in the reverse order if we want to feed the flat dict rows individually to Delta
-        delta2 = Delta(flat_dict_list=[flat_dict_list[0]], bidirectional=True, force=True)
+        delta2 = Delta(flat_rows_list=[flat_rows_list[0]], bidirectional=True, force=True)
         middle_t = t2 - delta2
         assert {'field_name1': ['yyy']} == middle_t
 
-        delta3 = Delta(flat_dict_list=[flat_dict_list[1]], bidirectional=True, force=True)
+        delta3 = Delta(flat_rows_list=[flat_rows_list[1]], bidirectional=True, force=True)
         delta3.DEBUG = True
         assert t1 == middle_t - delta3
+
+    def test_list_of_alphabet_and_its_delta(self):
+        l1 = "A B C D E F G D H".split()
+        l2 = "B C X D H Y Z".split()
+        diff = DeepDiff(l1, l2)
+
+        # Problem: The index of values_changed should be either all for AFTER removals or BEFORE removals.
+        # What we have here is that F & G transformation to Y and Z is not compatible with A and E removal
+        # it is really meant for the removals to happen first, and then have indexes in L2 for values changing
+        # rather than indexes in L1. Here what we need to have is:
+        # A B C D E F G D H
+        # A B C-X-E 
+        # B C D F G D H  # removal
+
+        # What we really need is to report is as it is in difflib for delta specifically:
+        # A B C D E F G D H
+        # B C D E F G D H     delete    t1[0:1] --> t2[0:0]    ['A'] --> []
+        # B C D E F G D H     equal     t1[1:3] --> t2[0:2] ['B', 'C'] --> ['B', 'C']
+        # B C X D H           replace   t1[3:7] --> t2[2:3] ['D', 'E', 'F', 'G'] --> ['X']
+        # B C X D H           equal     t1[7:9] --> t2[3:5] ['D', 'H'] --> ['D', 'H']
+        # B C X D H Y Z       insert    t1[9:9] --> t2[5:7]       [] --> ['Y', 'Z']
+
+        # So in this case, it needs to also include information about what stays equal in the delta
+        # NOTE: the problem is that these operations need to be performed in a specific order.
+        # DeepDiff removes that order and just buckets all insertions vs. replace vs. delete in their own buckets.
+        # For times that we use Difflib, we may want to keep the information for the array_change key
+        # just for the sake of delta, but not for reporting in deepdiff itself.
+        # that way we can re-apply the changes as they were reported in delta.
+
+        delta = Delta(diff)
+        assert l2 == l1 + delta
+        with pytest.raises(ValueError) as exc_info:
+            l1 == l2 - delta
+        assert "Please recreate the delta with bidirectional=True" == str(exc_info.value)
+
+        delta2 = Delta(diff, bidirectional=True)
+        assert l2 == l1 + delta2
+        assert l1 == l2 - delta2
+
+        dump = Delta(diff, bidirectional=True).dumps()
+        delta3 = Delta(dump, bidirectional=True)
+
+        assert l2 == l1 + delta3
+        assert l1 == l2 - delta3
+
+        dump4 = Delta(diff, bidirectional=True, serializer=json_dumps).dumps()
+        delta4 = Delta(dump4, bidirectional=True, deserializer=json_loads)
+
+        assert l2 == l1 + delta4
+        assert l1 == l2 - delta4
+
+    def test_delta_flat_rows(self):
+        t1 = {"key1": "value1"}
+        t2 = {"field2": {"key2": "value2"}}
+        diff = DeepDiff(t1, t2, verbose_level=2)
+        delta = Delta(diff, bidirectional=True)
+        assert t1 + delta == t2
+        flat_rows = delta.to_flat_rows()
+        # we need to set force=True because when we create flat rows, if a nested
+        # dictionary with a single key is created, the path in the flat row will be
+        # the path to the leaf node.
+        delta2 = Delta(flat_rows_list=flat_rows, bidirectional=True, force=True)
+        assert t1 + delta2 == t2
+
+    def test_flat_dict_and_deeply_nested_dict(self):
+        beforeImage = [
+            {
+                "usage": "Mailing",
+                "standardization": "YES",
+                "primaryIndicator": True,
+                "addressIdentifier": "Z8PDWBG42YC",
+                "addressLines": ["871 PHILLIPS FERRY RD"],
+            },
+            {
+                "usage": "Residence",
+                "standardization": "YES",
+                "primaryIndicator": False,
+                "addressIdentifier": "Z8PDWBG42YC",
+                "addressLines": ["871 PHILLIPS FERRY RD"],
+            },
+            {
+                "usage": "Mailing",
+                "standardization": None,
+                "primaryIndicator": False,
+                "addressIdentifier": "MHPP3BY0BYC",
+                "addressLines": ["871 PHILLIPS FERRY RD", "APT RV92"],
+            },
+        ]
+        allAfterImage = [
+            {
+                "usage": "Residence",
+                "standardization": "NO",
+                "primaryIndicator": False,
+                "addressIdentifier": "Z8PDWBG42YC",
+                "addressLines": ["871 PHILLIPS FERRY RD"],
+            },
+            {
+                "usage": "Mailing",
+                "standardization": None,
+                "primaryIndicator": False,
+                "addressIdentifier": "MHPP3BY0BYC",
+                "addressLines": ["871 PHILLIPS FERRY RD", "APT RV92"],
+            },
+            {
+                "usage": "Mailing",
+                "standardization": "NO",
+                "primaryIndicator": True,
+                "addressIdentifier": "Z8PDWBG42YC",
+                "addressLines": ["871 PHILLIPS FERRY RD"],
+            },
+        ]
+
+        diff = DeepDiff(
+            beforeImage,
+            allAfterImage,
+            ignore_order=True,
+            report_repetition=True,
+        )
+        # reverse_diff = DeepDiff(
+        #     allAfterImage,
+        #     beforeImage,
+        #     ignore_order=True,
+        #     report_repetition=True,
+        # )
+        delta = Delta(
+            diff, always_include_values=True, bidirectional=True
+        )
+        # reverse_delta = Delta(
+        #     reverse_diff, always_include_values=True, bidirectional=True
+        # )
+        allAfterImageAgain = beforeImage + delta
+        diff2 = DeepDiff(allAfterImage, allAfterImageAgain, ignore_order=True)
+        assert not diff2
+
+        # print("\ndelta.diff")
+        # pprint(delta.diff)
+        # print("\ndelta._get_reverse_diff()")
+        # pprint(delta._get_reverse_diff())
+        # print("\nreverse_delta.diff")
+        # pprint(reverse_delta.diff)
+        beforeImageAgain = allAfterImage - delta
+        diff3 = DeepDiff(beforeImage, beforeImageAgain, ignore_order=True)
+        assert not diff3
+
+        # ------ now let's recreate the delta from flat dicts -------
+
+        flat_dict_list = delta.to_flat_dicts()
+
+        delta2 = Delta(
+            flat_dict_list=flat_dict_list,
+            always_include_values=True,
+            bidirectional=True,
+            raise_errors=False,
+            force=True,
+        )
+        # print("\ndelta from flat dicts")
+        # pprint(delta2.diff)
+        allAfterImageAgain2 = beforeImage + delta2
+        diff4 = DeepDiff(allAfterImage, allAfterImageAgain2, ignore_order=True)
+        assert not diff4
+
+        beforeImageAgain2 = allAfterImage - delta2
+        diff4 = DeepDiff(beforeImage, beforeImageAgain2, ignore_order=True)
+        assert not diff4
```

### Comparing `deepdiff-6.7.1/tests/test_diff_datetime.py` & `deepdiff-7.0.0/tests/test_diff_datetime.py`

 * *Files identical despite different names*

### Comparing `deepdiff-6.7.1/tests/test_diff_math.py` & `deepdiff-7.0.0/tests/test_diff_math.py`

 * *Files identical despite different names*

### Comparing `deepdiff-6.7.1/tests/test_diff_numpy.py` & `deepdiff-7.0.0/tests/test_diff_numpy.py`

 * *Files 3% similar despite different names*

```diff
@@ -115,14 +115,20 @@
     },
     'numpy_almost_equal': {
         't1': np.array([1.0, 2.3333333333333]),
         't2': np.array([1.0, 2.33333334]),
         'deepdiff_kwargs': {'significant_digits': 3},
         'expected_result': {},
     },
+    'numpy_almost_equal2': {
+        't1': np.array(['a', 'b'], dtype=object),
+        't2': np.array(['a', 'b'], dtype=object),
+        'deepdiff_kwargs': {'significant_digits': 6},
+        'expected_result': {},
+    },
     'numpy_different_shape': {
         't1': np.array([[1, 1], [2, 3]]),
         't2': np.array([1]),
         'deepdiff_kwargs': {},
         'expected_result': {
             'type_changes': {
                 'root[0]': {
```

### Comparing `deepdiff-6.7.1/tests/test_diff_other.py` & `deepdiff-7.0.0/tests/test_diff_other.py`

 * *Files identical despite different names*

### Comparing `deepdiff-6.7.1/tests/test_diff_text.py` & `deepdiff-7.0.0/tests/test_diff_text.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import uuid
 from enum import Enum
 from typing import List
 from decimal import Decimal
 from deepdiff import DeepDiff
 from deepdiff.helper import pypy3, PydanticBaseModel
 from tests import CustomClass
+from deepdiff.helper import np_float64
 
 
 logging.disable(logging.CRITICAL)
 
 
 class TestDeepDiffText:
     """DeepDiff Tests."""
@@ -293,14 +294,36 @@
         result = {'values_changed': {'root': {'new_value': 'hello', 'old_value': 'Hello'}}}
         assert result == ddiff
 
         ddiff = DeepDiff(t1, t2, ignore_string_case=True)
         result = {}
         assert result == ddiff
 
+    def test_string_dict_key_ignore_case(self):
+        t1 = {'User': {'AboutMe': 1, 'ALIAS': 1}}
+        t2 = {'User': {'Alias': 1, 'AboutMe': 1}}
+        ddiff = DeepDiff(t1, t2)
+        result = {'dictionary_item_added': ["root['User']['Alias']"], 'dictionary_item_removed': ["root['User']['ALIAS']"]}
+        assert result == ddiff
+
+        ddiff = DeepDiff(t1, t2, ignore_string_case=True)
+        result = {}
+        assert result == ddiff
+
+    def test_string_list_ignore_case(self):
+        t1 = ['AboutMe', 'ALIAS']
+        t2 = ['aboutme', 'alias']
+        ddiff = DeepDiff(t1, t2)
+        result = {'values_changed': {'root[0]': {'new_value': 'aboutme', 'old_value': 'AboutMe'}, 'root[1]': {'new_value': 'alias', 'old_value': 'ALIAS'}}}
+        assert result == ddiff
+
+        ddiff = DeepDiff(t1, t2, ignore_string_case=True)
+        result = {}
+        assert result == ddiff
+
     def test_diff_quote_in_string(self):
         t1 = {
             "a']['b']['c": 1
         }
         t2 = {
             "a']['b']['c": 2
         }
@@ -620,14 +643,35 @@
                     'old_value': 1,
                     'new_value': 2
                 },
             }
         }
         assert ddiff == result
 
+    def test_enum_ignore_type_change(self):
+
+        class MyEnum1(Enum):
+            book = "book"
+            cake = "cake"
+
+        class MyEnum2(str, Enum):
+            book = "book"
+            cake = "cake"
+
+        diff = DeepDiff("book", MyEnum1.book)
+        expected = {
+            'type_changes': {'root': {'old_type': str, 'new_type': MyEnum1, 'old_value': 'book', 'new_value': MyEnum1.book}}}
+        assert expected == diff
+
+        diff2 = DeepDiff("book", MyEnum1.book, ignore_type_in_groups=[(Enum, str)])
+        assert not diff2
+
+        diff3 = DeepDiff("book", MyEnum2.book, ignore_type_in_groups=[(Enum, str)])
+        assert not diff3
+
     def test_precompiled_regex(self):
 
         pattern_1 = re.compile('foo')
         pattern_2 = re.compile('foo')
         pattern_3 = re.compile('foo', flags=re.I)
         pattern_4 = re.compile('(foo)')
         pattern_5 = re.compile('bar')
@@ -785,19 +829,19 @@
 
         class ClassC(ClassB):
             def __repr__(self):
                 return "obj c"
 
         obj_a = ClassA(1, 2)
         obj_c = ClassC(3)
-        ddiff = DeepDiff(obj_a, obj_c, ignore_type_in_groups=[(ClassA, ClassB)], ignore_type_subclasses=False)
+        ddiff = DeepDiff(obj_a, obj_c, ignore_type_in_groups=[(ClassA, ClassB)], ignore_type_subclasses=True)
         result = {'type_changes': {'root': {'old_type': ClassA, 'new_type': ClassC, 'old_value': obj_a, 'new_value': obj_c}}}
         assert result == ddiff
 
-        ddiff = DeepDiff(obj_a, obj_c, ignore_type_in_groups=[(ClassA, ClassB)], ignore_type_subclasses=True)
+        ddiff = DeepDiff(obj_a, obj_c, ignore_type_in_groups=[(ClassA, ClassB)], ignore_type_subclasses=False)
         result = {'values_changed': {'root.x': {'new_value': 3, 'old_value': 1}}, 'attribute_removed': ['root.y']}
         assert result == ddiff
 
     def test_custom_objects_slot_in_parent_class_change(self):
         class ClassA:
             __slots__ = ['x']
 
@@ -1251,14 +1295,15 @@
                                  (Decimal('10.01'), 10.01, 8, {}),
                                  (Decimal('10.010'), 10.01, 3, {}),
                                  (Decimal('100000.1'), 100000.1, 0, {}),
                                  (Decimal('100000.1'), 100000.1, 1, {}),
                                  (Decimal('100000.1'), 100000.1, 5, {}),
                                  (Decimal('100000'), 100000.1, 0, {}),
                                  (Decimal('100000'), 100000.1, 1, {'values_changed': {'root': {'new_value': 100000.1, 'old_value': Decimal('100000')}}}),
+                                 (np_float64(123.93420232), 123.93420232, 0, {}),
                              ])
     def test_decimal_digits(self, t1, t2, significant_digits, expected_result):
         ddiff = DeepDiff(t1, t2, ignore_numeric_type_changes=True, ignore_string_type_changes=True, significant_digits=significant_digits)
         assert expected_result == ddiff
 
     def test_ignore_type_in_groups(self):
         t1 = [1, 2, 3]
```

### Comparing `deepdiff-6.7.1/tests/test_diff_tree.py` & `deepdiff-7.0.0/tests/test_diff_tree.py`

 * *Files identical despite different names*

### Comparing `deepdiff-6.7.1/tests/test_distance.py` & `deepdiff-7.0.0/tests/test_distance.py`

 * *Files identical despite different names*

### Comparing `deepdiff-6.7.1/tests/test_hash.py` & `deepdiff-7.0.0/tests/test_hash.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,14 +82,35 @@
     def test_datetime(self):
         now = datetime.datetime.now()
         a = b = now
         a_hash = DeepHash(a)
         b_hash = DeepHash(b)
         assert a_hash[a] == b_hash[b]
 
+    def test_date1(self):
+        date = datetime.date(2024, 2, 1)
+        date_hash = DeepHash(date)
+        assert 'd90e95901f85ca09b2536d3cb81a49747c3a4fb14906d6fa0d492713ebb4309c' == date_hash[date]
+
+    def test_date2(self):
+        item = {'due_date': datetime.date(2024, 2, 1)}
+
+        result = DeepHash(
+            item,
+            significant_digits=12,
+            number_format_notation='f',
+            ignore_numeric_type_changes=True,
+            ignore_type_in_groups=[{int, float, complex, datetime.datetime, datetime.date, datetime.timedelta, datetime.time}],
+            ignore_type_subclasses=False,
+            ignore_encoding_errors=False,
+            ignore_repetition=True,
+            number_to_string_func=number_to_string,
+        )
+        assert 'e0d7ec984a0eda44ceb1e3c595f9b805530d715c779483e63a72c67cbce68615' == result[item]
+
     def test_datetime_truncate(self):
         a = datetime.datetime(2020, 5, 17, 22, 15, 34, 913070)
         b = datetime.datetime(2020, 5, 17, 22, 15, 39, 296583)
         c = datetime.datetime(2020, 5, 17, 22, 15, 34, 500000)
 
         a_hash = DeepHash(a, truncate_datetime='minute')
         b_hash = DeepHash(b, truncate_datetime='minute')
@@ -470,29 +491,28 @@
     obj_a = ClassA(1, 2)
     obj_b = ClassB(1, 2)
     obj_c = ClassC(1, 2)
 
     burrito = Burrito()
     taco = Taco()
 
-    @pytest.mark.parametrize("t1, t2, ignore_type_in_groups, ignore_type_subclasses, is_qual", [
-        (taco, burrito, [], False, False),
-        (taco, burrito, [(Taco, Burrito)], False, True),
-        ([taco], [burrito], [(Taco, Burrito)], False, True),
-        ([obj_a], [obj_c], [(ClassA, ClassB)], False, False),
-        ([obj_a], [obj_c], [(ClassA, ClassB)], True, True),
-        ([obj_b], [obj_c], [(ClassB, )], True, True),
+    @pytest.mark.parametrize("test_num, t1, t2, ignore_type_in_groups, ignore_type_subclasses, is_qual", [
+        (1, taco, burrito, [], False, False),
+        (2, taco, burrito, [(Taco, Burrito)], False, True),
+        (3, [taco], [burrito], [(Taco, Burrito)], False, True),
+        (4, [obj_a], [obj_c], [(ClassA, ClassB)], False, True),
+        (5, [obj_a], [obj_c], [(ClassA, ClassB)], True, False),
+        (6, [obj_b], [obj_c], [(ClassB, )], True, False),
     ])
-    def test_objects_with_same_content(self, t1, t2, ignore_type_in_groups, ignore_type_subclasses, is_qual):
-
+    def test_objects_with_same_content(self, test_num, t1, t2, ignore_type_in_groups, ignore_type_subclasses, is_qual):
         t1_result = DeepHashPrep(t1, ignore_type_in_groups=ignore_type_in_groups,
                                  ignore_type_subclasses=ignore_type_subclasses)
         t2_result = DeepHashPrep(t2, ignore_type_in_groups=ignore_type_in_groups,
                                  ignore_type_subclasses=ignore_type_subclasses)
-        assert is_qual == (t1_result[t1] == t2_result[t2])
+        assert is_qual == (t1_result[t1] == t2_result[t2]), f"test_objects_with_same_content #{test_num} failed."
 
     def test_custom_object(self):
         cc_a = CustomClass2(prop1=["a"], prop2=["b"])
         t1 = [cc_a, CustomClass2(prop1=["c"], prop2=["d"])]
         t1_result = DeepHashPrep(t1)
         expected = 'list:objCustomClass2:{str:prop1:list:str:a;str:prop2:list:str:b},objCustomClass2:{str:prop1:list:str:c;str:prop2:list:str:d}'  # NOQA
         assert expected == t1_result[t1]
```

### Comparing `deepdiff-6.7.1/tests/test_helper.py` & `deepdiff-7.0.0/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `deepdiff-6.7.1/tests/test_ignore_order.py` & `deepdiff-7.0.0/tests/test_ignore_order.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import pytest
 import re
+import datetime
 from unittest import mock
 from deepdiff.helper import number_to_string, CannotCompare
 from deepdiff import DeepDiff
 from decimal import Decimal
 from deepdiff.deephash import sha256hex
 from tests import CustomClass2
 
@@ -145,15 +146,15 @@
         t2 = [[4, 3, {1: 2}], 2, 1]
 
         ddiff = DeepDiff(t1, t2, ignore_order=True)
 
         result = {}
         assert result == ddiff
 
-    def test_list_difference_ignore_order_report_repetition(self):
+    def test_list_difference_ignore_order_report_repetition1(self):
         t1 = [1, 3, 1, 4]
         t2 = [4, 4, 1]
         ddiff = DeepDiff(t1, t2, ignore_order=True, report_repetition=True)
         result = {
             'iterable_item_removed': {
                 'root[1]': 3
             },
@@ -172,14 +173,67 @@
                     'value': 4,
                     'new_repeat': 2
                 }
             }
         }
         assert result == ddiff
 
+    @pytest.mark.skip
+    def test_list_difference_ignore_order_report_repetition2(self):
+        t1 = [1, 1, 1]
+        t2 = [2, 2]
+        ddiff = DeepDiff(t1, t2, ignore_order=True)
+        result = {'values_changed': {'root[0]': {'new_value': 2, 'old_value': 1}}}
+        assert result == ddiff
+
+        ddiff2 = DeepDiff(t1, t2, ignore_order=True, report_repetition=True, cutoff_intersection_for_pairs=1, cutoff_distance_for_pairs=1)
+        result2 = {
+            'iterable_item_removed': {
+                'root[0]': 1,
+                'root[1]': 1,
+                'root[2]': 1
+            },
+            'iterable_item_added': {
+                'root[0]': 2,
+                'root[1]': 2,
+            },
+        }
+        assert result2 == ddiff2
+
+    @pytest.mark.skip
+    def test_list_difference_ignore_order_report_repetition3(self):
+        t1 = [{"id": 1}, {"id": 1}, {"id": 1}]
+        t2 = [{"id": 1, "name": 1}]
+
+        ddiff2 = DeepDiff(t1, t2, ignore_order=True, report_repetition=True, cutoff_intersection_for_pairs=1, cutoff_distance_for_pairs=1)
+        result2 = {
+            'iterable_item_removed': {
+                'root[1]': {"id": 1},
+                'root[2]': {"id": 1},
+            },
+            'dictionary_item_added': ["root[0]['name']"]
+        }
+        assert result2 == ddiff2
+
+    @pytest.mark.skip
+    def test_list_difference_ignore_order_report_repetition4(self):
+        t1 = [{"id": 1}, {"id": 1}, {"id": 1}, {"name": "Joe"}, {"name": "Joe"}]
+        t2 = [{"id": 1, "name": 1}, {"id": 1, "name": "Joe"}]
+
+        ddiff2 = DeepDiff(t1, t2, ignore_order=True, report_repetition=True, cutoff_intersection_for_pairs=1, cutoff_distance_for_pairs=1)
+        result2 = {
+            'iterable_item_removed': {
+                'root[2]': {"id": 1},
+                'root[3]': {"name": "Joe"},
+                'root[4]': {"name": "Joe"},
+            },
+            'dictionary_item_added': ["root[0]['name']", "root[1]['name']"]
+        }
+        assert result2 == ddiff2
+
     def test_nested_list_ignore_order_report_repetition(self):
         t1 = [1, 2, [3, 4]]
         t2 = [[4, 3, 3], 2, 1]
         ddiff = DeepDiff(t1, t2, ignore_order=True, report_repetition=False)
         assert not ddiff
 
         ddiff2 = DeepDiff(t1, t2, ignore_order=True, report_repetition=True)
@@ -590,16 +644,16 @@
         }
 
         ddiff = DeepDiff(t1, t2, ignore_order=True, cutoff_intersection_for_pairs=1)
         assert ddiff == {}
 
     @pytest.mark.parametrize('max_passes, expected', [
         (0, {'values_changed': {'root[0]': {'new_value': {'key5': 'CHANGE', 'key6': 'val6'}, 'old_value': {'key3': [[[[[1, 2, 4, 5]]]]], 'key4': [7, 8]}}, 'root[1]': {'new_value': {'key3': [[[[[1, 3, 5, 4]]]]], 'key4': [7, 8]}, 'old_value': {'key5': 'val5', 'key6': 'val6'}}}}),
-        (1, {'values_changed': {"root[1]['key5']": {'new_value': 'CHANGE', 'old_value': 'val5'}, "root[0]['key3'][0]": {'new_value': [[[[1, 3, 5, 4]]]], 'old_value': [[[[1, 2, 4, 5]]]]}}}),
-        (22, {'values_changed': {"root[1]['key5']": {'new_value': 'CHANGE', 'old_value': 'val5'}, "root[0]['key3'][0][0][0][0][1]": {'new_value': 3, 'old_value': 2}}})
+        (1, {'values_changed': {"root[1]['key5']": {'new_value': 'CHANGE', 'old_value': 'val5', 'new_path': "root[0]['key5']"}, "root[0]['key3'][0]": {'new_value': [[[[1, 3, 5, 4]]]], 'old_value': [[[[1, 2, 4, 5]]]], 'new_path': "root[1]['key3'][0]"}}}),
+        (22, {'values_changed': {"root[1]['key5']": {'new_value': 'CHANGE', 'old_value': 'val5', 'new_path': "root[0]['key5']"}, "root[0]['key3'][0][0][0][0][1]": {'new_value': 3, 'old_value': 2, 'new_path': "root[1]['key3'][0][0][0][0][1]"}}})
     ])
     def test_ignore_order_max_passes(self, max_passes, expected):
         t1 = [
             {
                 'key3': [[[[[1, 2, 4, 5]]]]],
                 'key4': [7, 8],
             },
@@ -621,16 +675,16 @@
         ]
 
         ddiff = DeepDiff(t1, t2, ignore_order=True, max_passes=max_passes, verbose_level=2, cache_size=5000, cutoff_intersection_for_pairs=1)
         assert expected == ddiff
 
     @pytest.mark.parametrize('max_diffs, expected', [
         (1, {}),
-        (65, {'values_changed': {"root[1]['key5']": {'new_value': 'CHANGE', 'old_value': 'val5'}}}),
-        (80, {'values_changed': {"root[1]['key5']": {'new_value': 'CHANGE', 'old_value': 'val5'}, "root[0]['key3'][0][0][0][0][1]": {'new_value': 3, 'old_value': 2}}}),
+        (65, {'values_changed': {"root[1]['key5']": {'new_value': 'CHANGE', 'old_value': 'val5', 'new_path': "root[0]['key5']"}}}),
+        (80, {'values_changed': {"root[1]['key5']": {'new_value': 'CHANGE', 'old_value': 'val5', 'new_path': "root[0]['key5']"}, "root[0]['key3'][0][0][0][0][1]": {'new_value': 3, 'old_value': 2, 'new_path': "root[1]['key3'][0][0][0][0][1]"}}}),
     ])
     def test_ignore_order_max_diffs(self, max_diffs, expected):
         t1 = [
             {
                 'key3': [[[[[1, 2, 4, 5]]]]],
                 'key4': [7, 8],
             },
@@ -919,14 +973,24 @@
         a = [{'x': 0.001}, {'y': 2.00002}]
         b = [{'x': 0.0011}, {'y': 2}]
 
         diff = DeepDiff(a, b, ignore_order=True, math_epsilon=0.01)
         expected = {'values_changed': {'root[0]': {'new_value': {'x': 0.0011}, 'old_value': {'x': 0.001}}, 'root[1]': {'new_value': {'y': 2}, 'old_value': {'y': 2.00002}}}}
         assert expected == diff
 
+    def test_datetime_and_ignore_order(self):
+        diff = DeepDiff(
+            [{'due_date': datetime.date(2024, 2, 1)}],
+            [{'due_date': datetime.date(2024, 2, 2)}],
+            ignore_order=True,
+            ignore_numeric_type_changes=True
+        )
+        assert {} != diff
+
+
 
 class TestCompareFuncIgnoreOrder:
 
     def test_ignore_order_with_compare_func_to_guide_comparison(self):
         t1 = [
             {
                 'id': 1,
@@ -1068,14 +1132,129 @@
             except Exception:
                 raise CannotCompare() from None
 
         ddiff2 = DeepDiff(t1, t2, ignore_order=True, cutoff_intersection_for_pairs=1, cutoff_distance_for_pairs=1, iterable_compare_func=compare_func)
         assert expected_with_compare_func == ddiff2
         assert ddiff != ddiff2
 
+    def test_ignore_order_with_compare_func_with_one_each_hashes_added_hashes_removed(self):
+        """
+        Scenario:
+        In this example which demonstrates the problem... We have two dictionaries containing lists for
+        individualNames.  Each list contains exactly 2 elements. The effective change is that we are
+        replacing the 2nd element in the list.
+        NOTE: This is considered a REPLACEMENT of the second element and not an UPDATE of the element
+        because we are providing a custom compare_func which will determine matching elements based on
+        the value of the nameIdentifier field.  If the custom compare_func is not used, then
+        deepdiff.diff will mistakenly treat the difference as being individual field updates for every
+        field in the second element of the list.
+
+        Intent:
+        Use our custom compare_func, since we have provided it.
+        We need to fall into self._precalculate_distance_by_custom_compare_func
+        To do this, we are proposing a change to deepdiff.diff line 1128:
+
+        Original:
+            if hashes_added and hashes_removed and self.iterable_compare_func and len(hashes_added) > 1 and len(hashes_removed) > 1:
+
+        Proposed/Updated:
+            if hashes_added and hashes_removed \
+            and self.iterable_compare_func \
+            and len(hashes_added) > 0 and len(hashes_removed) > 0:
+
+        NOTE: It is worth mentioning that deepdiff.diff line 1121, might also benefit by changing the length conditions
+        to evaluate for > 0 (rather than > 1).
+        """
+
+        t1 = {
+            "individualNames": [
+                {
+                    "firstName": "Johnathan",
+                    "lastName": "Doe",
+                    "prefix": "COLONEL",
+                    "middleName": "A",
+                    "primaryIndicator": True,
+                    "professionalDesignation": "PHD",
+                    "suffix": "SR",
+                    "nameIdentifier": "00001"
+                },
+                {
+                    "firstName": "John",
+                    "lastName": "Doe",
+                    "prefix": "",
+                    "middleName": "",
+                    "primaryIndicator": False,
+                    "professionalDesignation": "",
+                    "suffix": "SR",
+                    "nameIdentifier": "00002"
+                }
+            ]
+        }
+
+        t2 = {
+            "individualNames": [
+                {
+                    "firstName": "Johnathan",
+                    "lastName": "Doe",
+                    "prefix": "COLONEL",
+                    "middleName": "A",
+                    "primaryIndicator": True,
+                    "professionalDesignation": "PHD",
+                    "suffix": "SR",
+                    "nameIdentifier": "00001"
+                },
+                {
+                    "firstName": "Johnny",
+                    "lastName": "Doe",
+                    "prefix": "",
+                    "middleName": "A",
+                    "primaryIndicator": False,
+                    "professionalDesignation": "",
+                    "suffix": "SR",
+                    "nameIdentifier": "00003"
+                }
+            ]
+        }
+        def compare_func(item1, item2, level=None):
+            print("*** inside compare ***")
+            it1_keys = item1.keys()
+
+            try:
+
+                # --- individualNames ---
+                if 'nameIdentifier' in it1_keys and 'lastName' in it1_keys:
+                    match_result = item1['nameIdentifier'] == item2['nameIdentifier']
+                    print("individualNames - matching result:", match_result)
+                    return match_result
+                else:
+                    print("Unknown list item...", "matching result:", item1 == item2)
+                    return item1 == item2
+            except Exception:
+                raise CannotCompare() from None
+        # ---------------------------- End of nested function
+
+        actual_diff = DeepDiff(t1, t2, report_repetition=True,
+                             ignore_order=True, iterable_compare_func=compare_func, cutoff_intersection_for_pairs=1)
+
+        old_invalid_diff = {
+            'values_changed': {"root['individualNames'][1]['firstName']": {'new_value': 'Johnny', 'old_value': 'John'},
+                               "root['individualNames'][1]['middleName']": {'new_value': 'A', 'old_value': ''},
+                               "root['individualNames'][1]['nameIdentifier']": {'new_value': '00003',
+                                                                                'old_value': '00002'}}}
+        new_expected_diff = {'iterable_item_added': {
+            "root['individualNames'][1]": {'firstName': 'Johnny', 'lastName': 'Doe', 'prefix': '', 'middleName': 'A',
+                                           'primaryIndicator': False, 'professionalDesignation': '', 'suffix': 'SR',
+                                           'nameIdentifier': '00003'}}, 'iterable_item_removed': {
+            "root['individualNames'][1]": {'firstName': 'John', 'lastName': 'Doe', 'prefix': '', 'middleName': '',
+                                           'primaryIndicator': False, 'professionalDesignation': '', 'suffix': 'SR',
+                                           'nameIdentifier': '00002'}}}
+
+        assert old_invalid_diff != actual_diff
+        assert new_expected_diff == actual_diff
+
 
 class TestDynamicIgnoreOrder:
     def test_ignore_order_func(self):
         t1 = {
             "order_matters": [
                 {1},
                 {
```

### Comparing `deepdiff-6.7.1/tests/test_lfucache.py` & `deepdiff-7.0.0/tests/test_lfucache.py`

 * *Files identical despite different names*

### Comparing `deepdiff-6.7.1/tests/test_operators.py` & `deepdiff-7.0.0/tests/test_operators.py`

 * *Files identical despite different names*

### Comparing `deepdiff-6.7.1/tests/test_path.py` & `deepdiff-7.0.0/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `deepdiff-6.7.1/tests/test_search.py` & `deepdiff-7.0.0/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `deepdiff-6.7.1/tests/test_serialization.py` & `deepdiff-7.0.0/tests/test_serialization.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 #!/usr/bin/env python
 import os
 import json
 import sys
 import pytest
 import datetime
+import numpy as np
+from typing import NamedTuple, Optional
 from pickle import UnpicklingError
 from decimal import Decimal
+from collections import Counter
 from deepdiff import DeepDiff
-from deepdiff.helper import pypy3
+from deepdiff.helper import pypy3, py_current_version, np_ndarray, Opcode
 from deepdiff.serialization import (
     pickle_load, pickle_dump, ForbiddenModule, ModuleNotFoundError,
     MODULE_NOT_FOUND_MSG, FORBIDDEN_MODULE_MSG, pretty_print_diff,
     load_path_content, UnsupportedFormatErr, json_dumps, json_loads)
 from conftest import FIXTURES_DIR
 from ordered_set import OrderedSet
 from tests import PicklableClass
@@ -19,14 +22,27 @@
 import logging
 logging.disable(logging.CRITICAL)
 
 t1 = {1: 1, 2: 2, 3: 3, 4: {"a": "hello", "b": [1, 2, 3]}}
 t2 = {1: 1, 2: 2, 3: 3, 4: {"a": "hello", "b": "world\n\n\nEnd"}}
 
 
+class SomeStats(NamedTuple):
+    counter: Optional[Counter]
+    context_aware_counter: Optional[Counter] = None
+    min_int: Optional[int] = 0
+    max_int: Optional[int] = 0
+
+
+field_stats1 = SomeStats(
+    counter=Counter(["a", "a", "b"]),
+    max_int=10
+)
+
+
 class TestSerialization:
     """Tests for Serializations."""
 
     def test_serialization_text(self):
         ddiff = DeepDiff(t1, t2)
         assert "builtins.list" in ddiff.to_json_pickle()
         jsoned = ddiff.to_json()
@@ -319,14 +335,28 @@
         (1, {'10': None}, None),
         (2, {"type_changes": {"root": {"old_type": None, "new_type": list, "new_value": ["你好", 2, 3, 5]}}}, None),
         (3, {'10': Decimal(2017)}, None),
         (4, Decimal(2017.1), None),
         (5, {1, 2, 10}, set),
         (6, datetime.datetime(2023, 10, 11), datetime.datetime.fromisoformat),
         (7, datetime.datetime.utcnow(), datetime.datetime.fromisoformat),
+        (8, field_stats1, lambda x: SomeStats(**x)),
+        (9, np.array([[ 101, 3533, 1998, 4532, 2024, 3415, 1012,  102]]), np.array)
     ])
     def test_json_dumps_and_loads(self, test_num, value, func_to_convert_back):
+        if test_num == 8 and py_current_version < 3.8:
+            print(f"Skipping test_json_dumps_and_loads #{test_num} on Python {py_current_version}")
+            return
         serialized = json_dumps(value)
         back = json_loads(serialized)
         if func_to_convert_back:
             back = func_to_convert_back(back)
-        assert value == back, f"test_json_dumps_and_loads test #{test_num} failed"
+        if isinstance(back, np_ndarray):
+            assert np.array_equal(value, back), f"test_json_dumps_and_loads test #{test_num} failed"
+        else:
+            assert value == back, f"test_json_dumps_and_loads test #{test_num} failed"
+
+    def test_namedtuple_seriazliation(self):
+        op_code = Opcode(tag="replace", t1_from_index=0, t1_to_index=1, t2_from_index=10, t2_to_index=20)
+        serialized = json_dumps(op_code)
+        expected = '{"tag":"replace","t1_from_index":0,"t1_to_index":1,"t2_from_index":10,"t2_to_index":20,"old_values":null,"new_values":null}'
+        assert serialized == expected
```

