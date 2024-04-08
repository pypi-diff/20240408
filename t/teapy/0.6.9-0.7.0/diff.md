# Comparing `tmp/teapy-0.6.9.tar.gz` & `tmp/teapy-0.7.0.tar.gz`

## Comparing `teapy-0.6.9.tar` & `teapy-0.7.0.tar`

### file list

```diff
@@ -1,163 +1,188 @@
--rw-r--r--   0        0        0     1704 1970-01-01 00:00:00.000000 teapy-0.6.9/local_dependencies/tea-core/Cargo.toml
--rw-r--r--   0     1001      127    15449 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-core/src/arbarray.rs
--rw-r--r--   0     1001      127    25285 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-core/src/arrok.rs
--rw-r--r--   0     1001      127    16304 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-core/src/impls/impl_1d_method.rs
--rw-r--r--   0     1001      127     4115 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-core/src/impls/impl_basic.rs
--rw-r--r--   0     1001      127     8421 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-core/src/impls/impl_method.rs
--rw-r--r--   0     1001      127     8160 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-core/src/impls/impl_numeric.rs
--rw-r--r--   0     1001      127      648 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-core/src/impls/impl_time.rs
--rw-r--r--   0     1001      127     6070 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-core/src/impls/impl_traits.rs
--rw-r--r--   0     1001      127      451 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-core/src/impls/linalg/generate.rs
--rw-r--r--   0     1001      127     7390 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-core/src/impls/linalg/layout.rs
--rw-r--r--   0     1001      127     9212 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-core/src/impls/linalg/least_squares.rs
--rw-r--r--   0     1001      127      242 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-core/src/impls/linalg/mod.rs
--rw-r--r--   0     1001      127     5016 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-core/src/impls/linalg/svd.rs
--rw-r--r--   0     1001      127      436 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-core/src/impls/linalg/utils.rs
--rw-r--r--   0     1001      127      312 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-core/src/impls/mod.rs
--rw-r--r--   0     1001      127    10460 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-core/src/iterators.rs
--rw-r--r--   0     1001      127    14095 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-core/src/lib.rs
--rw-r--r--   0     1001      127    10802 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-core/src/macros.rs
--rw-r--r--   0     1001      127     3011 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-core/src/own.rs
--rw-r--r--   0     1001      127      721 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-core/src/prelude.rs
--rw-r--r--   0     1001      127      694 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-core/src/traits.rs
--rw-r--r--   0     1001      127     3045 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-core/src/view.rs
--rw-r--r--   0     1001      127     2031 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-core/src/viewmut.rs
--rw-r--r--   0        0        0      276 1970-01-01 00:00:00.000000 teapy-0.6.9/local_dependencies/tea-utils/Cargo.toml
--rw-r--r--   0     1001      127     3666 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-utils/src/algos.rs
--rw-r--r--   0     1001      127     1798 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-utils/src/alloc.rs
--rw-r--r--   0     1001      127      231 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-utils/src/lib.rs
--rw-r--r--   0     1001      127      324 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-utils/src/macros.rs
--rw-r--r--   0     1001      127     2274 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-utils/src/traits.rs
--rw-r--r--   0        0        0     1086 1970-01-01 00:00:00.000000 teapy-0.6.9/local_dependencies/tea-groupby/Cargo.toml
--rw-r--r--   0     1001      127     1044 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-groupby/benches/groupby.rs
--rw-r--r--   0     1001      127      613 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-groupby/src/from_py.rs
--rw-r--r--   0     1001      127     9556 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-groupby/src/groupby_agg.rs
--rw-r--r--   0     1001      127     5194 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-groupby/src/impl_lazy.rs
--rw-r--r--   0     1001      127    15329 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-groupby/src/join.rs
--rw-r--r--   0     1001      127    15486 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-groupby/src/lib.rs
--rw-r--r--   0     1001      127     7104 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-groupby/src/unique.rs
--rw-r--r--   0        0        0      395 1970-01-01 00:00:00.000000 teapy-0.6.9/local_dependencies/tea-time/Cargo.toml
--rw-r--r--   0     1001      127      755 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-time/src/convert.rs
--rw-r--r--   0     1001      127     9104 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-time/src/datetime.rs
--rw-r--r--   0     1001      127     1995 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-time/src/impls/impl_datetime.rs
--rw-r--r--   0     1001      127     2094 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-time/src/impls/impl_ops.rs
--rw-r--r--   0     1001      127      869 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-time/src/impls/impl_timedelta.rs
--rw-r--r--   0     1001      127       53 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-time/src/impls/mod.rs
--rw-r--r--   0     1001      127      198 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-time/src/lib.rs
--rw-r--r--   0     1001      127     2980 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-time/src/timedelta.rs
--rw-r--r--   0     1001      127      842 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-time/src/timeunit.rs
--rw-r--r--   0        0        0      862 1970-01-01 00:00:00.000000 teapy-0.6.9/local_dependencies/tea-lazy/Cargo.toml
--rw-r--r--   0     1001      127      236 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-lazy/src/datadict/context.rs
--rw-r--r--   0     1001      127    23111 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-lazy/src/datadict/dict.rs
--rw-r--r--   0     1001      127     3254 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-lazy/src/datadict/get_set.rs
--rw-r--r--   0     1001      127      189 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-lazy/src/datadict/mod.rs
--rw-r--r--   0     1001      127     3114 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-lazy/src/datadict/selector.rs
--rw-r--r--   0     1001      127    11891 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-lazy/src/expr_core/data.rs
--rw-r--r--   0     1001      127    11857 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-lazy/src/expr_core/expr.rs
--rw-r--r--   0     1001      127     1172 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-lazy/src/expr_core/expr_element.rs
--rw-r--r--   0     1001      127    11553 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-lazy/src/expr_core/expr_inner.rs
--rw-r--r--   0     1001      127     6642 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-lazy/src/expr_core/impls/auto_impl.rs
--rw-r--r--   0     1001      127     3184 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-lazy/src/expr_core/impls/impl_cast.rs
--rw-r--r--   0     1001      127     1394 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-lazy/src/expr_core/impls/impl_dtype_judge.rs
--rw-r--r--   0     1001      127    15326 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-lazy/src/expr_core/impls/impl_ops.rs
--rw-r--r--   0     1001      127      889 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-lazy/src/expr_core/impls/mod.rs
--rw-r--r--   0     1001      127     2393 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-lazy/src/expr_core/impls/utils.rs
--rw-r--r--   0     1001      127      404 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-lazy/src/expr_core/mod.rs
--rw-r--r--   0     1001      127    14135 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-lazy/src/groupby.rs
--rw-r--r--   0     1001      127    11113 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-lazy/src/join.rs
--rw-r--r--   0     1001      127      415 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-lazy/src/lib.rs
--rw-r--r--   0     1001      127     8791 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-lazy/src/linalg.rs
--rw-r--r--   0        0        0     1370 1970-01-01 00:00:00.000000 teapy-0.6.9/local_dependencies/tea-ext/Cargo.toml
--rw-r--r--   0     1001      127      483 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-ext/benches/inplace.rs
--rw-r--r--   0     1001      127     3128 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-ext/benches/rolling.rs
--rw-r--r--   0     1001      127     7438 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-ext/src/agg/corr.rs
--rw-r--r--   0     1001      127     4196 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-ext/src/agg/impl_lazy.rs
--rw-r--r--   0     1001      127    15258 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-ext/src/agg/mod.rs
--rw-r--r--   0     1001      127     2200 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-ext/src/create.rs
--rw-r--r--   0     1001      127     3794 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-ext/src/from_py.rs
--rw-r--r--   0     1001      127      507 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-ext/src/lib.rs
--rw-r--r--   0     1001      127     8740 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-ext/src/linalg.rs
--rw-r--r--   0     1001      127     1993 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-ext/src/macros.rs
--rw-r--r--   0     1001      127     9597 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-ext/src/map/impl_1d.rs
--rw-r--r--   0     1001      127     8689 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-ext/src/map/impl_arrok.rs
--rw-r--r--   0     1001      127     9095 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-ext/src/map/impl_inplace.rs
--rw-r--r--   0     1001      127    10244 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-ext/src/map/impl_lazy/impl_view.rs
--rw-r--r--   0     1001      127    15659 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-ext/src/map/impl_lazy/mod.rs
--rw-r--r--   0     1001      127     2000 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-ext/src/map/impl_lazy/stat.rs
--rw-r--r--   0     1001      127     1220 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-ext/src/map/impl_lazy/time.rs
--rw-r--r--   0     1001      127      834 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-ext/src/map/impl_string.rs
--rw-r--r--   0     1001      127      787 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-ext/src/map/impl_time.rs
--rw-r--r--   0     1001      127    21550 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-ext/src/map/mod.rs
--rw-r--r--   0     1001      127    15701 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-ext/src/rolling/cmp.rs
--rw-r--r--   0     1001      127     8069 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-ext/src/rolling/corr.rs
--rw-r--r--   0     1001      127    26072 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-ext/src/rolling/feature.rs
--rw-r--r--   0     1001      127     1039 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-ext/src/rolling/impl_lazy/auto_impl.rs
--rw-r--r--   0     1001      127    22608 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-ext/src/rolling/impl_lazy/common.rs
--rw-r--r--   0     1001      127      311 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-ext/src/rolling/impl_lazy/mod.rs
--rw-r--r--   0     1001      127      225 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-ext/src/rolling/mod.rs
--rw-r--r--   0     1001      127     9721 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-ext/src/rolling/norm.rs
--rw-r--r--   0     1001      127    29920 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-ext/src/rolling/reg.rs
--rw-r--r--   0        0        0      717 1970-01-01 00:00:00.000000 teapy-0.6.9/local_dependencies/tea-dtype/Cargo.toml
--rw-r--r--   0     1001      127    13696 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-dtype/src/cast.rs
--rw-r--r--   0     1001      127    14610 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-dtype/src/lib.rs
--rw-r--r--   0     1001      127    12152 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-dtype/src/option_datatype.rs
--rw-r--r--   0     1001      127     2369 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-dtype/src/pyvalue.rs
--rw-r--r--   0        0        0      797 1970-01-01 00:00:00.000000 teapy-0.6.9/local_dependencies/tea-io/Cargo.toml
--rw-r--r--   0     1001      127     1895 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-io/src/arrow_io/impl_lazy.rs
--rw-r--r--   0     1001      127     5490 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-io/src/arrow_io/ipc.rs
--rw-r--r--   0     1001      127      188 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-io/src/arrow_io/mod.rs
--rw-r--r--   0     1001      127     1004 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-io/src/arrow_io/utils.rs
--rw-r--r--   0     1001      127     2394 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-io/src/colselect.rs
--rw-r--r--   0     1001      127      236 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-io/src/lib.rs
--rw-r--r--   0        0        0      521 1970-01-01 00:00:00.000000 teapy-0.6.9/local_dependencies/tea-macros/Cargo.toml
--rw-r--r--   0     1001      127    14011 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-macros/src/lazy_impls.rs
--rw-r--r--   0     1001      127     1606 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-macros/src/lib.rs
--rw-r--r--   0     1001      127     6291 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-macros/src/methods_impls.rs
--rw-r--r--   0     1001      127    21958 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-macros/src/tools.rs
--rw-r--r--   0        0        0      504 1970-01-01 00:00:00.000000 teapy-0.6.9/local_dependencies/tea-hash/Cargo.toml
--rw-r--r--   0     1001      127     3243 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-hash/src/lib.rs
--rw-r--r--   0        0        0      449 1970-01-01 00:00:00.000000 teapy-0.6.9/local_dependencies/tea-error/Cargo.toml
--rw-r--r--   0     1001      127     1398 2024-03-08 05:23:09.000000 teapy-0.6.9/local_dependencies/tea-error/src/lib.rs
--rw-r--r--   0        0        0     2213 1970-01-01 00:00:00.000000 teapy-0.6.9/Cargo.toml
--rw-r--r--   0     1001      127        8 2024-03-08 05:23:09.000000 teapy-0.6.9/.python-version
--rw-r--r--   0     1001      127     1053 2024-03-08 05:23:09.000000 teapy-0.6.9/LICENSE
--rw-r--r--   0     1001      127     1474 2024-03-08 05:23:09.000000 teapy-0.6.9/Makefile
--rw-r--r--   0     1001      127     2202 2024-03-08 05:23:09.000000 teapy-0.6.9/README.md
--rw-r--r--   0     1001      127      214 2024-03-08 05:23:09.000000 teapy-0.6.9/build.requirements.txt
--rw-r--r--   0     1001      127      850 2024-03-08 05:23:09.000000 teapy-0.6.9/pyproject.toml
--rw-r--r--   0     1001      127     2425 2024-03-08 05:23:09.000000 teapy-0.6.9/python/teapy/__init__.py
--rw-r--r--   0     1001      127     4513 2024-03-08 05:23:09.000000 teapy-0.6.9/python/teapy/array_func.py
--rw-r--r--   0     1001      127    14725 2024-03-08 05:23:09.000000 teapy-0.6.9/python/teapy/datadict.py
--rw-r--r--   0     1001      127    11271 2024-03-08 05:23:09.000000 teapy-0.6.9/python/teapy/expr.py
--rw-r--r--   0     1001      127     2747 2024-03-08 05:23:09.000000 teapy-0.6.9/python/teapy/mod_func.py
--rw-r--r--   0     1001      127     9297 2024-03-08 05:23:09.000000 teapy-0.6.9/python/teapy/regression.py
--rw-r--r--   0     1001      127     3440 2024-03-08 05:23:09.000000 teapy-0.6.9/python/teapy/testing.py
--rw-r--r--   0     1001      127    12432 2024-03-08 05:23:09.000000 teapy-0.6.9/python/teapy/tests/test_array_func.py
--rw-r--r--   0     1001      127     2142 2024-03-08 05:23:09.000000 teapy-0.6.9/python/teapy/tests/test_common.py
--rw-r--r--   0     1001      127     1061 2024-03-08 05:23:09.000000 teapy-0.6.9/python/teapy/tests/test_context.py
--rw-r--r--   0     1001      127     8570 2024-03-08 05:23:09.000000 teapy-0.6.9/python/teapy/tests/test_datadict.py
--rw-r--r--   0     1001      127     2309 2024-03-08 05:23:09.000000 teapy-0.6.9/python/teapy/tests/test_equity.py
--rw-r--r--   0     1001      127     4773 2024-03-08 05:23:09.000000 teapy-0.6.9/python/teapy/tests/test_expr.py
--rw-r--r--   0     1001      127      465 2024-03-08 05:23:09.000000 teapy-0.6.9/python/teapy/tests/test_memory.py
--rw-r--r--   0     1001      127      339 2024-03-08 05:23:09.000000 teapy-0.6.9/python/teapy/tests/test_time.py
--rw-r--r--   0     1001      127     3210 2024-03-08 05:23:09.000000 teapy-0.6.9/python/teapy/tests/window/test_compare.py
--rw-r--r--   0     1001      127     1417 2024-03-08 05:23:09.000000 teapy-0.6.9/python/teapy/tests/window/test_corr.py
--rw-r--r--   0     1001      127     5771 2024-03-08 05:23:09.000000 teapy-0.6.9/python/teapy/tests/window/test_feature.py
--rw-r--r--   0     1001      127     1994 2024-03-08 05:23:09.000000 teapy-0.6.9/python/teapy/tests/window/test_norm.py
--rw-r--r--   0     1001      127     3194 2024-03-08 05:23:09.000000 teapy-0.6.9/python/teapy/tests/window/test_reg.py
--rw-r--r--   0     1001      127     3458 2024-03-08 05:23:09.000000 teapy-0.6.9/python/teapy/window_func.py
--rw-r--r--   0     1001      127     1232 2024-03-08 05:23:09.000000 teapy-0.6.9/python/teapy/wrapper.py
--rw-r--r--   0     1001      127     1291 2024-03-08 05:23:09.000000 teapy-0.6.9/requirements-dev.lock
--rw-r--r--   0     1001      127      197 2024-03-08 05:23:09.000000 teapy-0.6.9/requirements.lock
--rw-r--r--   0     1001      127    23237 2024-03-08 05:23:09.000000 teapy-0.6.9/src/equity.rs
--rw-r--r--   0     1001      127     6762 2024-03-08 05:23:09.000000 teapy-0.6.9/src/from_py.rs
--rw-r--r--   0     1001      127     1127 2024-03-08 05:23:09.000000 teapy-0.6.9/src/lib.rs
--rw-r--r--   0     1001      127    20187 2024-03-08 05:23:09.000000 teapy-0.6.9/src/pylazy/datadict.rs
--rw-r--r--   0     1001      127      375 2024-03-08 05:23:09.000000 teapy-0.6.9/src/pylazy/export.rs
--rw-r--r--   0     1001      127     2929 2024-03-08 05:23:09.000000 teapy-0.6.9/src/pylazy/groupby.rs
--rw-r--r--   0     1001      127    96862 2024-03-08 05:23:09.000000 teapy-0.6.9/src/pylazy/impl_pyexpr.rs
--rw-r--r--   0     1001      127     1797 2024-03-08 05:23:09.000000 teapy-0.6.9/src/pylazy/mod.rs
--rw-r--r--   0     1001      127     5339 2024-03-08 05:23:09.000000 teapy-0.6.9/src/pylazy/pyexpr.rs
--rw-r--r--   0     1001      127    23425 2024-03-08 05:23:09.000000 teapy-0.6.9/src/pylazy/pyfunc.rs
--rw-r--r--   0     1001      127    54846 2024-03-08 05:23:53.000000 teapy-0.6.9/Cargo.lock
--rw-r--r--   0        0        0     2717 1970-01-01 00:00:00.000000 teapy-0.6.9/PKG-INFO
+-rw-r--r--   0     1001      127      811 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-lazy/Cargo.toml
+-rw-r--r--   0     1001      127      236 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-lazy/src/datadict/context.rs
+-rw-r--r--   0     1001      127    23111 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-lazy/src/datadict/dict.rs
+-rw-r--r--   0     1001      127     3254 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-lazy/src/datadict/get_set.rs
+-rw-r--r--   0     1001      127      189 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-lazy/src/datadict/mod.rs
+-rw-r--r--   0     1001      127     3114 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-lazy/src/datadict/selector.rs
+-rw-r--r--   0     1001      127    11891 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-lazy/src/expr_core/data.rs
+-rw-r--r--   0     1001      127    11857 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-lazy/src/expr_core/expr.rs
+-rw-r--r--   0     1001      127     1172 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-lazy/src/expr_core/expr_element.rs
+-rw-r--r--   0     1001      127    11553 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-lazy/src/expr_core/expr_inner.rs
+-rw-r--r--   0     1001      127     6642 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-lazy/src/expr_core/impls/auto_impl.rs
+-rw-r--r--   0     1001      127     3184 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-lazy/src/expr_core/impls/impl_cast.rs
+-rw-r--r--   0     1001      127     1394 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-lazy/src/expr_core/impls/impl_dtype_judge.rs
+-rw-r--r--   0     1001      127    15326 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-lazy/src/expr_core/impls/impl_ops.rs
+-rw-r--r--   0     1001      127      889 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-lazy/src/expr_core/impls/mod.rs
+-rw-r--r--   0     1001      127     2393 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-lazy/src/expr_core/impls/utils.rs
+-rw-r--r--   0     1001      127      404 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-lazy/src/expr_core/mod.rs
+-rw-r--r--   0     1001      127    14135 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-lazy/src/groupby.rs
+-rw-r--r--   0     1001      127    11113 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-lazy/src/join.rs
+-rw-r--r--   0     1001      127      415 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-lazy/src/lib.rs
+-rw-r--r--   0     1001      127     8791 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-lazy/src/linalg.rs
+-rw-r--r--   0     1001      127     1303 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-ext/Cargo.toml
+-rw-r--r--   0     1001      127      483 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-ext/benches/inplace.rs
+-rw-r--r--   0     1001      127     3128 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-ext/benches/rolling.rs
+-rw-r--r--   0     1001      127     7438 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-ext/src/agg/corr.rs
+-rw-r--r--   0     1001      127     4196 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-ext/src/agg/impl_lazy.rs
+-rw-r--r--   0     1001      127    15258 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-ext/src/agg/mod.rs
+-rw-r--r--   0     1001      127     2200 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-ext/src/create.rs
+-rw-r--r--   0     1001      127     3794 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-ext/src/from_py.rs
+-rw-r--r--   0     1001      127      507 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-ext/src/lib.rs
+-rw-r--r--   0     1001      127     8740 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-ext/src/linalg.rs
+-rw-r--r--   0     1001      127     1993 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-ext/src/macros.rs
+-rw-r--r--   0     1001      127     9597 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-ext/src/map/impl_1d.rs
+-rw-r--r--   0     1001      127     8689 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-ext/src/map/impl_arrok.rs
+-rw-r--r--   0     1001      127     9095 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-ext/src/map/impl_inplace.rs
+-rw-r--r--   0     1001      127    10244 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-ext/src/map/impl_lazy/impl_view.rs
+-rw-r--r--   0     1001      127    15659 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-ext/src/map/impl_lazy/mod.rs
+-rw-r--r--   0     1001      127     2000 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-ext/src/map/impl_lazy/stat.rs
+-rw-r--r--   0     1001      127     1220 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-ext/src/map/impl_lazy/time.rs
+-rw-r--r--   0     1001      127      834 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-ext/src/map/impl_string.rs
+-rw-r--r--   0     1001      127      787 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-ext/src/map/impl_time.rs
+-rw-r--r--   0     1001      127    21550 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-ext/src/map/mod.rs
+-rw-r--r--   0     1001      127    15701 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-ext/src/rolling/cmp.rs
+-rw-r--r--   0     1001      127     8069 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-ext/src/rolling/corr.rs
+-rw-r--r--   0     1001      127    26072 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-ext/src/rolling/feature.rs
+-rw-r--r--   0     1001      127    22608 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-ext/src/rolling/impl_lazy/common.rs
+-rw-r--r--   0     1001      127      311 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-ext/src/rolling/impl_lazy/mod.rs
+-rw-r--r--   0     1001      127      225 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-ext/src/rolling/mod.rs
+-rw-r--r--   0     1001      127     9721 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-ext/src/rolling/norm.rs
+-rw-r--r--   0     1001      127    32087 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-ext/src/rolling/reg.rs
+-rw-r--r--   0     1001      127      463 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-hash/Cargo.toml
+-rw-r--r--   0     1001      127     3243 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-hash/src/lib.rs
+-rw-r--r--   0     1001      127      289 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-time/Cargo.toml
+-rw-r--r--   0     1001      127      755 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-time/src/convert.rs
+-rw-r--r--   0     1001      127     9104 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-time/src/datetime.rs
+-rw-r--r--   0     1001      127     1995 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-time/src/impls/impl_datetime.rs
+-rw-r--r--   0     1001      127     2094 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-time/src/impls/impl_ops.rs
+-rw-r--r--   0     1001      127      869 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-time/src/impls/impl_timedelta.rs
+-rw-r--r--   0     1001      127       53 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-time/src/impls/mod.rs
+-rw-r--r--   0     1001      127      198 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-time/src/lib.rs
+-rw-r--r--   0     1001      127     2980 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-time/src/timedelta.rs
+-rw-r--r--   0     1001      127      842 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-time/src/timeunit.rs
+-rw-r--r--   0     1001      127     1583 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-core/Cargo.toml
+-rw-r--r--   0     1001      127    15449 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-core/src/arbarray.rs
+-rw-r--r--   0     1001      127    25285 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-core/src/arrok.rs
+-rw-r--r--   0     1001      127    16304 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-core/src/impls/impl_1d_method.rs
+-rw-r--r--   0     1001      127     4115 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-core/src/impls/impl_basic.rs
+-rw-r--r--   0     1001      127     8421 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-core/src/impls/impl_method.rs
+-rw-r--r--   0     1001      127     8160 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-core/src/impls/impl_numeric.rs
+-rw-r--r--   0     1001      127      648 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-core/src/impls/impl_time.rs
+-rw-r--r--   0     1001      127     6070 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-core/src/impls/impl_traits.rs
+-rw-r--r--   0     1001      127      451 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-core/src/impls/linalg/generate.rs
+-rw-r--r--   0     1001      127     7390 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-core/src/impls/linalg/layout.rs
+-rw-r--r--   0     1001      127     9212 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-core/src/impls/linalg/least_squares.rs
+-rw-r--r--   0     1001      127      242 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-core/src/impls/linalg/mod.rs
+-rw-r--r--   0     1001      127     5016 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-core/src/impls/linalg/svd.rs
+-rw-r--r--   0     1001      127      436 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-core/src/impls/linalg/utils.rs
+-rw-r--r--   0     1001      127      312 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-core/src/impls/mod.rs
+-rw-r--r--   0     1001      127    10460 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-core/src/iterators.rs
+-rw-r--r--   0     1001      127    14095 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-core/src/lib.rs
+-rw-r--r--   0     1001      127    10802 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-core/src/macros.rs
+-rw-r--r--   0     1001      127     3011 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-core/src/own.rs
+-rw-r--r--   0     1001      127      721 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-core/src/prelude.rs
+-rw-r--r--   0     1001      127      694 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-core/src/traits.rs
+-rw-r--r--   0     1001      127     3045 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-core/src/view.rs
+-rw-r--r--   0     1001      127     2031 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-core/src/viewmut.rs
+-rw-r--r--   0     1001      127     1030 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-groupby/Cargo.toml
+-rw-r--r--   0     1001      127     1044 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-groupby/benches/groupby.rs
+-rw-r--r--   0     1001      127      613 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-groupby/src/from_py.rs
+-rw-r--r--   0     1001      127     9556 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-groupby/src/groupby_agg.rs
+-rw-r--r--   0     1001      127     5194 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-groupby/src/impl_lazy.rs
+-rw-r--r--   0     1001      127    15329 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-groupby/src/join.rs
+-rw-r--r--   0     1001      127    15486 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-groupby/src/lib.rs
+-rw-r--r--   0     1001      127     7104 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-groupby/src/unique.rs
+-rw-r--r--   0     1001      127      708 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-io/Cargo.toml
+-rw-r--r--   0     1001      127     2062 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-io/src/arrow_io/impl_lazy.rs
+-rw-r--r--   0     1001      127     5490 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-io/src/arrow_io/ipc.rs
+-rw-r--r--   0     1001      127      203 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-io/src/arrow_io/mod.rs
+-rw-r--r--   0     1001      127     1004 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-io/src/arrow_io/utils.rs
+-rw-r--r--   0     1001      127     2394 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-io/src/colselect.rs
+-rw-r--r--   0     1001      127      251 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-io/src/lib.rs
+-rw-r--r--   0     1001      127      488 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-macros/Cargo.toml
+-rw-r--r--   0     1001      127    14011 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-macros/src/lazy_impls.rs
+-rw-r--r--   0     1001      127     1606 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-macros/src/lib.rs
+-rw-r--r--   0     1001      127     6291 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-macros/src/methods_impls.rs
+-rw-r--r--   0     1001      127    21958 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-macros/src/tools.rs
+-rw-r--r--   0     1001      127      619 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-dtype/Cargo.toml
+-rw-r--r--   0     1001      127    13696 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-dtype/src/cast.rs
+-rw-r--r--   0     1001      127    14610 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-dtype/src/lib.rs
+-rw-r--r--   0     1001      127    12152 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-dtype/src/option_datatype.rs
+-rw-r--r--   0     1001      127     2524 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-dtype/src/pyvalue.rs
+-rw-r--r--   0     1001      127      271 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-utils/Cargo.toml
+-rw-r--r--   0     1001      127     3666 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-utils/src/algos.rs
+-rw-r--r--   0     1001      127     1798 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-utils/src/alloc.rs
+-rw-r--r--   0     1001      127      231 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-utils/src/lib.rs
+-rw-r--r--   0     1001      127      324 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-utils/src/macros.rs
+-rw-r--r--   0     1001      127     2274 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-utils/src/traits.rs
+-rw-r--r--   0     1001      127      286 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-error/Cargo.toml
+-rw-r--r--   0     1001      127     1398 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-error/src/lib.rs
+-rw-r--r--   0        0        0     2069 1970-01-01 00:00:00.000000 teapy-0.7.0/tea-py/Cargo.toml
+-rw-r--r--   0     1001      127        8 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/.python-version
+-rw-r--r--   0     1001      127     1053 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/LICENSE
+-rw-r--r--   0     1001      127     1417 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/Makefile
+-rw-r--r--   0     1001      127     2202 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/README.md
+-rw-r--r--   0     1001      127      232 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/build.requirements.txt
+-rw-r--r--   0     1001      127     2765 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/python/teapy/__init__.py
+-rw-r--r--   0     1001      127     4525 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/python/teapy/array_func.py
+-rw-r--r--   0     1001      127    11351 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/python/teapy/expr.py
+-rw-r--r--   0     1001      127     3271 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/python/teapy/mod_func.py
+-rw-r--r--   0     1001      127    18730 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/python/teapy/py_datadict.py
+-rw-r--r--   0     1001      127     9635 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/python/teapy/regression.py
+-rw-r--r--   0     1001      127     7368 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/python/teapy/selector.py
+-rw-r--r--   0     1001      127     3455 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/python/teapy/testing.py
+-rw-r--r--   0     1001      127    12448 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/python/teapy/tests/test_array_func.py
+-rw-r--r--   0     1001      127     2094 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/python/teapy/tests/test_common.py
+-rw-r--r--   0     1001      127      967 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/python/teapy/tests/test_context.py
+-rw-r--r--   0     1001      127     8565 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/python/teapy/tests/test_datadict.py
+-rw-r--r--   0     1001      127     2303 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/python/teapy/tests/test_equity.py
+-rw-r--r--   0     1001      127     4772 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/python/teapy/tests/test_expr.py
+-rw-r--r--   0     1001      127      465 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/python/teapy/tests/test_memory.py
+-rw-r--r--   0     1001      127      339 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/python/teapy/tests/test_time.py
+-rw-r--r--   0     1001      127     3210 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/python/teapy/tests/window/test_compare.py
+-rw-r--r--   0     1001      127     1417 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/python/teapy/tests/window/test_corr.py
+-rw-r--r--   0     1001      127     5771 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/python/teapy/tests/window/test_feature.py
+-rw-r--r--   0     1001      127     1994 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/python/teapy/tests/window/test_norm.py
+-rw-r--r--   0     1001      127     3194 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/python/teapy/tests/window/test_reg.py
+-rw-r--r--   0     1001      127     3458 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/python/teapy/window_func.py
+-rw-r--r--   0     1001      127     1232 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/python/teapy/wrapper.py
+-rw-r--r--   0     1001      127     1291 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/requirements-dev.lock
+-rw-r--r--   0     1001      127      197 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/requirements.lock
+-rw-r--r--   0     1001      127    23237 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/src/equity.rs
+-rw-r--r--   0     1001      127     7135 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/src/from_py.rs
+-rw-r--r--   0     1001      127     1127 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/src/lib.rs
+-rw-r--r--   0     1001      127    13232 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/src/pylazy/datadict.rs
+-rw-r--r--   0     1001      127      322 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/src/pylazy/export.rs
+-rw-r--r--   0     1001      127     2929 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/src/pylazy/groupby.rs
+-rw-r--r--   0     1001      127    97443 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/src/pylazy/impl_pyexpr.rs
+-rw-r--r--   0     1001      127     1898 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/src/pylazy/mod.rs
+-rw-r--r--   0     1001      127     5339 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/src/pylazy/pyexpr.rs
+-rw-r--r--   0     1001      127    18850 2024-04-08 02:51:41.000000 teapy-0.7.0/tea-py/src/pylazy/pyfunc.rs
+-rw-r--r--   0     1001      127     2202 2024-04-08 02:51:41.000000 teapy-0.7.0/README.md
+-rw-r--r--   0     1001      127    55023 2024-04-08 02:52:23.000000 teapy-0.7.0/Cargo.lock
+-rw-r--r--   0        0        0     1049 1970-01-01 00:00:00.000000 teapy-0.7.0/Cargo.toml
+-rw-r--r--   0        0        0     2176 1970-01-01 00:00:00.000000 teapy-0.7.0/pyproject.toml
+-rw-r--r--   0     1001      127    11351 2024-04-08 02:51:41.000000 teapy-0.7.0/python/teapy/expr.py
+-rw-r--r--   0     1001      127     2765 2024-04-08 02:51:41.000000 teapy-0.7.0/python/teapy/__init__.py
+-rw-r--r--   0     1001      127     3271 2024-04-08 02:51:41.000000 teapy-0.7.0/python/teapy/mod_func.py
+-rw-r--r--   0     1001      127      339 2024-04-08 02:51:41.000000 teapy-0.7.0/python/teapy/tests/test_time.py
+-rw-r--r--   0     1001      127      967 2024-04-08 02:51:41.000000 teapy-0.7.0/python/teapy/tests/test_context.py
+-rw-r--r--   0     1001      127     2303 2024-04-08 02:51:41.000000 teapy-0.7.0/python/teapy/tests/test_equity.py
+-rw-r--r--   0     1001      127     2094 2024-04-08 02:51:41.000000 teapy-0.7.0/python/teapy/tests/test_common.py
+-rw-r--r--   0     1001      127     4772 2024-04-08 02:51:41.000000 teapy-0.7.0/python/teapy/tests/test_expr.py
+-rw-r--r--   0     1001      127      465 2024-04-08 02:51:41.000000 teapy-0.7.0/python/teapy/tests/test_memory.py
+-rw-r--r--   0     1001      127    12448 2024-04-08 02:51:41.000000 teapy-0.7.0/python/teapy/tests/test_array_func.py
+-rw-r--r--   0     1001      127     8565 2024-04-08 02:51:41.000000 teapy-0.7.0/python/teapy/tests/test_datadict.py
+-rw-r--r--   0     1001      127     3210 2024-04-08 02:51:41.000000 teapy-0.7.0/python/teapy/tests/window/test_compare.py
+-rw-r--r--   0     1001      127     1417 2024-04-08 02:51:41.000000 teapy-0.7.0/python/teapy/tests/window/test_corr.py
+-rw-r--r--   0     1001      127     5771 2024-04-08 02:51:41.000000 teapy-0.7.0/python/teapy/tests/window/test_feature.py
+-rw-r--r--   0     1001      127     3194 2024-04-08 02:51:41.000000 teapy-0.7.0/python/teapy/tests/window/test_reg.py
+-rw-r--r--   0     1001      127     1994 2024-04-08 02:51:41.000000 teapy-0.7.0/python/teapy/tests/window/test_norm.py
+-rw-r--r--   0     1001      127     9635 2024-04-08 02:51:41.000000 teapy-0.7.0/python/teapy/regression.py
+-rw-r--r--   0     1001      127    18730 2024-04-08 02:51:41.000000 teapy-0.7.0/python/teapy/py_datadict.py
+-rw-r--r--   0     1001      127     3458 2024-04-08 02:51:41.000000 teapy-0.7.0/python/teapy/window_func.py
+-rw-r--r--   0     1001      127     4525 2024-04-08 02:51:41.000000 teapy-0.7.0/python/teapy/array_func.py
+-rw-r--r--   0     1001      127     1232 2024-04-08 02:51:41.000000 teapy-0.7.0/python/teapy/wrapper.py
+-rw-r--r--   0     1001      127     7368 2024-04-08 02:51:41.000000 teapy-0.7.0/python/teapy/selector.py
+-rw-r--r--   0     1001      127     3455 2024-04-08 02:51:41.000000 teapy-0.7.0/python/teapy/testing.py
+-rw-r--r--   0        0        0     2804 1970-01-01 00:00:00.000000 teapy-0.7.0/PKG-INFO
```

