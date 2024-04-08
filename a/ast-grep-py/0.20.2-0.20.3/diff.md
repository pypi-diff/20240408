# Comparing `tmp/ast_grep_py-0.20.2.tar.gz` & `tmp/ast_grep_py-0.20.3.tar.gz`

## Comparing `ast_grep_py-0.20.2.tar` & `ast_grep_py-0.20.3.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0     1001      127      693 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/core/Cargo.toml
--rw-r--r--   0     1001      127     2331 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/core/src/language.rs
--rw-r--r--   0     1001      127     3904 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/core/src/lib.rs
--rw-r--r--   0     1001      127    14735 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/core/src/match_tree.rs
--rw-r--r--   0     1001      127     3610 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/core/src/matcher/kind.rs
--rw-r--r--   0     1001      127     3689 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/core/src/matcher/node_match.rs
--rw-r--r--   0     1001      127    13103 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/core/src/matcher/pattern.rs
--rw-r--r--   0     1001      127      982 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/core/src/matcher/text.rs
--rw-r--r--   0     1001      127     5317 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/core/src/matcher.rs
--rw-r--r--   0     1001      127    10527 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/core/src/meta_var.rs
--rw-r--r--   0     1001      127    17264 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/core/src/node.rs
--rw-r--r--   0     1001      127    15251 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/core/src/ops.rs
--rw-r--r--   0     1001      127     4789 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/core/src/pinned.rs
--rw-r--r--   0     1001      127    10854 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/core/src/replacer/indent.rs
--rw-r--r--   0     1001      127     6157 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/core/src/replacer/structural.rs
--rw-r--r--   0     1001      127     9470 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/core/src/replacer/template.rs
--rw-r--r--   0     1001      127     2651 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/core/src/replacer.rs
--rw-r--r--   0     1001      127     8489 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/core/src/source.rs
--rw-r--r--   0     1001      127    16602 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/core/src/traversal.rs
--rw-r--r--   0     1001      127     2296 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/language/Cargo.toml
--rw-r--r--   0     1001      127     1047 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/language/src/bash.rs
--rw-r--r--   0     1001      127     1023 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/language/src/cpp.rs
--rw-r--r--   0     1001      127      860 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/language/src/csharp.rs
--rw-r--r--   0     1001      127      815 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/language/src/css.rs
--rw-r--r--   0     1001      127     2412 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/language/src/elixir.rs
--rw-r--r--   0     1001      127     1192 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/language/src/go.rs
--rw-r--r--   0     1001      127     1142 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/language/src/html.rs
--rw-r--r--   0     1001      127     1013 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/language/src/json.rs
--rw-r--r--   0     1001      127     1216 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/language/src/kotlin.rs
--rw-r--r--   0     1001      127    13416 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/language/src/lib.rs
--rw-r--r--   0     1001      127      924 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/language/src/lua.rs
--rw-r--r--   0     1001      127     3410 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/language/src/parsers.rs
--rw-r--r--   0     1001      127      372 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/language/src/php.rs
--rw-r--r--   0     1001      127     2494 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/language/src/python.rs
--rw-r--r--   0     1001      127      846 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/language/src/ruby.rs
--rw-r--r--   0     1001      127     1727 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/language/src/rust.rs
--rw-r--r--   0     1001      127     1646 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/language/src/scala.rs
--rw-r--r--   0     1001      127     1362 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/language/src/swift.rs
--rw-r--r--   0     1001      127      683 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/config/Cargo.toml
--rw-r--r--   0     1001      127     7022 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/config/src/combined.rs
--rw-r--r--   0     1001      127     8636 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/config/src/fixer.rs
--rw-r--r--   0     1001      127     5198 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/config/src/lib.rs
--rw-r--r--   0     1001      127     3677 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/config/src/maybe.rs
--rw-r--r--   0     1001      127     7993 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/config/src/rule/deserialize_env.rs
--rw-r--r--   0     1001      127    16052 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/config/src/rule/mod.rs
--rw-r--r--   0     1001      127     7167 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/config/src/rule/referent_rule.rs
--rw-r--r--   0     1001      127    16111 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/config/src/rule/relational_rule.rs
--rw-r--r--   0     1001      127     4289 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/config/src/rule/stop_by.rs
--rw-r--r--   0     1001      127     6342 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/config/src/rule_collection.rs
--rw-r--r--   0     1001      127    13722 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/config/src/rule_config.rs
--rw-r--r--   0     1001      127    10975 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/config/src/rule_core.rs
--rw-r--r--   0     1001      127    10047 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/config/src/transform/mod.rs
--rw-r--r--   0     1001      127     9656 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/config/src/transform/rewrite.rs
--rw-r--r--   0     1001      127     7418 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/config/src/transform/string_case.rs
--rw-r--r--   0        0        0      884 1970-01-01 00:00:00.000000 ast_grep_py-0.20.2/crates/pyo3/Cargo.toml
--rw-r--r--   0     1001      127     1459 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/pyo3/README.md
--rw-r--r--   0     1001      127     1356 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/pyo3/ast_grep_py/__init__.py
--rw-r--r--   0     1001      127     1933 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/pyo3/ast_grep_py/ast_grep_py.pyi
--rw-r--r--   0     1001      127        0 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/pyo3/ast_grep_py/py.typed
--rw-r--r--   0     1001      127     1083 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/pyo3/src/lib.rs
--rw-r--r--   0     1001      127     7573 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/pyo3/src/py_node.rs
--rw-r--r--   0     1001      127     2358 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/pyo3/src/range.rs
--rw-r--r--   0     1001      127      893 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/pyo3/tests/test_range.py
--rw-r--r--   0     1001      127     3641 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/pyo3/tests/test_rule.py
--rw-r--r--   0     1001      127     3463 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/pyo3/tests/test_simple.py
--rw-r--r--   0     1001      127     3221 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/pyo3/tests/test_traversal.py
--rw-r--r--   0     1001      127     1214 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/crates/pyo3/tests/test_wrong_usage.py
--rw-r--r--   0     1001      127    61484 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/Cargo.lock
--rw-r--r--   0        0        0     1103 1970-01-01 00:00:00.000000 ast_grep_py-0.20.2/Cargo.toml
--rw-r--r--   0        0        0     1310 1970-01-01 00:00:00.000000 ast_grep_py-0.20.2/pyproject.toml
--rw-r--r--   0     1001      127     1356 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/ast_grep_py/__init__.py
--rw-r--r--   0     1001      127        0 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/ast_grep_py/py.typed
--rw-r--r--   0     1001      127     1933 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/ast_grep_py/ast_grep_py.pyi
--rw-r--r--   0     1001      127     1459 2024-03-27 20:47:53.000000 ast_grep_py-0.20.2/README.md
--rw-r--r--   0        0        0     2732 1970-01-01 00:00:00.000000 ast_grep_py-0.20.2/PKG-INFO
+-rw-r--r--   0     1001      127      683 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/config/Cargo.toml
+-rw-r--r--   0     1001      127     7022 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/config/src/combined.rs
+-rw-r--r--   0     1001      127     8636 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/config/src/fixer.rs
+-rw-r--r--   0     1001      127     5198 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/config/src/lib.rs
+-rw-r--r--   0     1001      127     3677 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/config/src/maybe.rs
+-rw-r--r--   0     1001      127     7993 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/config/src/rule/deserialize_env.rs
+-rw-r--r--   0     1001      127    16052 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/config/src/rule/mod.rs
+-rw-r--r--   0     1001      127     7167 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/config/src/rule/referent_rule.rs
+-rw-r--r--   0     1001      127    16111 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/config/src/rule/relational_rule.rs
+-rw-r--r--   0     1001      127     4289 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/config/src/rule/stop_by.rs
+-rw-r--r--   0     1001      127     6342 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/config/src/rule_collection.rs
+-rw-r--r--   0     1001      127    13722 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/config/src/rule_config.rs
+-rw-r--r--   0     1001      127    10975 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/config/src/rule_core.rs
+-rw-r--r--   0     1001      127    10047 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/config/src/transform/mod.rs
+-rw-r--r--   0     1001      127     9656 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/config/src/transform/rewrite.rs
+-rw-r--r--   0     1001      127     7418 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/config/src/transform/string_case.rs
+-rw-r--r--   0     1001      127      693 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/core/Cargo.toml
+-rw-r--r--   0     1001      127     2331 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/core/src/language.rs
+-rw-r--r--   0     1001      127     3904 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/core/src/lib.rs
+-rw-r--r--   0     1001      127    14735 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/core/src/match_tree.rs
+-rw-r--r--   0     1001      127     3610 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/core/src/matcher/kind.rs
+-rw-r--r--   0     1001      127     3689 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/core/src/matcher/node_match.rs
+-rw-r--r--   0     1001      127    13103 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/core/src/matcher/pattern.rs
+-rw-r--r--   0     1001      127      982 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/core/src/matcher/text.rs
+-rw-r--r--   0     1001      127     5317 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/core/src/matcher.rs
+-rw-r--r--   0     1001      127    10527 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/core/src/meta_var.rs
+-rw-r--r--   0     1001      127    17264 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/core/src/node.rs
+-rw-r--r--   0     1001      127    15251 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/core/src/ops.rs
+-rw-r--r--   0     1001      127     4789 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/core/src/pinned.rs
+-rw-r--r--   0     1001      127    10854 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/core/src/replacer/indent.rs
+-rw-r--r--   0     1001      127     6157 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/core/src/replacer/structural.rs
+-rw-r--r--   0     1001      127     9470 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/core/src/replacer/template.rs
+-rw-r--r--   0     1001      127     2651 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/core/src/replacer.rs
+-rw-r--r--   0     1001      127     8489 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/core/src/source.rs
+-rw-r--r--   0     1001      127    16602 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/core/src/traversal.rs
+-rw-r--r--   0     1001      127     2219 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/language/Cargo.toml
+-rw-r--r--   0     1001      127     1047 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/language/src/bash.rs
+-rw-r--r--   0     1001      127     1023 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/language/src/cpp.rs
+-rw-r--r--   0     1001      127      860 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/language/src/csharp.rs
+-rw-r--r--   0     1001      127      815 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/language/src/css.rs
+-rw-r--r--   0     1001      127     2412 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/language/src/elixir.rs
+-rw-r--r--   0     1001      127     1192 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/language/src/go.rs
+-rw-r--r--   0     1001      127     1142 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/language/src/html.rs
+-rw-r--r--   0     1001      127     1013 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/language/src/json.rs
+-rw-r--r--   0     1001      127     1216 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/language/src/kotlin.rs
+-rw-r--r--   0     1001      127    13416 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/language/src/lib.rs
+-rw-r--r--   0     1001      127      924 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/language/src/lua.rs
+-rw-r--r--   0     1001      127     3410 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/language/src/parsers.rs
+-rw-r--r--   0     1001      127      372 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/language/src/php.rs
+-rw-r--r--   0     1001      127     2494 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/language/src/python.rs
+-rw-r--r--   0     1001      127      846 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/language/src/ruby.rs
+-rw-r--r--   0     1001      127     1727 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/language/src/rust.rs
+-rw-r--r--   0     1001      127     1646 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/language/src/scala.rs
+-rw-r--r--   0     1001      127     1362 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/language/src/swift.rs
+-rw-r--r--   0        0        0      884 1970-01-01 00:00:00.000000 ast_grep_py-0.20.3/crates/pyo3/Cargo.toml
+-rw-r--r--   0     1001      127     1459 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/pyo3/README.md
+-rw-r--r--   0     1001      127     1356 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/pyo3/ast_grep_py/__init__.py
+-rw-r--r--   0     1001      127     1933 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/pyo3/ast_grep_py/ast_grep_py.pyi
+-rw-r--r--   0     1001      127        0 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/pyo3/ast_grep_py/py.typed
+-rw-r--r--   0     1001      127     1090 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/pyo3/src/lib.rs
+-rw-r--r--   0     1001      127     7731 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/pyo3/src/py_node.rs
+-rw-r--r--   0     1001      127     2358 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/pyo3/src/range.rs
+-rw-r--r--   0     1001      127      893 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/pyo3/tests/test_range.py
+-rw-r--r--   0     1001      127     3641 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/pyo3/tests/test_rule.py
+-rw-r--r--   0     1001      127     3463 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/pyo3/tests/test_simple.py
+-rw-r--r--   0     1001      127     3221 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/pyo3/tests/test_traversal.py
+-rw-r--r--   0     1001      127     1214 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/crates/pyo3/tests/test_wrong_usage.py
+-rw-r--r--   0     1001      127    61477 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/Cargo.lock
+-rw-r--r--   0        0        0     1103 1970-01-01 00:00:00.000000 ast_grep_py-0.20.3/Cargo.toml
+-rw-r--r--   0        0        0     1310 1970-01-01 00:00:00.000000 ast_grep_py-0.20.3/pyproject.toml
+-rw-r--r--   0     1001      127     1356 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/ast_grep_py/__init__.py
+-rw-r--r--   0     1001      127        0 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/ast_grep_py/py.typed
+-rw-r--r--   0     1001      127     1933 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/ast_grep_py/ast_grep_py.pyi
+-rw-r--r--   0     1001      127     1459 2024-04-08 00:26:45.000000 ast_grep_py-0.20.3/README.md
+-rw-r--r--   0        0        0     2732 1970-01-01 00:00:00.000000 ast_grep_py-0.20.3/PKG-INFO
```

### Comparing `ast_grep_py-0.20.2/crates/core/Cargo.toml` & `ast_grep_py-0.20.3/crates/core/Cargo.toml`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/crates/core/src/language.rs` & `ast_grep_py-0.20.3/crates/core/src/language.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/crates/core/src/lib.rs` & `ast_grep_py-0.20.3/crates/core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/crates/core/src/match_tree.rs` & `ast_grep_py-0.20.3/crates/core/src/match_tree.rs`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
       if *named && !candidate.is_named() {
         None
       } else {
         Some(candidate)
       }
     }
     // Ellipsis will be matched in parent level
