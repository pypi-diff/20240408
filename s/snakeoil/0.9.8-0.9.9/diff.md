# Comparing `tmp/snakeoil-0.9.8.tar.gz` & `tmp/snakeoil-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snakeoil-0.9.8.tar", last modified: Tue Dec 14 16:56:11 2021, max compression
+gzip compressed data, was "snakeoil-0.9.9.tar", last modified: Tue Dec 14 17:34:12 2021, max compression
```

## Comparing `snakeoil-0.9.8.tar` & `snakeoil-0.9.9.tar`

### file list

```diff
@@ -1,122 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 16:56:11.081922 snakeoil-0.9.8/
--rw-r--r--   0 runner    (1001) docker     (121)      302 2021-12-14 16:55:34.216321 snakeoil-0.9.8/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (121)     1497 2021-12-14 16:55:34.216321 snakeoil-0.9.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    37590 2021-12-14 16:55:34.216321 snakeoil-0.9.8/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1823 2021-12-14 16:56:11.081922 snakeoil-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1286 2021-12-14 16:55:34.216321 snakeoil-0.9.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      988 2021-12-14 16:55:34.216321 snakeoil-0.9.8/RELEASE.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 16:56:11.077922 snakeoil-0.9.8/doc/
--rw-r--r--   0 runner    (1001) docker     (121)     8097 2021-12-14 16:55:34.216321 snakeoil-0.9.8/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     8833 2021-12-14 16:55:34.216321 snakeoil-0.9.8/doc/index.rst
-lrwxrwxrwx   0 runner    (1001) docker     (121)        0 2021-12-14 16:55:34.216321 snakeoil-0.9.8/doc/news.rst -> ../NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (121)      184 2021-12-14 16:55:34.216321 snakeoil-0.9.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      247 2021-12-14 16:55:34.216321 snakeoil-0.9.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)      900 2021-12-14 16:55:34.216321 snakeoil-0.9.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 16:56:11.077922 snakeoil-0.9.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 16:56:11.085922 snakeoil-0.9.8/src/snakeoil/
--rw-r--r--   0 runner    (1001) docker     (121)      395 2021-12-14 16:55:34.216321 snakeoil-0.9.8/src/snakeoil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3916 2021-12-14 16:55:34.216321 snakeoil-0.9.8/src/snakeoil/_fileutils.py
--rw-r--r--   0 runner    (1001) docker     (121)   235701 2021-12-14 16:56:11.013919 snakeoil-0.9.8/src/snakeoil/_posix.c
--rw-r--r--   0 runner    (1001) docker     (121)     7993 2021-12-14 16:55:34.216321 snakeoil-0.9.8/src/snakeoil/_posix.pyx
--rw-r--r--   0 runner    (1001) docker     (121)   253863 2021-12-14 16:56:10.857914 snakeoil-0.9.8/src/snakeoil/_sequences.c
--rw-r--r--   0 runner    (1001) docker     (121)     1902 2021-12-14 16:55:34.216321 snakeoil-0.9.8/src/snakeoil/_sequences.pyx
--rw-r--r--   0 runner    (1001) docker     (121)       17 2021-12-14 16:56:11.085922 snakeoil-0.9.8/src/snakeoil/_verinfo.py
--rw-r--r--   0 runner    (1001) docker     (121)    11776 2021-12-14 16:55:34.216321 snakeoil-0.9.8/src/snakeoil/bash.py
--rw-r--r--   0 runner    (1001) docker     (121)     4919 2021-12-14 16:55:34.216321 snakeoil-0.9.8/src/snakeoil/caching.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 16:56:11.077922 snakeoil-0.9.8/src/snakeoil/chksum/
--rw-r--r--   0 runner    (1001) docker     (121)     4705 2021-12-14 16:55:34.216321 snakeoil-0.9.8/src/snakeoil/chksum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5477 2021-12-14 16:55:34.216321 snakeoil-0.9.8/src/snakeoil/chksum/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 16:56:11.077922 snakeoil-0.9.8/src/snakeoil/cli/
--rw-r--r--   0 runner    (1001) docker     (121)       43 2021-12-14 16:55:34.216321 snakeoil-0.9.8/src/snakeoil/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    55941 2021-12-14 16:55:34.216321 snakeoil-0.9.8/src/snakeoil/cli/arghparse.py
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2021-12-14 16:55:34.216321 snakeoil-0.9.8/src/snakeoil/cli/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     3877 2021-12-14 16:55:34.216321 snakeoil-0.9.8/src/snakeoil/cli/input.py
--rw-r--r--   0 runner    (1001) docker     (121)     8422 2021-12-14 16:55:34.216321 snakeoil-0.9.8/src/snakeoil/cli/tool.py
--rw-r--r--   0 runner    (1001) docker     (121)     1334 2021-12-14 16:55:34.220321 snakeoil-0.9.8/src/snakeoil/compatibility.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 16:56:11.077922 snakeoil-0.9.8/src/snakeoil/compression/
--rw-r--r--   0 runner    (1001) docker     (121)     7524 2021-12-14 16:55:34.220321 snakeoil-0.9.8/src/snakeoil/compression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2778 2021-12-14 16:55:34.220321 snakeoil-0.9.8/src/snakeoil/compression/_bzip2.py
--rw-r--r--   0 runner    (1001) docker     (121)     5265 2021-12-14 16:55:34.220321 snakeoil-0.9.8/src/snakeoil/compression/_util.py
--rw-r--r--   0 runner    (1001) docker     (121)     8930 2021-12-14 16:55:34.220321 snakeoil-0.9.8/src/snakeoil/containers.py
--rw-r--r--   0 runner    (1001) docker     (121)    17079 2021-12-14 16:55:34.220321 snakeoil-0.9.8/src/snakeoil/contexts.py
--rw-r--r--   0 runner    (1001) docker     (121)     5273 2021-12-14 16:55:34.220321 snakeoil-0.9.8/src/snakeoil/currying.py
--rw-r--r--   0 runner    (1001) docker     (121)    15556 2021-12-14 16:55:34.220321 snakeoil-0.9.8/src/snakeoil/data_source.py
--rw-r--r--   0 runner    (1001) docker     (121)      832 2021-12-14 16:55:34.220321 snakeoil-0.9.8/src/snakeoil/decorators.py
--rw-r--r--   0 runner    (1001) docker     (121)     3279 2021-12-14 16:55:34.220321 snakeoil-0.9.8/src/snakeoil/demandimport.py
--rw-r--r--   0 runner    (1001) docker     (121)    12797 2021-12-14 16:55:34.220321 snakeoil-0.9.8/src/snakeoil/demandload.py
--rw-r--r--   0 runner    (1001) docker     (121)     6234 2021-12-14 16:55:34.220321 snakeoil-0.9.8/src/snakeoil/dependant_methods.py
--rw-r--r--   0 runner    (1001) docker     (121)      712 2021-12-14 16:55:34.220321 snakeoil-0.9.8/src/snakeoil/descriptors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 16:56:11.081922 snakeoil-0.9.8/src/snakeoil/dist/
--rw-r--r--   0 runner    (1001) docker     (121)       70 2021-12-14 16:55:34.220321 snakeoil-0.9.8/src/snakeoil/dist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    40459 2021-12-14 16:55:34.220321 snakeoil-0.9.8/src/snakeoil/dist/distutils_extensions.py
--rw-r--r--   0 runner    (1001) docker     (121)     3488 2021-12-14 16:55:34.220321 snakeoil-0.9.8/src/snakeoil/dist/generate_docs.py
--rw-r--r--   0 runner    (1001) docker     (121)    10363 2021-12-14 16:55:34.220321 snakeoil-0.9.8/src/snakeoil/dist/generate_man_rsts.py
--rw-r--r--   0 runner    (1001) docker     (121)     1252 2021-12-14 16:55:34.220321 snakeoil-0.9.8/src/snakeoil/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     6035 2021-12-14 16:55:34.220321 snakeoil-0.9.8/src/snakeoil/fileutils.py
--rw-r--r--   0 runner    (1001) docker     (121)    20594 2021-12-14 16:55:34.220321 snakeoil-0.9.8/src/snakeoil/formatters.py
--rw-r--r--   0 runner    (1001) docker     (121)     9043 2021-12-14 16:55:34.220321 snakeoil-0.9.8/src/snakeoil/iterables.py
--rw-r--r--   0 runner    (1001) docker     (121)    25636 2021-12-14 16:55:34.220321 snakeoil-0.9.8/src/snakeoil/klass.py
--rw-r--r--   0 runner    (1001) docker     (121)      851 2021-12-14 16:55:34.220321 snakeoil-0.9.8/src/snakeoil/log.py
--rw-r--r--   0 runner    (1001) docker     (121)    24453 2021-12-14 16:55:34.220321 snakeoil-0.9.8/src/snakeoil/mappings.py
--rw-r--r--   0 runner    (1001) docker     (121)     2444 2021-12-14 16:55:34.220321 snakeoil-0.9.8/src/snakeoil/modules.py
--rw-r--r--   0 runner    (1001) docker     (121)    10358 2021-12-14 16:55:34.220321 snakeoil-0.9.8/src/snakeoil/obj.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 16:56:11.081922 snakeoil-0.9.8/src/snakeoil/osutils/
--rw-r--r--   0 runner    (1001) docker     (121)    12225 2021-12-14 16:55:34.220321 snakeoil-0.9.8/src/snakeoil/osutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1864 2021-12-14 16:55:34.220321 snakeoil-0.9.8/src/snakeoil/osutils/mount.py
--rw-r--r--   0 runner    (1001) docker     (121)     2674 2021-12-14 16:55:34.220321 snakeoil-0.9.8/src/snakeoil/osutils/native_readdir.py
--rw-r--r--   0 runner    (1001) docker     (121)     1075 2021-12-14 16:55:34.220321 snakeoil-0.9.8/src/snakeoil/pickling.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 16:56:11.081922 snakeoil-0.9.8/src/snakeoil/process/
--rw-r--r--   0 runner    (1001) docker     (121)     3365 2021-12-14 16:55:34.220321 snakeoil-0.9.8/src/snakeoil/process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9579 2021-12-14 16:55:34.220321 snakeoil-0.9.8/src/snakeoil/process/namespaces.py
--rw-r--r--   0 runner    (1001) docker     (121)    12909 2021-12-14 16:55:34.220321 snakeoil-0.9.8/src/snakeoil/process/spawn.py
--rw-r--r--   0 runner    (1001) docker     (121)     9067 2021-12-14 16:55:34.220321 snakeoil-0.9.8/src/snakeoil/sequences.py
--rw-r--r--   0 runner    (1001) docker     (121)     2141 2021-12-14 16:55:34.220321 snakeoil-0.9.8/src/snakeoil/stringio.py
--rw-r--r--   0 runner    (1001) docker     (121)     1177 2021-12-14 16:55:34.220321 snakeoil-0.9.8/src/snakeoil/strings.py
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2021-12-14 16:55:34.220321 snakeoil-0.9.8/src/snakeoil/struct_compat.py
--rw-r--r--   0 runner    (1001) docker     (121)     3167 2021-12-14 16:55:34.220321 snakeoil-0.9.8/src/snakeoil/tar.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 16:56:11.081922 snakeoil-0.9.8/src/snakeoil/test/
--rw-r--r--   0 runner    (1001) docker     (121)    14089 2021-12-14 16:55:34.220321 snakeoil-0.9.8/src/snakeoil/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5577 2021-12-14 16:55:34.220321 snakeoil-0.9.8/src/snakeoil/test/argparse_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1044 2021-12-14 16:55:34.220321 snakeoil-0.9.8/src/snakeoil/test/demandload.py
--rw-r--r--   0 runner    (1001) docker     (121)     1678 2021-12-14 16:55:34.220321 snakeoil-0.9.8/src/snakeoil/test/eq_hash_inheritance.py
--rw-r--r--   0 runner    (1001) docker     (121)      468 2021-12-14 16:55:34.220321 snakeoil-0.9.8/src/snakeoil/test/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (121)     8271 2021-12-14 16:55:34.220321 snakeoil-0.9.8/src/snakeoil/test/mixins.py
--rw-r--r--   0 runner    (1001) docker     (121)      480 2021-12-14 16:55:34.220321 snakeoil-0.9.8/src/snakeoil/test/modules.py
--rw-r--r--   0 runner    (1001) docker     (121)     2725 2021-12-14 16:55:34.220321 snakeoil-0.9.8/src/snakeoil/test/slot_shadowing.py
--rw-r--r--   0 runner    (1001) docker     (121)     3723 2021-12-14 16:55:34.220321 snakeoil-0.9.8/src/snakeoil/version.py
--rw-r--r--   0 runner    (1001) docker     (121)     1031 2021-12-14 16:55:34.220321 snakeoil-0.9.8/src/snakeoil/weakrefs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 16:56:11.081922 snakeoil-0.9.8/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 16:56:11.081922 snakeoil-0.9.8/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (121)    18420 2021-12-14 16:55:34.220321 snakeoil-0.9.8/tests/cli/test_arghparse.py
--rw-r--r--   0 runner    (1001) docker     (121)     4522 2021-12-14 16:55:34.220321 snakeoil-0.9.8/tests/cli/test_input.py
--rw-r--r--   0 runner    (1001) docker     (121)     8900 2021-12-14 16:55:34.220321 snakeoil-0.9.8/tests/test_bash.py
--rw-r--r--   0 runner    (1001) docker     (121)     5478 2021-12-14 16:55:34.220321 snakeoil-0.9.8/tests/test_caching.py
--rw-r--r--   0 runner    (1001) docker     (121)     1432 2021-12-14 16:55:34.220321 snakeoil-0.9.8/tests/test_chksum.py
--rw-r--r--   0 runner    (1001) docker     (121)     3978 2021-12-14 16:55:34.220321 snakeoil-0.9.8/tests/test_chksum_defaults.py
--rw-r--r--   0 runner    (1001) docker     (121)     7943 2021-12-14 16:55:34.220321 snakeoil-0.9.8/tests/test_containers.py
--rw-r--r--   0 runner    (1001) docker     (121)     4301 2021-12-14 16:55:34.220321 snakeoil-0.9.8/tests/test_contexts.py
--rw-r--r--   0 runner    (1001) docker     (121)     6918 2021-12-14 16:55:34.220321 snakeoil-0.9.8/tests/test_currying.py
--rw-r--r--   0 runner    (1001) docker     (121)     6403 2021-12-14 16:55:34.220321 snakeoil-0.9.8/tests/test_data_source.py
--rw-r--r--   0 runner    (1001) docker     (121)     1997 2021-12-14 16:55:34.220321 snakeoil-0.9.8/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (121)     4460 2021-12-14 16:55:34.220321 snakeoil-0.9.8/tests/test_demandload.py
--rw-r--r--   0 runner    (1001) docker     (121)      114 2021-12-14 16:55:34.220321 snakeoil-0.9.8/tests/test_demandload_usage.py
--rw-r--r--   0 runner    (1001) docker     (121)     2738 2021-12-14 16:55:34.220321 snakeoil-0.9.8/tests/test_dependant_methods.py
--rw-r--r--   0 runner    (1001) docker     (121)      328 2021-12-14 16:55:34.220321 snakeoil-0.9.8/tests/test_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (121)       88 2021-12-14 16:55:34.220321 snakeoil-0.9.8/tests/test_eq_hash_inheritance.py
--rw-r--r--   0 runner    (1001) docker     (121)    11167 2021-12-14 16:55:34.220321 snakeoil-0.9.8/tests/test_fileutils.py
--rw-r--r--   0 runner    (1001) docker     (121)     9615 2021-12-14 16:55:34.224321 snakeoil-0.9.8/tests/test_formatters.py
--rw-r--r--   0 runner    (1001) docker     (121)     4802 2021-12-14 16:55:34.224321 snakeoil-0.9.8/tests/test_iterables.py
--rw-r--r--   0 runner    (1001) docker     (121)    15215 2021-12-14 16:55:34.224321 snakeoil-0.9.8/tests/test_klass.py
--rw-r--r--   0 runner    (1001) docker     (121)    19002 2021-12-14 16:55:34.224321 snakeoil-0.9.8/tests/test_mappings.py
--rw-r--r--   0 runner    (1001) docker     (121)     4412 2021-12-14 16:55:34.224321 snakeoil-0.9.8/tests/test_modules.py
--rw-r--r--   0 runner    (1001) docker     (121)     4550 2021-12-14 16:55:34.224321 snakeoil-0.9.8/tests/test_obj.py
--rw-r--r--   0 runner    (1001) docker     (121)    17098 2021-12-14 16:55:34.224321 snakeoil-0.9.8/tests/test_osutils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2000 2021-12-14 16:55:34.224321 snakeoil-0.9.8/tests/test_process.py
--rw-r--r--   0 runner    (1001) docker     (121)     4545 2021-12-14 16:55:34.224321 snakeoil-0.9.8/tests/test_process_spawn.py
--rw-r--r--   0 runner    (1001) docker     (121)    10347 2021-12-14 16:55:34.224321 snakeoil-0.9.8/tests/test_sequences.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2021-12-14 16:55:34.224321 snakeoil-0.9.8/tests/test_slot_shadowing.py
--rw-r--r--   0 runner    (1001) docker     (121)       98 2021-12-14 16:55:34.224321 snakeoil-0.9.8/tests/test_source_hygene.py
--rw-r--r--   0 runner    (1001) docker     (121)     1600 2021-12-14 16:55:34.224321 snakeoil-0.9.8/tests/test_stringio.py
--rw-r--r--   0 runner    (1001) docker     (121)     1522 2021-12-14 16:55:34.224321 snakeoil-0.9.8/tests/test_strings.py
--rw-r--r--   0 runner    (1001) docker     (121)     5921 2021-12-14 16:55:34.224321 snakeoil-0.9.8/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (121)      458 2021-12-14 16:55:34.224321 snakeoil-0.9.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 17:34:12.120603 snakeoil-0.9.9/
+-rw-r--r--   0 runner    (1001) docker     (121)      302 2021-12-14 17:33:30.572597 snakeoil-0.9.9/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (121)     1497 2021-12-14 17:33:30.572597 snakeoil-0.9.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)    37690 2021-12-14 17:33:30.572597 snakeoil-0.9.9/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1823 2021-12-14 17:34:12.120603 snakeoil-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1286 2021-12-14 17:33:30.572597 snakeoil-0.9.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      988 2021-12-14 17:33:30.572597 snakeoil-0.9.9/RELEASE.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 17:34:12.112603 snakeoil-0.9.9/doc/
+-rw-r--r--   0 runner    (1001) docker     (121)     8097 2021-12-14 17:33:30.572597 snakeoil-0.9.9/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8833 2021-12-14 17:33:30.572597 snakeoil-0.9.9/doc/index.rst
+lrwxrwxrwx   0 runner    (1001) docker     (121)        0 2021-12-14 17:33:30.572597 snakeoil-0.9.9/doc/news.rst -> ../NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      184 2021-12-14 17:33:30.572597 snakeoil-0.9.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 17:34:12.116603 snakeoil-0.9.9/requirements/
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2021-12-14 17:33:30.572597 snakeoil-0.9.9/requirements/build.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       11 2021-12-14 17:33:30.572597 snakeoil-0.9.9/requirements/ci.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2021-12-14 17:33:30.572597 snakeoil-0.9.9/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       88 2021-12-14 17:33:30.572597 snakeoil-0.9.9/requirements/dist.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       36 2021-12-14 17:33:30.572597 snakeoil-0.9.9/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2021-12-14 17:33:30.572597 snakeoil-0.9.9/requirements/install.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2021-12-14 17:33:30.572597 snakeoil-0.9.9/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2021-12-14 17:33:30.572597 snakeoil-0.9.9/requirements/tox.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      247 2021-12-14 17:33:30.572597 snakeoil-0.9.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (121)      900 2021-12-14 17:33:30.572597 snakeoil-0.9.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 17:34:12.104603 snakeoil-0.9.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 17:34:12.124603 snakeoil-0.9.9/src/snakeoil/
+-rw-r--r--   0 runner    (1001) docker     (121)      395 2021-12-14 17:33:30.576597 snakeoil-0.9.9/src/snakeoil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3916 2021-12-14 17:33:30.576597 snakeoil-0.9.9/src/snakeoil/_fileutils.py
+-rw-r--r--   0 runner    (1001) docker     (121)   235701 2021-12-14 17:34:12.032603 snakeoil-0.9.9/src/snakeoil/_posix.c
+-rw-r--r--   0 runner    (1001) docker     (121)     7993 2021-12-14 17:33:30.576597 snakeoil-0.9.9/src/snakeoil/_posix.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)   253863 2021-12-14 17:34:11.844604 snakeoil-0.9.9/src/snakeoil/_sequences.c
+-rw-r--r--   0 runner    (1001) docker     (121)     1902 2021-12-14 17:33:30.576597 snakeoil-0.9.9/src/snakeoil/_sequences.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2021-12-14 17:34:12.124603 snakeoil-0.9.9/src/snakeoil/_verinfo.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11776 2021-12-14 17:33:30.576597 snakeoil-0.9.9/src/snakeoil/bash.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4919 2021-12-14 17:33:30.576597 snakeoil-0.9.9/src/snakeoil/caching.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 17:34:12.116603 snakeoil-0.9.9/src/snakeoil/chksum/
+-rw-r--r--   0 runner    (1001) docker     (121)     4705 2021-12-14 17:33:30.576597 snakeoil-0.9.9/src/snakeoil/chksum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5477 2021-12-14 17:33:30.576597 snakeoil-0.9.9/src/snakeoil/chksum/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 17:34:12.116603 snakeoil-0.9.9/src/snakeoil/cli/
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2021-12-14 17:33:30.576597 snakeoil-0.9.9/src/snakeoil/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    55941 2021-12-14 17:33:30.576597 snakeoil-0.9.9/src/snakeoil/cli/arghparse.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1078 2021-12-14 17:33:30.576597 snakeoil-0.9.9/src/snakeoil/cli/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3877 2021-12-14 17:33:30.576597 snakeoil-0.9.9/src/snakeoil/cli/input.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8422 2021-12-14 17:33:30.576597 snakeoil-0.9.9/src/snakeoil/cli/tool.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1334 2021-12-14 17:33:30.576597 snakeoil-0.9.9/src/snakeoil/compatibility.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 17:34:12.116603 snakeoil-0.9.9/src/snakeoil/compression/
+-rw-r--r--   0 runner    (1001) docker     (121)     7524 2021-12-14 17:33:30.576597 snakeoil-0.9.9/src/snakeoil/compression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2778 2021-12-14 17:33:30.576597 snakeoil-0.9.9/src/snakeoil/compression/_bzip2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5265 2021-12-14 17:33:30.576597 snakeoil-0.9.9/src/snakeoil/compression/_util.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8930 2021-12-14 17:33:30.576597 snakeoil-0.9.9/src/snakeoil/containers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17079 2021-12-14 17:33:30.576597 snakeoil-0.9.9/src/snakeoil/contexts.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5273 2021-12-14 17:33:30.576597 snakeoil-0.9.9/src/snakeoil/currying.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15556 2021-12-14 17:33:30.576597 snakeoil-0.9.9/src/snakeoil/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)      832 2021-12-14 17:33:30.576597 snakeoil-0.9.9/src/snakeoil/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3279 2021-12-14 17:33:30.576597 snakeoil-0.9.9/src/snakeoil/demandimport.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12797 2021-12-14 17:33:30.576597 snakeoil-0.9.9/src/snakeoil/demandload.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6234 2021-12-14 17:33:30.576597 snakeoil-0.9.9/src/snakeoil/dependant_methods.py
+-rw-r--r--   0 runner    (1001) docker     (121)      712 2021-12-14 17:33:30.576597 snakeoil-0.9.9/src/snakeoil/descriptors.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 17:34:12.116603 snakeoil-0.9.9/src/snakeoil/dist/
+-rw-r--r--   0 runner    (1001) docker     (121)       70 2021-12-14 17:33:30.576597 snakeoil-0.9.9/src/snakeoil/dist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    40459 2021-12-14 17:33:30.576597 snakeoil-0.9.9/src/snakeoil/dist/distutils_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3488 2021-12-14 17:33:30.576597 snakeoil-0.9.9/src/snakeoil/dist/generate_docs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10363 2021-12-14 17:33:30.576597 snakeoil-0.9.9/src/snakeoil/dist/generate_man_rsts.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1252 2021-12-14 17:33:30.576597 snakeoil-0.9.9/src/snakeoil/errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6035 2021-12-14 17:33:30.576597 snakeoil-0.9.9/src/snakeoil/fileutils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20594 2021-12-14 17:33:30.576597 snakeoil-0.9.9/src/snakeoil/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9043 2021-12-14 17:33:30.576597 snakeoil-0.9.9/src/snakeoil/iterables.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25636 2021-12-14 17:33:30.576597 snakeoil-0.9.9/src/snakeoil/klass.py
+-rw-r--r--   0 runner    (1001) docker     (121)      851 2021-12-14 17:33:30.576597 snakeoil-0.9.9/src/snakeoil/log.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24453 2021-12-14 17:33:30.576597 snakeoil-0.9.9/src/snakeoil/mappings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2444 2021-12-14 17:33:30.576597 snakeoil-0.9.9/src/snakeoil/modules.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10358 2021-12-14 17:33:30.576597 snakeoil-0.9.9/src/snakeoil/obj.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 17:34:12.116603 snakeoil-0.9.9/src/snakeoil/osutils/
+-rw-r--r--   0 runner    (1001) docker     (121)    12225 2021-12-14 17:33:30.576597 snakeoil-0.9.9/src/snakeoil/osutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1864 2021-12-14 17:33:30.576597 snakeoil-0.9.9/src/snakeoil/osutils/mount.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2674 2021-12-14 17:33:30.576597 snakeoil-0.9.9/src/snakeoil/osutils/native_readdir.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1075 2021-12-14 17:33:30.576597 snakeoil-0.9.9/src/snakeoil/pickling.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 17:34:12.116603 snakeoil-0.9.9/src/snakeoil/process/
+-rw-r--r--   0 runner    (1001) docker     (121)     3365 2021-12-14 17:33:30.576597 snakeoil-0.9.9/src/snakeoil/process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9579 2021-12-14 17:33:30.576597 snakeoil-0.9.9/src/snakeoil/process/namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12909 2021-12-14 17:33:30.576597 snakeoil-0.9.9/src/snakeoil/process/spawn.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9067 2021-12-14 17:33:30.576597 snakeoil-0.9.9/src/snakeoil/sequences.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2141 2021-12-14 17:33:30.576597 snakeoil-0.9.9/src/snakeoil/stringio.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1177 2021-12-14 17:33:30.576597 snakeoil-0.9.9/src/snakeoil/strings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1068 2021-12-14 17:33:30.576597 snakeoil-0.9.9/src/snakeoil/struct_compat.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3167 2021-12-14 17:33:30.576597 snakeoil-0.9.9/src/snakeoil/tar.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 17:34:12.116603 snakeoil-0.9.9/src/snakeoil/test/
+-rw-r--r--   0 runner    (1001) docker     (121)    14089 2021-12-14 17:33:30.576597 snakeoil-0.9.9/src/snakeoil/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5577 2021-12-14 17:33:30.580597 snakeoil-0.9.9/src/snakeoil/test/argparse_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1044 2021-12-14 17:33:30.580597 snakeoil-0.9.9/src/snakeoil/test/demandload.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1678 2021-12-14 17:33:30.580597 snakeoil-0.9.9/src/snakeoil/test/eq_hash_inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (121)      468 2021-12-14 17:33:30.580597 snakeoil-0.9.9/src/snakeoil/test/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8271 2021-12-14 17:33:30.580597 snakeoil-0.9.9/src/snakeoil/test/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (121)      480 2021-12-14 17:33:30.580597 snakeoil-0.9.9/src/snakeoil/test/modules.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2725 2021-12-14 17:33:30.580597 snakeoil-0.9.9/src/snakeoil/test/slot_shadowing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3723 2021-12-14 17:33:30.580597 snakeoil-0.9.9/src/snakeoil/version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1031 2021-12-14 17:33:30.580597 snakeoil-0.9.9/src/snakeoil/weakrefs.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 17:34:12.120603 snakeoil-0.9.9/tests/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 17:34:12.120603 snakeoil-0.9.9/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (121)    18420 2021-12-14 17:33:30.580597 snakeoil-0.9.9/tests/cli/test_arghparse.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4522 2021-12-14 17:33:30.580597 snakeoil-0.9.9/tests/cli/test_input.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8900 2021-12-14 17:33:30.580597 snakeoil-0.9.9/tests/test_bash.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5478 2021-12-14 17:33:30.580597 snakeoil-0.9.9/tests/test_caching.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1432 2021-12-14 17:33:30.580597 snakeoil-0.9.9/tests/test_chksum.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3978 2021-12-14 17:33:30.580597 snakeoil-0.9.9/tests/test_chksum_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7943 2021-12-14 17:33:30.580597 snakeoil-0.9.9/tests/test_containers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4301 2021-12-14 17:33:30.580597 snakeoil-0.9.9/tests/test_contexts.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6918 2021-12-14 17:33:30.580597 snakeoil-0.9.9/tests/test_currying.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6403 2021-12-14 17:33:30.580597 snakeoil-0.9.9/tests/test_data_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1997 2021-12-14 17:33:30.580597 snakeoil-0.9.9/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4460 2021-12-14 17:33:30.580597 snakeoil-0.9.9/tests/test_demandload.py
+-rw-r--r--   0 runner    (1001) docker     (121)      114 2021-12-14 17:33:30.580597 snakeoil-0.9.9/tests/test_demandload_usage.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2738 2021-12-14 17:33:30.580597 snakeoil-0.9.9/tests/test_dependant_methods.py
+-rw-r--r--   0 runner    (1001) docker     (121)      328 2021-12-14 17:33:30.580597 snakeoil-0.9.9/tests/test_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (121)       88 2021-12-14 17:33:30.580597 snakeoil-0.9.9/tests/test_eq_hash_inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11167 2021-12-14 17:33:30.580597 snakeoil-0.9.9/tests/test_fileutils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9615 2021-12-14 17:33:30.580597 snakeoil-0.9.9/tests/test_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4802 2021-12-14 17:33:30.580597 snakeoil-0.9.9/tests/test_iterables.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15215 2021-12-14 17:33:30.580597 snakeoil-0.9.9/tests/test_klass.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19002 2021-12-14 17:33:30.580597 snakeoil-0.9.9/tests/test_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4412 2021-12-14 17:33:30.580597 snakeoil-0.9.9/tests/test_modules.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4550 2021-12-14 17:33:30.580597 snakeoil-0.9.9/tests/test_obj.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17098 2021-12-14 17:33:30.580597 snakeoil-0.9.9/tests/test_osutils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2000 2021-12-14 17:33:30.580597 snakeoil-0.9.9/tests/test_process.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4545 2021-12-14 17:33:30.580597 snakeoil-0.9.9/tests/test_process_spawn.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10347 2021-12-14 17:33:30.580597 snakeoil-0.9.9/tests/test_sequences.py
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2021-12-14 17:33:30.580597 snakeoil-0.9.9/tests/test_slot_shadowing.py
+-rw-r--r--   0 runner    (1001) docker     (121)       98 2021-12-14 17:33:30.580597 snakeoil-0.9.9/tests/test_source_hygene.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1600 2021-12-14 17:33:30.580597 snakeoil-0.9.9/tests/test_stringio.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1522 2021-12-14 17:33:30.580597 snakeoil-0.9.9/tests/test_strings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5921 2021-12-14 17:33:30.580597 snakeoil-0.9.9/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)      458 2021-12-14 17:33:30.580597 snakeoil-0.9.9/tox.ini
```

### Comparing `snakeoil-0.9.8/LICENSE` & `snakeoil-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/NEWS.rst` & `snakeoil-0.9.9/NEWS.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =============
 Release Notes
 =============
 