### Comparing `teapy-0.6.9/local_dependencies/tea-core/Cargo.toml` & `teapy-0.7.0/tea-core/Cargo.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 [package]
 name = "tea-core"
-version= "0.6.9"
-authors= ["Teamon"]
-edition= "2021"
-repository= "https://github.com/Teamon9161/teapy"
-license= "MIT"
-resolver = "2"
+version.workspace = true
+authors.workspace = true
+edition.workspace = true
+repository.workspace = true
+license.workspace = true
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [features]
 # default = ["extend", "method_1d", "ops", "blas", "concat", "arw"]
 # default = ["extend", "ops"]
 default = []
 extend = ["option_dtype", "time"]
@@ -30,20 +29,20 @@
 openblas-system = ["openblas-src/system"]
 
 intel-mkl-static = ["intel-mkl-src/mkl-static-lp64-seq"]
 intel-mkl-system = ["intel-mkl-src/mkl-dynamic-lp64-seq"]
 
 [dependencies]
 tea-dtype = { path = "../tea-dtype", default-features = false}
-tea-utils = { path = "../tea-utils" }
+tea-utils = { path = "../tea-utils"}
 tea-error = { path = "../tea-error", default-features = false }
-ndarray = {features=['rayon', 'serde'], version="0.15"}
-num = "0.4"
-rayon = "1.5"
-libc = "0.2"
+ndarray = { workspace = true }
+num = { workspace = true }
+rayon = { workspace = true }
+libc = { workspace=true }
 
-pyo3 = {version = "0.20.0", features = ["extension-module", "abi3-py38", "macros", "serde"]}
+pyo3 = { workspace = true}
 lapack-sys = { version="0.14.0", optional=true }
 intel-mkl-src = { version = "0.8.1", default-features = false, optional = true }
 openblas-src = { version = "0.10.4", optional = true, default-features = false, features = ["cblas"] }
 # statrs = { version = "0.16", optional=true }
-arrow = {package = "arrow2", version = "0.18.0", default-features = false, features = ["io_ipc", "io_ipc_compression"]}
+arrow = { workspace=true, default-features = false }
```

### Comparing `teapy-0.6.9/local_dependencies/tea-core/src/arbarray.rs` & `teapy-0.7.0/tea-core/src/arbarray.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-core/src/arrok.rs` & `teapy-0.7.0/tea-core/src/arrok.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-core/src/impls/impl_1d_method.rs` & `teapy-0.7.0/tea-core/src/impls/impl_1d_method.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-core/src/impls/impl_basic.rs` & `teapy-0.7.0/tea-core/src/impls/impl_basic.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-core/src/impls/impl_method.rs` & `teapy-0.7.0/tea-core/src/impls/impl_method.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-core/src/impls/impl_numeric.rs` & `teapy-0.7.0/tea-core/src/impls/impl_numeric.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-core/src/impls/impl_time.rs` & `teapy-0.7.0/tea-core/src/impls/impl_time.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-core/src/impls/impl_traits.rs` & `teapy-0.7.0/tea-core/src/impls/impl_traits.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-core/src/impls/linalg/layout.rs` & `teapy-0.7.0/tea-core/src/impls/linalg/layout.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-core/src/impls/linalg/least_squares.rs` & `teapy-0.7.0/tea-core/src/impls/linalg/least_squares.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-core/src/impls/linalg/svd.rs` & `teapy-0.7.0/tea-core/src/impls/linalg/svd.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-core/src/iterators.rs` & `teapy-0.7.0/tea-core/src/iterators.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-core/src/lib.rs` & `teapy-0.7.0/tea-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-core/src/macros.rs` & `teapy-0.7.0/tea-core/src/macros.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-core/src/own.rs` & `teapy-0.7.0/tea-core/src/own.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-core/src/prelude.rs` & `teapy-0.7.0/tea-core/src/prelude.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-core/src/traits.rs` & `teapy-0.7.0/tea-core/src/traits.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-core/src/view.rs` & `teapy-0.7.0/tea-core/src/view.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-core/src/viewmut.rs` & `teapy-0.7.0/tea-core/src/viewmut.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-utils/src/algos.rs` & `teapy-0.7.0/tea-utils/src/algos.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-utils/src/alloc.rs` & `teapy-0.7.0/tea-utils/src/alloc.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-utils/src/traits.rs` & `teapy-0.7.0/tea-utils/src/traits.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-groupby/Cargo.toml` & `teapy-0.7.0/tea-groupby/Cargo.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 [package]
 name = "tea-groupby"
-version= "0.6.9"
-authors= ["Teamon"]
-edition= "2021"
-repository= "https://github.com/Teamon9161/teapy"
-license= "MIT"
-resolver = "2"
+version.workspace = true
+authors.workspace = true
+edition.workspace = true
+repository.workspace = true
+license.workspace = true
 
 [features]
 default = ["extend"]
 extend = ["lazy", "lazy_time", "lazy_option_dtype"]
 
 lazy_option_dtype = ["option_dtype", "tea-lazy/option_dtype"]
 lazy = ["tea-lazy"]
 lazy_time = ["lazy", "time", "tea-lazy/time"]
 
 time = ["tea-core/time", "tea-hash/time"]
 option_dtype = ["tea-core/option_dtype"]
 
 [dependencies]
-pyo3 = {version = "0.20.0", features = ["extension-module", "abi3-py38", "macros", "serde","extension-module", "abi3-py38", "macros", "serde"]}
+pyo3 = { workspace = true, features = ["extension-module", "abi3-py38", "macros", "serde"]}
 tea-core = { path = "../tea-core", default-features=false, features=["method_1d", "concat", "extend"] }
 tea-lazy = { path = "../tea-lazy", optional=true, default-features = false}
 tea-macros = { path = "../tea-macros" }
 tea-hash = { path = "../tea-hash" }
 tea-ext = { path = "../tea-ext", default-features = false, features = ["agg", "map"]}
 # once_cell = { workspace = true }
-rayon = "1.5"
-ndarray = {features=['rayon', 'serde','rayon', 'serde'], version="0.15"}
+rayon = { workspace = true }
+ndarray = { workspace = true, features=['rayon', 'serde'] }
```

### Comparing `teapy-0.6.9/local_dependencies/tea-groupby/benches/groupby.rs` & `teapy-0.7.0/tea-groupby/benches/groupby.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-groupby/src/from_py.rs` & `teapy-0.7.0/tea-groupby/src/from_py.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-groupby/src/groupby_agg.rs` & `teapy-0.7.0/tea-groupby/src/groupby_agg.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-groupby/src/impl_lazy.rs` & `teapy-0.7.0/tea-groupby/src/impl_lazy.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-groupby/src/join.rs` & `teapy-0.7.0/tea-groupby/src/join.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-groupby/src/lib.rs` & `teapy-0.7.0/tea-groupby/src/lib.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-groupby/src/unique.rs` & `teapy-0.7.0/tea-groupby/src/unique.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-time/src/convert.rs` & `teapy-0.7.0/tea-time/src/convert.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-time/src/datetime.rs` & `teapy-0.7.0/tea-time/src/datetime.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-time/src/impls/impl_datetime.rs` & `teapy-0.7.0/tea-time/src/impls/impl_datetime.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-time/src/impls/impl_ops.rs` & `teapy-0.7.0/tea-time/src/impls/impl_ops.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-time/src/impls/impl_timedelta.rs` & `teapy-0.7.0/tea-time/src/impls/impl_timedelta.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-time/src/timedelta.rs` & `teapy-0.7.0/tea-time/src/timedelta.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-time/src/timeunit.rs` & `teapy-0.7.0/tea-time/src/timeunit.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-lazy/src/datadict/dict.rs` & `teapy-0.7.0/tea-lazy/src/datadict/dict.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-lazy/src/datadict/get_set.rs` & `teapy-0.7.0/tea-lazy/src/datadict/get_set.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-lazy/src/datadict/selector.rs` & `teapy-0.7.0/tea-lazy/src/datadict/selector.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-lazy/src/expr_core/data.rs` & `teapy-0.7.0/tea-lazy/src/expr_core/data.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-lazy/src/expr_core/expr.rs` & `teapy-0.7.0/tea-lazy/src/expr_core/expr.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-lazy/src/expr_core/expr_element.rs` & `teapy-0.7.0/tea-lazy/src/expr_core/expr_element.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-lazy/src/expr_core/expr_inner.rs` & `teapy-0.7.0/tea-lazy/src/expr_core/expr_inner.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-lazy/src/expr_core/impls/auto_impl.rs` & `teapy-0.7.0/tea-lazy/src/expr_core/impls/auto_impl.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-lazy/src/expr_core/impls/impl_cast.rs` & `teapy-0.7.0/tea-lazy/src/expr_core/impls/impl_cast.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-lazy/src/expr_core/impls/impl_dtype_judge.rs` & `teapy-0.7.0/tea-lazy/src/expr_core/impls/impl_dtype_judge.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-lazy/src/expr_core/impls/impl_ops.rs` & `teapy-0.7.0/tea-lazy/src/expr_core/impls/impl_ops.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-lazy/src/expr_core/impls/mod.rs` & `teapy-0.7.0/tea-lazy/src/expr_core/impls/mod.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-lazy/src/expr_core/impls/utils.rs` & `teapy-0.7.0/tea-lazy/src/expr_core/impls/utils.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-lazy/src/groupby.rs` & `teapy-0.7.0/tea-lazy/src/groupby.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-lazy/src/join.rs` & `teapy-0.7.0/tea-lazy/src/join.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-lazy/src/linalg.rs` & `teapy-0.7.0/tea-lazy/src/linalg.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-ext/Cargo.toml` & `teapy-0.7.0/tea-ext/Cargo.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 [package]
 name = "tea-ext"
-version= "0.6.9"
-authors= ["Teamon"]
-edition= "2021"
-repository= "https://github.com/Teamon9161/teapy"
-license= "MIT"
-resolver = "2"
+version.workspace = true
+authors.workspace = true
+edition.workspace = true
+repository.workspace = true
+license.workspace = true
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [features]
 # default = ["rolling", "agg", "lazy", "concat"]
 default = ["extend", "methods"]
 
 extend = ["lazy_time", "option_dtype"]
@@ -25,17 +24,17 @@
 map = ["tea-core/ops"]  # map functions
 rolling = ["num"]  # rolling functions
 create = ["lazy"]
 stat = ["statrs"]
 concat = ["tea-core/concat", "tea-hash"]  # used in rolling_common
 
 [dependencies]
-pyo3 = {version = "0.20.0", features = ["extension-module", "abi3-py38", "macros", "serde"]}
+pyo3 = { workspace = true }
 tea-core = { path = "../tea-core", default-features=false, features=["method_1d"] }
 tea-hash = { path = "../tea-hash", optional=true, default-features = false}
 tea-lazy = { path = "../tea-lazy", optional=true, default-features=false, features=["extend"]}
 tea-macros = { path = "../tea-macros" }
-ndarray = {features=['rayon', 'serde'], version="0.15"}
-paste = "1.0"
-rayon = "1.5"
-num = { version = "0.4", optional = true}
-statrs = { version = "0.16", optional=true }
+ndarray = { workspace=true }
+paste = { workspace = true }
+rayon = { workspace = true }
+num = { workspace = true, optional = true}
+statrs = { version = "0.16", optional=true }
```

### Comparing `teapy-0.6.9/local_dependencies/tea-ext/benches/rolling.rs` & `teapy-0.7.0/tea-ext/benches/rolling.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-ext/src/agg/corr.rs` & `teapy-0.7.0/tea-ext/src/agg/corr.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-ext/src/agg/impl_lazy.rs` & `teapy-0.7.0/tea-ext/src/agg/impl_lazy.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-ext/src/agg/mod.rs` & `teapy-0.7.0/tea-ext/src/agg/mod.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-ext/src/create.rs` & `teapy-0.7.0/tea-ext/src/create.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-ext/src/from_py.rs` & `teapy-0.7.0/tea-ext/src/from_py.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-ext/src/linalg.rs` & `teapy-0.7.0/tea-ext/src/linalg.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-ext/src/macros.rs` & `teapy-0.7.0/tea-ext/src/macros.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-ext/src/map/impl_1d.rs` & `teapy-0.7.0/tea-ext/src/map/impl_1d.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-ext/src/map/impl_arrok.rs` & `teapy-0.7.0/tea-ext/src/map/impl_arrok.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-ext/src/map/impl_inplace.rs` & `teapy-0.7.0/tea-ext/src/map/impl_inplace.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-ext/src/map/impl_lazy/impl_view.rs` & `teapy-0.7.0/tea-ext/src/map/impl_lazy/impl_view.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-ext/src/map/impl_lazy/mod.rs` & `teapy-0.7.0/tea-ext/src/map/impl_lazy/mod.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-ext/src/map/impl_lazy/stat.rs` & `teapy-0.7.0/tea-ext/src/map/impl_lazy/stat.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-ext/src/map/impl_lazy/time.rs` & `teapy-0.7.0/tea-ext/src/map/impl_lazy/time.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-ext/src/map/impl_string.rs` & `teapy-0.7.0/tea-ext/src/map/impl_string.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-ext/src/map/impl_time.rs` & `teapy-0.7.0/tea-ext/src/map/impl_time.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-ext/src/map/mod.rs` & `teapy-0.7.0/tea-ext/src/map/mod.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-ext/src/rolling/cmp.rs` & `teapy-0.7.0/tea-ext/src/rolling/cmp.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-ext/src/rolling/corr.rs` & `teapy-0.7.0/tea-ext/src/rolling/corr.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-ext/src/rolling/feature.rs` & `teapy-0.7.0/tea-ext/src/rolling/feature.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-ext/src/rolling/impl_lazy/common.rs` & `teapy-0.7.0/tea-ext/src/rolling/impl_lazy/common.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-ext/src/rolling/norm.rs` & `teapy-0.7.0/tea-ext/src/rolling/norm.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-ext/src/rolling/reg.rs` & `teapy-0.7.0/tea-ext/src/rolling/reg.rs`

 * *Files 2% similar despite different names*

```diff
@@ -340,14 +340,75 @@
                         sum.kh_sum(-v.f64(), c4);
                     };
                 }
                 res
             })
         }
     }