-    MV::Mutliple => {
+    MV::Multiple => {
       debug_assert!(false, "Ellipsis should be matched in parent level");
       Some(candidate)
     }
     MV::MultiCapture(name) => {
       env.to_mut().insert(name, candidate.clone())?;
       Some(candidate)
     }
@@ -40,15 +40,15 @@
 /// Returns Ok if ellipsis pattern is found. If the ellipsis is named, returns it name.
 /// If the ellipsis is unnamed, returns None. If it is not ellipsis node, returns Err.
 fn try_get_ellipsis_mode(node: &Pattern<impl Language>) -> Result<Option<String>, ()> {
   let Pattern::MetaVar { meta_var, .. } = node else {
     return Err(());
   };
   match meta_var {
-    MetaVariable::Mutliple => Ok(None),
+    MetaVariable::Multiple => Ok(None),
     MetaVariable::MultiCapture(n) => Ok(Some(n.into())),
     _ => Err(()),
   }
 }
 
 fn update_ellipsis_env<'t, D: Doc>(
   optional_name: &Option<String>,
```

### Comparing `ast_grep_py-0.20.2/crates/core/src/matcher/kind.rs` & `ast_grep_py-0.20.3/crates/core/src/matcher/kind.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/crates/core/src/matcher/node_match.rs` & `ast_grep_py-0.20.3/crates/core/src/matcher/node_match.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/crates/core/src/matcher/pattern.rs` & `ast_grep_py-0.20.3/crates/core/src/matcher/pattern.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/crates/core/src/matcher/text.rs` & `ast_grep_py-0.20.3/crates/core/src/matcher/text.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/crates/core/src/matcher.rs` & `ast_grep_py-0.20.3/crates/core/src/matcher.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/crates/core/src/meta_var.rs` & `ast_grep_py-0.20.3/crates/core/src/meta_var.rs`

 * *Files 5% similar despite different names*

```diff
@@ -192,31 +192,31 @@
 #[derive(Clone, Debug, PartialEq, Eq)]
 pub enum MetaVariable {
   /// $A for captured meta var
   Capture(MetaVariableID, bool),
   /// $_ for non-captured meta var
   Dropped(bool),
   /// $$$ for non-captured multi var
-  Mutliple,
+  Multiple,
   /// $$$A for captured ellipsis
   MultiCapture(MetaVariableID),
 }
 
 pub(crate) fn extract_meta_var(src: &str, meta_char: char) -> Option<MetaVariable> {
   use MetaVariable::*;
   let ellipsis: String = std::iter::repeat(meta_char).take(3).collect();
   if src == ellipsis {
-    return Some(Mutliple);
+    return Some(Multiple);
   }
   if let Some(trimmed) = src.strip_prefix(&ellipsis) {
     if !trimmed.chars().all(is_valid_meta_var_char) {
       return None;
     }
     if trimmed.starts_with('_') {
-      return Some(Mutliple);
+      return Some(Multiple);
     } else {
       return Some(MultiCapture(trimmed.to_owned()));
     }
   }
   if !src.starts_with(meta_char) {
     return None;
   }
@@ -278,15 +278,15 @@
 
   fn extract_var(s: &str) -> Option<MetaVariable> {
     extract_meta_var(s, '$')
   }
   #[test]
   fn test_match_var() {
     use MetaVariable::*;
-    assert_eq!(extract_var("$$$"), Some(Mutliple));
+    assert_eq!(extract_var("$$$"), Some(Multiple));
     assert_eq!(extract_var("$ABC"), Some(Capture("ABC".into(), true)));
     assert_eq!(extract_var("$$ABC"), Some(Capture("ABC".into(), false)));
     assert_eq!(extract_var("$MATCH1"), Some(Capture("MATCH1".into(), true)));
     assert_eq!(extract_var("$$$ABC"), Some(MultiCapture("ABC".into())));
     assert_eq!(extract_var("$_"), Some(Dropped(true)));
     assert_eq!(extract_var("$_123"), Some(Dropped(true)));
     assert_eq!(extract_var("$$_"), Some(Dropped(false)));
@@ -311,15 +311,15 @@
     env.match_constraints(&matchers)
   }
 
   #[test]
   fn test_non_ascii_meta_var() {
     let extract = |s| extract_meta_var(s, 'µ');
     use MetaVariable::*;
-    assert_eq!(extract("µµµ"), Some(Mutliple));
+    assert_eq!(extract("µµµ"), Some(Multiple));
     assert_eq!(extract("µABC"), Some(Capture("ABC".into(), true)));
     assert_eq!(extract("µµABC"), Some(Capture("ABC".into(), false)));
     assert_eq!(extract("µµµABC"), Some(MultiCapture("ABC".into())));
     assert_eq!(extract("µ_"), Some(Dropped(true)));
     assert_eq!(extract("abc"), None);
     assert_eq!(extract("µabc"), None);
   }
```

### Comparing `ast_grep_py-0.20.2/crates/core/src/node.rs` & `ast_grep_py-0.20.3/crates/core/src/node.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/crates/core/src/ops.rs` & `ast_grep_py-0.20.3/crates/core/src/ops.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/crates/core/src/pinned.rs` & `ast_grep_py-0.20.3/crates/core/src/pinned.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/crates/core/src/replacer/indent.rs` & `ast_grep_py-0.20.3/crates/core/src/replacer/indent.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/crates/core/src/replacer/structural.rs` & `ast_grep_py-0.20.3/crates/core/src/replacer/structural.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/crates/core/src/replacer/template.rs` & `ast_grep_py-0.20.3/crates/core/src/replacer/template.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/crates/core/src/replacer.rs` & `ast_grep_py-0.20.3/crates/core/src/replacer.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/crates/core/src/source.rs` & `ast_grep_py-0.20.3/crates/core/src/source.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/crates/core/src/traversal.rs` & `ast_grep_py-0.20.3/crates/core/src/traversal.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/crates/language/Cargo.toml` & `ast_grep_py-0.20.3/crates/language/Cargo.toml`

 * *Files 7% similar despite different names*

```diff
@@ -15,20 +15,20 @@
 
 ignore.workspace = true
 serde.workspace = true
 
 tree-sitter-bash = { version = "0.20.5", optional = true }
 tree-sitter-c = { version = "0.20.8", optional = true }
 tree-sitter-cpp = { version = "0.20.5", optional = true }
-tree-sitter-c-sharp = { version = "0.20.0", package = "ast-grep-tree-sitter-c-sharp", optional = true }
+tree-sitter-c-sharp = { version = "0.20.0", optional = true }
 tree-sitter-css = { version = "0.20.0", optional = true }
 tree-sitter-dart= { version = "0.0.3", optional = true }
 tree-sitter-elixir = { version = "0.1.1", optional = true }
 tree-sitter-go = { version = "0.20.0", optional = true }
-tree-sitter-html = { version = "0.20.0", package = "tree-sitter-html-dvdb", optional = true }
+tree-sitter-html = { version = "0.20.0", optional = true }
 tree-sitter-java = { version = "0.20.2", optional = true }
 tree-sitter-javascript = { version = "0.20.4", optional = true }
 tree-sitter-json = { version = "0.20.2", optional = true }
 tree-sitter-kotlin = { version = "0.3.5", optional = true }
 tree-sitter-lua = { version = "0.0.19", optional = true }
 tree-sitter-php = { version = "0.22.2", optional = true }
 tree-sitter-python = { version = "0.20.4", optional = true }
```

### Comparing `ast_grep_py-0.20.2/crates/language/src/bash.rs` & `ast_grep_py-0.20.3/crates/language/src/bash.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/crates/language/src/cpp.rs` & `ast_grep_py-0.20.3/crates/language/src/cpp.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/crates/language/src/csharp.rs` & `ast_grep_py-0.20.3/crates/language/src/csharp.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/crates/language/src/css.rs` & `ast_grep_py-0.20.3/crates/language/src/css.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/crates/language/src/elixir.rs` & `ast_grep_py-0.20.3/crates/language/src/elixir.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/crates/language/src/go.rs` & `ast_grep_py-0.20.3/crates/language/src/go.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/crates/language/src/html.rs` & `ast_grep_py-0.20.3/crates/language/src/html.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/crates/language/src/json.rs` & `ast_grep_py-0.20.3/crates/language/src/json.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/crates/language/src/kotlin.rs` & `ast_grep_py-0.20.3/crates/language/src/kotlin.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/crates/language/src/lib.rs` & `ast_grep_py-0.20.3/crates/language/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/crates/language/src/lua.rs` & `ast_grep_py-0.20.3/crates/language/src/lua.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/crates/language/src/parsers.rs` & `ast_grep_py-0.20.3/crates/language/src/parsers.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/crates/language/src/python.rs` & `ast_grep_py-0.20.3/crates/language/src/python.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/crates/language/src/ruby.rs` & `ast_grep_py-0.20.3/crates/language/src/ruby.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/crates/language/src/rust.rs` & `ast_grep_py-0.20.3/crates/language/src/rust.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/crates/language/src/scala.rs` & `ast_grep_py-0.20.3/crates/language/src/scala.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/crates/language/src/swift.rs` & `ast_grep_py-0.20.3/crates/language/src/swift.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/crates/config/Cargo.toml` & `ast_grep_py-0.20.3/crates/config/Cargo.toml`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/crates/config/src/combined.rs` & `ast_grep_py-0.20.3/crates/config/src/combined.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/crates/config/src/fixer.rs` & `ast_grep_py-0.20.3/crates/config/src/fixer.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/crates/config/src/lib.rs` & `ast_grep_py-0.20.3/crates/config/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/crates/config/src/maybe.rs` & `ast_grep_py-0.20.3/crates/config/src/maybe.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/crates/config/src/rule/deserialize_env.rs` & `ast_grep_py-0.20.3/crates/config/src/rule/deserialize_env.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/crates/config/src/rule/mod.rs` & `ast_grep_py-0.20.3/crates/config/src/rule/mod.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/crates/config/src/rule/referent_rule.rs` & `ast_grep_py-0.20.3/crates/config/src/rule/referent_rule.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/crates/config/src/rule/relational_rule.rs` & `ast_grep_py-0.20.3/crates/config/src/rule/relational_rule.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/crates/config/src/rule/stop_by.rs` & `ast_grep_py-0.20.3/crates/config/src/rule/stop_by.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/crates/config/src/rule_collection.rs` & `ast_grep_py-0.20.3/crates/config/src/rule_collection.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/crates/config/src/rule_config.rs` & `ast_grep_py-0.20.3/crates/config/src/rule_config.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/crates/config/src/rule_core.rs` & `ast_grep_py-0.20.3/crates/config/src/rule_core.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/crates/config/src/transform/mod.rs` & `ast_grep_py-0.20.3/crates/config/src/transform/mod.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/crates/config/src/transform/rewrite.rs` & `ast_grep_py-0.20.3/crates/config/src/transform/rewrite.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/crates/config/src/transform/string_case.rs` & `ast_grep_py-0.20.3/crates/config/src/transform/string_case.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/crates/pyo3/Cargo.toml` & `ast_grep_py-0.20.3/crates/pyo3/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,14 @@
 crate-type = ["cdylib"]
 
 [dependencies]
 ast-grep-core.workspace = true
 ast-grep-config.workspace = true
 ast-grep-language.workspace = true
 anyhow.workspace = true
-pyo3 = { version = "0.20.3", optional = true, features = ["anyhow"] }
-pythonize = { version = "0.20.0", optional = true }
+pyo3 = { version = "0.21.1", optional = true, features = ["anyhow"] }
+pythonize = { version = "0.21.1", optional = true }
 
 # uncomment default features when developing pyo3
 [features]
 # default = ["python"]
 python = ["pythonize", "pyo3", "pyo3/extension-module"]
```

### Comparing `ast_grep_py-0.20.2/crates/pyo3/README.md` & `ast_grep_py-0.20.3/crates/pyo3/README.md`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/crates/pyo3/ast_grep_py/__init__.py` & `ast_grep_py-0.20.3/crates/pyo3/ast_grep_py/__init__.py`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/crates/pyo3/ast_grep_py/ast_grep_py.pyi` & `ast_grep_py-0.20.3/crates/pyo3/ast_grep_py/ast_grep_py.pyi`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/crates/pyo3/src/lib.rs` & `ast_grep_py-0.20.3/crates/pyo3/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 use ast_grep_core::{AstGrep, Language, NodeMatch, StrDoc};
 use ast_grep_language::SupportLang;
 use pyo3::prelude::*;
 
 /// A Python module implemented in Rust.
 #[pymodule]
-fn ast_grep_py(_py: Python, m: &PyModule) -> PyResult<()> {
+fn ast_grep_py(_py: Python, m: &Bound<PyModule>) -> PyResult<()> {
   m.add_class::<SgRoot>()?;
   m.add_class::<SgNode>()?;
   m.add_class::<Range>()?;
   m.add_class::<Pos>()?;
   Ok(())
 }
```

### Comparing `ast_grep_py-0.20.2/crates/pyo3/src/py_node.rs` & `ast_grep_py-0.20.3/crates/pyo3/src/py_node.rs`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 use std::collections::hash_map::DefaultHasher;
 use std::hash::{Hash, Hasher};
 
 use anyhow::Context;
 use pyo3::exceptions::{PyKeyError, PyValueError};
 use pyo3::prelude::*;
 use pyo3::types::PyDict;
-use pythonize::depythonize;
+use pythonize::depythonize_bound;
 
 #[pyclass(mapping)]
 pub struct SgNode {
   pub inner: NodeMatch<'static, StrDoc<SupportLang>>,
   // refcount SgRoot
   pub(crate) root: Py<SgRoot>,
 }
@@ -50,39 +50,39 @@
 
   fn text(&self) -> String {
     self.inner.text().to_string()
   }
 
   /*---------- Search Refinement  ----------*/
   #[pyo3(signature = (**kwargs))]
-  fn matches(&self, kwargs: Option<&PyDict>) -> PyResult<bool> {
+  fn matches(&self, kwargs: Option<Bound<PyDict>>) -> PyResult<bool> {
     let matcher = get_matcher_from_rule(self.inner.lang(), kwargs)?;
     Ok(self.inner.matches(matcher))
   }
 
   #[pyo3(signature = (**kwargs))]
-  fn inside(&self, kwargs: Option<&PyDict>) -> PyResult<bool> {
+  fn inside(&self, kwargs: Option<Bound<PyDict>>) -> PyResult<bool> {
     let matcher = get_matcher_from_rule(self.inner.lang(), kwargs)?;
     Ok(self.inner.inside(matcher))
   }
 
   #[pyo3(signature = (**kwargs))]
-  fn has(&self, kwargs: Option<&PyDict>) -> PyResult<bool> {
+  fn has(&self, kwargs: Option<Bound<PyDict>>) -> PyResult<bool> {
     let matcher = get_matcher_from_rule(self.inner.lang(), kwargs)?;
     Ok(self.inner.has(matcher))
   }
 
   #[pyo3(signature = (**kwargs))]
-  fn precedes(&self, kwargs: Option<&PyDict>) -> PyResult<bool> {
+  fn precedes(&self, kwargs: Option<Bound<PyDict>>) -> PyResult<bool> {
     let matcher = get_matcher_from_rule(self.inner.lang(), kwargs)?;
     Ok(self.inner.precedes(matcher))
   }
 
   #[pyo3(signature = (**kwargs))]
-  fn follows(&self, kwargs: Option<&PyDict>) -> PyResult<bool> {
+  fn follows(&self, kwargs: Option<Bound<PyDict>>) -> PyResult<bool> {
     let matcher = get_matcher_from_rule(self.inner.lang(), kwargs)?;
     Ok(self.inner.follows(matcher))
   }
 
   fn get_match(&self, meta_var: &str) -> Option<Self> {
     self
       .inner
@@ -118,28 +118,36 @@
 
   /*---------- Tree Traversal  ----------*/
   fn get_root(&self) -> Py<SgRoot> {
     self.root.clone()
   }
 
   #[pyo3(signature = (config=None, **rule))]
-  fn find(&self, config: Option<&PyDict>, rule: Option<&PyDict>) -> PyResult<Option<Self>> {
+  fn find(
+    &self,
+    config: Option<Bound<PyDict>>,
+    rule: Option<Bound<PyDict>>,
+  ) -> PyResult<Option<Self>> {
     let matcher = self.get_matcher(config, rule)?;
     if let Some(inner) = self.inner.find(matcher) {
       Ok(Some(Self {
         inner,
         root: self.root.clone(),
       }))
     } else {
       Ok(None)
     }
   }
 
   #[pyo3(signature = (config=None, **rule))]
-  fn find_all(&self, config: Option<&PyDict>, rule: Option<&PyDict>) -> PyResult<Vec<Self>> {
+  fn find_all(
+    &self,
+    config: Option<Bound<PyDict>>,
+    rule: Option<Bound<PyDict>>,
+  ) -> PyResult<Vec<Self>> {
     let matcher = self.get_matcher(config, rule)?;
     Ok(
       self
         .inner
         .find_all(matcher)
         .map(|n| Self {
           inner: n,
@@ -260,16 +268,16 @@
     }
   }
 }
 
 impl SgNode {
   fn get_matcher(
     &self,
-    config: Option<&PyDict>,
-    kwargs: Option<&PyDict>,
+    config: Option<Bound<PyDict>>,
+    kwargs: Option<Bound<PyDict>>,
   ) -> PyResult<RuleCore<SupportLang>> {
     let lang = self.inner.lang();
     let config = if let Some(config) = config {
       config_from_dict(config)?
     } else if let Some(rule) = kwargs {
       config_from_rule(rule)?
     } else {
@@ -277,32 +285,32 @@
     };
     let env = DeserializeEnv::new(*lang);
     let matcher = config.get_matcher(env).context("cannot get matcher")?;
     Ok(matcher)
   }
 }
 
-fn config_from_dict(dict: &PyDict) -> PyResult<SerializableRuleCore> {
-  Ok(depythonize(dict)?)
+fn config_from_dict(dict: Bound<PyDict>) -> PyResult<SerializableRuleCore> {
+  Ok(depythonize_bound(dict.into_any())?)
 }
 
-fn config_from_rule(dict: &PyDict) -> PyResult<SerializableRuleCore> {
-  let rule = depythonize(dict)?;
+fn config_from_rule(dict: Bound<PyDict>) -> PyResult<SerializableRuleCore> {
+  let rule = depythonize_bound(dict.into_any())?;
   Ok(SerializableRuleCore {
     rule,
     constraints: None,
     utils: None,
     transform: None,
     fix: None,
   })
 }
 
 fn get_matcher_from_rule(
   lang: &SupportLang,
-  dict: Option<&PyDict>,
+  dict: Option<Bound<PyDict>>,
 ) -> PyResult<RuleCore<SupportLang>> {
   let rule = dict.ok_or_else(|| PyErr::new::<PyValueError, _>("rule must not be empty"))?;
   let env = DeserializeEnv::new(*lang);
   let config = config_from_rule(rule)?;
   let matcher = config.get_matcher(env).context("cannot get matcher")?;
   Ok(matcher)
 }
```

### Comparing `ast_grep_py-0.20.2/crates/pyo3/src/range.rs` & `ast_grep_py-0.20.3/crates/pyo3/src/range.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/crates/pyo3/tests/test_range.py` & `ast_grep_py-0.20.3/crates/pyo3/tests/test_range.py`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/crates/pyo3/tests/test_rule.py` & `ast_grep_py-0.20.3/crates/pyo3/tests/test_rule.py`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/crates/pyo3/tests/test_simple.py` & `ast_grep_py-0.20.3/crates/pyo3/tests/test_simple.py`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/crates/pyo3/tests/test_traversal.py` & `ast_grep_py-0.20.3/crates/pyo3/tests/test_traversal.py`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/crates/pyo3/tests/test_wrong_usage.py` & `ast_grep_py-0.20.3/crates/pyo3/tests/test_wrong_usage.py`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/Cargo.lock` & `ast_grep_py-0.20.3/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 name = "adler"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
 
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
 name = "anes"
 version = "0.1.6"
@@ -39,17 +39,17 @@
 checksum = "d52a9bb7ec0cf484c551830a7ce27bd20d67eac647e1befb56b0be4ee39a55d2"
 dependencies = [
  "winapi",
 ]
 
 [[package]]
 name = "anstream"
-version = "0.6.12"
+version = "0.6.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "96b09b5178381e0874812a9b157f7fe84982617e48f71f4e3235482775e5b540"
+checksum = "d96bd03f33fe50a863e394ee9718a706f988b9079b20c3784fb726e7678b62fb"
 dependencies = [
  "anstyle",
  "anstyle-parse",
  "anstyle-query",
  "anstyle-wincon",
  "colorchoice",
  "utf8parse",
@@ -108,15 +108,15 @@
  "predicates-core",
  "predicates-tree",
  "wait-timeout",
 ]
 
 [[package]]
 name = "ast-grep"
-version = "0.20.2"
+version = "0.20.3"
 dependencies = [
  "ansi_term",
  "anyhow",
  "assert_cmd",
  "ast-grep-config",
  "ast-grep-core",
  "ast-grep-dynamic",
@@ -139,15 +139,15 @@
  "similar",
  "tempfile",
  "tokio",
 ]
 
 [[package]]
 name = "ast-grep-config"
-version = "0.20.2"
+version = "0.20.3"
 dependencies = [
  "anyhow",
  "ast-grep-core",
  "bit-set",
  "globset",
  "regex",
  "schemars",
@@ -155,51 +155,51 @@
  "serde_yaml",
  "thiserror",
  "tree-sitter-typescript",
 ]
 
 [[package]]
 name = "ast-grep-core"
-version = "0.20.2"
+version = "0.20.3"
 dependencies = [
  "bit-set",
  "regex",
  "thiserror",
  "tree-sitter-facade-sg",
  "tree-sitter-typescript",
 ]
 
 [[package]]
 name = "ast-grep-dynamic"
-version = "0.20.2"
+version = "0.20.3"
 dependencies = [
  "ast-grep-core",
  "ignore",
  "libloading",
  "serde",
  "thiserror",
  "tree-sitter",
 ]
 
 [[package]]
 name = "ast-grep-language"
-version = "0.20.2"
+version = "0.20.3"
 dependencies = [
  "ast-grep-core",
- "ast-grep-tree-sitter-c-sharp",
  "ignore",
  "serde",
  "tree-sitter-bash",
  "tree-sitter-c",
+ "tree-sitter-c-sharp",
  "tree-sitter-cpp",
  "tree-sitter-css",
  "tree-sitter-dart",
  "tree-sitter-elixir",
  "tree-sitter-go",
- "tree-sitter-html-dvdb",
+ "tree-sitter-html",
  "tree-sitter-java",
  "tree-sitter-javascript",
  "tree-sitter-json",
  "tree-sitter-kotlin",
  "tree-sitter-lua",
  "tree-sitter-php",
  "tree-sitter-python",
@@ -208,74 +208,65 @@
  "tree-sitter-scala",
  "tree-sitter-swift",
  "tree-sitter-typescript",
 ]
 
 [[package]]
 name = "ast-grep-lsp"
-version = "0.20.2"
+version = "0.20.3"
 dependencies = [
  "ast-grep-config",
  "ast-grep-core",
+ "ast-grep-language",
  "dashmap",
  "serde",
+ "serde_json",
  "tokio",
  "tower-lsp",
- "tree-sitter-typescript",
 ]
 
 [[package]]
 name = "ast-grep-napi"
-version = "0.20.2"
+version = "0.20.3"
 dependencies = [
  "ast-grep-config",
  "ast-grep-core",
  "ignore",
  "napi",
  "napi-build",
  "napi-derive",
  "serde_json",
  "tree-sitter-css",
  "tree-sitter-facade-sg",
- "tree-sitter-html-dvdb",
+ "tree-sitter-html",
  "tree-sitter-javascript",
  "tree-sitter-typescript",
 ]
 
 [[package]]
 name = "ast-grep-py"
-version = "0.20.2"
+version = "0.20.3"
 dependencies = [
  "anyhow",
  "ast-grep-config",
  "ast-grep-core",
  "ast-grep-language",
  "pyo3",
  "pythonize",
 ]
 
 [[package]]
-name = "ast-grep-tree-sitter-c-sharp"
-version = "0.20.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "69bb67af006de48085e828eb70bdf65adfd148d6cee34aad192ffaec0bc04538"
-dependencies = [
- "cc",
- "tree-sitter",
-]
-
-[[package]]
 name = "async-trait"
-version = "0.1.77"
+version = "0.1.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c980ee35e870bd1a4d2c8294d4c04d0499e67bca1e4b5cefcc693c2fa00caea9"
+checksum = "a507401cad91ec6a857ed5513a2073c82a9b9048762b885bb98655b306964681"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.49",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "atty"
 version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d9b39be18770d11421cdb1b9947a45dd3f37e93092cbf377614828a319d5fee8"
@@ -283,47 +274,47 @@
  "hermit-abi 0.1.19",
  "libc",
  "winapi",
 ]
 
 [[package]]
 name = "auto_impl"
-version = "1.1.2"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "823b8bb275161044e2ac7a25879cb3e2480cb403e3943022c7c769c599b756aa"
+checksum = "3c87f3f15e7794432337fc718554eaa4dc8f04c9677a950ffe366f20a162ae42"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.49",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "autocfg"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
+checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
 
 [[package]]
 name = "backtrace"
-version = "0.3.69"
+version = "0.3.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2089b7e3f35b9dd2d0ed921ead4f6d318c27680d4a5bd167b3ee120edb105837"
+checksum = "26b05800d2e817c8b3b4b54abd461726265fa9789ae34330622f2db9ee696f9d"
 dependencies = [
  "addr2line",
  "cc",
  "cfg-if",
  "libc",
  "miniz_oxide",
  "object",
  "rustc-demangle",
 ]
 
 [[package]]
 name = "benches"
-version = "0.20.2"
+version = "0.20.3"
 dependencies = [
  "ast-grep-config",
  "ast-grep-core",
  "ast-grep-language",
  "criterion",
 ]
 
@@ -346,23 +337,23 @@
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
 name = "bstr"
-version = "1.9.0"
+version = "1.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c48f0051a4b4c5e0b6d365cd04af53aeaa209e3cc15ec2cdb69e73cc87fbd0dc"
+checksum = "05efc5cfd9110c8416e471df0e96702d58690178e206e61b7173706673c93706"
 dependencies = [
  "memchr",
  "regex-automata",
  "serde",
 ]
 
 [[package]]
@@ -375,17 +366,17 @@
 name = "byteorder"
 version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1fd0f2584146f6f2ef48085050886acf353beff7305ebd1ae69500e27c67f64b"
 
 [[package]]
 name = "bytes"
-version = "1.5.0"
+version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a2bd12c1caf447e69cd4528f47f94d203fd2582878ecb9e9465484c4148a8223"
+checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 
 [[package]]
 name = "cast"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "37b2a672a2cb129a2e41c10b1224bb368f9f37a2b16b612598138befd7b37eb5"
 
@@ -426,17 +417,17 @@
 dependencies = [
  "ciborium-io",
  "half",
 ]
 
 [[package]]
 name = "clap"
-version = "4.5.3"
+version = "4.5.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "949626d00e063efc93b6dca932419ceb5432f99769911c0b995f7e884c778813"
+checksum = "90bc066a67923782aa8515dbaea16946c5bcc5addbd668bb80af688e53e548a0"
 dependencies = [
  "clap_builder",
  "clap_derive",
 ]
 
 [[package]]
 name = "clap_builder"
@@ -457,22 +448,22 @@
 checksum = "885e4d7d5af40bfb99ae6f9433e292feac98d452dcb3ec3d25dfe7552b77da8c"
 dependencies = [
  "clap",
 ]
 
 [[package]]
 name = "clap_derive"
-version = "4.5.3"
+version = "4.5.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "90239a040c80f5e14809ca132ddc4176ab33d5e17e49691793296e3fcb34d72f"
+checksum = "528131438037fd55894f62d6e9f068b8f45ac57ffa77517819645d10aed04f64"
 dependencies = [
  "heck 0.5.0",
  "proc-macro2",
  "quote",
- "syn 2.0.49",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "clap_lex"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "98cc8fbded0c607b7ba9dd60cd98df59af97e84d24e49c8557331cfc26d301ce"
@@ -581,15 +572,15 @@
 
 [[package]]
 name = "crossterm"
 version = "0.27.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f476fe445d41c9e991fd07515a6f463074b782242ccf4a5b7b1d1012e70824df"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "crossterm_winapi",
  "libc",
  "mio",
  "parking_lot",
  "signal-hook",
  "signal-hook-mio",
  "winapi",
@@ -608,20 +599,20 @@
 name = "crunchy"
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7a81dae078cea95a014a339291cec439d2f232ebe854a9d672b796c6afafa9b7"
 
 [[package]]
 name = "ctor"
-version = "0.2.6"
+version = "0.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "30d2b3721e861707777e3195b0158f950ae6dc4a27e4d02ff9f67e3eb3de199e"
+checksum = "ad291aa74992b9b7a7e88c38acbbf6ad7e107f1d90ee8775b7bc1fc3394f485c"
 dependencies = [
  "quote",
- "syn 2.0.49",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "dashmap"
 version = "5.5.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "978747c1d849a7d2ee5e8adc0159961c48fb7e5db2f06af6723b80123bb53856"
@@ -643,17 +634,17 @@
 name = "doc-comment"
 version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fea41bba32d969b513997752735605054bc0dfa92b4c56bf1189f2e174be7a10"
 
 [[package]]
 name = "dyn-clone"
-version = "1.0.16"
+version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "545b22097d44f8a9581187cdf93de7a71e4722bf51200cfaba810865b49a495d"
+checksum = "0d6ef0072f8a535281e4876be788938b528e9a1d43900b82c2569af7da799125"
 
 [[package]]
 name = "either"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "11157ac094ffbdde99aa67b23417ebdd801842852b500e395a45a9c0aac03e4a"
 
@@ -671,17 +662,17 @@
 dependencies = [
  "libc",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "fastrand"
-version = "2.0.1"
+version = "2.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "25cbce373ec4653f1a01a31e8a5e5ec0c622dc27ff9c4e6606eefef5cbbed4a5"
+checksum = "658bd65b1cf4c852a3cc96f18a8ce7b5640f6b703f905c7d74532294c2a63984"
 
 [[package]]
 name = "float-cmp"
 version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "98de4bbd547a563b716d8dfa9aad1cb19bfab00f4fa09a6a4ed21dbcf44ce9c4"
 dependencies = [
@@ -737,15 +728,15 @@
 name = "futures-macro"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87750cf4b7a4c0625b1529e4c543c2182106e4dedc60a2a6455e00d212c489ac"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.49",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9fb8e00e87438d937621c1c6269e53f536c14d3fbd6a042bb24879e57d474fb5"
@@ -809,17 +800,17 @@
  "log",
  "regex-automata",
  "regex-syntax",
 ]
 
 [[package]]
 name = "half"
-version = "2.3.1"
+version = "2.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bc52e53916c08643f1b56ec082790d1e86a32e58dc5268f897f313fbae7b4872"
+checksum = "b5eceaaeec696539ddaf7b333340f1af35a5aa87ae3e4f3ead0532f72affab2e"
 dependencies = [
  "cfg-if",
  "crunchy",
 ]
 
 [[package]]
 name = "hashbrown"
@@ -846,17 +837,17 @@
 checksum = "62b467343b94ba476dcb2500d242dadbb39557df889310ac77c5d99100aaac33"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "hermit-abi"
-version = "0.3.6"
+version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bd5256b483761cd23699d0da46cc6fd2ee3be420bbe6d020ae4a091e70b7e9fd"
+checksum = "d231dfb89cfffdbc30e7fc41579ed6066ad03abda9e567ccafae602b97ec5024"
 
 [[package]]
 name = "httparse"
 version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d897f394bad6a705d5f4104762e116a75639e470d80901eed05a860a95cb1904"
 
@@ -884,35 +875,35 @@
  "same-file",
  "walkdir",
  "winapi-util",
 ]
 
 [[package]]
 name = "indexmap"
-version = "2.2.3"
+version = "2.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "233cf39063f058ea2caae4091bf4a3ef70a653afbc026f5c4a4135d114e3c177"
+checksum = "168fb715dda47215e360912c096649d23d58bf392ac62f73919e831745e40f26"
 dependencies = [
  "equivalent",
  "hashbrown",
 ]
 
 [[package]]
 name = "indoc"
-version = "2.0.4"
+version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1e186cfbae8084e513daff4240b4797e342f988cecda4fb6c939150f96315fd8"
+checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
 name = "inquire"
-version = "0.7.3"
+version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0fca231a35040487041f975afae9272ecd3701cc95a5efbbda36c6ecc22a269c"
+checksum = "fe95f33091b9b7b517a5849bce4dce1b550b430fc20d58059fcaa319ed895d8b"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "crossterm 0.25.0",
  "dyn-clone",
  "fuzzy-matcher",
  "fxhash",
  "newline-converter",
  "once_cell",
  "unicode-segmentation",
@@ -921,15 +912,15 @@
 
 [[package]]
 name = "is-terminal"
 version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f23ff5ef2b80d608d61efee834934d862cd92461afc0560dedf493e4c033738b"
 dependencies = [
- "hermit-abi 0.3.6",
+ "hermit-abi 0.3.9",
  "libc",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "itertools"
 version = "0.10.5"
@@ -937,41 +928,41 @@
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "itoa"
-version = "1.0.10"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1a46d1a171d865aa5f83f92695765caa047a9b4cbae2cbf37dbd613a793fd4c"
+checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
 
 [[package]]
 name = "js-sys"
-version = "0.3.68"
+version = "0.3.69"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "406cda4b368d531c842222cf9d2600a9a4acce8d29423695379c6868a143a9ee"
+checksum = "29c15563dc2726973df627357ce0c9ddddbea194836909d655df6a75d2cf296d"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "libc"
 version = "0.2.153"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
 
 [[package]]
 name = "libloading"
-version = "0.8.1"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c571b676ddfc9a8c12f1f3d3085a7b163966a8fd8098a90640953ce5f6170161"
+checksum = "0c2a198fb6b0eada2a8df47933734e6d35d350665a33a3593d7164fa52c75c19"
 dependencies = [
  "cfg-if",
- "windows-sys 0.48.0",
+ "windows-targets 0.52.4",
 ]
 
 [[package]]
 name = "linux-raw-sys"
 version = "0.4.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "01cda141df6706de531b6c46c3a33ecca755538219bd484262fa09410c13539c"
@@ -984,17 +975,17 @@
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.20"
+version = "0.4.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b5e6163cb8c49088c2c36f57875e58ccd8c87c7427f7fbd50ea6710b2f3f2e8f"
+checksum = "90ed8c1e510134f979dbc4f070f87d4313098b704861a105fe34231c70a3901c"
 
 [[package]]
 name = "lsp-types"
 version = "0.94.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c66bfd44a06ae10647fe3f8214762e9369fd4248df1350924b4ef9e770a85ea1"
 dependencies = [
@@ -1003,23 +994,23 @@
  "serde_json",
  "serde_repr",
  "url",
 ]
 
 [[package]]
 name = "memchr"
-version = "2.7.1"
+version = "2.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "523dc4f511e55ab87b694dc30d0f820d60906ef06413f93d4d7a1385599cc149"
+checksum = "6c8640c5d730cb13ebd907d8d04b52f55ac9a2eec55b440c8892f40d56c76c1d"
 
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
@@ -1027,32 +1018,32 @@
 checksum = "9d811f3e15f28568be3407c8e7fdb6514c1cda3cb30683f15b6a1a1dc4ea14a7"
 dependencies = [
  "adler",
 ]
 
 [[package]]
 name = "mio"
-version = "0.8.10"
+version = "0.8.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f3d0b296e374a4e6f3c7b0a1f5a51d748a0d34c85e7dc48fc3fa9a87657fe09"
+checksum = "a4a650543ca06a924e8b371db273b2756685faae30f8487da1b56505a8f78b0c"
 dependencies = [
  "libc",
  "log",
  "wasi",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "napi"
-version = "2.16.0"
+version = "2.16.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "54a63d0570e4c3e0daf7a8d380563610e159f538e20448d6c911337246f40e84"
+checksum = "c4ca998356d8ff9fba7a070dae4508a2298439c98c9f3bc9c07669538b999e8f"
 dependencies = [
  "anyhow",
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "ctor",
  "napi-derive",
  "napi-sys",
  "once_cell",
  "serde",
  "serde_json",
 ]
@@ -1061,39 +1052,39 @@
 name = "napi-build"
 version = "2.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2f9130fccc5f763cf2069b34a089a18f0d0883c66aceb81f2fad541a3d823c43"
 
 [[package]]
 name = "napi-derive"
-version = "2.16.0"
+version = "2.16.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "05bb7c37e3c1dda9312fdbe4a9fc7507fca72288ba154ec093e2d49114e727ce"
+checksum = "b138cecf1141ae0ff5d62f4aa0e2f269aec339f66070f346ba6fb4279f1fc178"
 dependencies = [
  "cfg-if",
  "convert_case",
  "napi-derive-backend",
  "proc-macro2",
  "quote",
- "syn 2.0.49",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "napi-derive-backend"
-version = "1.0.62"
+version = "1.0.63"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f785a8b8d7b83e925f5aa6d2ae3c159d17fe137ac368dc185bef410e7acdaeb4"
+checksum = "ce5126b64f6ad9e28e30e6d15213dd378626b38f556454afebc42f7f02a90902"
 dependencies = [
  "convert_case",
  "once_cell",
  "proc-macro2",
  "quote",
  "regex",
  "semver",
- "syn 2.0.49",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "napi-sys"
 version = "2.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2503fa6af34dc83fb74888df8b22afe933b58d37daf7d80424b1c60c68196b8b"
@@ -1127,15 +1118,15 @@
 
 [[package]]
 name = "num_cpus"
 version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4161fcb6d602d4d2081af7c3a45852d875a03dd337a6bfdd6e06407b61342a43"
 dependencies = [
- "hermit-abi 0.3.6",
+ "hermit-abi 0.3.9",
  "libc",
 ]
 
 [[package]]
 name = "object"
 version = "0.32.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1183,37 +1174,37 @@
 name = "percent-encoding"
 version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3148f5046208a5d56bcfc03053e3ca6334e51da8dfb19b6cdc8b306fae3283e"
 
 [[package]]
 name = "pin-project"
-version = "1.1.4"
+version = "1.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0302c4a0442c456bd56f841aee5c3bfd17967563f6fadc9ceb9f9c23cf3807e0"
+checksum = "b6bf43b791c5b9e34c3d182969b4abb522f9343702850a2e57f460d00d09b4b3"
 dependencies = [
  "pin-project-internal",
 ]
 
 [[package]]
 name = "pin-project-internal"
-version = "1.1.4"
+version = "1.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "266c042b60c9c76b8d53061e52b2e0d1116abc57cefc8c5cd671619a56ac3690"
+checksum = "2f38a4412a78282e09a2cf38d195ea5420d15ba0602cb375210efbc877243965"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.49",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "pin-project-lite"
-version = "0.2.13"
+version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8afb450f006bf6385ca15ef45d71d2288452bc3683ce2e2cacc0d18e4be60b58"
+checksum = "bda66fc9667c18cb2758a2ac84d1167245054bcf85d5d1aaa6923f45801bdd02"
 
 [[package]]
 name = "pin-utils"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
 
@@ -1279,26 +1270,26 @@
 dependencies = [
  "predicates-core",
  "termtree",
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
  "anyhow",
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
@@ -1307,62 +1298,62 @@
  "pyo3-ffi",
  "pyo3-macros",
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
- "syn 2.0.49",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.20.3"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7c7e9b68bb9c3149c5b0cade5d07f953d6d125eb4337723c4ccdb665f1f96185"
+checksum = "93fbbfd7eb553d10036513cb122b888dcd362a945a00b06c165f2ab480d4cc3b"
 dependencies = [
  "heck 0.4.1",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
- "syn 2.0.49",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "pythonize"
-version = "0.20.0"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ffd1c3ef39c725d63db5f9bc455461bafd80540cb7824c61afb823501921a850"
+checksum = "9d0664248812c38cc55a4ed07f88e4df516ce82604b93b1ffdc041aa77a6cb3c"
 dependencies = [
  "pyo3",
  "serde",
 ]
 
 [[package]]
 name = "quote"
@@ -1371,17 +1362,17 @@
 checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rayon"
-version = "1.8.1"
+version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fa7237101a77a10773db45d62004a272517633fbcc3df19d96455ede1122e051"
+checksum = "b418a60154510ca1a002a752ca9714984e21e4241e804d32555251faf8b78ffa"
 dependencies = [
  "either",
  "rayon-core",
 ]
 
 [[package]]
 name = "rayon-core"
@@ -1412,42 +1403,42 @@
  "memchr",
  "regex-automata",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-automata"
-version = "0.4.5"
+version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5bb987efffd3c6d0d8f5f89510bb458559eab11e4f869acb20bf845e016259cd"
+checksum = "86b83b8b9847f9bf95ef68afb0b8e6cdb80f498442f5179a29fad448fcc1eaea"
 dependencies = [
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
 name = "rustc-demangle"
 version = "0.1.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
 
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
  "windows-sys 0.52.0",
 ]
 
 [[package]]
@@ -1499,30 +1490,30 @@
 name = "semver"
 version = "1.0.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "92d43fe69e652f3df9bdc2b85b2854a0825b86e4fb76bc44d945137d053639ca"
 
 [[package]]
 name = "serde"
-version = "1.0.196"
+version = "1.0.197"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "870026e60fa08c69f064aa766c10f10b1d62db9ccd4d0abb206472bee0ce3b32"
+checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.196"
+version = "1.0.197"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "33c85360c95e7d137454dc81d9a4ed2b8efd8fbe19cee57357b32b9771fccb67"
+checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.49",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "serde_derive_internals"
 version = "0.26.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "85bf8229e7920a9f636479437026331ce11aa132b4dde37d121944a44d6e5f3c"
@@ -1530,17 +1521,17 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.114"
+version = "1.0.115"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c5f09b1bd632ef549eaa9f60a1f8de742bdbc698e6cee2095fc84dde5f549ae0"
+checksum = "12dc5c46daa8e9fdf4f5e71b6cf9a53f2487da0e86e55808e2d35539666497dd"
 dependencies = [
  "indexmap",
  "itoa",
  "ryu",
  "serde",
 ]
 
@@ -1548,22 +1539,22 @@
 name = "serde_repr"
 version = "0.1.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b2e6b945e9d3df726b65d6ee24060aff8e3533d431f677a9695db04eff9dfdb"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.49",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "serde_yaml"
-version = "0.9.33"
+version = "0.9.34+deprecated"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a0623d197252096520c6f2a5e1171ee436e5af99a5d7caa2891e55e61950e6d9"
+checksum = "6a8b1a1a2ebf674015cc02edccce75287f1a0130d394307b36743c2f5d504b47"
 dependencies = [
  "indexmap",
  "itoa",
  "ryu",
  "serde",
  "unsafe-libyaml",
 ]
@@ -1596,66 +1587,66 @@
 checksum = "d8229b473baa5980ac72ef434c4415e70c4b5e71b423043adb4ba059f89c99a1"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "similar"
-version = "2.4.0"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "32fea41aca09ee824cc9724996433064c89f7777e60762749a4170a14abbfa21"
+checksum = "fa42c91313f1d05da9b26f267f931cf178d4aba455b4c4622dd7355eb80c6640"
 
 [[package]]
 name = "slab"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f92a496fb766b417c996b9c5e57daf2f7ad3b0bebe1ccfca4856390e3d3bb67"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.13.1"
+version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e6ecd384b10a64542d77071bd64bd7b231f4ed5940fba55e98c3de13824cf3d7"
+checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "strsim"
-version = "0.11.0"
+version = "0.11.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5ee073c9e4cd00e28217186dbe12796d692868f432bf2e97ee73bed0c56dfa01"
+checksum = "7da8b5736845d9f2fcb837ea5d9e2628564b3b043a70948a3f0b778838c5fb4f"
 
 [[package]]
 name = "syn"
 version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.49"
+version = "2.0.57"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "915aea9e586f80826ee59f8453c1101f9d1c4b3964cd2460185ee8e299ada496"
+checksum = "11a6ae1e52eb25aab8f3fb9fca13be982a373b8f1157ca14b897a825ba4a2d35"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.13"
+version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "69758bda2e78f098e4ccb393021a0963bb3442eac05f135c30f61b7370bbafae"
+checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
 name = "tempfile"
 version = "3.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "85b77fafb263dd9d05cbeac119526425676db3784113aa9295c88498cbf8bff1"
 dependencies = [
@@ -1693,15 +1684,15 @@
 name = "thiserror-impl"
 version = "1.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c61f3ba182994efc43764a46c018c347bc492c79f024e705f46567b418f6d4f7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.49",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "thread_local"
 version = "1.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b9ef9bad013ada3808854ceac7b46812a6465ba368859a37e2100283d2d719c"
@@ -1733,17 +1724,17 @@
 name = "tinyvec_macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
 name = "tokio"
-version = "1.36.0"
+version = "1.37.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "61285f6515fa018fb2d1e46eb21223fff441ee8db5d0f1435e8ab4f5cdb80931"
+checksum = "1adbebffeca75fcfd058afa480fb6c0b81e165a0323f9c9d39c9697e37c46787"
 dependencies = [
  "backtrace",
  "bytes",
  "num_cpus",
  "pin-project-lite",
 ]
 
@@ -1825,15 +1816,15 @@
 name = "tower-lsp-macros"
 version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "84fd902d4e0b9a4b27f2f440108dc034e1758628a9b702f8ec61ad66355422fa"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.49",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "tower-service"
 version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b6bc1c9ce2b5135ac7f93c72918fc37feb872bdc6a5533a8b85eb4b86bfdae52"
@@ -1853,15 +1844,15 @@
 name = "tracing-attributes"
 version = "0.1.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "34704c8d6ebcbc939824180af020566b01a7c01f80641264eba0999f6c2b6be7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.49",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "tracing-core"
 version = "0.1.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c06d3da6113f116aaee68e4d601191614c9053067f9ab7f6edbcb161237daa54"
@@ -1896,14 +1887,24 @@
 checksum = "4bbd5f3d8658c08581f8f2adac6c391c2e9fa00fe9246bf6c5f52213b9cc6b72"
 dependencies = [
  "cc",
  "tree-sitter",
 ]
 
 [[package]]
+name = "tree-sitter-c-sharp"
+version = "0.20.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b9ab3dc608f34924fa9e10533a95f62dbc14b6de0ddd7107722eba66fe19ae31"
+dependencies = [
+ "cc",
+ "tree-sitter",
+]
+
+[[package]]
 name = "tree-sitter-cpp"
 version = "0.20.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "46b04a5ada71059afb9895966a6cc1094acc8d2ea1971006db26573e7dfebb74"
 dependencies = [
  "cc",
  "tree-sitter",
@@ -1959,18 +1960,18 @@
 checksum = "1ad6d11f19441b961af2fda7f12f5d0dac325f6d6de83836a1d3750018cc5114"
 dependencies = [
  "cc",
  "tree-sitter",
 ]
 
 [[package]]
-name = "tree-sitter-html-dvdb"
+name = "tree-sitter-html"
 version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1c6805488422bca82cc4d399e7b8177126b68287ff3d8ae209e4022c8fa44829"
+checksum = "017822b6bd42843c4bd67fabb834f61ce23254e866282dd93871350fd6b7fa1d"
 dependencies = [
  "cc",
  "tree-sitter",
 ]
 
 [[package]]
 name = "tree-sitter-java"
@@ -2102,17 +2103,17 @@
 name = "unicode-ident"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
 
 [[package]]
 name = "unicode-normalization"
-version = "0.1.22"
+version = "0.1.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5c5713f0fc4b5db668a2ac63cdb7bb4469d8c9fed047b1d0292cc7b0ce2ba921"
+checksum = "a56d1686db2308d901306f92a263857ef59ea39678a5458e7cb17f01415101f5"
 dependencies = [
  "tinyvec",
 ]
 
 [[package]]
 name = "unicode-segmentation"
 version = "1.11.0"
@@ -2162,99 +2163,99 @@
 checksum = "9f200f5b12eb75f8c1ed65abd4b2db8a6e1b138a20de009dacee265a2498f3f6"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "walkdir"
-version = "2.4.0"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d71d857dc86794ca4c280d616f7da00d2dbfd8cd788846559a6813e6aa4b54ee"
+checksum = "29790946404f91d9c5d06f9874efddea1dc06c5efe94541a7d6863108e3a5e4b"
 dependencies = [
  "same-file",
  "winapi-util",
 ]
 
 [[package]]
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.91"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1e124130aee3fb58c5bdd6b639a0509486b0338acaaae0c84a5124b0f588b7f"
+checksum = "4be2531df63900aeb2bca0daaaddec08491ee64ceecbee5076636a3b026795a8"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.91"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c9e7e1900c352b609c8488ad12639a311045f40a35491fb69ba8c12f758af70b"
+checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.49",
+ "syn 2.0.57",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-futures"
-version = "0.4.41"
+version = "0.4.42"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "877b9c3f61ceea0e56331985743b13f3d25c406a7098d45180fb5f09bc19ed97"
+checksum = "76bc14366121efc8dbb487ab05bcc9d346b3b5ec0eaa76e46594cabbe51762c0"
 dependencies = [
  "cfg-if",
  "js-sys",
  "wasm-bindgen",
  "web-sys",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.91"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b30af9e2d358182b5c7449424f017eba305ed32a7010509ede96cdc4696c46ed"
+checksum = "a1f8823de937b71b9460c0c34e25f3da88250760bec0ebac694b49997550d726"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.91"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "642f325be6301eb8107a83d12a8ac6c1e1c54345a7ef1a9261962dfefda09e66"
+checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.49",
+ "syn 2.0.57",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.91"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4f186bd2dcf04330886ce82d6f33dd75a7bfcf69ecf5763b89fcde53b6ac9838"
+checksum = "af190c94f2773fdb3729c55b007a722abb5384da03bc0986df4c289bf5567e96"
 
 [[package]]
 name = "web-sys"
-version = "0.3.68"
+version = "0.3.69"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "96565907687f7aceb35bc5fc03770a8a0471d82e479f25832f54a0e3f4b28446"
+checksum = "77afa9a11836342370f4817622a2f0f418b134426d91a82dfb48f532d2ec13ef"
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "web-tree-sitter-sg"
@@ -2309,15 +2310,15 @@
 
 [[package]]
 name = "windows-sys"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
 dependencies = [
- "windows-targets 0.52.0",
+ "windows-targets 0.52.4",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
@@ -2329,116 +2330,116 @@
  "windows_x86_64_gnu 0.48.5",
  "windows_x86_64_gnullvm 0.48.5",
  "windows_x86_64_msvc 0.48.5",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.52.0"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a18201040b24831fbb9e4eb208f8892e1f50a37feb53cc7ff887feb8f50e7cd"
+checksum = "7dd37b7e5ab9018759f893a1952c9420d060016fc19a472b4bb20d1bdd694d1b"
 dependencies = [
- "windows_aarch64_gnullvm 0.52.0",
- "windows_aarch64_msvc 0.52.0",
- "windows_i686_gnu 0.52.0",
- "windows_i686_msvc 0.52.0",
- "windows_x86_64_gnu 0.52.0",
- "windows_x86_64_gnullvm 0.52.0",
- "windows_x86_64_msvc 0.52.0",
+ "windows_aarch64_gnullvm 0.52.4",
+ "windows_aarch64_msvc 0.52.4",
+ "windows_i686_gnu 0.52.4",
+ "windows_i686_msvc 0.52.4",
+ "windows_x86_64_gnu 0.52.4",
+ "windows_x86_64_gnullvm 0.52.4",
+ "windows_x86_64_msvc 0.52.4",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.52.0"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cb7764e35d4db8a7921e09562a0304bf2f93e0a51bfccee0bd0bb0b666b015ea"
+checksum = "bcf46cf4c365c6f2d1cc93ce535f2c8b244591df96ceee75d8e83deb70a9cac9"
 
 [[package]]
 name = "windows_aarch64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.52.0"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bbaa0368d4f1d2aaefc55b6fcfee13f41544ddf36801e793edbbfd7d7df075ef"
+checksum = "da9f259dd3bcf6990b55bffd094c4f7235817ba4ceebde8e6d11cd0c5633b675"
 
 [[package]]
 name = "windows_i686_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.52.0"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a28637cb1fa3560a16915793afb20081aba2c92ee8af57b4d5f28e4b3e7df313"
+checksum = "b474d8268f99e0995f25b9f095bc7434632601028cf86590aea5c8a5cb7801d3"
 
 [[package]]
 name = "windows_i686_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.52.0"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ffe5e8e31046ce6230cc7215707b816e339ff4d4d67c65dffa206fd0f7aa7b9a"
+checksum = "1515e9a29e5bed743cb4415a9ecf5dfca648ce85ee42e15873c3cd8610ff8e02"
 
 [[package]]
 name = "windows_x86_64_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.52.0"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3d6fa32db2bc4a2f5abeacf2b69f7992cd09dca97498da74a151a3132c26befd"
+checksum = "5eee091590e89cc02ad514ffe3ead9eb6b660aedca2183455434b93546371a03"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.52.0"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1a657e1e9d3f514745a572a6846d3c7aa7dbe1658c056ed9c3344c4109a6949e"
+checksum = "77ca79f2451b49fa9e2af39f0747fe999fcda4f5e241b2898624dca97a1f2177"
 
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.52.0"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dff9641d1cd4be8d1a070daf9e3773c5f67e78b4d9d42263020c057706765c04"
+checksum = "32b752e52a2da0ddfbdbcc6fceadfeede4c939ed16d13e648833a61dfb611ed8"
 
 [[package]]
 name = "winnow"
-version = "0.6.2"
+version = "0.6.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7a4191c47f15cc3ec71fcb4913cb83d58def65dd3787610213c649283b5ce178"
+checksum = "dffa400e67ed5a4dd237983829e66475f0a4a26938c4b04c21baede6262215b8"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "xtask"
 version = "0.0.0"
```

### Comparing `ast_grep_py-0.20.2/Cargo.toml` & `ast_grep_py-0.20.3/Cargo.toml`

 * *Files 15% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 default-members = ["crates/*"]
 resolver = "2"
 
 [profile.release]
 lto = true
 
 [workspace.package]
-version = "0.20.2"
+version = "0.20.3"
 authors = ["Herrington Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com>"]
 edition = "2021"
 license = "MIT"
 documentation = "https://ast-grep.github.io/guide/introduction.html"
 homepage = "https://ast-grep.github.io/"
 repository = "https://github.com/ast-grep/ast-grep"
 rust-version = "1.63"
 readme = "README.md"
 
 [workspace.dependencies]
-ast-grep-core = { path = "crates/core", version = "0.20.2" }
-ast-grep-config = { path = "crates/config", version = "0.20.2" }
-ast-grep-dynamic = { path = "crates/dynamic", version = "0.20.2" }
-ast-grep-language = { path = "crates/language", version = "0.20.2" }
-ast-grep-lsp = { path = "crates/lsp", version = "0.20.2" }
+ast-grep-core = { path = "crates/core", version = "0.20.3" }
+ast-grep-config = { path = "crates/config", version = "0.20.3" }
+ast-grep-dynamic = { path = "crates/dynamic", version = "0.20.3" }
+ast-grep-language = { path = "crates/language", version = "0.20.3" }
+ast-grep-lsp = { path = "crates/lsp", version = "0.20.3" }
 
 bit-set = { version = "0.5.3" }
 ignore = { version = "0.4.22" }
 regex = { version = "1.10.4" }
 serde = { version = "1.0", features = ["derive"] }
 tree-sitter = { version = "0.9.2", package = "tree-sitter-facade-sg" }
 thiserror = "1.0.58"
```

### Comparing `ast_grep_py-0.20.2/pyproject.toml` & `ast_grep_py-0.20.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["maturin>=1.1,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "ast-grep-py"
 requires-python = ">=3.8"
-version = "0.20.2"
+version = "0.20.3"
 description = "Structural Search and Rewrite code at large scale using precise AST pattern."
 authors = [{ name = "Herrington Darkholme", email = "2883231+HerringtonDarkholme@users.noreply.github.com" }]
 maintainers = [{ name = "Herrington Darkholme", email = "2883231+HerringtonDarkholme@users.noreply.github.com" }]
 readme = "README.md"
 license = { text = "MIT" }
 keywords = [
   "ast",
```

### Comparing `ast_grep_py-0.20.2/ast_grep_py/__init__.py` & `ast_grep_py-0.20.3/ast_grep_py/__init__.py`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/ast_grep_py/ast_grep_py.pyi` & `ast_grep_py-0.20.3/ast_grep_py/ast_grep_py.pyi`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/README.md` & `ast_grep_py-0.20.3/README.md`

 * *Files identical despite different names*

### Comparing `ast_grep_py-0.20.2/PKG-INFO` & `ast_grep_py-0.20.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ast-grep-py
-Version: 0.20.2
+Version: 0.20.3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Rust
 Classifier: Topic :: Security
```