+snakeoil 0.9.9 (2021-12-14)
+---------------------------
+
+- Fix missing requirement files in sdist.
+
 snakeoil 0.9.8 (2021-12-14)
 ---------------------------
 
 - Fix ``setup.py develop`` support.
 
 - snakeoil.chksum: Add Whirlpool support.
```

### Comparing `snakeoil-0.9.8/PKG-INFO` & `snakeoil-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snakeoil
-Version: 0.9.8
+Version: 0.9.9
 Summary: misc common functionality and useful optimizations
 Home-page: https://github.com/pkgcore/snakeoil
 Author: Tim Harder
 Author-email: radhermit@gmail.com
 License: BSD
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `snakeoil-0.9.8/README.rst` & `snakeoil-0.9.9/README.rst`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/RELEASE.rst` & `snakeoil-0.9.9/RELEASE.rst`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/doc/conf.py` & `snakeoil-0.9.9/doc/conf.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/doc/index.rst` & `snakeoil-0.9.9/doc/index.rst`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/setup.py` & `snakeoil-0.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/src/snakeoil/_fileutils.py` & `snakeoil-0.9.9/src/snakeoil/_fileutils.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/src/snakeoil/_posix.c` & `snakeoil-0.9.9/src/snakeoil/_posix.c`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/src/snakeoil/_posix.pyx` & `snakeoil-0.9.9/src/snakeoil/_posix.pyx`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/src/snakeoil/_sequences.c` & `snakeoil-0.9.9/src/snakeoil/_sequences.c`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/src/snakeoil/_sequences.pyx` & `snakeoil-0.9.9/src/snakeoil/_sequences.pyx`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/src/snakeoil/bash.py` & `snakeoil-0.9.9/src/snakeoil/bash.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/src/snakeoil/caching.py` & `snakeoil-0.9.9/src/snakeoil/caching.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/src/snakeoil/chksum/__init__.py` & `snakeoil-0.9.9/src/snakeoil/chksum/__init__.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/src/snakeoil/chksum/defaults.py` & `snakeoil-0.9.9/src/snakeoil/chksum/defaults.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/src/snakeoil/cli/arghparse.py` & `snakeoil-0.9.9/src/snakeoil/cli/arghparse.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/src/snakeoil/cli/exceptions.py` & `snakeoil-0.9.9/src/snakeoil/cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/src/snakeoil/cli/input.py` & `snakeoil-0.9.9/src/snakeoil/cli/input.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/src/snakeoil/cli/tool.py` & `snakeoil-0.9.9/src/snakeoil/cli/tool.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/src/snakeoil/compatibility.py` & `snakeoil-0.9.9/src/snakeoil/compatibility.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/src/snakeoil/compression/__init__.py` & `snakeoil-0.9.9/src/snakeoil/compression/__init__.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/src/snakeoil/compression/_bzip2.py` & `snakeoil-0.9.9/src/snakeoil/compression/_bzip2.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/src/snakeoil/compression/_util.py` & `snakeoil-0.9.9/src/snakeoil/compression/_util.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/src/snakeoil/containers.py` & `snakeoil-0.9.9/src/snakeoil/containers.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/src/snakeoil/contexts.py` & `snakeoil-0.9.9/src/snakeoil/contexts.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/src/snakeoil/currying.py` & `snakeoil-0.9.9/src/snakeoil/currying.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/src/snakeoil/data_source.py` & `snakeoil-0.9.9/src/snakeoil/data_source.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/src/snakeoil/decorators.py` & `snakeoil-0.9.9/src/snakeoil/decorators.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/src/snakeoil/demandimport.py` & `snakeoil-0.9.9/src/snakeoil/demandimport.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/src/snakeoil/demandload.py` & `snakeoil-0.9.9/src/snakeoil/demandload.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/src/snakeoil/dependant_methods.py` & `snakeoil-0.9.9/src/snakeoil/dependant_methods.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/src/snakeoil/descriptors.py` & `snakeoil-0.9.9/src/snakeoil/descriptors.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/src/snakeoil/dist/distutils_extensions.py` & `snakeoil-0.9.9/src/snakeoil/dist/distutils_extensions.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/src/snakeoil/dist/generate_docs.py` & `snakeoil-0.9.9/src/snakeoil/dist/generate_docs.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/src/snakeoil/dist/generate_man_rsts.py` & `snakeoil-0.9.9/src/snakeoil/dist/generate_man_rsts.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/src/snakeoil/errors.py` & `snakeoil-0.9.9/src/snakeoil/errors.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/src/snakeoil/fileutils.py` & `snakeoil-0.9.9/src/snakeoil/fileutils.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/src/snakeoil/formatters.py` & `snakeoil-0.9.9/src/snakeoil/formatters.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/src/snakeoil/iterables.py` & `snakeoil-0.9.9/src/snakeoil/iterables.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/src/snakeoil/klass.py` & `snakeoil-0.9.9/src/snakeoil/klass.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/src/snakeoil/log.py` & `snakeoil-0.9.9/src/snakeoil/log.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/src/snakeoil/mappings.py` & `snakeoil-0.9.9/src/snakeoil/mappings.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/src/snakeoil/modules.py` & `snakeoil-0.9.9/src/snakeoil/modules.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/src/snakeoil/obj.py` & `snakeoil-0.9.9/src/snakeoil/obj.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/src/snakeoil/osutils/__init__.py` & `snakeoil-0.9.9/src/snakeoil/osutils/__init__.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/src/snakeoil/osutils/mount.py` & `snakeoil-0.9.9/src/snakeoil/osutils/mount.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/src/snakeoil/osutils/native_readdir.py` & `snakeoil-0.9.9/src/snakeoil/osutils/native_readdir.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/src/snakeoil/pickling.py` & `snakeoil-0.9.9/src/snakeoil/pickling.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/src/snakeoil/process/__init__.py` & `snakeoil-0.9.9/src/snakeoil/process/__init__.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/src/snakeoil/process/namespaces.py` & `snakeoil-0.9.9/src/snakeoil/process/namespaces.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/src/snakeoil/process/spawn.py` & `snakeoil-0.9.9/src/snakeoil/process/spawn.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/src/snakeoil/sequences.py` & `snakeoil-0.9.9/src/snakeoil/sequences.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/src/snakeoil/stringio.py` & `snakeoil-0.9.9/src/snakeoil/stringio.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/src/snakeoil/strings.py` & `snakeoil-0.9.9/src/snakeoil/strings.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/src/snakeoil/struct_compat.py` & `snakeoil-0.9.9/src/snakeoil/struct_compat.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/src/snakeoil/tar.py` & `snakeoil-0.9.9/src/snakeoil/tar.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/src/snakeoil/test/__init__.py` & `snakeoil-0.9.9/src/snakeoil/test/__init__.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/src/snakeoil/test/argparse_helpers.py` & `snakeoil-0.9.9/src/snakeoil/test/argparse_helpers.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/src/snakeoil/test/demandload.py` & `snakeoil-0.9.9/src/snakeoil/test/demandload.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/src/snakeoil/test/eq_hash_inheritance.py` & `snakeoil-0.9.9/src/snakeoil/test/eq_hash_inheritance.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/src/snakeoil/test/mixins.py` & `snakeoil-0.9.9/src/snakeoil/test/mixins.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/src/snakeoil/test/slot_shadowing.py` & `snakeoil-0.9.9/src/snakeoil/test/slot_shadowing.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/src/snakeoil/version.py` & `snakeoil-0.9.9/src/snakeoil/version.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/src/snakeoil/weakrefs.py` & `snakeoil-0.9.9/src/snakeoil/weakrefs.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/tests/cli/test_arghparse.py` & `snakeoil-0.9.9/tests/cli/test_arghparse.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/tests/cli/test_input.py` & `snakeoil-0.9.9/tests/cli/test_input.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/tests/test_bash.py` & `snakeoil-0.9.9/tests/test_bash.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/tests/test_caching.py` & `snakeoil-0.9.9/tests/test_caching.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/tests/test_chksum.py` & `snakeoil-0.9.9/tests/test_chksum.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/tests/test_chksum_defaults.py` & `snakeoil-0.9.9/tests/test_chksum_defaults.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/tests/test_containers.py` & `snakeoil-0.9.9/tests/test_containers.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/tests/test_contexts.py` & `snakeoil-0.9.9/tests/test_contexts.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/tests/test_currying.py` & `snakeoil-0.9.9/tests/test_currying.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/tests/test_data_source.py` & `snakeoil-0.9.9/tests/test_data_source.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/tests/test_decorators.py` & `snakeoil-0.9.9/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/tests/test_demandload.py` & `snakeoil-0.9.9/tests/test_demandload.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/tests/test_dependant_methods.py` & `snakeoil-0.9.9/tests/test_dependant_methods.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/tests/test_fileutils.py` & `snakeoil-0.9.9/tests/test_fileutils.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/tests/test_formatters.py` & `snakeoil-0.9.9/tests/test_formatters.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/tests/test_iterables.py` & `snakeoil-0.9.9/tests/test_iterables.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/tests/test_klass.py` & `snakeoil-0.9.9/tests/test_klass.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/tests/test_mappings.py` & `snakeoil-0.9.9/tests/test_mappings.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/tests/test_modules.py` & `snakeoil-0.9.9/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/tests/test_obj.py` & `snakeoil-0.9.9/tests/test_obj.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/tests/test_osutils.py` & `snakeoil-0.9.9/tests/test_osutils.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/tests/test_process.py` & `snakeoil-0.9.9/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/tests/test_process_spawn.py` & `snakeoil-0.9.9/tests/test_process_spawn.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/tests/test_sequences.py` & `snakeoil-0.9.9/tests/test_sequences.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/tests/test_stringio.py` & `snakeoil-0.9.9/tests/test_stringio.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/tests/test_strings.py` & `snakeoil-0.9.9/tests/test_strings.py`

 * *Files identical despite different names*

### Comparing `snakeoil-0.9.8/tests/test_version.py` & `snakeoil-0.9.9/tests/test_version.py`

 * *Files identical despite different names*