+
+    fn ts_reg_resid_mean<SO>(
+        &self,
+        out: &mut ArrBase<SO, Ix1>,
+        window: usize,
+        min_periods: usize,
+    ) -> f64
+    where
+        SO: DataMut<Elem = MaybeUninit<f64>>,
+        T: Number,
+    {
+        let arr = self.as_dim1();
+        // 错位相减核心公式：sum_xt(t) = sum_xt(t-1) - sum_x + n * new_element
+        let window = min(arr.len(), window);
+        if window < min_periods {
+            // 如果滚动窗口是1则返回全nan
+            return out.apply_mut(|v| {
+                v.write(f64::NAN);
+            });
+        }
+        let mut sum = 0.;
+        let mut sum_xx = 0.;
+        let mut sum_xt = 0.;
+        let mut n = 0;
+        arr.apply_window_to(out, window, |v, v_rm| {
+            if v.notnan() {
+                n += 1;
+                let v = v.f64();
+                sum_xt += n.f64() * v; // 错位相减法, 忽略nan带来的系数和window不一致问题
+                sum += v;
+                sum_xx += v * v;
+            };
+            let res = if n >= min_periods {
+                let n_f64 = n.f64();
+                let nn_add_n = n.mul_add(n, n);
+                let sum_t = (nn_add_n >> 1).f64(); // sum of time from 1 to window
+                                                   // denominator of slope
+                let sum_tt = (n * nn_add_n * n.mul_add(2, 1)).f64() / 6.;
+                let divisor = sum_tt - sum_t.powi(2);
+                let beta = (n_f64 * sum_xt - sum_t * sum) / divisor;
+                let alpha = sum_t.mul_add(-beta, sum) / n_f64;
+                let resid_sum = sum_xx - 2. * alpha * sum - 2. * beta * sum_xt
+                    + alpha * alpha * n_f64
+                    + 2. * alpha * beta * sum_t
+                    + beta * beta * sum_tt;
+                resid_sum / n_f64
+            } else {
+                f64::NAN
+            };
+            if let Some(v) = v_rm {
+                if v.notnan() {
+                    let v = v.f64();
+                    n -= 1;
+                    sum_xt -= sum;
+                    sum -= v;
+                    sum_xx -= v * v;
+                };
+            }
+            res
+        });
+    }
 }
 
 #[arr_map2_ext(lazy = "view2", type = "numeric", type2 = "numeric")]
 impl<T: Send + Sync, S: Data<Elem = T>, D: Dimension> Reg2Ts for ArrBase<S, D> {
     fn ts_regx_beta<S2, D2, T2, SO>(
         &self,
         x: &ArrBase<S2, D2>,
```

### Comparing `teapy-0.6.9/local_dependencies/tea-dtype/src/cast.rs` & `teapy-0.7.0/tea-dtype/src/cast.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-dtype/src/lib.rs` & `teapy-0.7.0/tea-dtype/src/lib.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-dtype/src/option_datatype.rs` & `teapy-0.7.0/tea-dtype/src/option_datatype.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-dtype/src/pyvalue.rs` & `teapy-0.7.0/tea-dtype/src/pyvalue.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 use std::fmt::Debug;
 
 use super::cast::Cast;
 use crate::{DataType, GetDataType, GetNone};
 use numpy::{Element, PyArrayDescr};
-use pyo3::{FromPyObject, PyAny, PyObject, PyResult, Python, ToPyObject};
+use pyo3::{Bound, FromPyObject, PyAny, PyObject, PyResult, Python, ToPyObject};
 #[cfg(feature = "serde")]
 use serde::{Serialize, Serializer};
 use std::string::ToString;
 
 #[derive(Clone)]
 #[repr(transparent)]
 pub struct PyValue(pub PyObject);
@@ -74,17 +74,22 @@
 }
 
 // #[cfg(feature = "lazy")]
 // impl ExprElement for PyValue {}
 
 unsafe impl Element for PyValue {
     const IS_COPY: bool = false;
+    // #[inline(always)]
+    // fn get_dtype(py: Python) -> &PyArrayDescr {
+    //     PyArrayDescr::object(py)
+    // }
+
     #[inline(always)]
-    fn get_dtype(py: Python) -> &PyArrayDescr {
-        PyArrayDescr::object(py)
+    fn get_dtype_bound(py: Python<'_>) -> Bound<'_, PyArrayDescr> {
+        PyArrayDescr::object_bound(py)
     }
 }
 
 impl<'source> FromPyObject<'source> for PyValue {
     #[inline(always)]
     fn extract(ob: &'source PyAny) -> PyResult<Self> {
         Ok(PyValue(ob.to_object(ob.py())))
```

### Comparing `teapy-0.6.9/local_dependencies/tea-io/src/arrow_io/impl_lazy.rs` & `teapy-0.7.0/tea-io/src/arrow_io/impl_lazy.rs`

 * *Files 11% similar despite different names*

```diff
@@ -24,14 +24,31 @@
             let arr = arr.pop().unwrap();
             Ok((arr.into(), None))
         });
         e
     }
 }
 
+pub fn scan_ipc_lazy<'a, P>(path: P, columns: ColSelect<'_>) -> TpResult<Vec<Expr<'a>>>
+where
+    P: AsRef<Path> + Send + Sync + Clone + 'a,
+{
+    let mut schema = super::read_ipc_schema(path.clone())?;
+    let proj = columns.into_proj(&schema)?;
+    if let Some(proj) = proj {
+        schema = schema.filter(|i, _f| proj.contains(&i));
+    }
+    let out = schema
+        .fields
+        .into_iter()
+        .map(|f| Expr::read_ipc(path.clone(), f.name.into()))
+        .collect_trusted();
+    Ok(out)
+}
+
 #[ext_trait]
 impl<'a> DataDictIPCExt for DataDict<'a> {
     pub fn read_ipc<P: AsRef<Path>>(path: P, columns: ColSelect<'_>) -> TpResult<DataDict<'a>> {
         let (schema, arr_vec) = super::read_ipc(path, columns)?;
         let data: Vec<Expr<'a>> = schema
             .fields
             .into_iter()
@@ -41,20 +58,11 @@
         Ok(DataDict::new(data, None))
     }
 
     pub fn scan_ipc<P>(path: P, columns: ColSelect<'_>) -> TpResult<DataDict<'a>>
     where
         P: AsRef<Path> + Send + Sync + Clone + 'a,
     {
-        let mut schema = super::read_ipc_schema(path.clone())?;
-        let proj = columns.into_proj(&schema)?;
-        if let Some(proj) = proj {
-            schema = schema.filter(|i, _f| proj.contains(&i));
-        }
-        let out = schema
-            .fields
-            .into_iter()
-            .map(|f| Expr::read_ipc(path.clone(), f.name.into()))
-            .collect_trusted();
+        let out = scan_ipc_lazy(path, columns)?;
         Ok(Self::new(out, None))
     }
 }
```

### Comparing `teapy-0.6.9/local_dependencies/tea-io/src/arrow_io/ipc.rs` & `teapy-0.7.0/tea-io/src/arrow_io/ipc.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-io/src/arrow_io/utils.rs` & `teapy-0.7.0/tea-io/src/arrow_io/utils.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-io/src/colselect.rs` & `teapy-0.7.0/tea-io/src/colselect.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-macros/src/lazy_impls.rs` & `teapy-0.7.0/tea-macros/src/lazy_impls.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-macros/src/lib.rs` & `teapy-0.7.0/tea-macros/src/lib.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-macros/src/methods_impls.rs` & `teapy-0.7.0/tea-macros/src/methods_impls.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-macros/src/tools.rs` & `teapy-0.7.0/tea-macros/src/tools.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-hash/src/lib.rs` & `teapy-0.7.0/tea-hash/src/lib.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/local_dependencies/tea-error/src/lib.rs` & `teapy-0.7.0/tea-error/src/lib.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/Cargo.toml` & `teapy-0.7.0/tea-py/Cargo.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 [package]
 name = "tea-py"
-version = "0.6.9"
-authors = ["Teamon"]
-edition = "2021"
-license = "MIT"
-repository = "https://github.com/Teamon9161/teapy"
+version = { workspace = true }
+authors = { workspace = true }
+edition = { workspace = true }
+license = { workspace = true }
+repository = { workspace = true }
 description = "Fast DataDict Library in Python"
-resolver = "2"
 
 
 [features]
 default = ["extend", "methods_extend", "groupby_extend", "lazy_io", "blas"]
-# default = ["lazy"]
+# default = ["extend", "blas", "agg", "map"]
 
 # methods includes extend datatype
 methods_extend = ["extend", "methods", "tea-ext/extend"]
 # groupby methods includes extend datatype
 groupby_extend = ["extend", "groupby", "tea-groupby/extend"]
 
 blas = ["tea-core/blas", "tea-lazy/blas", "tea-ext/map", "stat", "lazy"] # linalg
@@ -54,22 +53,22 @@
 arw = ["tea-io/arw"]
 
 
 srd = ["tea-core/srd"]
 
 
 [dependencies]
-tea-core = {path = "local_dependencies/tea-core", default-features = false}
-tea-hash = {path = "local_dependencies/tea-hash" }
-tea-lazy = {path = "local_dependencies/tea-lazy", optional = true}
-tea-ext = {path = "local_dependencies/tea-ext", default-features = false}
-tea-groupby = {path = "local_dependencies/tea-groupby", optional = true}
-tea-io = {path = "local_dependencies/tea-io", default-features = false, optional = true}
-pyo3 = {version = "0.20.0", features = ["extension-module", "abi3-py38", "macros", "serde"]}
-numpy = "0.20.0"
-parking_lot = "0.12"
-ahash = { version = "0.8", features = ["std", "runtime-rng"]}
-rayon = "1.5"
-regex = "1"
-once_cell = "1.18"
-ndarray = {features=['rayon', 'serde'], version="0.15"}
-chrono = {version = "0.4.31", features = ["serde"]}
+tea-core = {path = "../tea-core", default-features = false}
+tea-hash = {path = "../tea-hash"}
+tea-lazy = {path = "../tea-lazy", optional = true}
+tea-ext = {path = "../tea-ext", default-features = false}
+tea-groupby = {path = "../tea-groupby", optional = true}
+tea-io = {path = "../tea-io", default-features = false, optional = true}
+pyo3 = { workspace=true }
+numpy = { workspace=true }
+parking_lot = { workspace=true }
+ahash = { workspace=true }
+rayon = { workspace=true }
+regex = { workspace=true }
+once_cell = { workspace=true }
+ndarray = { workspace=true }
+chrono = { workspace=true }
```

### Comparing `teapy-0.6.9/LICENSE` & `teapy-0.7.0/tea-py/LICENSE`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/Makefile` & `teapy-0.7.0/tea-py/Makefile`

 * *Files 9% similar despite different names*

```diff
@@ -24,18 +24,17 @@
 	-s \
 	--cov=teapy \
 	--cov-report xml \
 	--import-mode=importlib
 
 .PHONY: format
 format:  ## format and check
-	isort . --profile black
-	black .
+	ruff check --fix
 	cargo fmt --all
-	flake8 --ignore E501,F401,F403,W503 --exclude=.venv
+	ruff check
 	cargo clippy -- -D warnings
 
 .PHONY: coverage
 coverage: # rust and python coverage
 	@bash -c "\
 		$(MAKE) venv; \
 		source venv/bin/activate; \
```

### Comparing `teapy-0.6.9/README.md` & `teapy-0.7.0/tea-py/README.md`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/python/teapy/__init__.py` & `teapy-0.7.0/tea-py/python/teapy/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,64 @@
-# from numpy import nan
-
 from .array_func import *
-from .datadict import (
-    DataDict,
-    from_pd,
-    from_pl,
-    read_feather,
-    read_ipc,
-    scan_feather,
-    scan_ipc,
-)
 from .expr import Expr, register
 from .mod_func import *
-from .tears import arange
+from .py_datadict import DataDict, from_dataframe, from_pd, from_pl, scan_ipc
+from .selector import Selector
+from .tears import (
+    arange,
+    concat,
+    context,
+    eval_exprs,
+    expr_register,
+    get_version,
+    nan,
+    stack,
+    timedelta,
+    where_,
+)
 from .tears import calc_ret_single as _calc_ret_single
 from .tears import calc_ret_single_with_spread as _calc_ret_single_with_spread
-from .tears import concat
-from .tears import context as ct
-from .tears import eval_dicts, eval_exprs, expr_register, full, get_version, nan
+from .tears import full as _full
 from .tears import parse_expr as asexpr
 from .tears import parse_expr_list as asexprs
-from .tears import stack, timedelta
-from .tears import where_ as where
 from .window_func import *
 
 __version__ = get_version()
 
+s = Selector
+
 
 def eval(lazy_list):
     if not isinstance(lazy_list, (tuple, list)):
         lazy_list = [lazy_list]
     if len(lazy_list) == 0:
         return
     else:
         if isinstance(lazy_list[0], Expr):
             return eval_exprs(lazy_list, inplace=True)
         elif isinstance(lazy_list[0], DataDict):
-            return eval_dicts(lazy_list, inplace=True)
+            exprs = []
+            for dd in lazy_list:
+                exprs.extend(dd.exprs)
+            return eval_exprs(exprs, inplace=True)
         else:
-            raise ValueError(
-                f"eval() only accept list of Expr or DataDict, but the type is {type(lazy_list[0])}"
-            )
+            msg = f"eval only accept list(Expr | DataDict), find {type(lazy_list[0])}"
+            raise ValueError(msg)
+
+
+def full(shape, fill_value=nan):
+    if isinstance(shape, Selector):
+        return Selector().mod_func("full")(shape, fill_value=fill_value)
+    return _full(shape, fill_value)
+
+
+def where(cond, x, y):
+    if any(isinstance(i, Selector) for i in [cond, x, y]):
+        return Selector().mod_func("where")(cond, x, y)
+    return where_(cond, x, y)
 
 
 def calc_ret_single(
     pos,
     opening_cost,
     closing_cost,
     init_cash,
```

### Comparing `teapy-0.6.9/python/teapy/array_func.py` & `teapy-0.7.0/tea-py/python/teapy/array_func.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,20 +163,21 @@
         quantile: if method_params is 1%, then all elements greater than the
             99% quantile will be set to the 99% quantile, and all elements less
             than the 1% quantile will be set to the 1% quantile.
 
         median: if method_params is 3, calculate median value at first, and then
             calculate MAD. MAD is the median of the `|v - median|` array where v is the
             element of the array. All elements greater than `median + 3 * MAD` will be
-            set to `median + 3 * MAD`, and all elements less than `median - 3 * MAD` will
-            be set to `median - 3 * MAD` by default.
+            set to `median + 3 * MAD`, and all elements less than
+            `median - 3 * MAD` will be set to `median - 3 * MAD` by default.
 
         sigma: if method_params is 3, calulate the mean and standard deviation of the
-            array, all elements greater than `mean + 3 * std` will be set `mean + 3 * std`,
-            and all elements less than `mean - 3 * std` will be set to `mean - 3 * std`.
+            array, all elements greater than `mean + 3 * std` will be set
+            `mean + 3 * std`, and all elements less than `mean - 3 * std`
+            will be set to `mean - 3 * std`.
     method_params : float64
         if method is quantile: the default is 1%.
         if method is median: the default is 3.
         if method is sigma: the default is 3.
     stable :  bool
         whether to use Kahan summation to reduce the numerical error
     axis : int or None
```

### Comparing `teapy-0.6.9/python/teapy/datadict.py` & `teapy-0.7.0/tea-py/python/teapy/py_datadict.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,152 +1,268 @@
-from .tears import Expr
-from .tears import PyDataDict as _DataDict
-from .tears import from_dataframe
-from .tears import read_ipc as __read_ipc
-from .tears import scan_ipc as __scan_ipc
-from .tears import stack
+from .selector import selector_to_expr
+from .tears import Expr, eval_exprs, stack
+from .tears import context as ct
+from .tears import scan_ipc as _scan_ipc
 
 name_prefix = "column_"
 
 
-def _new_with_dd(dd=None):
-    if dd is None:
-        # for inplace functions
-        return None
-    out = DataDict()
-    if isinstance(dd, _DataDict):
-        out._dd = dd
-    else:
-        raise ValueError("the return is not teapy DataDict")
-    return out
-
+def scan_ipc(path, columns=None):
+    return DataDict(_scan_ipc(path, columns=columns))
 
-def construct(func):
-    """For functions that return a DataDict"""
 
-    def inner(*args, **kwargs):
-        dd = func(*args, **kwargs)
-        return _new_with_dd(dd)
+def from_dataframe(df, copy=False):
+    return DataDict(df.to_dict(), copy=copy)
 
-    return inner
 
+def from_pd(df, copy=False):
+    return from_dataframe(df, copy=copy)
 
-def from_pd(*args, **kwargs):
-    dd = from_dataframe(*args, **kwargs)
-    return _new_with_dd(dd)
 
+def from_pl(df, copy=False):
+    return from_dataframe(df, copy=copy)
 
-def from_pl(*args, **kwargs):
-    dd = from_dataframe(*args, **kwargs)
-    return _new_with_dd(dd)
 
+class DataDict:
+    default_name = name_prefix
 
-def read_ipc(path, columns=None):
-    dd = __read_ipc(str(path), columns=columns)
-    return _new_with_dd(dd)
+    def __init__(self, data=None, columns=None, copy=False, **kwargs):
+        self.copy_flag = copy
+        self.col_map = None
+        self.auto_idx = 0
+        if data is None:
+            self.exprs = []
+        elif isinstance(data, dict):
+            if columns is None:
+                self.exprs = [Expr(v, copy=copy).alias(k) for k, v in data.items()]
+            else:  # columns has a higher priority
+                assert len(columns) == len(data)
+                self.exprs = [
+                    Expr(v, copy=copy).alias(name)
+                    for name, (k, v) in zip(columns, data.items())
+                ]
+        else:
+            if isinstance(data, (list, tuple)):
+                if columns is not None:
+                    if len(columns) != len(data):
+                        raise ValueError("columns and data must have the same length")
+                else:  # use expr name in data and auto generate column names if missing
+                    columns = [
+                        e.name
+                        if isinstance(e, Expr) and e.name is not None
+                        else self._auto_name()
+                        for e in data
+                    ]
+                self.exprs = [
+                    Expr(v, copy=copy).alias(k) for k, v in zip(columns, data)
+                ]
+            else:
+                raise ValueError("data must be a dict, list or tuple")
+        if len(kwargs):
+            for k, v in kwargs.items():
+                self.exprs.append(Expr(v, copy=copy).alias(k))
 
+    def _init_col_map(self, force_init=False):
+        if self.col_map is None or force_init:
+            self.col_map = {e.name: i for i, e in enumerate(self.exprs)}
+
+    def _auto_name(self) -> str:
+        """Generate a new column name."""
+        name = self.default_name + str(self.auto_idx)
+        self.auto_idx += 1
+        return name
+
+    def __iter__(self):
+        return iter(self.exprs)
+
+    @property
+    def columns(self):
+        return [e.name for e in self.exprs]
+
+    @property
+    def dtypes(self):
+        return {e.name: e.dtype for e in self.exprs}
+
+    @property
+    def raw_data(self):
+        from warnings import warn
+
+        warn(
+            "raw_data will be deprecated in future release, use exprs instead",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        return self.exprs
 
-def scan_ipc(path, columns=None):
-    dd = __scan_ipc(str(path), columns=columns)
-    return _new_with_dd(dd)
+    def is_empty(self):
+        return len(self) == 0
 
+    def _new_with_exprs(self, exprs, copy_map=False):
+        dd = DataDict(exprs, copy=self.copy_flag)
+        if copy_map and self.col_map is not None:
+            dd.col_map = self.col_map.copy()
+        return dd
 
-read_feather, scan_feather = read_ipc, scan_ipc
+    def copy(self):
+        return self._new_with_exprs(self.exprs, copy_map=True)
 
+    def get(self, key):
+        if isinstance(key, int):
+            return self.exprs[key]
+        elif isinstance(key, str):
+            self._init_col_map()
+            if key.startswith("^") and key.endswith("$"):
+                import re
 
-class DataDict:
-    def __init__(self, data=None, columns=None, copy=False, **kwargs):
-        if data is not None or len(kwargs):
-            if data is None:
-                data = []
-            elif isinstance(data, dict):
-                columns = list(data.keys()) if columns is None else columns
-                data = list(data.values())
-            if len(kwargs):
-                if columns is None:
-                    columns = []
-                if isinstance(data, tuple):
-                    data = list(data)
-                for k, v in kwargs.items():
-                    data.append(v)
-                    columns.append(k)
-            self._dd = _DataDict(data=data, columns=columns, copy=copy)
+                key = re.compile(key)
+                return self._new_with_exprs(
+                    [e for e in self.exprs if key.match(e.name)], copy_map=False
+                )
+            return self.exprs[self.col_map[key]]
+        elif isinstance(key, (list, tuple)):
+            new_data = []
+            for k in key:
+                res = self.get(k)
+                if not isinstance(res, DataDict):
+                    new_data.append(res)
+                else:
+                    new_data.extend(res.exprs)
+            return DataDict(new_data, copy=self.copy_flag)
         else:
-            self._dd = _DataDict([])
+            raise TypeError("key must be int, str, list or tuple")
+
+    def set(self, key, value):
+        if isinstance(key, int):
+            ori_name = self.exprs[key].name
+            value = Expr(value, copy=self.copy_flag)
+            new_name = ori_name if value.name is None else value.name
+            self.exprs[key] = value.alias(new_name)
+            # update col_map
+            if self.col_map is not None and new_name != ori_name:
+                self.col_map[new_name] = self.col_map.pop(ori_name)
+        elif isinstance(key, str):
+            self._init_col_map()
+            if key in self.col_map:  # update an existing column
+                idx = self.col_map[key]
+                self.exprs[idx] = Expr(value, copy=self.copy_flag).alias(key)
+            elif key.startswith("^") and key.endswith("$"):
+                exprs = self.get(key)
+                columns = [exprs.name] if isinstance(exprs, Expr) else exprs.columns
+                for k, v in zip(columns, value):
+                    self.set(k, v)
+            else:  # add a new column
+                self.exprs.append(Expr(value, copy=self.copy_flag).alias(key))
+                self.col_map[key] = len(self.exprs) - 1
+        elif isinstance(key, (list, tuple)):
+            for k, v in zip(key, value):
+                self.set(k, v)
 
     def __getitem__(self, key):
-        out = self._dd[key]
-        if isinstance(out, list):
-            return DataDict(data=out)
-        else:
-            return out
+        return self.get(key)
 
-    def __setitem__(self, item, value):
-        self._dd.__setitem__(item, value)
+    def __setitem__(self, key, value):
+        return self.set(key, value)
 
-    def __delitem__(self, item):
-        self._dd.__delitem__(item)
+    def __delitem__(self, key):
+        self.drop(key, inplace=True)
 
-    def __getattr__(self, attr):
-        return getattr(self._dd, attr)
+    def __len__(self):
+        return len(self.exprs)
 
-    def __repr__(self):
-        return self._dd.__repr__()
+    def to_dict(self):
+        return {e.name: e.view for e in self.exprs}
 
-    def __len__(self):
-        return len(self._dd)
+    def to_pd(self):
+        import pandas as pd
 
-    @construct
-    def copy(self):
-        return self._dd.copy()
+        return pd.DataFrame(self.to_dict())
 
-    def eval(self, cols=None, inplace=True, context=False):
-        dd = self if inplace else self.copy()
-        if isinstance(cols, bool):
-            cols, inplace = None, cols
-        dd._dd.eval(cols, context=context)
-        return None if inplace else dd
+    def to_pl(self):
+        import polars as pl
 
-    def drop(self, cols, inplace=False):
-        dd = self if inplace else self.copy()
-        dd._dd.drop(cols)
-        return None if inplace else dd
+        return pl.DataFrame(self.to_dict())
 
-    def simplify(self):
-        def simplify_f(e):
-            e.simplify()
-            return e
+    def __repr__(self) -> str:
+        return {e.name: e for e in self.exprs}.__repr__()
 
-        self.apply(simplify_f, inplace=True)
+    def eval(self, columns=None, inplace=False):
+        if columns is None:
+            self.exprs = eval_exprs(self.exprs)
+        else:
+            exprs = self.get(columns)
+            if isinstance(exprs, Expr):
+                exprs.eval(inplace=True)
+            else:
+                exprs = eval_exprs(exprs.exprs)
+            self.set(columns, exprs)
+        return self if not inplace else None
+
+    def apply(self, func, *args, inplace=False, exclude=None, **kwargs):
+        if exclude is None:
+            exprs = [func(e, *args, **kwargs) for e in self.exprs]
+        else:
+            exprs = [func(e, *args, **kwargs) for e in self.exclude(exclude).exprs]
+        if inplace:
+            self.exprs = exprs
+            return self
+        return self._new_with_exprs(exprs)
 
-    @construct
-    def select(self, exprs, **kwargs):
+    def _process_selector_exprs(self, exprs, context=False):
+        return selector_to_expr(exprs, dd=self, context=context)
+
+    def select(self, exprs, *args, **kwargs):
         if not isinstance(exprs, list):
             exprs = [exprs]
-        for i, e in enumerate(exprs):
-            if isinstance(e, str):
-                exprs[i] = self[e]
+        if len(args):
+            exprs += list(args)
         if len(kwargs):
             for k, v in kwargs.items():
                 exprs.append(v.alias(k))
-        return self._dd.select(exprs)
+        exprs = self._process_selector_exprs(exprs)
+        return self._new_with_exprs(exprs)
 
-    def with_columns(self, exprs, inplace=False, **kwargs):
+    def with_columns(self, exprs, *args, inplace=False, **kwargs):
         dd = self if inplace else self.copy()
         if not isinstance(exprs, list):
             exprs = [exprs]
+        if len(args):
+            exprs += list(args)
         if len(kwargs):
             for k, v in kwargs.items():
                 exprs.append(v.alias(k))
-        dd._dd.with_columns(exprs)
+        exprs = self._process_selector_exprs(exprs)
+        expr_names = [e.name for e in exprs]
+        dd[expr_names] = exprs
         return None if inplace else dd
 
+    def drop(self, key, inplace=False):
+        dd = self.copy() if not inplace else self
+        if isinstance(key, int):
+            dd.exprs.pop(key)
+        elif isinstance(key, str):
+            dd.exprs = [e for e in dd.exprs if e.name != key]
+        elif isinstance(key, (list, tuple)):
+            exprs = []
+            for i, e in enumerate(dd.exprs):
+                if e.name not in key and i not in key:
+                    exprs.append(e)
+            dd.exprs = exprs
+        dd._init_col_map(force_init=True)
+        return dd
+
+    def simplify(self):
+        def simplify_f(e):
+            e.simplify()
+            return e
+
+        self.apply(simplify_f, inplace=True)
+
     def dropna(self, subset=None, how="all", inplace=False):
         if subset is None:
-            subset = self._dd.columns
+            subset = self.columns
         elif isinstance(subset, (str, int)):
             subset = [subset]
         if len(subset) == 0:
             return None if inplace else self
         else:
             nan_mask = self[subset[0]].is_nan()
             if how == "any":
@@ -158,85 +274,93 @@
             else:
                 raise ValueError("how should be either 'any' or 'all'")
             dd = self if inplace else self.copy()
             for c in subset:
                 dd[c] = dd[c].filter(~nan_mask)
             return None if inplace else dd
 
+    def _select_on_axis(self, idx, axis=0, inplace=False, check=True):
+        return self.apply(
+            lambda e: e.select(idx, axis=axis, check=check), inplace=inplace
+        )
+
+    def slice(self, idx, axis=0, check=True, inplace=False):
+        return self._select_on_axis(idx, axis=axis, inplace=inplace, check=check)
+
     def filter(self, mask, inplace=False):
         dd = self if inplace else self.copy()
         idx = mask.mask_to_idx()
-        dd._select_on_axis_unchecked(idx, axis=0, inplace=True)
+        dd._select_on_axis(idx, axis=0, inplace=True, check=False)
         return None if inplace else dd
 
     def mean(self, axis=-1, stable=False, par=False, min_periods=1):
         if axis == -1:
-            return stack(self.raw_data, axis=axis).mean(
+            return stack(self.exprs, axis=axis).mean(
                 axis=-1, stable=stable, par=par, min_periods=min_periods
             )
         else:
             axis = axis + 1 if axis < 0 else axis
             return self.apply(
                 lambda e: e.mean(
                     axis=axis, stable=stable, par=par, min_periods=min_periods
                 )
             )
 
     def std(self, axis=-1, stable=False, par=False, min_periods=3):
         if axis == -1:
-            return stack(self.raw_data, axis=axis).std(
+            return stack(self.exprs, axis=axis).std(
                 axis=-1, stable=stable, par=par, min_periods=min_periods
             )
         else:
             axis = axis + 1 if axis < 0 else axis
             return self.apply(
                 lambda e: e.std(
                     axis=axis, stable=stable, par=par, min_periods=min_periods
                 )
             )
 
     def sum(self, axis=-1, stable=False, par=False):
         if axis == -1:
-            return stack(self.raw_data, axis=axis).sum(axis=-1, stable=stable, par=par)
+            return stack(self.exprs, axis=axis).sum(axis=-1, stable=stable, par=par)
         else:
             axis = axis + 1 if axis < 0 else axis
             return self.apply(lambda e: e.sum(axis=axis, stable=stable, par=par))
 
     def min(self, axis=-1, par=False):
         if axis == -1:
-            return stack(self.raw_data, axis=axis).min(axis=-1, par=par)
+            return stack(self.exprs, axis=axis).min(axis=-1, par=par)
         else:
             axis = axis + 1 if axis < 0 else axis
             return self.apply(lambda e: e.min(axis=axis, par=par))
 
     def max(self, axis=-1, par=False):
         if axis == -1:
-            return stack(self.raw_data, axis=axis).max(axis=-1, par=par)
+            return stack(self.exprs, axis=axis).max(axis=-1, par=par)
         else:
             axis = axis + 1 if axis < 0 else axis
             return self.apply(lambda e: e.max(axis=axis, par=par))
 
     def rename(self, mapper, inplace=False):
         dd = self if inplace else self.copy()
         if isinstance(mapper, (list, tuple)):
             assert len(mapper) == len(dd.columns)
-            dd.columns = list(mapper)
+            dd.exprs = [e.alias(m) for e, m in zip(dd.exprs, mapper)]
         elif isinstance(mapper, dict):
             for key, value in mapper.items():
                 dd[value] = dd[key].alias(value)
                 if key != value:
                     del dd[key]
         else:
-            raise ValueError("mapper should be either list or dict")
+            raise TypeError("mapper should be either list or dict")
         return None if inplace else dd
 
     def exclude(self, cols):
         if not isinstance(cols, (tuple, list)):
             cols = [cols]
-        return DataDict([self[key] for key in self.columns if key not in cols])
+        return self._new_with_exprs([e for e in self.exprs if e.name not in cols])
 
     def join(
         self,
         right,
         on=None,
         left_on=None,
         right_on=None,
@@ -258,98 +382,86 @@
                 inplace=inplace,
                 eager=eager,
             )
         else:
             dd = self if inplace else self.copy()
             left_on = [left_on] if isinstance(left_on, (str, int)) else left_on
             right_on = [right_on] if isinstance(right_on, (str, int)) else right_on
-            left_keys = self[left_on].raw_data
-            right_keys = right[right_on].raw_data
+            left_keys = self[left_on].exprs
+            right_keys = right[right_on].exprs
             left_other = left_keys[1:] if len(left_keys) > 1 else None
             if how == "left":
                 idx = left_keys[0]._get_left_join_idx(
                     left_other=left_other, right=right_keys
                 )
                 dd.with_columns(
                     right.drop(right_on, inplace=False)
-                    ._select_on_axis_unchecked(idx, 0)
-                    .raw_data,
+                    ._select_on_axis(idx, 0, check=False)
+                    .exprs,
                     inplace=True,
                 )
                 if simplify:
                     dd.simplify()
                 if eager:
-                    dd.eval(inplace=True)
+                    dd.eval()
                 return None if inplace else dd
             elif how == "outer":
                 *outer_keys, left_idx, right_idx = left_keys[0]._get_outer_join_idx(
                     left_other=left_other, right=right_keys, sort=sort, rev=rev
                 )
                 dd.drop(left_on, inplace=True)
                 dd.apply(lambda e: e.select(left_idx, check=False), inplace=True)
                 dd.with_columns(outer_keys, inplace=True)
                 dd.with_columns(
                     right.drop(right_on, inplace=False)
-                    ._select_on_axis_unchecked(right_idx, 0)
-                    .raw_data,
+                    .slice(right_idx, 0, check=False)
+                    .exprs,
                     inplace=True,
                 )
                 if simplify:
                     dd.simplify()
                 if eager:
-                    dd.eval(inplace=True)
+                    dd.eval()
                 return None if inplace else dd
             else:
                 raise NotImplementedError(
                     "Only left | right | outer join is supported for now"
                 )
 
-    def apply(self, func, inplace=False, exclude=None, **kwargs):
-        dd = self if inplace else self.copy()
-        if isinstance(exclude, str):
-            exclude = [exclude]
-        dd._dd.apply(func, exclude=exclude, **kwargs)
-        return None if inplace else dd
-
-    # def rolling(self, window, index=None, check=True, axis=0):
-    #     return Rolling(window, self._dd, index, check, axis)
-
-    def _select_on_axis(self, idx, axis=0, inplace=False):
-        return self.apply(lambda e: e.select(idx, axis=axis), inplace=inplace)
-
-    def _select_on_axis_unchecked(self, idx, axis=0, inplace=False):
-        return self.apply(
-            lambda e: e.select(idx, axis=axis, check=False), inplace=inplace
-        )
-
     def sort(self, by, rev=False, inplace=False):
         if isinstance(by, (str, int)):
             by = [by]
         if self.is_empty():
             return None if inplace else self
-        idx = self[0].sort(self[by], rev=rev, return_idx=True)
+        idx = self[0].sort(self[by].exprs, rev=rev, return_idx=True)
         dd = self if inplace else self.copy()
-        dd._select_on_axis_unchecked(idx, axis=0, inplace=True)
+        dd.slice(idx, axis=0, inplace=True, check=False)
         return None if inplace else dd
 
     def unique(self, subset, keep="first", inplace=False):
         if isinstance(subset, (str, int)):
             subset = [subset]
         if self.is_empty():
             return None if inplace else self
         first_key, subset = subset[0], subset[1:]
-        subset = None if len(subset) == 0 else self[subset]
+        subset = None if len(subset) == 0 else self[subset].exprs
         idx = self[first_key]._get_unique_idx(subset, keep=keep)
         dd = self if inplace else self.copy()
-        dd._select_on_axis_unchecked(idx, axis=0, inplace=True)
+        dd.slice(idx, axis=0, inplace=True, check=False)
         return None if inplace else dd
 
     def groupby(self, by=None, time_col=None, closed="left", group=True):
         return GroupBy(self, by=by, time_col=time_col, closed=closed, group=group)
 
+    def corr(self, columns=None, method="pearson", min_periods=1, stable=False):
+        from .tears import corr
+
+        exprs = self.exprs if columns is None else self[columns].exprs
+        return corr(exprs, method=method, min_periods=min_periods, stable=stable)
+
 
 class GroupBy:
     def __init__(self, dd, by=None, time_col=None, closed="left", group=True) -> None:
         self.dd = dd
         self.by = by
         self.time_col = time_col
         self.closed = closed
@@ -357,41 +469,28 @@
 
     def agg(self, exprs=None, **kwargs):
         if self.dd.is_empty():
             return self.dd
         time_expr = self.dd[self.time_col] if self.time_col is not None else None
         e = self.dd[0]
         columns = self.dd.columns
-        others = self.dd[columns[1:]].raw_data
+        others = self.dd[columns[1:]].exprs
         by = self.by if time_expr is not None else self.dd[self.by]
         groupby_obj = e.groupby(
             by=by, time_expr=time_expr, closed=self.closed, others=others
         )
         info, type_ = groupby_obj.info, groupby_obj.type
         self.info = info
         data = []
         if exprs is not None:
-            # if isinstance(exprs, list):
-            #     expr_names = [e.name for e in exprs]
-            # else:
-            #     if hasattr(exprs, 'name') and isinstance(exprs.name, str):
-            #         exprs = [exprs.name]
-            #     else:
-            #         exprs = [None]
             if time_expr is None:
                 data_agg = groupby_obj.agg(exprs)
             else:
                 _, data_agg = groupby_obj.agg(exprs)
             data_agg = [data_agg] if not isinstance(data_agg, list) else data_agg
-            # for name, agg_expr in zip(expr_names, data_agg):
-            #     if agg_expr.name is None:
-            #         agg_expr.name = name
-            # data.append(data_agg) if not isinstance(data_agg, list) else data.extend(
-            #     data_agg
-            # )
             data.extend(data_agg)
         if self.group and type_ == "time":
             data.append(info[0])
         else:
             if not isinstance(self.by, (list, tuple)):
                 by = [self.by]
             for g in by:
@@ -403,22 +502,22 @@
 
                 if "(" in v and v.split("(")[0] in ["corr"]:
                     pattern = r"\((.*?))"
                     if "," in v:  # call function with args
                         pattern = r"\((.*?),"
                         eval_info = re.sub(
                             pattern,
-                            "(self.dd['{}'],".format(re.findall(pattern, v)[0]),
+                            f"(self.dd['{re.findall(pattern, v)[0]}'],",
                             v,
                         )
                     else:
                         pattern = r"\((.*?)\)"
                         eval_info = re.sub(
                             pattern,
-                            "(self.dd['{}'])".format(re.findall(pattern, v)[0]),
+                            f"(self.dd['{re.findall(pattern, v)[0]}'])",
                             v,
                         )
                 else:
                     eval_info = v if "(" in v else v + "()"
                 data_direct.append(
                     eval(f"self.dd['{k}'].groupby(idxs=info, type_=type_)." + eval_info)
                 )
```

### Comparing `teapy-0.6.9/python/teapy/expr.py` & `teapy-0.7.0/tea-py/python/teapy/expr.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 from __future__ import annotations
 
-from .datadict import name_prefix
+from typing import Optional
+
+from .py_datadict import name_prefix
+from .selector import selector_to_expr
 from .tears import Expr
 from .tears import expr_register as _expr_register
 from .tears import parse_expr_list as asexprs
 
 Expr.where = Expr.where_
 
 
@@ -51,36 +54,31 @@
 
 
 @register
 def __setstate__(self, state):
     return Expr(state["arr"], state.get("name"))
 
 
-# @register
-# def outer_join(self, right, left_other=None, sort=True, rev=False):
-#     out = self._get_outer_join_idx(left_other=left_other, right=right, sort=sort, rev=rev)
-
-
 @register
 def mask_to_idx(self):
     from .tears import arange
 
     idx = arange(self.shape[0])
     return idx.filter(self)
 
 
 @register
 def rolling(
     self,
-    window: str | int = None,
+    window: str | int | None = None,
     time_expr=None,
     idx=None,
     offset=None,
     start_by="full",
-    others=None,
+    others: Expr | list(Expr) | None = None,
     by=None,
     type_=None,
 ) -> ExprRolling:
     """
     window: int | duration, such as 1y, 2mo, 3d, 4h, 5m, 6s, or combine them
     start_by: full | duration_start, only valid if window is a duration
     others: only available in rolling.apply, this can add other expressions into the rolling context
@@ -145,15 +143,16 @@
     def __init__(self, expr, window, time_expr=None, others=None, by=None):
         self.expr = expr
         self.time_expr = time_expr
         if by is not None:
             import warnings
 
             warnings.warn(
-                "by will be deprecated in future release, please use time_expr instead"
+                "by will be deprecated in future release, please use time_expr instead",
+                stacklevel=2,
             )
             self.time_expr = by
 
         self.window = window
         self.others = asexprs(others, copy=False) if others is not None else None
         self.name_auto = 0
         self.prepare()
@@ -240,14 +239,15 @@
             else:
                 raise ValueError
 
         return wrap_func
 
     def apply(self, agg_expr):
         idx = self.idx
+        agg_expr = selector_to_expr(agg_expr, context=True)
         if self.type in ["fix", "start", "time_start"]:
             if isinstance(agg_expr, (list, tuple)):
                 return [
                     self.expr.rolling_apply_with_start(
                         ae, roll_start=idx, others=self.others
                     )
                     for ae in agg_expr
@@ -337,14 +337,15 @@
                 )
             else:
                 raise ValueError
 
         return wrap_func
 
     def agg(self, agg_expr):
+        agg_expr = selector_to_expr(agg_expr, context=True)
         if self.type == "time":
             label, start_idx = self.info
             if isinstance(agg_expr, (list, tuple)):
                 return label, [
                     self.expr.group_by_startidx(ae, idx=start_idx, others=self.others)
                     for ae in agg_expr
                 ]
```

### Comparing `teapy-0.6.9/python/teapy/mod_func.py` & `teapy-0.7.0/tea-py/python/teapy/mod_func.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,86 +1,109 @@
-from .datadict import DataDict
-from .tears import PyDataDict, arange, stack
+from functools import wraps
 
+from .selector import Selector
+from .tears import arange, stack
+from .tears import corr as _corr
 
+
+def select_wrapper(func):
+    name = func.__qualname__
+    print(name)
+
+    @wraps(func)
+    def _wrap_func(exprs, *args, **kwargs):
+        if len(exprs) and isinstance(exprs[0], Selector):
+            return Selector().mod_func(name)(exprs, *args, **kwargs)
+        else:
+            return func(exprs, *args, **kwargs)
+
+    return _wrap_func
+
+
+@select_wrapper
 def hcorr(exprs, method="pearson", stable=False):
-    return PyDataDict(exprs).corr(method=method, stable=stable)
+    return _corr(exprs, method=method, stable=stable)
+    # return PyDataDict(exprs).corr(method=method, stable=stable)
 
 
+@select_wrapper
 def hmax(exprs, par=False):
     """horizontal max"""
     return stack(exprs, axis=-1).max(axis=-1, par=par)
 
 
+@select_wrapper
 def hmin(exprs, par=False):
     """horizontal min"""
     return stack(exprs, axis=-1).min(axis=-1, par=par)
 
 
+@select_wrapper
 def hmean(exprs, par=False, min_periods=1):
     """horizontal mean"""
     return stack(exprs, axis=-1).mean(axis=-1, par=par, min_periods=min_periods)
 
 
+@select_wrapper
 def hstd(exprs, par=False, min_periods=3):
     """horizontal std"""
     return stack(exprs, axis=-1).std(axis=-1, par=par, min_periods=min_periods)
 
 
+@select_wrapper
 def hsum(exprs, par=False):
     return stack(exprs, axis=-1).sum(axis=-1, par=par)
 
 
 def align_frames(dds, by, sort=True, rev=False, outer_df=False, with_by=True):
     suffix = "__align_by"
     if len(dds) <= 1:
         return dds
     if not isinstance(by, (list, tuple)):
         by = [by]
 
     dd_outer = dds[0].apply(lambda e: e.suffix(suffix + "0"), exclude=by)
     # s = 0
     for i, rdd in enumerate(dds[1:]):
-        rdd = rdd.apply(lambda e: e.suffix(suffix + str(i + 1)), exclude=by)
+        rdd = rdd.apply(lambda e, i=i: e.suffix(suffix + str(i + 1)), exclude=by)
         dd_outer.join(rdd, on=by, how="outer", sort=False, inplace=True)
         # # to avoid stack overflow
         # s += 1
         # if s == step:
         #     s = 0
         #     dd_outer.eval()
     if sort:
         dd_outer.sort(by=by, rev=rev, inplace=True)
     if outer_df:
         return dd_outer if with_by else dd_outer.exclude(by)
     if with_by:
         return [
-            dd_outer[by + ["^.*" + suffix + f"{i}$"]].apply(
-                lambda e: e.alias(e.name.replace(suffix + str(i), ""))
+            dd_outer[[*by, "^.*" + suffix + f"{i}$"]].apply(
+                lambda e, i=i: e.alias(e.name.replace(suffix + str(i), ""))
             )
             for i in range(len(dds))
         ]
     else:
         return dd_outer[by], [
             dd_outer["^.*" + suffix + f"{i}$"].apply(
-                lambda e: e.alias(e.name.replace(suffix + str(i), ""))
+                lambda e, i=i: e.alias(e.name.replace(suffix + str(i), ""))
             )
             for i in range(len(dds))
         ]
 
 
 def get_align_frames_idx(dds, by, sort=True, rev=False, return_by=False):
     if len(dds) <= 1:
         return dds
     if not isinstance(by, (list, tuple)):
         by = [by]
-    by0 = dds[0][by].raw_data
+    by0 = dds[0][by].exprs
     out_idxs = [arange(by0[0].shape[0])]
     for i, rdd in enumerate(dds[1:]):
-        # right_idx = arange(rdd.shape[0])
         left_other = by0[1:] if len(by) > 1 else None
         *by0, left_idx, right_idx = by0[0]._get_outer_join_idx(
-            left_other=left_other, right=rdd[by], sort=sort, rev=rev
+            left_other=left_other, right=rdd[by].exprs, sort=sort, rev=rev
         )
         for i, idx in enumerate(out_idxs):
             out_idxs[i] = idx.select(left_idx, check=False).cast("opt<usize>")
         out_idxs.append(right_idx)
     return out_idxs if not return_by else (by0, out_idxs)
```

### Comparing `teapy-0.6.9/python/teapy/regression.py` & `teapy-0.7.0/tea-py/python/teapy/regression.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 from functools import partial
 
 import teapy as tp
 from teapy import Expr, asexprs, nan
 
-from .tears import get_newey_west_adjust_s
+from .selector import Selector
+from .tears import get_newey_west_adjust_s as _get_newey_west_adjust_s
+
+
+def get_newey_west_adjust_s(x, resid, lag):
+    if isinstance(x, Selector):
+        return x.mod_func("regression.get_newey_west_adjust_s")(x, resid, lag)
+    return _get_newey_west_adjust_s(x, resid, lag)
 
 
 def mark_star(value_to_mark, t_value, p_value, precision=2, split="\r\n"):
     """用于标显著程度"""
     value_to_mark, t_value, p_value = asexprs((value_to_mark, t_value, p_value))
     value_to_mark = value_to_mark.round_string(precision)
     t_value = t_value.round_string(precision)
@@ -31,24 +38,25 @@
         calc_t=False,
         keep_shape=True,
         adjust_t=False,
         lag=None,
     ):
         """
         线性回归
-        y: 因变量，需是一维，支持的类型：能被转为Expr的所有类型
-        x: 自变量，支持的类型：能被转为Expr的所有类型
+        y: 因变量, 需是一维, 支持的类型: 能被转为Expr的所有类型
+        x: 自变量, 支持的类型: 能被转为Expr的所有类型
         constant: 是否在回归时给x加上常数项
-        dropna: 是否需要去掉nan，如果无nan却去除nan会略微降低效率
-        calc_t: 是否需要计算t值和p值，由于不需要计算时可以直接使用lapack求解，因此可以显著提高速度
-        keep_shape: 返回的残差序列resid是否保留原有序列的长度（默认会先去除nan，序列长度可能会改变
-        adjust_t: 是否需要对回归的t值和p值进行Newey-West调整，如果会True则默认calc_t也为True
-        lag: Newey-West调整时的最大滞后阶数，为None时使用最优滞后阶数的公式进行计算.
+        dropna: 是否需要去掉nan, 如果无nan却去除nan会略微降低效率
+        calc_t: 是否需要计算t值和p值, 由于不需要计算时可以直接使用lapack求解, 因此可以显著提高速度
+        keep_shape: 返回的残差序列resid是否保留原有序列的长度(默认会先去除nan, 序列长度可能会改变
+        adjust_t: 是否需要对回归的t值和p值进行Newey-West调整, 如果会True则默认calc_t也为True
+        lag: Newey-West调整时的最大滞后阶数, 为None时使用最优滞后阶数的公式进行计算.
         """
-        y, x = Expr(y), Expr(x)
+        if not isinstance(y, tp.Selector) and not isinstance(x, tp.Selector):
+            y, x = Expr(y), Expr(x)
         self.n_ori = y.shape[0]
         self.keep_shape = keep_shape
         self.dropna = dropna
         x = x.if_then(x.ndim() == 1, x.insert_axis(1))
         if dropna:
             nan_mask = y.is_nan() | x.is_nan().any(axis=1)
             y, x = y.filter(~nan_mask), x.filter(~nan_mask)
@@ -106,37 +114,38 @@
         if self.keep_shape and self.dropna:
             resid = tp.full(self.nan_mask.shape, nan)
             return resid.put_mask(~self.nan_mask, self.y - self.fitted_values)
         else:
             return self.y - self.fitted_values
 
     def result(self, i=1, mark=False, multiplier=1, precision=4, split="\r\n"):
-        """返回第i个位置的回归结果
-        i: 返回第i个位置（从0开始）的自变量的回归结果
+        """
+        返回第i个位置的回归结果
+        i: 返回第i个位置(从0开始)的自变量的回归结果
         mark: 是否需要直接返回标记星号的结果
         """
         if hasattr(self, "tvalues"):
             ret = [self.params[i] * multiplier, self.tvalues[i], self.pvalues[i]]
             for i, v in enumerate(ret):
                 ret[i] = v.round(precision)
             return mark_star(*ret, precision=precision, split=split) if mark else ret
         else:
             return (self.params[i] * multiplier).round(precision)
 
 
 # t统计量经过Newey West调整的线性回归
 NwOls = partial(Ols, calc_t=True, adjust_t=True)
 
-# 旧版本的api，后面可能会弃用
+# 旧版本的api, 后面可能会弃用
 sp_ols = partial(Ols, adjust_t=False)
 nw_ols = NwOls
 
 
 class ChowTest:
-    """邹检验，参考chowtest库，注意原库进行f检验时自由度似乎写错了，本函数已进行修正"""
+    """邹检验, 参考chowtest库, 注意原库进行f检验时自由度似乎写错了, 本函数已进行修正"""
 
     def __init__(self, y, x, x1_idx, x2_idx, constant=True):
         y, x, x1_idx, x2_idx = asexprs((y, x, x1_idx, x2_idx))
         res_all = Ols(y, x, constant=True)  # 全部数据的回归结果
         rss_all = res_all.resid.pow(2).sum()  # 总残差平方和rss
         x1, y1 = x[x1_idx], y[x1_idx]
         x2, y2 = x[x2_idx], y[x2_idx]
@@ -148,16 +157,17 @@
         numerator = (rss_all - (rss1 + rss2)) / k  # 邹统计量的分子
         denominator = (rss1 + rss2) / (N1 + N2 - 2 * k)  # 邹统计量的分母
         self.params = res1.params - res2.params
         self.chowvalues = numerator / denominator
         self.pvalues = 1 - self.chowvalues.f_cdf(df1=k, df2=(N1 + N2 - 2 * k))
 
     def result(self, i=1, mark=False, multiplier=1, precision=4, split="\r\n"):
-        """返回第i个位置的回归结果
-        i: 返回第i个位置（从0开始）的自变量的回归结果
+        """
+        返回第i个位置的回归结果
+        i: 返回第i个位置(从0开始)的自变量的回归结果
         mark: 是否需要直接返回标记星号的结果
         """
         ret = [self.params[i] * multiplier, self.chowvalues, self.pvalues]
         for i, v in enumerate(ret):
             ret[i] = v.round(precision)
         return mark_star(*ret, precision=precision, split=split) if mark else ret
 
@@ -167,21 +177,21 @@
 # =============================================================================
 if __name__ == "__main__":
     import numpy as np
     import statsmodels.api as sm
     from numpy.testing import assert_allclose
 
     def sp_ols_sm(y, x, constant=True):
-        """statsmodels的ols回归函数，效率较低，constant为True则加常数项"""
+        """statsmodels的ols回归函数, 效率较低, constant为True则加常数项"""
         x = np.asanyarray(x)
         x = np.vstack([np.ones(x.shape[0]), x.T]).T if constant else x
         return sm.OLS(np.asanyarray(y), x, missing="drop").fit()
 
     def nw_ols_sm(y, x, lag=None, constant=True):
-        """statsmodels实现的ols函数，效率较低，constant为True则加常数项, lag: 滞后阶数"""
+        """statsmodels实现的ols函数, 效率较低, constant为True则加常数项, lag: 滞后阶数"""
         nlag = int(np.ceil(4 * (y.size / 100) ** (2 / 9))) if lag is None else lag
         x = np.asanyarray(x)
         x = np.vstack([np.ones(x.shape[0]), x.T]).T if constant else x
         return sm.OLS(np.asanyarray(y), x, missing="drop").fit(
             cov_type="HAC", cov_kwds={"maxlags": nlag}
         )
```

### Comparing `teapy-0.6.9/python/teapy/testing.py` & `teapy-0.7.0/tea-py/python/teapy/testing.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 def assert_allclose3(a, b, c, *args):
     assert_allclose(a, b)
     assert_allclose(b, c)
     for v in args:
         assert_allclose(a, v)
 
 
-# 同个数组中的数如果差距过大，在计算时太小的数会被忽略
+# 同个数组中的数如果差距过大, 在计算时太小的数会被忽略
 STABLE_FLOAT_MIN, STABLE_FLOAT_MAX = -10, 10
 STABLE_INT_MIN, STABLE_INT_MAX = int(-1e3), int(1e3)
 dtype_list = [np.float64, np.float32, np.int32, np.int64]
 dtype_element_map_stable = {
     np.float64: st.floats(
         width=16, min_value=STABLE_FLOAT_MIN, max_value=STABLE_FLOAT_MAX
     ),
@@ -67,22 +67,25 @@
     np.int32: st.integers(min_value=-(2**25), max_value=2**25 - 1),
     np.int64: st.integers(min_value=-(2**55), max_value=2**55 - 1),
 }
 
 
 @defines_strategy()
 def make_arr(shape=100, nan_p=0.05, unique=False, dtype=None, stable=True):
-    """make a random array using hypothesis
+    """
+    make a random array using hypothesis
     shape: Array shape
     nan_p: Probability of nan in array
     dtype: Dtype of the array
     stable: Limit the difference of array elements to avoid floating point errors
     """
-    assert nan_p >= 0 and nan_p <= 1, "nan_p must in 0 - 1"
-    if type(shape) is int:
+    assert nan_p >= 0, "nan_p must in 0 - 1"
+    assert nan_p <= 1, "nan_p must in 0 - 1"
+
+    if isinstance(shape, int):
         shape = (shape,)
 
     @st.composite
     def draw_arr(draw):
         arr_dtype = draw(st.sampled_from(dtype_list)) if dtype is None else dtype
         dtype_map = dtype_element_map_stable if stable else dtype_element_map_unstable
         arr = draw(
@@ -92,17 +95,16 @@
                 elements=dtype_map[arr_dtype],
                 unique=unique,
             )
         )
         if nan_p > 0 and arr_dtype in [np.float64, np.float32]:
             nan_mask = np.random.binomial(1, nan_p, shape)
             np.putmask(arr, nan_mask, np.nan)
-        if stable:
-            if arr_dtype in [np.float64, np.float32]:
-                min_, max_ = np.nanmax(arr), np.nanmin(arr)
-                if ~np.isnan(max_) and max_ - abs(min_) * 1e6:  # suppose max > 0
-                    arr = np.where(arr < 1e-4, np.random.randn(*arr.shape), arr)
+        if stable and arr_dtype in [np.float64, np.float32]:
+            min_, max_ = np.nanmax(arr), np.nanmin(arr)
+            if ~np.isnan(max_) and max_ - abs(min_) * 1e6:  # suppose max > 0
+                arr = np.where(arr < 1e-4, np.random.randn(*arr.shape), arr)
             # else:
             #     min_, max_ = np.max(arr), np.min(arr)
         return arr
 
     return draw_arr()
```

### Comparing `teapy-0.6.9/python/teapy/tests/test_array_func.py` & `teapy-0.7.0/tea-py/python/teapy/tests/test_array_func.py`

 * *Files 1% similar despite different names*

```diff
@@ -293,14 +293,17 @@
         tp.Expr(s.copy()).fillna("bfill", 0).eview(), [5, 5, 6, 733, 34, 34, 0, 0]
     )
     # test inplace
     tp.fillna(s, value=fill_value, inplace=True)
     assert_allclose(s, np.array([101, 5, 6, 733, 101, 34, 101, 101]))
 
 
+test_fillna()
+
+
 def test_clip():
     s = pd.Series([np.nan, 5, 6, 733, np.nan, 34, 456, np.nan])
     assert_allclose3(
         tp.clip(s, 5, 100), Expr(s, copy=True).clip(5, 100).eview(), s.clip(5, 100)
     )
     # test inplace
     s1 = s.copy()
```

### Comparing `teapy-0.6.9/python/teapy/tests/test_common.py` & `teapy-0.7.0/tea-py/python/teapy/tests/test_common.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,11 @@
-# from time import time
-
 import numpy as np
 import teapy as tp
 from teapy.testing import assert_allclose
 
-# import pandas as pd
-
 
 def test_continuity():
     # test output continuity
     arr1 = np.array(np.random.randn(100, 20), order="c")
     assert tp.ts_sma(arr1, window=3).flags["C_CONTIGUOUS"]
     arr2 = np.array(np.random.randn(100, 20), order="f")
     assert tp.ts_sma(arr2, window=3).flags["F_CONTIGUOUS"]
```

### Comparing `teapy-0.6.9/python/teapy/tests/test_context.py` & `teapy-0.7.0/tea-py/python/teapy/tests/test_context.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 import numpy as np
 import teapy as tp
-from teapy import ct
+from teapy import s
 from teapy.regression import Ols
 from teapy.testing import assert_allclose
 
 
 def test_base():
-    c = ct("b").ts_sum(2)
-    d = ct("a").mean().alias("d")
+    c = s("b").ts_sum(2).alias("c")
+    d = s("a").mean().alias("d")
 
     dd = tp.DataDict(a=[1.0, 2, 3, 4], b=[4, 3, 1])
-    dd = dd.with_columns(d)
-
-    assert_allclose(c.eview(dd, freeze=False), [4, 7, 4])
-    assert c.step > 0
-    assert_allclose(c.eview(dd, freeze=True), [4, 7, 4])
-    assert_allclose(c.view, [4, 7, 4])
-    dd.eval(context=True)
+    dd = dd.with_columns(c, d)
+    # assert_allclose(c.eview(), [4, 7, 4])
+    assert_allclose(dd["c"].view, [4, 7, 4])
+    dd.eval()
     assert dd["d"].view == 2.5
 
 
 def test_rolling_context():
     x = tp.Expr([1, 2, 3, 4, 5])
     y = tp.Expr([2, 3, 4, 5, 6])
-    assert_allclose(x.rolling(2).apply(ct(0).sum()).eview(), np.array([1, 3, 5, 7, 9]))
+    assert_allclose(x.rolling(2).apply(s(0).sum()).eview(), np.array([1, 3, 5, 7, 9]))
     assert_allclose(
-        x.rolling(2, others=y).apply(-ct(0).sum() + ct(1).sum()).eview(),
+        x.rolling(2, others=y).apply(-s(0).sum() + s(1).sum()).eview(),
         np.array([1, 2, 2, 2, 2]),
     )
     x = tp.Expr([1, 2, np.nan, 4, 5])
     y = tp.Expr([2, 3, 4, 5, 6])
 
     assert_allclose(
-        x.rolling(4, others=y).apply(Ols(ct(1), ct(0)).params.last()).eview(),
+        x.rolling(4, others=y).apply(Ols(s(1), s(0)).params.last()).eview(),
         np.array([0, 1, 1, 1, 1]),
     )
```

### Comparing `teapy-0.6.9/python/teapy/tests/test_datadict.py` & `teapy-0.7.0/tea-py/python/teapy/tests/test_datadict.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import numpy as np
 import pandas as pd
 import teapy as tp
 from numpy.testing import assert_array_equal
-from teapy import DataDict, Expr, ct, get_align_frames_idx
+from teapy import Expr, get_align_frames_idx, s
+from teapy.py_datadict import DataDict
 from teapy.testing import assert_allclose, assert_allclose3
 
 
 def test_memory():
     a = np.random.randn(1000, 1000)
     b = a.copy()
     dd = DataDict(a=a)
@@ -36,17 +37,17 @@
     assert DataDict([ea, eb]).columns == ["a", "b"]
     assert DataDict([ea, eb], columns=["c", "d"]).columns == ["c", "d"]
 
 
 def test_rename():
     dd = DataDict({"a": [2], "b": [45]})
     dd.rename({"a": "c"}, inplace=True)
-    assert set(dd.columns) == set(["c", "b"])
+    assert set(dd.columns) == {"c", "b"}
     dd = dd.rename({"b": "a"})
-    assert set(dd.columns) == set(["c", "a"])
+    assert set(dd.columns) == {"c", "a"}
     dd = dd.rename(["a", "b"])
     assert dd.columns == ["a", "b"]
 
 
 def test_get_and_set_item():
     dd = DataDict()
     a = np.random.randn(100)
@@ -82,16 +83,16 @@
     assert dd.columns == []
 
 
 def test_to_dict():
     data = {"a": 1, "b": 2}
     dd = DataDict(data)
     assert dd.to_dict() == data
-    dd = dd.with_columns((ct("a") * 2).alias("c"))
-    assert dd.to_dict(context=True) == {"a": 1, "b": 2, "c": 2}
+    dd = dd.with_columns((s("a") * 2).alias("c"))
+    assert dd.to_dict() == {"a": 1, "b": 2, "c": 2}
 
 
 def test_dropna():
     dd = DataDict(
         {
             "a": [1, 2, np.nan, 3, 2, np.nan],
             "b": [np.nan, 3, np.nan, 4, np.nan, 5],
@@ -196,15 +197,15 @@
     ldd = DataDict({"left_on": ["a", "b", "a", "c"], "va": [1, 2, 3, 4]})
     rdd = DataDict({"right_on": ["b", "b", "c"], "vb": [10, 20, 30]})
     ldd.join(rdd, left_on="left_on", right_on="right_on", how="right", inplace=True)
     assert_allclose(rdd["va"].eview(), np.array([2, 2, 4]))
 
     ldd = DataDict({"on": ["a", "b", "d", "c"], "va": [1, 2, 3, 4]})
     rdd = DataDict({"on": ["b", "a", "e"], "vb": [10, 20, 30]})
-    dd = ldd.join(rdd, how="outer", on="on").eval(False)
+    dd = ldd.join(rdd, how="outer", on="on").eval()
     assert_allclose(dd["va"].eview(), np.array([1, 2, 4, 3, np.nan]))
     assert_allclose(dd["vb"].eview(), np.array([20, 10, np.nan, np.nan, 30]))
     assert_array_equal(dd["on"].eview(), np.array(["a", "b", "c", "d", "e"]))
 
     by, idxs = get_align_frames_idx([ldd, rdd], by="on", return_by=True)
     assert_allclose(ldd["va"].select(idxs[0]).eview(), np.array([1, 2, 4, 3, np.nan]))
     assert_allclose(
@@ -214,33 +215,33 @@
 
 
 def test_groupby():
     n = 100
     dd = DataDict(
         {
             "g": ["e", "e"] + ["a", "b", "a", "a", "c"] * n + ["d"],
-            "v": [-0.1, -5] + np.random.randn(5 * n).tolist() + [1],
+            "v": [-0.1, -5, *np.random.randn(5 * n).tolist(), 1],
         }
     )
     df = dd.to_pd()
     assert_allclose(
-        dd.groupby("g").agg(ct(1).max().alias("v"))["v"].eview(),
+        dd.groupby("g").agg(s(1).max().alias("v"))["v"].eview(),
         df.groupby("g", sort=False).v.max(),
     )
 
     dd = DataDict(
         {
             "a": ["a", "b", "a", "b", "b", "c"],
             "b": [1, 2, 3, 4, 5, 6],
             "c": [6, 5, 4, 3, 2, 1],
         }
     )
 
     res = dd.groupby("a").agg(
-        ct("c").sum().alias("c1"),
+        s("c").sum().alias("c1"),
         c="max",
     )
     assert_allclose(res["c1"].eview(), np.array([10, 10, 1]))
     assert_allclose(res["c"].eview(), np.array([6, 5, 1]))
 
 
 def test_unique():
```

### Comparing `teapy-0.6.9/python/teapy/tests/test_equity.py` & `teapy-0.7.0/tea-py/python/teapy/tests/test_equity.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,36 +25,36 @@
         leverage=2,
     ).eview()
 
     # time0: 1_000_000
     # time1:
     #   买入 1_000_000 * 2 * 1 / (100 * 10) = 2000手
     #   手续费: 1_000_000 * 2 * 0.0003 = 600
-    #   当期损益： (102-100) * 2000 * 10 = 40000
+    #   当期损益:  (102-100) * 2000 * 10 = 40000
     #   1_000_000 - 600 + 40000 = 1_039_400
     # time2:
     #   1_039_400 + (105-102) * 2000 * 10 = 1_099_400
     # time3:
     #   目标持仓手数: 1_099_400 * 2 * 0.5 / (105 * 10) = 1047
     #   换仓手续费: (2000 - 1047) * 10 * 105 * 0.0003 = 300.195
     #   当期损益: (96 - 105) * 1047 * 10  = -94230
     #   1_099_400 - 94230 - 300.195 = 1_004_869.805
     # time4:
     #   目标持仓手数: 1_004_869.805 * 2 * -0.5 / (96 * 10) = -1046
     #   手续费: (1047 + 1046) * 96 * 10 * 0.0003 = 602.784
-    #   当期损益：(90 - 96) * -1046 * 10 = 62760
+    #   当期损益: (90 - 96) * -1046 * 10 = 62760
     #   1_004_869.805 - 602.784 + 62760 = 1067027.021
     # time5: 换月
-    #   新的目标持仓手数：(1067027.021 * 2 * -0.5) / (10 * 220) = -485
+    #   新的目标持仓手数: (1067027.021 * 2 * -0.5) / (10 * 220) = -485
     #   平仓并重新开仓的手续费(以新的开仓价近似计算手续费): 485 * 2 * 220 * 10 * 0.0003=640.20
-    #   当期损益： (226 - 220) * -485 * 10 = -29100
+    #   当期损益:  (226 - 220) * -485 * 10 = -29100
     #   1067027.021 - 29100 - 640.20 = 1037286.821
     # time6:
-    #   平仓手续费： 485 * 226 * 10 * 0.0003 = 328.83
-    #   损益： -485 * (226 - 226) * 10 = 0
+    #   平仓手续费:  485 * 226 * 10 * 0.0003 = 328.83
+    #   损益:  -485 * (226 - 226) * 10 = 0
     #   1037286.821 - 328.83 = 1036957.991
 
     expect = Expr(
         [
             1_000_000,
             1_039_400,
             1_099_400,
```

### Comparing `teapy-0.6.9/python/teapy/tests/test_expr.py` & `teapy-0.7.0/tea-py/python/teapy/tests/test_expr.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,13 +138,13 @@
         [5, 5, 9, 5, 8, 8, 2, 7, 3, 3, 8, 6, 4, 7, 8, 3, 1, 5, 3, 4, 4, 7, 9, 3]
     )
     for closed in ["left", "right"]:
         df = pd.DataFrame({"time": time.view, "value": value.view})
         df_pd = df.set_index("time").resample("12h", closed=closed).sum()
 
         label, v = value.groupby("12h", time_expr=time, closed=closed).agg(
-            tp.ct(0).sum()
+            tp.s(0).sum()
         )
         label = label.eview()
         v = v.eview()
         assert_allclose(v, df_pd["value"])
         assert_series_equal(pd.Series(label), df_pd.index.to_series())
```

### Comparing `teapy-0.6.9/python/teapy/tests/window/test_compare.py` & `teapy-0.7.0/tea-py/python/teapy/tests/window/test_compare.py`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/python/teapy/tests/window/test_corr.py` & `teapy-0.7.0/tea-py/python/teapy/tests/window/test_corr.py`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/python/teapy/tests/window/test_feature.py` & `teapy-0.7.0/tea-py/python/teapy/tests/window/test_feature.py`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/python/teapy/tests/window/test_norm.py` & `teapy-0.7.0/tea-py/python/teapy/tests/window/test_norm.py`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/python/teapy/tests/window/test_reg.py` & `teapy-0.7.0/tea-py/python/teapy/tests/window/test_reg.py`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/python/teapy/window_func.py` & `teapy-0.7.0/tea-py/python/teapy/window_func.py`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/python/teapy/wrapper.py` & `teapy-0.7.0/tea-py/python/teapy/wrapper.py`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/requirements-dev.lock` & `teapy-0.7.0/tea-py/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/src/equity.rs` & `teapy-0.7.0/tea-py/src/equity.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/src/from_py.rs` & `teapy-0.7.0/tea-py/src/from_py.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-#[cfg(feature = "lazy")]
-use crate::pylazy::PyDataDict;
+// #[cfg(feature = "lazy")]
+// use crate::pylazy::PyDataDict;
 #[cfg(feature = "lazy")]
 use crate::pylazy::RefObj;
 use ahash::HashMap;
 use numpy::{
     datetime::{units, Datetime},
-    PyArray, PyArrayDyn,
+    PyArray, PyArrayDyn, PyUntypedArrayMethods,
+};
+use pyo3::{
+    exceptions::PyValueError, prelude::PyAnyMethods, Bound, FromPyObject, PyAny, PyObject,
+    PyResult, Python, ToPyObject,
 };
-use pyo3::{exceptions::PyValueError, FromPyObject, PyAny, PyObject, PyResult, Python, ToPyObject};
-use std::sync::Arc;
+// use std::sync::Arc;
 #[cfg(feature = "option_dtype")]
 use tea_core::datatype::{OptF64, OptI64};
 use tea_core::prelude::*;
 #[cfg(feature = "arw")]
 use tea_io::ColSelect;
 #[cfg(feature = "lazy")]
 use tea_lazy::Context;
@@ -151,14 +154,24 @@
             Ok(self.call_method0("item")?.to_object(py))
         } else {
             Ok(self.to_object(py))
         }
     }
 }
 
+impl<T, D> NoDim0 for Bound<'_, PyArray<T, D>> {
+    fn no_dim0(self, py: Python) -> PyResult<PyObject> {
+        if self.ndim() == 0 {
+            Ok(self.call_method0("item")?.to_object(py))
+        } else {
+            Ok(self.to_object(py))
+        }
+    }
+}
+
 #[cfg(feature = "lazy")]
 #[derive(Clone, Default)]
 pub struct PyContext<'py> {
     pub ct: Option<Context<'py>>,
     pub obj_map: HashMap<String, RefObj>,
 }
 
@@ -176,26 +189,26 @@
 impl<'py> FromPyObject<'py> for PyContext<'py> {
     fn extract(ob: &'py PyAny) -> PyResult<PyContext<'py>> {
         if ob.is_none() {
             Ok(Self {
                 ct: None,
                 obj_map: Default::default(),
             })
-        } else if let Ok(dd) = ob.extract::<PyDataDict>() {
-            Ok(Self {
-                // safety: we can cast 'py to 'static as we are running in python
-                ct: unsafe { Some(std::mem::transmute(Arc::new(dd.dd))) },
-                obj_map: dd.obj_map,
-            })
-        } else if ob.hasattr("_dd")? && ob.get_type().name()? == "DataDict" {
-            let dd = ob.getattr("_dd")?.extract::<PyDataDict>()?;
-            Ok(Self {
-                ct: unsafe { Some(std::mem::transmute(Arc::new(dd.dd))) },
-                obj_map: dd.obj_map,
-            })
+        // } else if let Ok(dd) = ob.extract::<PyDataDict>() {
+        //     Ok(Self {
+        //         // safety: we can cast 'py to 'static as we are running in python
+        //         ct: unsafe { Some(std::mem::transmute(Arc::new(dd.dd))) },
+        //         obj_map: dd.obj_map,
+        //     })
+        // } else if ob.hasattr("_dd")? && ob.get_type().name()? == "DataDict" {
+        //     let dd = ob.getattr("_dd")?.extract::<PyDataDict>()?;
+        //     Ok(Self {
+        //         ct: unsafe { Some(std::mem::transmute(Arc::new(dd.dd))) },
+        //         obj_map: dd.obj_map,
+        //     })
         } else {
             Err(PyValueError::new_err(
                 "Cannot extract a Context from the object",
             ))
         }
     }
 }
```

### Comparing `teapy-0.6.9/src/lib.rs` & `teapy-0.7.0/tea-py/src/lib.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/src/pylazy/datadict.rs` & `teapy-0.7.0/tea-py/src/pylazy/pyfunc.rs`

 * *Files 22% similar despite different names*

```diff
@@ -1,624 +1,516 @@
-use ahash::HashMap;
-use pyo3::{PyTraverseError, PyVisit};
-use std::borrow::Cow;
-use std::fmt::Debug;
-use std::ops::{Deref, DerefMut};
-
+use super::super::from_py::{PyArrayOk, PyList};
+// use super::datadict::{IntoPyDataDict, PyDataDict, PyVecExprToRs};
 use super::export::*;
-use super::pyexpr::RefObj;
-use tea_core::prelude::StrError;
-use tea_core::utils::CollectTrustedToVec;
-use tea_lazy::{ColumnSelector, DataDict, Expr, GetOutput};
+use pyo3::types::{PyList as PyList3, PyTuple};
+use tea_core::prelude::*;
+use tea_lazy::{ColumnSelector, Data, Expr};
 
 #[cfg(feature = "agg")]
-use tea_ext::agg::*;
+use tea_ext::agg::{corr, CorrMethod};
 
-#[pyclass]
-#[derive(Clone, Default)]
-pub struct PyDataDict {
-    pub dd: DataDict<'static>,
-    pub obj_map: HashMap<String, RefObj>,
-}
-
-impl DerefMut for PyDataDict {
-    fn deref_mut(&mut self) -> &mut Self::Target {
-        &mut self.dd
-    }
+#[cfg(feature = "arw")]
+use crate::from_py::PyColSelect;
+#[cfg(feature = "arw")]
+use tea_core::prelude::StrError;
+#[cfg(feature = "create")]
+use tea_ext::create::*;
+#[cfg(feature = "map")]
+use tea_ext::map::*;
+// #[cfg(feature = "io")]
+// use tea_io::*;
+
+#[pyfunction]
+/// A util function to convert python object to PyExpr without copy
+pub fn parse_expr_nocopy(obj: &PyAny) -> PyResult<PyExpr> {
+    unsafe { parse_expr(obj, false) }
 }
 
-impl Deref for PyDataDict {
-    type Target = DataDict<'static>;
+#[pyfunction]
+#[pyo3(signature=(obj, copy=false))]
+/// A util function to convert python object to PyExpr
+///
+/// copy: whether to copy numpy.ndarray when creating the PyExpr
+pub unsafe fn parse_expr(obj: &PyAny, copy: bool) -> PyResult<PyExpr> {
+    if let Ok(expr) = obj.extract::<PyExpr>() {
+        Ok(expr)
+    } else if obj.get_type().qualname()? == "Expr" {
+        // For any crate that extends this crate
+        let module_name = obj.getattr("__module__")?.extract::<&str>()?;
+        if module_name == "teapy" {
+            // let cell: &PyCell<PyExpr> = PyTryFrom::try_from_unchecked(obj);
+            let cell: &PyCell<PyExpr> = obj.downcast_unchecked();
+            Ok(cell.try_borrow()?.clone())
+        } else {
+            Err(PyValueError::new_err(format!(
+                "Unknown Expr type from {module_name}"
+            )))
+        }
+    } else if obj.get_type().qualname()? == "Selector" {
+        let module_name = obj.getattr("__module__")?.extract::<&str>()?;
+        let module_name = module_name.split('.').next().unwrap();
+        if module_name == "teapy" {
+            let kwargs = PyDict::new(obj.py());
+            kwargs.set_item("context", true)?;
+            let expr_obj = obj.call_method("to_expr", (), Some(kwargs))?;
+            return parse_expr(expr_obj, copy);
+        } else {
+            Err(PyValueError::new_err(format!(
+                "Unknown Selector type from {module_name}"
+            )))
+        }
+    } else if obj.get_type().qualname()? == "DataFrame" {
+        // cast pandas.DataFrame or polars DataFrame to PyExpr
+        let module_name = obj.getattr("__module__")?.extract::<&str>()?;
+        let module_name = module_name.split('.').next().unwrap();
+        if module_name == "pandas" {
+            let obj = obj.getattr("values")?;
+            return parse_expr(obj, copy);
+        } else if module_name == "polars" {
+            let kwargs = PyDict::new(obj.py());
+            kwargs.set_item("writable", false)?;
+            let obj = obj.call_method("to_numpy", (), Some(kwargs))?;
+            // let obj = obj.getattr("to_numpy")?.call((), Some(kwargs))?;
+            return parse_expr(obj, copy);
+        } else {
+            return Err(PyValueError::new_err(format!(
+                "DataFrame of module {module_name} is not supported"
+            )));
+        }
+    } else if obj.get_type().qualname()? == "Series" {
+        // cast pandas.Series to PyExpr
+        let module_name = obj.getattr("__module__")?.extract::<&str>()?;
+        let module_name = module_name.split('.').next().unwrap();
+        if module_name == "pandas" {
+            dbg!("parse pd Series");
+            let obj = obj.getattr("values")?;
+            return parse_expr(obj, copy);
+        } else if module_name == "polars" {
+            let kwargs = PyDict::new(obj.py());
+            kwargs.set_item("writable", false)?;
+            let dtype = obj.getattr("dtype")?.str()?.to_str()?;
+            // let mut obj = obj.getattr("to_numpy")?.call((), Some(kwargs))?;
+            let mut obj = obj.call_method("to_numpy", (), Some(kwargs))?;
+            if dtype == "Utf8" {
+                // obj = obj.getattr("astype")?.call1(("str",))?;
+                obj = obj.call_method("astype", ("str",), None)?;
+            }
+            return parse_expr(obj, copy);
+        } else {
+            return Err(PyValueError::new_err(format!(
+                "Series of module {module_name} is not supported"
+            )));
+        }
+    } else if let Ok(pyarr) = obj.extract::<PyArrayOk>() {
+        // cast numpy.ndarray to PyExpr
+        if pyarr.is_object() {
+            let arr = pyarr.into_object()?;
+            if copy {
+                let e: Expr<'static> = arr.to_owned_array().wrap().into();
+                return Ok(e.into());
+            } else {
+                let arr_res = arr.try_readwrite();
+                if let Ok(mut arr) = arr_res {
+                    let arr_write = arr.as_array_mut();
+                    let arb_arr = ArbArray::ViewMut(arr_write.wrap());
+                    // This is safe when the pyarray exists on the python side
+                    // so we should keep a reference to the pyobject
+                    return Ok(
+                        std::mem::transmute::<Expr<'_>, Expr<'static>>(arb_arr.into())
+                            .to_py(Some(vec![obj.to_object(obj.py())])),
+                    );
+                } else {
+                    // not writable
+                    let arr_read = arr.as_array();
+                    let arb_arr = ArbArray::View(arr_read.wrap());
+                    // This is only safe when the pyarray exists
+                    return Ok(
+                        std::mem::transmute::<Expr<'_>, Expr<'static>>(arb_arr.into())
+                            .to_py(Some(vec![obj.to_object(obj.py())])),
+                    );
+                };
+            }
+        } else {
+            #[cfg(feature = "time")]
+            {
+                if pyarr.is_datetime() {
+                    // we don't need to reference to the pyobject here because we made a copy
+                    use PyArrayOk::*;
+                    {
+                        let out: PyExpr = match pyarr {
+                            DateTimeMs(arr) => Expr::new_from_owned(
+                                arr.readonly()
+                                    .as_array()
+                                    .map(|v| Into::<DateTime>::into(*v))
+                                    .wrap(),
+                                None,
+                            )
+                            .into(),
+                            DateTimeNs(arr) => Expr::new_from_owned(
+                                arr.readonly()
+                                    .as_array()
+                                    .map(|v| Into::<DateTime>::into(*v))
+                                    .wrap(),
+                                None,
+                            )
+                            .into(),
+                            DateTimeUs(arr) => Expr::new_from_owned(
+                                arr.readonly()
+                                    .as_array()
+                                    .map(|v| Into::<DateTime>::into(*v))
+                                    .wrap(),
+                                None,
+                            )
+                            .into(),
+                            _ => unreachable!(),
+                        };
+                        return Ok(out);
+                    }
+                }
+            }
+        }
 
-    fn deref(&self) -> &Self::Target {
-        &self.dd
+        if copy {
+            match_pyarray!(
+                pyarr,
+                arr,
+                { Ok(Expr::new_from_owned(arr.to_owned_array().wrap(), None).into()) },
+                F64,
+                F32,
+                I64,
+                I32,
+                Bool
+            )
+        } else {
+            match_pyarray!(
+                pyarr,
+                arr,
+                {
+                    let arr_res = arr.try_readwrite();
+                    if let Ok(mut arr) = arr_res {
+                        let arr_write = arr.as_array_mut();
+                        let arb_arr = ArbArray::ViewMut(arr_write.wrap());
+                        // safe when pyarray exists
+                        Ok(
+                            std::mem::transmute::<Expr<'_>, Expr<'static>>(Expr::new(
+                                arb_arr, None,
+                            ))
+                            .to_py(Some(vec![obj.to_object(obj.py())])),
+                        )
+                    } else {
+                        let arr_read = arr.as_array();
+                        let arb_arr = ArbArray::View(arr_read.wrap());
+                        // safe when pyarray exists
+                        Ok(
+                            std::mem::transmute::<Expr<'_>, Expr<'static>>(Expr::new(
+                                arb_arr, None,
+                            ))
+                            .to_py(Some(vec![obj.to_object(obj.py())])),
+                        )
+                    }
+                },
+                F64,
+                F32,
+                I64,
+                I32,
+                Bool
+            )
+        }
+    } else if let Ok(pylist) = obj.extract::<PyList>() {
+        match_pylist!(pylist, l, {
+            Ok(Expr::new_from_owned(Arr1::from_vec(l).to_dimd(), None).into())
+        })
+    } else if let Ok(val) = obj.extract::<i32>() {
+        Ok(Expr::new(val.into(), None).into())
+    } else if let Ok(val) = obj.extract::<f64>() {
+        Ok(Expr::new(val.into(), None).into())
+    } else if let Ok(val) = obj.extract::<String>() {
+        Ok(Expr::new(val.into(), None).into())
+    } else {
+        Err(PyValueError::new_err(format!(
+            "Not support this type of Pyobject {}",
+            obj.get_type()
+        )))
     }
 }
 
-impl Debug for PyDataDict {
-    fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
-        self.dd.fmt(f)
+#[pyfunction]
+#[allow(clippy::missing_safety_doc)]
+#[pyo3(signature=(obj, copy=false))]
+pub unsafe fn parse_expr_list(obj: &PyAny, copy: bool) -> PyResult<Vec<PyExpr>> {
+    if obj.is_instance_of::<PyList3>() || obj.is_instance_of::<PyTuple>() {
+        if let Ok(seq) = obj.extract::<Vec<&PyAny>>() {
+            Ok(seq
+                .into_iter()
+                .map(|obj| parse_expr(obj, copy).expect("Not support this type of Pyobject"))
+                .collect_trusted())
+        } else {
+            unreachable!()
+        }
+    // } else if let Ok(datadict) = obj.extract::<PyDataDict>() {
+    //     // let data = datadict.dd.data;
+    //     let mut obj_map = datadict.obj_map;
+    //     Ok(datadict
+    //         .dd
+    //         .data
+    //         .into_iter()
+    //         .map(|e| {
+    //             if let Some(obj) = obj_map.remove(e.ref_name().unwrap()) {
+    //                 e.to_py(obj)
+    //             } else {
+    //                 e.to_py(None)
+    //             }
+    //         })
+    //         .collect())
+    // } else if obj.hasattr("_dd")? && obj.get_type().name()? == "DataDict" {
+    //     parse_expr_list(obj.getattr("_dd")?, copy)
+    } else if obj.hasattr("exprs")? && obj.get_type().name()? == "DataDict" {
+        parse_expr_list(obj.getattr("exprs")?, copy)
+    } else if let Ok(pyexpr) = parse_expr(obj, copy) {
+        Ok(vec![pyexpr])
+    } else {
+        Err(PyValueError::new_err(
+            "Can't parse the Object to a vector of expr",
+        ))
     }
 }
 
-pub trait IntoPyDataDict {
-    fn to_py(self, obj_map: HashMap<String, RefObj>) -> PyDataDict;
+#[cfg(all(feature = "concat", feature = "map"))]
+#[pyfunction]
+#[pyo3(signature=(exprs, axis=0))]
+#[allow(unreachable_patterns)]
+pub fn concat_expr(exprs: Vec<PyExpr>, axis: i32) -> PyResult<PyExpr> {
+    let mut e1 = exprs.get(0).unwrap().clone();
+    let obj_vec = exprs.iter().skip(1).map(|e| e.obj()).collect_trusted();
+    e1.e.concat(
+        exprs.into_iter().skip(1).map(|e| e.e).collect_trusted(),
+        axis,
+    );
+    Ok(e1.add_obj_vec_into(obj_vec))
 }
 
-impl IntoPyDataDict for DataDict<'static> {
-    fn to_py(self, obj_map: HashMap<String, RefObj>) -> PyDataDict {
-        PyDataDict { dd: self, obj_map }
-    }
+#[cfg(all(feature = "concat", feature = "map"))]
+#[pyfunction]
+#[allow(clippy::missing_safety_doc)]
+#[pyo3(name="concat", signature=(exprs, axis=0))]
+pub unsafe fn concat_expr_py(exprs: Vec<&PyAny>, axis: i32) -> PyResult<PyExpr> {
+    let exprs = exprs
+        .into_iter()
+        .map(parse_expr_nocopy)
+        .collect::<PyResult<Vec<PyExpr>>>()?;
+    concat_expr(exprs, axis)
 }
 
-pub trait PyVecExprToRs {
-    fn into_rs(
-        self,
-        names: Option<Vec<String>>,
-    ) -> PyResult<(Vec<Expr<'static>>, HashMap<String, RefObj>)>;
-}
-
-impl PyVecExprToRs for Vec<PyExpr> {
-    fn into_rs(
-        self,
-        names: Option<Vec<String>>,
-    ) -> PyResult<(Vec<Expr<'static>>, HashMap<String, RefObj>)> {
-        let obj_map = if let Some(names) = names {
-            if names.len() != self.len() {
-                return Err(StrError(
-                    "The length of names are not equal to the number of expressions".into(),
-                )
-                .to_py());
-            }
-            zip(&self, names).map(|(e, name)| (name, e.obj())).collect()
-        } else {
-            let mut name_auto = -1;
-            self.iter()
-                .map(|e| {
-                    (
-                        e.e.name().unwrap_or_else(|| {
-                            name_auto += 1;
-                            format!("column_{name_auto}")
-                        }),
-                        e.obj(),
-                    )
-                })
-                .collect()
-        };
-        let expr_rs = self.into_iter().map(|e| e.e).collect_trusted();
-        Ok((expr_rs, obj_map))
-    }
+#[cfg(all(feature = "concat", feature = "map"))]
+#[pyfunction]
+#[pyo3(signature=(exprs, axis=0))]
+#[allow(unreachable_patterns)]
+pub fn stack_expr(exprs: Vec<PyExpr>, axis: i32) -> PyResult<PyExpr> {
+    let mut e1 = exprs.get(0).unwrap().clone();
+    let obj_vec = exprs.iter().skip(1).map(|e| e.obj()).collect_trusted();
+    e1.e.stack(
+        exprs.into_iter().skip(1).map(|e| e.e).collect_trusted(),
+        axis,
+    );
+    Ok(e1.add_obj_vec_into(obj_vec))
 }
 
-impl PyDataDict {
-    pub fn remove_ref_obj(&mut self, select: Vec<String>) {
-        select.into_iter().for_each(|e| {
-            self.obj_map.remove(&e);
-        });
-    }
-
-    pub fn update_ref_obj_name(&mut self, old_name: &str, new_name: &str) {
-        if let Some(obj) = self.obj_map.remove(old_name) {
-            self.obj_map.insert(new_name.to_string(), obj);
-        }
-    }
+#[cfg(all(feature = "concat", feature = "map"))]
+#[pyfunction]
+#[allow(clippy::missing_safety_doc)]
+#[pyo3(name="stack", signature=(exprs, axis=0))]
+pub unsafe fn stack_expr_py(exprs: Vec<&PyAny>, axis: i32) -> PyResult<PyExpr> {
+    let exprs = exprs
+        .into_iter()
+        .map(|e| parse_expr_nocopy(e).expect("can not parse thid type into Expr"))
+        .collect::<Vec<PyExpr>>();
+    stack_expr(exprs, axis)
+}
 
-    pub fn add_ref_obj(&mut self, name: &str, obj: RefObj) -> Option<RefObj> {
-        self.obj_map.insert(name.to_string(), obj)
-    }
+#[cfg(feature = "agg")]
+#[pyfunction]
+#[pyo3(name="corr", signature=(exprs, method=CorrMethod::Pearson, min_periods=1, stable=false))]
+pub fn corr_py(
+    exprs: Vec<&PyAny>,
+    method: CorrMethod,
+    min_periods: usize,
+    stable: bool,
+) -> PyResult<PyExpr> {
+    let exprs = exprs
+        .into_iter()
+        .map(|e| parse_expr_nocopy(e).expect("can not parse thid type into Expr"))
+        .collect::<Vec<PyExpr>>();
+    let obj_vec = exprs.iter().map(|e| e.obj()).collect_trusted();
+    let exprs = exprs.into_iter().map(|e| e.e).collect_trusted();
+    let out: PyExpr = corr(exprs, method, min_periods, stable).into();
+    Ok(out.add_obj_vec_into(obj_vec))
+}
 
-    pub fn add_obj_map(&mut self, obj_map: HashMap<String, RefObj>) {
-        self.obj_map.extend(obj_map);
+#[pyfunction]
+#[pyo3(signature=(exprs, inplace=false, freeze=true))]
+pub fn eval_exprs(
+    mut exprs: Vec<PyExpr>,
+    inplace: bool,
+    freeze: bool,
+) -> PyResult<Option<Vec<PyExpr>>> {
+    exprs
+        .par_iter_mut()
+        .try_for_each(|e| e.eval_inplace(None, freeze))?;
+    if inplace {
+        Ok(None)
+    } else {
+        Ok(Some(exprs))
     }
+}
 
-    /// Remove the reference of if the Expression owns the data
-    pub fn organize_obj_map(&mut self) {
-        let cols_to_remove = self
-            .dd
-            .data
-            .iter()
-            .filter(|e| e.is_owned())
-            .map(|e| e.name().unwrap())
-            .collect_trusted();
-        self.remove_ref_obj(cols_to_remove);
-    }
+// #[pyfunction]
+// #[pyo3(signature=(dds, inplace=true, context=false))]
+// pub fn eval_dicts(
+//     dds: Vec<&PyAny>,
+//     inplace: bool,
+//     context: bool,
+// ) -> PyResult<Option<Vec<PyDataDict>>> {
+//     let mut dds = dds
+//         .into_iter()
+//         .map(|dd| {
+//             if dd.hasattr("_dd").unwrap() && dd.get_type().name().unwrap() == "DataDict" {
+//                 dd.getattr("_dd").unwrap().extract::<PyDataDict>().unwrap()
+//             } else {
+//                 dd.extract::<PyDataDict>().unwrap()
+//             }
+//         })
+//         .collect_trusted();
+//     dds.par_iter_mut().try_for_each(|dd| dd.eval_all(context))?;
+//     if inplace {
+//         Ok(None)
+//     } else {
+//         Ok(Some(dds))
+//     }
+// }
 
-    pub fn map_expr_to_py(&self, e: Expr<'static>) -> PyExpr {
-        let name = &e.name().unwrap();
-        e.to_py(self.obj_map.get(name).cloned().unwrap_or(None))
-    }
+#[cfg(feature = "map")]
+#[pyfunction]
+#[pyo3(name="where_", signature=(mask, expr, value, par=false))]
+#[allow(clippy::missing_safety_doc, clippy::redundant_clone)]
+pub unsafe fn where_py(mask: &PyAny, expr: &PyAny, value: &PyAny, par: bool) -> PyResult<PyExpr> {
+    let expr = parse_expr_nocopy(expr)?;
+    let mask = parse_expr_nocopy(mask)?;
+    let value = parse_expr_nocopy(value)?;
+    where_(expr.clone(), mask, value, par)
+}
 
-    pub fn get_selector_out_name(&self, cs: ColumnSelector) -> Vec<String> {
-        self.dd.get_selector_out_name(cs)
-    }
+#[cfg(feature = "map")]
+pub fn where_(mut expr: PyExpr, mask: PyExpr, value: PyExpr, par: bool) -> PyResult<PyExpr> {
+    let obj_vec = vec![mask.obj(), value.obj()];
+    expr.e.where_(mask.e, value.e, par);
+    Ok(expr.add_obj_vec_into(obj_vec))
 }
 
-/// Be careful when implement a new method as we should also deal with the reference of the object.
-#[pymethods]
+#[cfg(feature = "create")]
+#[pyfunction]
 #[allow(clippy::missing_safety_doc)]
-impl PyDataDict {
-    #[new]
-    #[pyo3(signature=(data, columns=None, copy=false))]
-    pub fn init(data: &PyAny, columns: Option<Vec<String>>, copy: bool) -> PyResult<Self> {
-        let data = unsafe { parse_expr_list(data, copy)? };
-        let (data, obj_map) = data.into_rs(columns.clone())?;
-        Ok(DataDict::new(data, columns).to_py(obj_map))
-    }
-
-    #[pyo3(name = "is_empty")]
-    pub fn is_empty_py(&self) -> bool {
-        self.is_empty()
-    }
-
-    #[allow(clippy::wrong_self_convention)]
-    #[pyo3(signature=(context=false))]
-    pub fn to_pd(&mut self, context: bool) -> PyResult<PyObject> {
-        self.eval_all(context)?;
-        Python::with_gil(|py| {
-            let pd = PyModule::import(py, "pandas").unwrap(); //.to_object(py)
-            Ok(pd
-                .getattr("DataFrame")?
-                .call1((self.to_dict(context, py)?,))?
-                .into())
-        })
-    }
-
-    fn __traverse__(&self, visit: PyVisit<'_>) -> Result<(), PyTraverseError> {
-        if self.obj_map.is_empty() {
-            return Ok(());
-        }
-        self.obj_map
-            .values()
-            .flatten()
-            .flatten()
-            .try_for_each(|e| visit.call(e))
-    }
-
-    fn __clear__(&mut self) {
-        self.obj_map = Default::default();
-    }
-
-    #[cfg(feature = "agg")]
-    #[pyo3(signature=(method=CorrMethod::Pearson, cols=None, min_periods=3, stable=false))]
-    pub fn corr(
-        &self,
-        method: CorrMethod,
-        cols: Option<&PyAny>,
-        min_periods: usize,
-        stable: bool,
-    ) -> PyExpr {
-        let selector = ColumnSelector::from(cols);
-        let out = self.dd.corr(Some(selector), method, min_periods, stable);
-        out.to_py(None)
-            .add_obj_vec_into(self.obj_map.values().cloned().collect())
-    }
-
-    #[pyo3(signature=(columns))]
-    pub fn drop(&mut self, columns: &PyAny) -> PyResult<()> {
-        let selector: ColumnSelector = columns.into();
-        let drop_cols = self.drop_inplace(selector).map_err(StrError::to_py)?;
-        self.remove_ref_obj(drop_cols);
-        Ok(())
-    }
-
-    pub fn __repr__(&self) -> Cow<'_, str> {
-        Cow::from(format!("{self:#?}"))
-    }
-
-    #[getter]
-    pub fn get_dtypes<'py>(&'py self, py: Python<'py>) -> PyResult<&'py PyDict> {
-        let res = PyDict::new(py);
-        for e in &self.data {
-            res.set_item(e.name().unwrap(), e.dtype())?;
-        }
-        Ok(res)
-    }
-
-    #[allow(clippy::wrong_self_convention)]
-    #[pyo3(signature=(context=false))]
-    pub fn to_dict<'py>(&'py mut self, context: bool, py: Python<'py>) -> PyResult<&'py PyDict> {
-        self.eval_all(context)?;
-        let dict = PyDict::new(py);
-        for expr in &self.data {
-            dict.set_item(expr.name(), expr.clone().to_py(None).value(None, None, py)?)?;
-        }
-        Ok(dict)
-    }
-
-    pub fn __len__(&self) -> usize {
-        self.len()
-    }
-
-    pub fn copy(&self) -> Self {
-        PyDataDict {
-            dd: self.dd.clone(),
-            obj_map: self.obj_map.clone(),
-        }
-    }
-
-    #[getter]
-    pub fn get_len(&self) -> usize {
-        self.len()
-    }
-
-    #[getter]
-    pub fn get_columns(&self) -> Vec<String> {
-        self.dd.columns_owned()
-    }
-
-    #[getter]
-    fn get_map(&self) -> HashMap<String, usize> {
-        (*self.map).clone().into()
-    }
-
-    #[getter]
-    pub fn get_raw_data(&self) -> Vec<PyExpr> {
-        // out data must keep the reference
-        self.data
-            .clone()
-            .into_iter()
-            .map(|e| self.map_expr_to_py(e))
-            .collect_trusted()
-    }
-
-    #[getter]
-    pub fn get_obj_map(&self) -> HashMap<String, RefObj> {
-        self.obj_map.clone()
-    }
-
-    #[setter]
-    pub fn set_columns(&mut self, columns: Vec<String>) {
-        // Be careful when alter the name of the map
-        let ori_columns = self.dd.columns_owned();
-        let new_columns = columns.iter().map(|e| e.as_str()).collect_trusted();
-        for (ori, new) in zip(&ori_columns, new_columns) {
-            self.update_ref_obj_name(ori, new);
-        }
-        self.dd.set_columns(columns)
-    }
-
-    #[pyo3(signature=(context=false))]
-    pub fn eval_all(&mut self, context: bool) -> PyResult<()> {
-        self.eval(None, context)
-    }
-
-    #[pyo3(signature=(cols=None, context=false))]
-    pub fn eval(&mut self, cols: Option<&PyAny>, context: bool) -> PyResult<()> {
-        let cs = ColumnSelector::from(cols);
-        let ori_name = self.get_selector_out_name(cs.clone());
-        let eval_idx = ori_name
-            .iter()
-            .map(|e| {
-                *self
-                    .dd
-                    .map
-                    .get(e)
-                    .unwrap_or_else(|| panic!("Can not find the column: {:?}", e))
-            })
-            .collect_trusted();
-        self.dd.eval_inplace(cs, context).map_err(StrError::to_py)?;
-
-        let new_name = eval_idx
-            .into_iter()
-            .map(|idx| self.dd.data.get(idx).unwrap().name().unwrap())
-            .collect_trusted();
-        for (ori, new) in zip(&ori_name, &new_name) {
-            if self
-                .dd
-                .get(new.as_str().into())
-                .map_err(StrError::to_py)?
-                .into_expr()
-                .unwrap()
-                .is_owned()
-            {
-                self.remove_ref_obj(vec![ori.clone()]);
-            } else {
-                self.update_ref_obj_name(ori, new);
-            }
-        }
-        Ok(())
-    }
-
-    fn __getitem__(&self, ob: &PyAny, py: Python) -> PyResult<PyObject> {
-        let out = self.get(ob.into()).map_err(StrError::to_py)?;
-        match out {
-            GetOutput::Expr(expr) => Ok(self.map_expr_to_py(expr.clone()).into_py(py)),
-            GetOutput::Exprs(exprs) => Ok(exprs
-                .into_iter()
-                .map(|e| self.map_expr_to_py(e.clone()))
-                .collect_trusted()
-                .into_py(py)),
-        }
-    }
-
-    pub unsafe fn __setitem__(&mut self, key: &PyAny, value: &PyAny) -> PyResult<()> {
-        let value = parse_expr_list(value, false)?;
-        let cs = ColumnSelector::from(key);
-        let ori_name = self.get_selector_out_name(cs.clone());
-        if ori_name.len() != value.len() {
-            return Err(StrError("The length of keys and values are not equal".into()).to_py());
-        }
-        let (value, value_obj_map) = value.into_rs(Some(ori_name.clone()))?;
-        self.remove_ref_obj(ori_name);
-        self.set(cs, value.into()).map_err(StrError::to_py)?;
-        self.add_obj_map(value_obj_map);
-        Ok(())
-    }
+#[allow(unreachable_patterns)]
+pub unsafe fn full(shape: &PyAny, value: &PyAny) -> PyResult<PyExpr> {
+    let shape = parse_expr_nocopy(shape)?;
+    let value = parse_expr_nocopy(value)?;
+    let (obj, obj2) = (shape.obj(), value.obj());
+    let out = Expr::full(&shape.e, value.e).to_py(obj);
+    Ok(out.add_obj_into(obj2))
+}
 
-    pub fn __delitem__(&mut self, item: &PyAny) -> PyResult<()> {
-        self.drop(item)
+#[cfg(feature = "create")]
+#[pyfunction]
+#[pyo3(signature=(start, end=None, step=None))]
+#[allow(unreachable_patterns, clippy::missing_safety_doc)]
+pub unsafe fn arange(start: &PyAny, end: Option<&PyAny>, step: Option<f64>) -> PyResult<PyExpr> {
+    let start = parse_expr_nocopy(start)?;
+    let step = step.map(|s| s.into());
+    let obj_start = start.obj();
+    if let Some(end) = end {
+        let end = parse_expr_nocopy(end)?;
+        let obj_end = end.obj();
+        Ok(Expr::arange(Some(start.e), &end.e, step)
+            .to_py(obj_start)
+            .add_obj_into(obj_end))
+    } else {
+        // we only have start argument, this is actually end argument
+        Ok(Expr::arange(None, &start.e, step).to_py(obj_start))
     }
+}
 
-    // pub unsafe fn insert(&mut self, value: &PyAny) -> PyResult<()> {
-    //     let value = parse_expr_list(value, false)?;
-    //     for e in value {
-    //         self.insert_inplace(e.inner).map_err(StrError::to_py)?;
-    //     }
-    //     Ok(())
-    // }
-
-    #[pyo3(name = "select")]
-    pub unsafe fn select_py(&mut self, exprs: &PyAny) -> PyResult<Self> {
-        let exprs = parse_expr_list(exprs, false)?;
-        let (exprs, obj_map) = exprs.into_rs(None)?;
-        Ok(DataDict::new(exprs, None).to_py(obj_map))
-    }
+#[cfg(feature = "time")]
+#[pyfunction]
+pub fn timedelta(rule: &str) -> PyExpr {
+    let e: Expr<'static> = TimeDelta::parse(rule).into();
+    e.into()
+}
 
-    #[pyo3(signature=(exprs))]
-    pub unsafe fn with_columns(&mut self, exprs: &PyAny) -> PyResult<()> {
-        let exprs = parse_expr_list(exprs, false)?;
-        let (exprs, obj_map) = exprs.into_rs(None)?;
-        exprs
-            .into_iter()
-            .try_for_each(|e| self.dd.insert_inplace(e))
-            .map_err(StrError::to_py)?;
-        self.add_obj_map(obj_map);
-        Ok(())
-    }
+#[cfg(feature = "time")]
+#[pyfunction]
+pub fn datetime(s: &str, fmt: &str) -> PyResult<PyExpr> {
+    let e: Expr<'static> = DateTime::parse(s, fmt)
+        .map_err(PyValueError::new_err)?
+        .into();
+    Ok(e.into())
+}
 
-    #[pyo3(signature=(func, exclude=None, **py_kwargs))]
-    pub fn apply(
-        &mut self,
-        func: &PyAny,
-        exclude: Option<Vec<&str>>,
-        py_kwargs: Option<&PyDict>,
-    ) -> PyResult<()> {
-        if self.is_empty() {
-            return Ok(());
-        }
-        let ori_name = self.dd.columns_owned();
-        let out_data = self
-            .dd
-            .data
-            .iter()
-            .map(|e| {
-                if let Some(exclude) = &exclude {
-                    if !exclude.contains(&e.ref_name().unwrap()) {
-                        return parse_expr_nocopy(
-                            func.call((e.clone().to_py(None),), py_kwargs)
-                                .expect("Call python function error!"),
-                        )
-                        .expect("Can not parse function return as Expr");
-                    } else {
-                        e.clone().to_py(None)
-                    }
-                } else {
-                    return parse_expr_nocopy(
-                        func.call((e.clone().to_py(None),), py_kwargs)
-                            .expect("Call python function error!"),
-                    )
-                    .expect("Can not parse function return as Expr");
-                }
-            })
-            .collect_trusted();
-        let new_name = out_data
-            .iter()
-            .map(|e| e.e.name().unwrap())
-            .collect_trusted();
-        for (ori, new) in zip(ori_name, new_name) {
-            if ori != new {
-                self.update_ref_obj_name(ori.as_str(), new.as_str());
-                self.dd.update_column_map(ori, new)?
-            }
-        }
-        let (rs_data, obj_map) = out_data.into_rs(None)?;
-        self.add_obj_map(obj_map);
-        self.dd.data = rs_data;
-        Ok(())
+#[pyfunction]
+#[cfg(feature = "blas")]
+#[allow(clippy::redundant_clone)]
+pub fn get_newey_west_adjust_s(x: PyExpr, resid: PyExpr, lag: PyExpr) -> PyResult<PyExpr> {
+    let obj_vec = [x.obj(), resid.obj(), lag.obj()];
+    let mut out = x.clone();
+    out.e.get_newey_west_adjust_s(resid.e, lag.e);
+    for obj in obj_vec {
+        out.add_obj(obj);
     }
+    Ok(out)
 }
-// #[pyo3(signature=(window, func, axis=0, check=true, **py_kwargs))]
-// #[allow(unreachable_patterns)]
-// pub fn rolling_apply(
-//     &mut self,
-//     window: usize,
-//     func: &PyAny,
-//     axis: i32,
-//     check: bool,
-//     py_kwargs: Option<&PyDict>,
-// ) -> PyResult<Self> {
-//     if self.is_empty() {
-//         return Ok(self.clone());
-//     }
-//     if window == 0 {
-//         return Err(PyValueError::new_err("Window should be greater than 0"));
-//     }
-//     self.eval_all()?;
-//     let axis = match_exprs!(&self.data[0].inner, expr, {
-//         expr.view_arr().norm_axis(axis)
-//     });
-//     let axis_i = axis.index() as i32;
-//     let length = match_exprs!(&self.data[0].inner, expr, {
-//         expr.view_arr().shape()[axis.index()]
-//     });
-//     if check {
-//         for e in &self.data {
-//             let len_ = match_exprs!(&e.inner, expr, { expr.view_arr().shape()[axis.index()] });
-//             if length != len_ {
-//                 return Err(PyValueError::new_err(
-//                     "Each Expressions should have the same length on given axis",
-//                 ));
-//             }
-//         }
-//     }
-//     let mut column_num = 0;
-//     let mut output = zip(repeat(0).take(window - 1), 0..window - 1)
-//         .chain((window - 1..length).enumerate())
-//         .map(|(start, end)| {
-//             let mut step_df = Vec::with_capacity(self.len());
-//             self.data.iter().for_each(|pyexpr| unsafe {
-//                 step_df.push(pyexpr.select_by_slice_eager(Some(axis_i), start, end, None));
-//             });
-//             let step_df = PyDataDict {
-//                 data: step_df,
-//                 column_map: self.column_map.clone(),
-//             };
-//             let res = func
-//                 .call((step_df,), py_kwargs)
-//                 .expect("Call python function error!");
-//             let res = unsafe {
-//                 parse_expr_list(res, false).expect("Can not parse fucntion return as Expr list")
-//             };
-//             column_num = res.len();
-//             res
-//         })
-//         .collect_trusted();
-//     let eval_res: Vec<_> = output
-//         .par_iter_mut()
-//         .flatten()
-//         .map(|e| e.eval_inplace())
-//         .collect();
-//     if eval_res.iter().any(|e| e.is_err()) {
-//         return Err(PyRuntimeError::new_err(
-//             "Some of the expressions can't be evaluated",
-//         ));
-//     }
 
-//     let out_data = (0..column_num)
-//         .into_par_iter()
-//         .map(|i| {
-//             let group_vec = output
-//                 .iter()
-//                 .map(|single_output_exprs| single_output_exprs.get(i).unwrap().no_dim0())
-//                 .collect_trusted();
-//             concat_expr(group_vec, axis_i).expect("Concat expr error")
-//         })
-//         .collect();
-//     Ok(PyDataDict::new(out_data, None))
-// }
-
-// #[pyo3(signature=(duration, func, index=None, axis=0, check=true, **py_kwargs))]
-// #[allow(unreachable_patterns)]
-// pub fn rolling_apply_by_time(
-//     &mut self,
-//     duration: &str,
-//     func: &PyAny,
-//     index: Option<&str>,
-//     axis: i32,
-//     check: bool,
-//     py_kwargs: Option<&PyDict>,
-// ) -> PyResult<Self> {
-//     if self.is_empty() {
-//         return Ok(self.clone());
-//     }
-//     self.eval_all()?;
-//     let index = if let Some(index) = index {
-//         self.get_by_str(index)
-//     } else {
-//         let mut dt_num = 0; // number of datetime expression in datadict
-//         let mut out = None;
-//         for expr in &self.data {
-//             if expr.dtype() == "DateTime" {
-//                 out = Some(expr);
-//                 dt_num += 1;
-//             }
-//         }
-//         if dt_num != 1 {
-//             return Err(PyValueError::new_err(
-//                 "The Number of DateTime Expression in DataDict should be 1",
-//             ));
-//         } else {
-//             out.unwrap()
-//         }
-//     };
-//     let axis = match_exprs!(&self.data[0].inner, expr, {
-//         expr.view_arr().norm_axis(axis)
-//     });
-//     let axis_i = axis.index() as i32;
-//     let length = match_exprs!(&self.data[0].inner, expr, {
-//         expr.view_arr().shape()[axis.index()]
-//     });
-//     if check {
-//         for e in &self.data {
-//             let len_ = match_exprs!(&e.inner, expr, { expr.view_arr().shape()[axis.index()] });
-//             if length != len_ {
-//                 return Err(PyValueError::new_err(
-//                     "Each Expressions should have the same length on given axis",
-//                 ));
-//             }
-//         }
-//     }
-//     let mut rolling_idx = index
-//         .clone()
-//         .cast_datetime(None)?
-//         .get_time_rolling_idx(duration, tears::RollingTimeStartBy::Full);
-//     rolling_idx.eval_inplace()?;
-//     let mut column_num = 0;
-//     let mut output = rolling_idx
-//         .view_arr()
-//         .to_dim1()
-//         .unwrap()
-//         .into_iter()
-//         .enumerate()
-//         .map(|(end, start)| {
-//             let mut step_df = Vec::with_capacity(self.len());
-//             self.data.iter().for_each(|pyexpr| unsafe {
-//                 step_df.push(pyexpr.select_by_slice_eager(Some(axis_i), start, end, None));
-//             });
-//             let step_df = PyDataDict {
-//                 data: step_df,
-//                 column_map: self.column_map.clone(),
-//             };
-//             let res = func
-//                 .call((step_df,), py_kwargs)
-//                 .expect("Call python function error!");
-//             let res = unsafe {
-//                 parse_expr_list(res, false).expect("Can not parse fucntion return as Expr list")
-//             };
-//             column_num = res.len();
-//             res
-//         })
-//         .collect_trusted();
-//     let eval_res: Vec<_> = output
-//         .par_iter_mut()
-//         .flatten()
-//         .map(|e| e.eval_inplace())
-//         .collect();
-//     if eval_res.iter().any(|e| e.is_err()) {
-//         return Err(PyRuntimeError::new_err(
-//             "Some of the expressions can't be evaluated",
-//         ));
+// #[pyfunction]
+// pub fn from_dataframe(df: &PyAny) -> PyResult<PyDataDict> {
+//     let columns = df.getattr("columns")?.extract::<Vec<String>>()?;
+//     let mut data = Vec::with_capacity(columns.len());
+//     for col in &columns {
+//         data.push(parse_expr_nocopy(df.get_item(col)?)?);
 //     }
-//     let out_data = (0..column_num)
-//         .into_par_iter()
-//         .map(|i| {
-//             let group_vec = output
-//                 .iter()
-//                 .map(|single_output_exprs| single_output_exprs.get(i).unwrap().no_dim0())
-//                 .collect_trusted();
-//             concat_expr(group_vec, axis_i).expect("Concat expr error")
-//         })
-//         .collect();
-//     Ok(PyDataDict::new(out_data, None))
+//     let (data, obj_map) = data.into_rs(Some(columns.clone()))?;
+//     Ok(DataDict::new(data, Some(columns)).to_py(obj_map))
 // }
 
-// fn parse_one_or_more_str(s: &PyAny) -> PyResult<Vec<&str>> {
-//     if let Ok(s) = s.extract::<&str>() {
-//         Ok(vec![s])
-//     } else if let Ok(s) = s.extract::<Vec<&str>>() {
-//         Ok(s)
-//     } else {
-//         Err(PyValueError::new_err(
-//             "the param cann't be parsed as a vector of string",
-//         ))
-//     }
+#[pyfunction]
+pub fn context<'py>(s: Option<&'py PyAny>) -> PyResult<PyExpr> {
+    let s: ColumnSelector<'py> = s.into();
+    let name = s.name();
+    let a: Data = s.into();
+    // safety: this function is using in python
+    let mut e = unsafe { std::mem::transmute::<Expr<'_>, Expr<'static>>(a.into()) };
+    e.set_name(name);
+    Ok(e.to_py(None))
+}
+
+// #[cfg(all(feature = "arw", feature = "io"))]
+// #[pyfunction]
+// pub fn read_ipc(path: &str, columns: PyColSelect) -> PyResult<PyDataDict> {
+//     let dd = DataDict::read_ipc(path, columns.0).map_err(StrError::to_py)?;
+//     Ok(PyDataDict {
+//         dd,
+//         obj_map: Default::default(),
+//     })
 // }
+
+#[cfg(all(feature = "arw", feature = "io"))]
+#[pyfunction]
+pub fn scan_ipc(path: String, columns: PyColSelect) -> PyResult<Vec<PyExpr>> {
+    use tea_io::scan_ipc_lazy;
+    let out: Vec<PyExpr> = scan_ipc_lazy(path, columns.0)
+        .map_err(StrError::to_py)?
+        .into_iter()
+        .map(|e| e.into())
+        .collect();
+    Ok(out)
+    // let dd = DataDict::scan_ipc(path, columns.0).map_err(StrError::to_py)?;
+    // Ok(PyDataDict {
+    //     dd,
+    //     obj_map: Default::default(),
+    // })
+}
```

### Comparing `teapy-0.6.9/src/pylazy/groupby.rs` & `teapy-0.7.0/tea-py/src/pylazy/groupby.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/src/pylazy/impl_pyexpr.rs` & `teapy-0.7.0/tea-py/src/pylazy/impl_pyexpr.rs`

 * *Files 0% similar despite different names*

```diff
@@ -228,34 +228,40 @@
             Ok(None)
         }
     }
 
     #[pyo3(signature=(context=None))]
     // #[cfg(feature = "time")]
     pub fn view_in(
-        slf: PyRefMut<'_, Self>,
-        context: Option<&PyAny>,
+        // slf: PyRefMut<'_, Self>,
+        slf: Bound<'_, PyExpr>,
+        context: Option<&Bound<'_, PyAny>>,
         py: Python,
     ) -> PyResult<PyObject> {
         let ct: PyContext<'static> = if let Some(context) = context {
             unsafe { std::mem::transmute(context.extract::<PyContext>()?) }
         } else {
             Default::default()
         };
         let (ct_rs, _obj_map) = (ct.ct, ct.obj_map);
-        let data = slf.e.view_data(ct_rs.as_ref()).map_err(StrError::to_py)?;
-        let container = unsafe { PyAny::from_borrowed_ptr(py, slf.as_ptr()) };
+        let slf_ref = slf.borrow();
+        let data = slf_ref
+            .e
+            .view_data(ct_rs.as_ref())
+            .map_err(StrError::to_py)?;
+        let container = slf.into_any();
         if matches!(&data, Data::ArrVec(_)) {
             if let Data::ArrVec(arr_vec) = data {
                 let out = arr_vec
                     .iter()
                     .map(|arr| {
                         match_arrok!(pyelement arr, a, {
                             unsafe{
-                                PyArray::borrow_from_array(&a.view().0, container)
+                                // PyArray::borrow_from_array(&a.view().0, container)
+                                PyArray::borrow_from_array_bound(&a.view().0, container.clone())
                                 .no_dim0(py)
                                 .unwrap()
                             }
                         })
                     })
                     .collect_trusted();
                 return Ok(out.into_py(py));
@@ -268,41 +274,40 @@
                 a,
                 { a.view().to_object(py) },
                 Str,
                 String,
                 #[cfg(feature = "time")]
                 TimeDelta
             );
-            return PyArray::from_owned_array(py, arr.0).no_dim0(py);
+            return PyArray::from_owned_array_bound(py, arr.0).no_dim0(py);
         }
         #[cfg(feature = "time")]
         if let ArrOk::DateTime(arr) = arr {
             let arr = arr
                 .view()
                 .map(|v| v.into_np_datetime::<numpy::datetime::units::Microseconds>());
-            return PyArray::from_owned_array(py, arr.0).no_dim0(py);
+            return PyArray::from_owned_array_bound(py, arr.0).no_dim0(py);
         }
         match_arrok!(
             pyelement arr,
             a,
             {
                 unsafe {
-                    Ok(PyArray::borrow_from_array(
+                    Ok(PyArray::borrow_from_array_bound(
                         &a.view().0,
                         container,
                     )
                     .no_dim0(py)?)
                 }
             }
         )
     }
 
     #[getter]
-    pub fn get_view(slf: PyRefMut<'_, Self>, py: Python) -> PyResult<PyObject> {
-        // slf.view_in(None, py)
+    pub fn get_view(slf: Bound<'_, Self>, py: Python) -> PyResult<PyObject> {
         PyExpr::view_in(slf, None, py)
     }
 
     // #[allow(unreachable_patterns)]
     // #[pyo3(signature=(context=None))]
     // /// eval and view, used for fast test
     // pub fn eview(
@@ -316,15 +321,15 @@
 
     #[allow(unreachable_patterns)]
     #[pyo3(signature=(unit=None, context=None))]
     // #[cfg(feature = "time")]
     pub fn value<'py>(
         &'py mut self,
         unit: Option<&'py str>,
-        context: Option<&'py PyAny>,
+        context: Option<&Bound<'py, PyAny>>,
         py: Python<'py>,
     ) -> PyResult<PyObject> {
         let ct: PyContext<'static> = if let Some(context) = context {
             unsafe { std::mem::transmute(context.extract::<PyContext>()?) }
         } else {
             Default::default()
         };
@@ -334,15 +339,15 @@
         if matches!(&data, Data::ArrVec(_)) {
             if let Data::ArrVec(_) = data {
                 let arr_vec = data.view_arr_vec(ct_rs.as_ref()).map_err(StrError::to_py)?;
                 let out = arr_vec
                     .into_iter()
                     .map(|arr| {
                         match_arrok!(pyelement arr, a, {
-                            PyArray::from_owned_array(py, a.view().to_owned().0)
+                            PyArray::from_owned_array_bound(py, a.view().to_owned().0)
                             .no_dim0(py)
                             .unwrap()
                         })
                     })
                     .collect_trusted();
                 return Ok(out.into_py(py));
             }
@@ -354,45 +359,45 @@
                 a,
                 { a.view().to_object(py) },
                 Str,
                 String,
                 #[cfg(feature = "time")]
                 TimeDelta
             );
-            return PyArray::from_owned_array(py, arr.0).no_dim0(py);
+            return PyArray::from_owned_array_bound(py, arr.0).no_dim0(py);
         }
         #[cfg(feature = "time")]
         if let ArrOk::DateTime(arr) = &arr {
             match unit.unwrap_or("us").to_lowercase().as_str() {
                 "ms" => {
                     let arr = arr
                         .view()
                         .map(|v| v.into_np_datetime::<numpy::datetime::units::Milliseconds>());
-                    return PyArray::from_owned_array(py, arr.0).no_dim0(py);
+                    return PyArray::from_owned_array_bound(py, arr.0).no_dim0(py);
                 }
                 "us" => {
                     let arr = arr
                         .view()
                         .map(|v| v.into_np_datetime::<numpy::datetime::units::Microseconds>());
-                    return PyArray::from_owned_array(py, arr.0).no_dim0(py);
+                    return PyArray::from_owned_array_bound(py, arr.0).no_dim0(py);
                 }
                 "ns" => {
                     let arr = arr
                         .view()
                         .map(|v| v.into_np_datetime::<numpy::datetime::units::Nanoseconds>());
-                    return PyArray::from_owned_array(py, arr.0).no_dim0(py);
+                    return PyArray::from_owned_array_bound(py, arr.0).no_dim0(py);
                 }
                 _ => unimplemented!("not support datetime unit"),
             }
         }
         match_arrok!(
             pyelement arr,
             a,
             {
-                Ok(PyArray::from_owned_array(
+                Ok(PyArray::from_owned_array_bound(
                     py,
                     a.view().to_owned().0
                 )
                 .no_dim0(py)?)
             }
         )
     }
@@ -430,25 +435,25 @@
         let obj = shape.obj();
         let mut out = self.clone();
         out.e.reshape(shape.e);
         Ok(out.add_obj_into(obj))
     }
 
     pub fn __getattr__<'py>(
-        slc: PyRef<'py, Self>,
+        slf: PyRef<'py, Self>,
         attr: &'py str,
         py: Python<'py>,
     ) -> PyResult<&'py PyAny> {
         let attr_dict = PYEXPR_ATTRIBUTE.lock();
         let res = attr_dict.get(attr);
         if let Some(res) = res {
             let func = res.clone();
             let functools = py.import("functools")?;
             let partial = functools.getattr("partial")?;
-            partial.call1((func, slc))
+            partial.call1((func, slf))
         } else {
             Err(PyAttributeError::new_err(format!(
                 "'PyExpr' object has no attribute {attr}"
             )))
         }
     }
 
@@ -1928,14 +1933,28 @@
     ) -> Self {
         let mut out = self.clone();
         out.e.ts_reg_slope(window, min_periods, stable, axis, par);
         out
     }
 
     #[cfg(feature = "rolling")]
+    #[pyo3(signature=(window, min_periods=1, axis=0, par=false))]
+    pub fn ts_reg_resid_mean(
+        &self,
+        window: usize,
+        min_periods: usize,
+        axis: i32,
+        par: bool,
+    ) -> Self {
+        let mut out = self.clone();
+        out.e.ts_reg_resid_mean(window, min_periods, axis, par);
+        out
+    }
+
+    #[cfg(feature = "rolling")]
     #[pyo3(signature=(window, min_periods=1, stable=false, axis=0, par=false))]
     pub fn ts_reg_intercept(
         &self,
         window: usize,
         min_periods: usize,
         stable: bool,
         axis: i32,
@@ -2036,15 +2055,15 @@
         }
     }
 
     pub fn cast(&self, ty: &PyAny, py: Python) -> PyResult<Self> {
         if let Ok(ty_name) = ty.extract::<&str>() {
             self.cast_by_str(ty_name, py)
         } else if let Ok(py_type) = ty.extract::<&pyo3::types::PyType>() {
-            self.cast_by_str(py_type.name().unwrap(), py)
+            self.cast_by_str(&py_type.name().unwrap(), py)
         } else {
             unimplemented!("Incorrect type for casting")
         }
     }
 
     #[cfg(all(feature = "map", feature = "agg"))]
     #[pyo3(signature=(mask, value, axis=0, par=false, inplace=false))]
```

### Comparing `teapy-0.6.9/src/pylazy/mod.rs` & `teapy-0.7.0/tea-py/src/pylazy/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,48 +1,50 @@
-mod datadict;
+// mod datadict;
 mod export;
 // mod groupby;
 mod impl_pyexpr;
 mod pyexpr;
 mod pyfunc;
 
-pub use datadict::PyDataDict;
+// pub use datadict::PyDataDict;
 pub use impl_pyexpr::expr_register;
 pub use pyexpr::{ExprToPy, IntoPyExpr};
 pub use pyexpr::{PyExpr, RefObj};
 pub use pyfunc::*;
 
 use pyo3::prelude::{wrap_pyfunction, PyModule, PyResult};
 
 pub(crate) fn add_lazy(m: &PyModule) -> PyResult<()> {
     m.add_class::<PyExpr>()?;
-    m.add_class::<PyDataDict>()?;
+    // m.add_class::<PyDataDict>()?;
     // m.add_class::<PyGroupBy>()?;
     m.add_function(wrap_pyfunction!(expr_register, m)?)?;
     #[cfg(all(feature = "concat", feature = "map"))]
     m.add_function(wrap_pyfunction!(concat_expr_py, m)?)?;
     #[cfg(all(feature = "concat", feature = "map"))]
     m.add_function(wrap_pyfunction!(stack_expr_py, m)?)?;
     m.add_function(wrap_pyfunction!(eval_exprs, m)?)?;
-    m.add_function(wrap_pyfunction!(eval_dicts, m)?)?;
+    // m.add_function(wrap_pyfunction!(eval_dicts, m)?)?;
+    #[cfg(feature = "agg")]
+    m.add_function(wrap_pyfunction!(corr_py, m)?)?;
     #[cfg(feature = "map")]
     m.add_function(wrap_pyfunction!(where_py, m)?)?;
     #[cfg(feature = "create")]
     m.add_function(wrap_pyfunction!(full, m)?)?;
     #[cfg(feature = "create")]
     m.add_function(wrap_pyfunction!(arange, m)?)?;
     #[cfg(feature = "time")]
     m.add_function(wrap_pyfunction!(datetime, m)?)?;
     #[cfg(feature = "time")]
     m.add_function(wrap_pyfunction!(timedelta, m)?)?;
-    m.add_function(wrap_pyfunction!(from_dataframe, m)?)?;
+    // m.add_function(wrap_pyfunction!(from_dataframe, m)?)?;
     #[cfg(feature = "blas")]
     m.add_function(wrap_pyfunction!(get_newey_west_adjust_s, m)?)?;
     m.add_function(wrap_pyfunction!(parse_expr, m)?)?;
     m.add_function(wrap_pyfunction!(parse_expr_list, m)?)?;
     m.add_function(wrap_pyfunction!(context, m)?)?;
-    #[cfg(all(feature = "arw", feature = "io"))]
-    m.add_function(wrap_pyfunction!(read_ipc, m)?)?;
+    // #[cfg(all(feature = "arw", feature = "io"))]
+    // m.add_function(wrap_pyfunction!(read_ipc, m)?)?;
     #[cfg(all(feature = "arw", feature = "io"))]
     m.add_function(wrap_pyfunction!(scan_ipc, m)?)?;
     Ok(())
 }
```

### Comparing `teapy-0.6.9/src/pylazy/pyexpr.rs` & `teapy-0.7.0/tea-py/src/pylazy/pyexpr.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.6.9/Cargo.lock` & `teapy-0.7.0/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -19,17 +19,17 @@
  "once_cell",
  "version_check",
  "zerocopy",
 ]
 
 [[package]]
 name = "aho-corasick"
-version = "1.1.2"
+version = "1.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b2969dcb958b36655471fc61f7e416fa76033bdd4bfed0678d8fee1e2d07a1f0"
+checksum = "8e60d3430d3a69478ad0993f19238d2df97c507009a52b3c10addcd7f6bcb916"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "android-tzdata"
 version = "0.1.1"
@@ -43,17 +43,17 @@
 checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "anyhow"
-version = "1.0.80"
+version = "1.0.81"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5ad32ce52e4161730f7098c077cd2ed6229b5804ccf99e5366be1ab72a98b4e1"
+checksum = "0952808a6c2afd1aa8947271f3a60f1a6763c7b912d210184c5149b5cf147247"
 
 [[package]]
 name = "approx"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cab112f0a86d568ea0e627cc1d6be74a1e9cd55214684db5561995f6dad897c6"
 dependencies = [
@@ -98,17 +98,17 @@
  "rustc_version",
  "simdutf8",
  "zstd",
 ]
 
 [[package]]
 name = "autocfg"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
+checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
 
 [[package]]
 name = "base16ct"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "349a06037c7bf932dd7e7d1f653678b2038b9ad46a74102f1fc7bd7872678cce"
 
@@ -121,24 +121,30 @@
 [[package]]
 name = "base64"
 version = "0.21.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9d297deb1925b89f2ccc13d7635fa0714f12c87adce1c75356b39ca9b7178567"
 
 [[package]]
+name = "base64"
+version = "0.22.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9475866fec1451be56a3c2400fd081ff546538961565ccb5b7142cbd22bc7a51"
+
+[[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bitflags"
-version = "2.4.2"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ed570934406eb16438a4e976b1b4500774099c13b8cb96eec99f620f05090ddf"
+checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
 [[package]]
 name = "block-buffer"
 version = "0.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3078c7629b62d3f0439517fa394996acacc5cbc91c5a20d8c658e77abd503a71"
 dependencies = [
@@ -149,62 +155,62 @@
 name = "bumpalo"
 version = "3.15.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7ff69b9dd49fd426c69a0db9fc04dd934cdb6645ff000864d98f7e2af8830eaa"
 
 [[package]]
 name = "bytemuck"
-version = "1.14.3"
+version = "1.15.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a2ef034f05691a48569bd920a96c81b9d91bbad1ab5ac7c4616c1f6ef36cb79f"
+checksum = "5d6d68c57235a3a081186990eca2867354726650f42f7516ca50c28d6281fd15"
 dependencies = [
  "bytemuck_derive",
 ]
 
 [[package]]
 name = "bytemuck_derive"
-version = "1.5.0"
+version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "965ab7eb5f8f97d2a083c799f3a1b994fc397b2fe2da5d1da1626ce15a39f2b1"
+checksum = "4da9a32f3fed317401fa3c862968128267c3106685286e15d5aaa3d7389c2f60"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "cblas-sys"
 version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b6feecd82cce51b0204cf063f0041d69f24ce83f680d87514b004248e7b0fa65"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "cc"
-version = "1.0.90"
+version = "1.0.91"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8cd6604a82acf3039f1144f54b8eb34e91ffba622051189e71b781822d5ee1f5"
+checksum = "1fd97381a8cc6493395a5afc4c691c1084b3768db713b73aa215217aa245d153"
 dependencies = [
  "jobserver",
  "libc",
 ]
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chrono"
-version = "0.4.35"
+version = "0.4.37"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8eaf5903dcbc0a39312feb77df2ff4c76387d591b9fc7b04a238dcf8bb62639a"
+checksum = "8a0d04d43504c61aa6c7531f1871dd0d418d91130162063b789da00fd7057a5e"
 dependencies = [
  "android-tzdata",
  "iana-time-zone",
  "js-sys",
  "num-traits",
  "serde",
  "wasm-bindgen",
@@ -411,17 +417,17 @@
 name = "ethnum"
 version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b90ca2580b73ab6a1f724b76ca11ab632df820fd6040c336200d2c1df7b3c82c"
 
 [[package]]
 name = "fastrand"
-version = "2.0.1"
+version = "2.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "25cbce373ec4653f1a01a31e8a5e5ec0c622dc27ff9c4e6606eefef5cbbed4a5"
+checksum = "658bd65b1cf4c852a3cc96f18a8ce7b5640f6b703f905c7d74532294c2a63984"
 
 [[package]]
 name = "filetime"
 version = "0.2.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1ee447700ac8aa0b2f2bd7bc4462ad686ba06baa6727ac149a2d6277f0d240fd"
 dependencies = [
@@ -485,17 +491,17 @@
 dependencies = [
  "typenum",
  "version_check",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.12"
+version = "0.2.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "190092ea657667030ac6a35e305e62fc4dd69fd98ac98631e5d3a2b1575a12b5"
+checksum = "a06fddc2749e0528d2813f95e050e87e52c8cbbae56223b9babf73b3e53b0cc6"
 dependencies = [
  "cfg-if",
  "js-sys",
  "libc",
  "wasi",
  "wasm-bindgen",
 ]
@@ -579,17 +585,17 @@
 dependencies = [
  "unicode-bidi",
  "unicode-normalization",
 ]
 
 [[package]]
 name = "indoc"
-version = "2.0.4"
+version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1e186cfbae8084e513daff4240b4797e342f988cecda4fb6c939150f96315fd8"
+checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
 name = "intel-mkl-src"
 version = "0.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2ee70586cd5b3e772a8739a1bd43eaa90d4f4bf0fb2a4edc202e979937ee7f5e"
 dependencies = [
@@ -607,17 +613,17 @@
  "anyhow",
  "log",
  "walkdir",
 ]
 
 [[package]]
 name = "itoa"
-version = "1.0.10"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1a46d1a171d865aa5f83f92695765caa047a9b4cbae2cbf37dbd613a793fd4c"
+checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
 
 [[package]]
 name = "jobserver"
 version = "0.1.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ab46a6e9526ddef3ae7f787c06f0f2600639ba80ea3eade3d8e670a2230f51d6"
 dependencies = [
@@ -658,21 +664,20 @@
 name = "libm"
 version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4ec2a862134d2a7d32d7983ddcdd1c4923530833c9f2ea1a44fc5fa473989058"
 
 [[package]]
 name = "libredox"
-version = "0.0.1"
+version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "85c833ca1e66078851dba29046874e38f08b2c883700aa29a03ddd3b23814ee8"
+checksum = "c0ff37bd590ca25063e35af745c343cb7a0271906fb7b37e4813e8f79f00268d"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "libc",
- "redox_syscall",
 ]
 
 [[package]]
 name = "linux-raw-sys"
 version = "0.4.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "01cda141df6706de531b6c46c3a33ecca755538219bd484262fa09410c13539c"
@@ -721,32 +726,32 @@
 dependencies = [
  "autocfg",
  "rawpointer",
 ]
 
 [[package]]
 name = "memchr"
-version = "2.7.1"
+version = "2.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "523dc4f511e55ab87b694dc30d0f820d60906ef06413f93d4d7a1385599cc149"
+checksum = "6c8640c5d730cb13ebd907d8d04b52f55ac9a2eec55b440c8892f40d56c76c1d"
 
 [[package]]
 name = "memmap2"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fe751422e4a8caa417e13c3ea66452215d7d63e19e604f4980461212f3ae1322"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "memoffset"
-version = "0.9.0"
+version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
+checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "miniz_oxide"
 version = "0.7.2"
@@ -894,17 +899,17 @@
 dependencies = [
  "autocfg",
  "libm",
 ]
 
 [[package]]
 name = "numpy"
-version = "0.20.0"
+version = "0.21.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bef41cbb417ea83b30525259e30ccef6af39b31c240bda578889494c5392d331"
+checksum = "ec170733ca37175f5d75a5bea5911d6ff45d2cd52849ce98b685394e4f2f37f4"
 dependencies = [
  "libc",
  "ndarray",
  "num-complex",
  "num-integer",
  "num-traits",
  "pyo3",
@@ -985,15 +990,15 @@
 
 [[package]]
 name = "openssl"
 version = "0.10.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95a0481286a310808298130d22dd1fef0fa571e05a8f44ec801801e84b216b1f"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "cfg-if",
  "foreign-types",
  "libc",
  "once_cell",
  "openssl-macros",
  "openssl-sys",
 ]
@@ -1002,28 +1007,28 @@
 name = "openssl-macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a948666b637a0f465e8564c73e89d4dde00d72d4d473cc972f390fc3dcee7d9c"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "openssl-probe"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ff011a302c396a5197692431fc1948019154afc178baf7d8e37367442a4601cf"
 
 [[package]]
 name = "openssl-sys"
-version = "0.9.101"
+version = "0.9.102"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dda2b0f344e78efc2facf7d195d098df0dd72151b26ab98da807afc26c198dff"
+checksum = "c597637d56fbc83893a35eb0dd04b2b8e7a50c91e64e9493e398b5df4fb45fa2"
 dependencies = [
  "cc",
  "libc",
  "pkg-config",
  "vcpkg",
 ]
 
@@ -1111,26 +1116,26 @@
  "proc-macro2",
  "quote",
  "version_check",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.78"
+version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e2422ad645d89c99f8f3e6b88a9fdeca7fabeac836b1002371c4367c8f984aae"
+checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.20.3"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "53bdbb96d49157e65d45cc287af5f32ffadd5f4761438b527b055fb0d4bb8233"
+checksum = "a7a8b1990bd018761768d5e608a13df8bd1ac5f678456e0f301bb93e5f3ea16b"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "portable-atomic",
@@ -1139,55 +1144,55 @@
  "pyo3-macros",
  "serde",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.20.3"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "deaa5745de3f5231ce10517a1f5dd97d53e5a2fd77aa6b5842292085831d48d7"
+checksum = "650dca34d463b6cdbdb02b1d71bfd6eb6b6816afc708faebb3bac1380ff4aef7"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.20.3"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "62b42531d03e08d4ef1f6e85a2ed422eb678b8cd62b762e53891c05faf0d4afa"
+checksum = "09a7da8fc04a8a2084909b59f29e1b8474decac98b951d77b80b26dc45f046ad"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.20.3"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7305c720fa01b8055ec95e484a6eca7a83c841267f0dd5280f0c8b8551d2c158"
+checksum = "4b8a199fce11ebb28e3569387228836ea98110e43a804a530a9fd83ade36d513"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.20.3"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7c7e9b68bb9c3149c5b0cade5d07f953d6d125eb4337723c4ccdb665f1f96185"
+checksum = "93fbbfd7eb553d10036513cb122b888dcd362a945a00b06c165f2ab480d4cc3b"
 dependencies = [
  "heck",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "quote"
 version = "1.0.35"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
@@ -1239,17 +1244,17 @@
 name = "rawpointer"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "60a357793950651c4ed0f3f52338f53b2f809f32d83a07f72909fa13e4c6c1e3"
 
 [[package]]
 name = "rayon"
-version = "1.9.0"
+version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e4963ed1bc86e4f3ee217022bd855b297cef07fb9eac5dfa1f788b220b49b3bd"
+checksum = "b418a60154510ca1a002a752ca9714984e21e4241e804d32555251faf8b78ffa"
 dependencies = [
  "either",
  "rayon-core",
 ]
 
 [[package]]
 name = "rayon-core"
@@ -1268,28 +1273,28 @@
 checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
  "bitflags 1.3.2",
 ]
 
 [[package]]
 name = "redox_users"
-version = "0.4.4"
+version = "0.4.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a18479200779601e498ada4e8c1e1f50e3ee19deb0259c25825a98b5603b2cb4"
+checksum = "bd283d9651eeda4b2a83a43c1c91b266c40fd76ecd39a50a8c630ae69dc72891"
 dependencies = [
  "getrandom",
  "libredox",
  "thiserror",
 ]
 
 [[package]]
 name = "regex"
-version = "1.10.3"
+version = "1.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b62dbe01f0b06f9d8dc7d49e05a0785f153b00b2c227856282f671e0318c9b15"
+checksum = "c117dbdfde9c8308975b6a18d71f3f385c89461f7b3fb054288ecf2a2058ba4c"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-automata",
  "regex-syntax",
 ]
 
@@ -1302,17 +1307,17 @@
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.8.2"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c08c74e62047bb2de4ff487b251e4a92e24f48745648451635cec7d591162d9f"
+checksum = "adad44e29e4c806119491a7f06f03de4d1af22c3a680dd47f1e6e179439d1f56"
 
 [[package]]
 name = "ring"
 version = "0.17.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c17fa4cb658e3583423e915b9f3acc01cceaee1860e33d59ebae66adc3a2dc0d"
 dependencies = [
@@ -1338,30 +1343,30 @@
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
  "semver",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.38.31"
+version = "0.38.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6ea3e1a662af26cd7a3ba09c0297a31af215563ecf42817c98df621387f4e949"
+checksum = "65e04861e65f21776e67888bfbea442b3642beaa0138fdb1dd7a84a52dffdb89"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "errno",
  "libc",
  "linux-raw-sys",
  "windows-sys",
 ]
 
 [[package]]
 name = "rustls"
-version = "0.22.2"
+version = "0.22.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e87c9956bd9807afa1f77e0f7594af32566e830e088a5576d27c5b6f30f49d41"
+checksum = "99008d7ad0bbbea527ec27bddbc0e432c5b87d8175178cee68d2eec9c4a1813c"
 dependencies = [
  "log",
  "ring",
  "rustls-pki-types",
  "rustls-webpki",
  "subtle",
  "zeroize",
@@ -1378,27 +1383,27 @@
  "rustls-pki-types",
  "schannel",
  "security-framework",
 ]
 
 [[package]]
 name = "rustls-pemfile"
-version = "2.1.1"
+version = "2.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f48172685e6ff52a556baa527774f61fcaa884f59daf3375c62a3f1cd2549dab"
+checksum = "29993a25686778eb88d4189742cd713c9bce943bc54251a33509dc63cbacf73d"
 dependencies = [
- "base64 0.21.7",
+ "base64 0.22.0",
  "rustls-pki-types",
 ]
 
 [[package]]
 name = "rustls-pki-types"
-version = "1.3.1"
+version = "1.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5ede67b28608b4c60685c7d54122d4400d90f62b40caee7700e700380a390fa8"
+checksum = "ecd36cc4259e3e4514335c4a138c6b43171a8d61d8f5c9348f9fc7529416f247"
 
 [[package]]
 name = "rustls-webpki"
 version = "0.102.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "faaa0a62740bedb9b2ef5afa303da42764c012f743917351dc9a237ea1663610"
 dependencies = [
@@ -1444,30 +1449,30 @@
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "security-framework"
-version = "2.9.2"
+version = "2.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "05b64fb303737d99b81884b2c63433e9ae28abebe5eb5045dcdd175dc2ecf4de"
+checksum = "770452e37cad93e0a50d5abc3990d2bc351c36d0328f86cefec2f2fb206eaef6"
 dependencies = [
  "bitflags 1.3.2",
  "core-foundation",
  "core-foundation-sys",
  "libc",
  "security-framework-sys",
 ]
 
 [[package]]
 name = "security-framework-sys"
-version = "2.9.1"
+version = "2.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e932934257d3b408ed8f30db49d85ea163bfe74961f017f405b025af298f0c7a"
+checksum = "41f3cc463c0ef97e11c3461a9d3787412d30e8e7eb907c79180c4a57bf7c04ef"
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "semver"
@@ -1488,22 +1493,22 @@
 name = "serde_derive"
 version = "1.0.197"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.114"
+version = "1.0.115"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c5f09b1bd632ef549eaa9f60a1f8de742bdbc698e6cee2095fc84dde5f549ae0"
+checksum = "12dc5c46daa8e9fdf4f5e71b6cf9a53f2487da0e86e55808e2d35539666497dd"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -1534,17 +1539,17 @@
 name = "simdutf8"
 version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f27f6278552951f1f2b8cf9da965d10969b2efdea95a6ec47987ab46edfe263a"
 
 [[package]]
 name = "smallvec"
-version = "1.13.1"
+version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e6ecd384b10a64542d77071bd64bd7b231f4ed5940fba55e98c3de13824cf3d7"
+checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "spin"
 version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6980e8d7511241f8acf4aebddbb1ff938df5eebe98691418c4468d0b72a96a67"
 
@@ -1582,17 +1587,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.52"
+version = "2.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b699d15b36d1f02c3e7c69f8ffef53de37aefae075d8488d4ba1a7788d574a07"
+checksum = "44cfb93f38070beee36b3fef7d4f5a16f27751d94b187b666a5cc5e9b0d30687"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -1610,15 +1615,15 @@
 name = "target-lexicon"
 version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
 name = "tea-core"
-version = "0.6.9"
+version = "0.7.0"
 dependencies = [
  "arrow2",
  "intel-mkl-src",
  "lapack-sys",
  "libc",
  "ndarray",
  "num",
@@ -1628,36 +1633,36 @@
  "tea-dtype",
  "tea-error",
  "tea-utils",
 ]
 
 [[package]]
 name = "tea-dtype"
-version = "0.6.9"
+version = "0.7.0"
 dependencies = [
  "ndarray",
  "num",
  "numpy",
  "pyo3",
  "serde",
  "tea-time",
  "tea-utils",
 ]
 
 [[package]]
 name = "tea-error"
-version = "0.6.9"
+version = "0.7.0"
 dependencies = [
  "arrow2",
  "pyo3",
 ]
 
 [[package]]
 name = "tea-ext"
-version = "0.6.9"
+version = "0.7.0"
 dependencies = [
  "ndarray",
  "num",
  "paste",
  "pyo3",
  "rayon",
  "statrs",
@@ -1665,74 +1670,74 @@
  "tea-hash",
  "tea-lazy",
  "tea-macros",
 ]
 
 [[package]]
 name = "tea-groupby"
-version = "0.6.9"
+version = "0.7.0"
 dependencies = [
  "ndarray",
  "pyo3",
  "rayon",
  "tea-core",
  "tea-ext",
  "tea-hash",
  "tea-lazy",
  "tea-macros",
 ]
 
 [[package]]
 name = "tea-hash"
-version = "0.6.9"
+version = "0.7.0"
 dependencies = [
  "ahash",
  "gxhash",
  "tea-dtype",
 ]
 
 [[package]]
 name = "tea-io"
-version = "0.6.9"
+version = "0.7.0"
 dependencies = [
  "arrow2",
  "memmap2",
  "rayon",
  "tea-core",
  "tea-hash",
  "tea-lazy",
  "tea-macros",
 ]
 
 [[package]]
 name = "tea-lazy"
-version = "0.6.9"
+version = "0.7.0"
 dependencies = [
  "ndarray",
  "parking_lot",
  "pyo3",
  "rayon",
  "regex",
  "tea-core",
  "tea-hash",
 ]
 
 [[package]]
 name = "tea-macros"
-version = "0.6.9"
+version = "0.7.0"
 dependencies = [
  "ndarray",
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "tea-py"
-version = "0.6.9"
+version = "0.7.0"
 dependencies = [
  "ahash",
  "chrono",
  "ndarray",
  "numpy",
  "once_cell",
  "parking_lot",
@@ -1745,25 +1750,25 @@
  "tea-hash",
  "tea-io",
  "tea-lazy",
 ]
 
 [[package]]
 name = "tea-time"
-version = "0.6.9"
+version = "0.7.0"
 dependencies = [
  "chrono",
  "ndarray",
  "numpy",
  "pyo3",
 ]
 
 [[package]]
 name = "tea-utils"
-version = "0.6.9"
+version = "0.7.0"
 
 [[package]]
 name = "tempfile"
 version = "3.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "85b77fafb263dd9d05cbeac119526425676db3784113aa9295c88498cbf8bff1"
 dependencies = [
@@ -1771,30 +1776,30 @@
  "fastrand",
  "rustix",
  "windows-sys",
 ]
 
 [[package]]
 name = "thiserror"
-version = "1.0.57"
+version = "1.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1e45bcbe8ed29775f228095caf2cd67af7a4ccf756ebff23a306bf3e8b47b24b"
+checksum = "03468839009160513471e86a034bb2c5c0e4baae3b43f79ffc55c4a5427b3297"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.57"
+version = "1.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a953cb265bef375dae3de6663da4d3804eee9682ea80d8e2542529b73c531c81"
+checksum = "c61f3ba182994efc43764a46c018c347bc492c79f024e705f46567b418f6d4f7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "tinyvec"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87cc5ceb3875bb20c2890005a4e226a4651264a5c75edb2421b52861a0a0cb50"
@@ -1886,17 +1891,17 @@
  "form_urlencoded",
  "idna",
  "percent-encoding",
 ]
 
 [[package]]
 name = "uuid"
-version = "1.7.0"
+version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f00cc9702ca12d3c81455259621e676d0f7251cec66a21e98fe2e9a37db93b2a"
+checksum = "a183cf7feeba97b4dd1c0d46788634f6221d87fa961b305bed08c851829efcc0"
 dependencies = [
  "getrandom",
 ]
 
 [[package]]
 name = "vcpkg"
 version = "0.2.15"
@@ -1942,15 +1947,15 @@
 checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.58",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1964,15 +1969,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.58",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.92"
@@ -2185,15 +2190,15 @@
 name = "zerocopy-derive"
 version = "0.7.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ce1b18ccd8e73a9321186f97e46f9f04b778851177567b1975109d26a08d2a6"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "zeroize"
 version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "525b4ec142c6b68a2d10f01f7bbf6755599ca3f81ea53b8431b7dd348f5fdb2d"
@@ -2215,14 +2220,14 @@
 dependencies = [
  "libc",
  "zstd-sys",
 ]
 
 [[package]]
 name = "zstd-sys"
-version = "2.0.9+zstd.1.5.5"
+version = "2.0.10+zstd.1.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9e16efa8a874a0481a574084d34cc26fdb3b99627480f785888deb6386506656"
+checksum = "c253a4914af5bafc8fa8c86ee400827e83cf6ec01195ec1f1ed8441bf00d65aa"
 dependencies = [
  "cc",
  "pkg-config",
 ]
```

### Comparing `teapy-0.6.9/PKG-INFO` & `teapy-0.7.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: teapy
-Version: 0.6.9
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Dist: numpy >=1.16.0
-License-File: LICENSE
-Summary: A blazingly fast datadict library
-Author: Teamon
-Author-email: Teamon <teamon9161@163.com>
-License: MIT
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: Source Code, https://github.com/Teamon9161/teapy
-
 # Teapy
 [![Build](https://github.com/teamon9161/teapy/workflows/Build/badge.svg)](https://github.com/teamon9161/teapy/actions)
 [![PyPI](https://img.shields.io/pypi/v/teapy)](https://pypi.org/project/teapy)
 [![codecov](https://codecov.io/gh/teamon9161/teapy/branch/master/graph/badge.svg?token=WK0F7P1VC6)](https://codecov.io/gh/teamon9161/teapy)
 
 ## Blazingly fast datadict library in Python
 
@@ -71,8 +55,8 @@
     dd['a'].ts_mean(3).alias('d'), 
     dd['b'].ts_std(4).alias('e')
 ])
 dd.eval(['d', 'e'])  # Evaluate specific keys in parallel
 dd.eval()  # Or evaluate all expressions in parallel
 print(dd['d'])
 
-```
+```
```

