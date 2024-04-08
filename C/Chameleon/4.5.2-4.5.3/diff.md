# Comparing `tmp/Chameleon-4.5.2.tar.gz` & `tmp/Chameleon-4.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Chameleon-4.5.2.tar", last modified: Mon Jan 29 20:56:20 2024, max compression
+gzip compressed data, was "Chameleon-4.5.3.tar", last modified: Fri Apr  5 06:12:15 2024, max compression
```

## Comparing `Chameleon-4.5.2.tar` & `Chameleon-4.5.3.tar`

### file list

```diff
@@ -1,426 +1,429 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 20:56:20.678569 Chameleon-4.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-01-29 20:56:19.000000 Chameleon-4.5.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    48653 2024-01-29 20:56:19.000000 Chameleon-4.5.2/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-01-29 20:56:19.000000 Chameleon-4.5.2/COPYRIGHT.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8496 2024-01-29 20:56:19.000000 Chameleon-4.5.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-01-29 20:56:19.000000 Chameleon-4.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-01-29 20:56:19.000000 Chameleon-4.5.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    50391 2024-01-29 20:56:20.678569 Chameleon-4.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-01-29 20:56:19.000000 Chameleon-4.5.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 20:56:20.618568 Chameleon-4.5.2/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-01-29 20:56:19.000000 Chameleon-4.5.2/benchmarks/bm_chameleon.py
--rw-r--r--   0 runner    (1001) docker     (127)     3874 2024-01-29 20:56:19.000000 Chameleon-4.5.2/benchmarks/bm_mako.py
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-01-29 20:56:19.000000 Chameleon-4.5.2/benchmarks/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 20:56:20.618568 Chameleon-4.5.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6803 2024-01-29 20:56:19.000000 Chameleon-4.5.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-01-29 20:56:19.000000 Chameleon-4.5.2/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7053 2024-01-29 20:56:19.000000 Chameleon-4.5.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-01-29 20:56:19.000000 Chameleon-4.5.2/docs/integration.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-01-29 20:56:19.000000 Chameleon-4.5.2/docs/library.rst
--rw-r--r--   0 runner    (1001) docker     (127)    53550 2024-01-29 20:56:19.000000 Chameleon-4.5.2/docs/reference.rst
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-01-29 20:56:19.000000 Chameleon-4.5.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-01-29 20:56:19.000000 Chameleon-4.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-01-29 20:56:20.678569 Chameleon-4.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-01-29 20:56:19.000000 Chameleon-4.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 20:56:20.614568 Chameleon-4.5.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 20:56:20.618568 Chameleon-4.5.2/src/Chameleon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    50391 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/Chameleon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15899 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/Chameleon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/Chameleon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/Chameleon.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/Chameleon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/Chameleon.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 20:56:20.622568 Chameleon-4.5.2/src/chameleon/
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3960 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/astutil.py
--rw-r--r--   0 runner    (1001) docker     (127)    15120 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/codegen.py
--rw-r--r--   0 runner    (1001) docker     (127)    59022 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9594 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/exc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/i18n.py
--rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/metal.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/namespaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     4884 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     7447 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/program.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    11594 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tal.py
--rw-r--r--   0 runner    (1001) docker     (127)    16365 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tales.py
--rw-r--r--   0 runner    (1001) docker     (127)    14332 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 20:56:20.626568 Chameleon-4.5.2/src/chameleon/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 20:56:20.658568 Chameleon-4.5.2/src/chameleon/tests/inputs/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/001-interpolation.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/001-variable-scope.html
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/001-variable-scope.pt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/001.xml
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/002-repeat-scope.pt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/002.xml
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/003-content.pt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/003.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/004-attributes.pt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/004.xml
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/005-default.pt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/005.xml
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/006-attribute-interpolation.pt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/006.xml
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/007-content-interpolation.pt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/007.xml
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/008-builtins.pt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/008.xml
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/009-literals.pt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/009.xml
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/010-structure.pt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/010.xml
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/011-messages.pt
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/011.xml
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/012-translation.pt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/012.xml
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/013-repeat-nested.pt
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/013.xml
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/014-repeat-nested-similar.pt
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/014.xml
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/015-translation-nested.pt
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/015.xml
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/016-explicit-translation.pt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/016.xml
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/017-omit-tag.pt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/017.xml
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/018-translation-nested-dynamic.pt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/018.xml
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/019-replace.pt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/019.xml
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/020-on-error.pt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/020.xml
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/021-translation-domain.pt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/021.xml
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/022-switch.pt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/022.xml
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/023-condition.pt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/023.xml
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/024-namespace-elements.pt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/024.xml
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/025-repeat-whitespace.pt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/025.xml
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/026-repeat-variable.pt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/026.xml
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/027-attribute-replacement.pt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/027.xml
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/028-attribute-toggle.pt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/028.xml
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/029-attribute-ordering.pt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/029.xml
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/030-repeat-tuples.pt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/030.xml
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/031-namespace-with-tal.pt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/031.xml
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/032-master-template.pt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/032.xml
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/033-use-macro-trivial.pt
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/033.xml
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/034-use-template-as-macro.pt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/034.xml
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/035-use-macro-with-fill-slot.pt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/035.xml
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/036-use-macro-inherits-dynamic-scope.pt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/036.xml
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/037-use-macro-local-variable-scope.pt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/037.xml
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/038-use-macro-globals.pt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/038.xml
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/039-globals.pt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/039.xml
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/040-macro-using-template-symbol.pt
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/040.xml
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/041-translate-nested-names.pt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/041.xml
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/042-use-macro-fill-footer.pt
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/042.xml
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/043-macro-nested-dynamic-vars.pt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/043.xml
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/044-tuple-define.pt
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/044.xml
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/045-namespaces.pt
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/045.xml
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/046-extend-macro.pt
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/046.xml
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/047-use-extended-macro.pt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/047.xml
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/048-use-extended-macro-fill-original.pt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/048.xml
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/049-entities-in-attributes.pt
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/049.xml
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/050-define-macro-and-use-not-extend.pt
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/050.xml
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/051-use-non-extended-macro.pt
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/051.xml
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/052-i18n-domain-inside-filled-slot.pt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/052.xml
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/053-special-characters-in-attributes.pt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/053.xml
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/054-import-expression.pt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/054.xml
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/055-attribute-fallback-to-dict-lookup.pt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/055.xml
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/056-comment-attribute.pt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/056.xml
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/057-order.pt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/057.xml
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/058-script.pt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/058.xml
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/059-embedded-javascript.pt
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/059.xml
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/060-macro-with-multiple-same-slots.pt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/060.xml
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/061-fill-one-slot-but-two-defined.pt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/061.xml
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/062-comments-and-expressions.pt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/062.xml
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/063-continuation.pt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/063.xml
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/064-tags-and-special-characters.pt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/064.xml
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/065-use-macro-in-fill.pt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/065.xml
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/066-load-expression.pt
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/066.xml
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/067-attribute-decode.pt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/067.xml
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/068-less-than-greater-than-in-attributes.pt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/068.xml
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/069-translation-domain-and-macro.pt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/069.xml
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/070-translation-domain-and-use-macro.pt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/070.xml
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/071-html-attribute-defaults.pt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/071.xml
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/072-repeat-interpolation.pt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/072.xml
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/073-utf8-encoded.pt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/073.xml
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/074-encoded-template.pt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/074.xml
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/075-nested-macros.pt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/075.xml
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/076-nested-macro-override.pt
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/076.xml
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/077-i18n-attributes.pt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/077.xml
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/078-tags-and-newlines.pt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/078.xml
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/079-implicit-i18n.pt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/079.xml
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/080-xmlns-namespace-on-tal.pt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/080.xml
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/081-load-spec.pt
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/081.xml
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/082-load-spec-computed.pt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/082.xml
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/083-template-dict-to-macro.pt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/083.xml
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/084-interpolation-in-cdata.pt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/084.xml
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/085-nested-translation.pt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/085.xml
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/086-self-closing.pt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/086.xml
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/087-code-blocks.pt
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/087.xml
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/088-python-newlines.pt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/088.xml
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/089-load-fallback.pt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/089.xml
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/090-tuple-expression.pt
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/090.xml
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/091-repeat-none.pt
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/091.xml
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/092.xml
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/093.xml
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/094.xml
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/095.xml
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/096.xml
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/097.xml
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/098.xml
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/099.xml
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/100.xml
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/101-unclosed-tags.html
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/101.xml
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/102-unquoted-attributes.html
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/102.xml
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/103-simple-attribute.html
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/103.xml
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/104.xml
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/105.xml
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/106.xml
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/107.xml
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/108.xml
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/109.xml
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/110.xml
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/111.xml
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/112.xml
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/113.xml
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/114.xml
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/115.xml
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/116.xml
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/117.xml
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/118.xml
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/119.xml
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/120-translation-context.pt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/121-translation-comment.pt
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/122-translation-ignore.pt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/123-html5-data-attributes.pt
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/124-translation-target.pt
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/125-macro-translation-ordering.pt
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/126-define-escaping.pt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/127-tags-and-attributes-special-chars.pt
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/237-double-define.pt
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/238-macroname.pt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/greeting.pt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-01-29 20:56:19.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/hello_world.pt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/hello_world.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/inputs/multinode-implicit-i18n.pt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 20:56:20.678569 Chameleon-4.5.2/src/chameleon/tests/outputs/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/001.html
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/001.pt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/001.txt
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/002.pt
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/003.pt
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/004.pt
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/005.pt
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/006.pt
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/007.pt
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/008.pt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/009.pt
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/010.pt
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/011-en.pt
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/011.pt
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/012-en.pt
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/012.pt
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/013.pt
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/014.pt
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/015-en.pt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/015.pt
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/016-en.pt
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/016.pt
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/017.pt
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/018-en.pt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/018.pt
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/019.pt
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/020.pt
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/021-en.pt
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/021.pt
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/022.pt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/023.pt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/024.pt
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/025.pt
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/026.pt
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/027.pt
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/028.pt
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/029.pt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/030.pt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/031.pt
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/032.pt
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/033.pt
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/034.pt
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/035.pt
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/036.pt
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/037.pt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/038.pt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/039.pt
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/040.pt
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/041.pt
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/042.pt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/043.pt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/044.pt
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/045.pt
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/046.pt
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/047.pt
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/048.pt
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/049.pt
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/050.pt
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/051.pt
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/052.pt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/053.pt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/054.pt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/055.pt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/056.pt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/057.pt
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/058.pt
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/059.pt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/060.pt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/061.pt
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/062.pt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/063.pt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/064.pt
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/065.pt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/066.pt
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/067.pt
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/068.pt
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/069-en.pt
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/069.pt
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/070-en.pt
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/070.pt
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/071.pt
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/072.pt
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/073.pt
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/074.pt
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/075.pt
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/076.pt
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/077-en.pt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/077.pt
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/078.pt
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/079-en.pt
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/079.pt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/080.pt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/081.pt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/082.pt
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/083.pt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/084.pt
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/085-en.pt
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/085.pt
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/086.pt
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/087.pt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/088.pt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/089.pt
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/090.pt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/091.pt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/101.html
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/102.html
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/103.html
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/120-en.pt
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/120.pt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/121.pt
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/122.pt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/123.pt
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/124-en.pt
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/124.pt
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/125.pt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/126.pt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/127.pt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/237.pt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/238.pt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/greeting.pt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/hello_world.pt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/hello_world.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/multinode-en.pt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/outputs/multinode.pt
--rw-r--r--   0 runner    (1001) docker     (127)    10636 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/test_bools_plus_sniffing.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/test_exc.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/test_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     7380 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/test_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/test_sniffing.py
--rw-r--r--   0 runner    (1001) docker     (127)    25600 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/test_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/test_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5176 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/tokenize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    13205 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 20:56:20.678569 Chameleon-4.5.2/src/chameleon/zpt/
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/zpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/zpt/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    28494 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/zpt/program.py
--rw-r--r--   0 runner    (1001) docker     (127)    17587 2024-01-29 20:56:20.000000 Chameleon-4.5.2/src/chameleon/zpt/template.py
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-01-29 20:56:20.000000 Chameleon-4.5.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 06:12:15.598334 Chameleon-4.5.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-05 06:12:13.000000 Chameleon-4.5.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    48957 2024-04-05 06:12:13.000000 Chameleon-4.5.3/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-05 06:12:13.000000 Chameleon-4.5.3/COPYRIGHT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8496 2024-04-05 06:12:13.000000 Chameleon-4.5.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-05 06:12:13.000000 Chameleon-4.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-04-05 06:12:13.000000 Chameleon-4.5.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    50920 2024-04-05 06:12:15.598334 Chameleon-4.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-05 06:12:13.000000 Chameleon-4.5.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 06:12:15.538334 Chameleon-4.5.3/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-04-05 06:12:13.000000 Chameleon-4.5.3/benchmarks/bm_chameleon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3874 2024-04-05 06:12:13.000000 Chameleon-4.5.3/benchmarks/bm_mako.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-05 06:12:13.000000 Chameleon-4.5.3/benchmarks/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 06:12:15.538334 Chameleon-4.5.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6803 2024-04-05 06:12:13.000000 Chameleon-4.5.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-05 06:12:13.000000 Chameleon-4.5.3/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7053 2024-04-05 06:12:13.000000 Chameleon-4.5.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-05 06:12:13.000000 Chameleon-4.5.3/docs/integration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-04-05 06:12:13.000000 Chameleon-4.5.3/docs/library.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    53550 2024-04-05 06:12:13.000000 Chameleon-4.5.3/docs/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-05 06:12:13.000000 Chameleon-4.5.3/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-05 06:12:13.000000 Chameleon-4.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-05 06:12:15.598334 Chameleon-4.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-05 06:12:13.000000 Chameleon-4.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 06:12:15.534334 Chameleon-4.5.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 06:12:15.538334 Chameleon-4.5.3/src/Chameleon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    50920 2024-04-05 06:12:15.000000 Chameleon-4.5.3/src/Chameleon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16029 2024-04-05 06:12:15.000000 Chameleon-4.5.3/src/Chameleon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 06:12:15.000000 Chameleon-4.5.3/src/Chameleon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 06:12:15.000000 Chameleon-4.5.3/src/Chameleon.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-05 06:12:15.000000 Chameleon-4.5.3/src/Chameleon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-05 06:12:15.000000 Chameleon-4.5.3/src/Chameleon.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 06:12:15.542334 Chameleon-4.5.3/src/chameleon/
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/astutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15120 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6357 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/codegen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59352 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9594 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/exc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4141 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/metal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4884 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7447 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/program.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    11594 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16365 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tales.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14363 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 06:12:15.546334 Chameleon-4.5.3/src/chameleon/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 06:12:15.578334 Chameleon-4.5.3/src/chameleon/tests/inputs/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/001-interpolation.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/001-variable-scope.html
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/001-variable-scope.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/001.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/002-repeat-scope.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/002.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/003-content.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/003.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/004-attributes.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/004.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/005-default.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/005.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/006-attribute-interpolation.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/006.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/007-content-interpolation.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/007.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/008-builtins.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/008.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/009-literals.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/009.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/010-structure.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/010.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/011-messages.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/011.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/012-translation.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/012.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/013-repeat-nested.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/013.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/014-repeat-nested-similar.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/014.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/015-translation-nested.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/015.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/016-explicit-translation.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/016.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/017-omit-tag.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/017.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/018-translation-nested-dynamic.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/018.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/019-replace.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/019.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/020-on-error.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/020.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/021-translation-domain.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/021.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/022-switch.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/022.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/023-condition.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/023.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/024-namespace-elements.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/024.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/025-repeat-whitespace.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/025.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/026-repeat-variable.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/026.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/027-attribute-replacement.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/027.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/028-attribute-toggle.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/028.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/029-attribute-ordering.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/029.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/030-repeat-tuples.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/030.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/031-namespace-with-tal.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/031.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/032-master-template.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/032.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/033-use-macro-trivial.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/033.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/034-use-template-as-macro.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/034.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/035-use-macro-with-fill-slot.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/035.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/036-use-macro-inherits-dynamic-scope.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/036.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/037-use-macro-local-variable-scope.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/037.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/038-use-macro-globals.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/038.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/039-globals.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/039.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/040-macro-using-template-symbol.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/040.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/041-translate-nested-names.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/041.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/042-use-macro-fill-footer.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/042.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/043-macro-nested-dynamic-vars.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/043.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/044-tuple-define.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/044.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/045-namespaces.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/045.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/046-extend-macro.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/046.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/047-use-extended-macro.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/047.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/048-use-extended-macro-fill-original.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/048.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/049-entities-in-attributes.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/049.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/050-define-macro-and-use-not-extend.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/050.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/051-use-non-extended-macro.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/051.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/052-i18n-domain-inside-filled-slot.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/052.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/053-special-characters-in-attributes.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/053.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/054-import-expression.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/054.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/055-attribute-fallback-to-dict-lookup.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/055.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/056-comment-attribute.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/056.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/057-order.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/057.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/058-script.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/058.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/059-embedded-javascript.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/059.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/060-macro-with-multiple-same-slots.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/060.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/061-fill-one-slot-but-two-defined.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/061.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/062-comments-and-expressions.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/062.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/063-continuation.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/063.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/064-tags-and-special-characters.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/064.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/065-use-macro-in-fill.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/065.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/066-load-expression.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/066.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/067-attribute-decode.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/067.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/068-less-than-greater-than-in-attributes.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/068.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/069-translation-domain-and-macro.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/069.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/070-translation-domain-and-use-macro.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/070.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/071-html-attribute-defaults.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/071.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/072-repeat-interpolation.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/072.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/073-utf8-encoded.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/073.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/074-encoded-template.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/074.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/075-nested-macros.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/075.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/076-nested-macro-override.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/076.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/077-i18n-attributes.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/077.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/078-tags-and-newlines.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/078.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/079-implicit-i18n.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/079.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/080-xmlns-namespace-on-tal.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/080.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/081-load-spec.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/081.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/082-load-spec-computed.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/082.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/083-template-dict-to-macro.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/083.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/084-interpolation-in-cdata.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/084.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/085-nested-translation.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/085.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/086-self-closing.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/086.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/087-code-blocks.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/087.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/088-python-newlines.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/088.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/089-load-fallback.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/089.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/090-tuple-expression.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/090.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/091-repeat-none.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/091.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/092.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/093.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/094.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/095.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/096.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/097.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/098.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/099.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/100.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/101-unclosed-tags.html
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/101.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/102-unquoted-attributes.html
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/102.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/103-simple-attribute.html
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/103.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/104.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/105.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/106.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/107.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/108.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/109.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/110.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/111.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/112.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/113.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/114.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/115.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/116.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/117.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/118.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/119.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/120-translation-context.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/121-translation-comment.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/122-translation-ignore.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/123-html5-data-attributes.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/124-translation-target.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/125-macro-translation-ordering.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/126-define-escaping.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/127-tags-and-attributes-special-chars.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/128-translation-macro-name.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/237-double-define.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/238-macroname.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/greeting.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/hello_world.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/hello_world.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/inputs/multinode-implicit-i18n.pt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 06:12:15.594334 Chameleon-4.5.3/src/chameleon/tests/outputs/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/001.html
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/001.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/001.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/002.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/003.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/004.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/005.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/006.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/007.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/008.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/009.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/010.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/011-en.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/011.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/012-en.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/012.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/013.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/014.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/015-en.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/015.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/016-en.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/016.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/017.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/018-en.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/018.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/019.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/020.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/021-en.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/021.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/022.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/023.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/024.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/025.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/026.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/027.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/028.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/029.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/030.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/031.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/032.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/033.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/034.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/035.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/036.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/037.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/038.pt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/039.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/040.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/041.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/042.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/043.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/044.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/045.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/046.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/047.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/048.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/049.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/050.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/051.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/052.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/053.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/054.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/055.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/056.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/057.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/058.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/059.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/060.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/061.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/062.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/063.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/064.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/065.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/066.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/067.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/068.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/069-en.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/069.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/070-en.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/070.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/071.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/072.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/073.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/074.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/075.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/076.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/077-en.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/077.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/078.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/079-en.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/079.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/080.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/081.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/082.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/083.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/084.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/085-en.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/085.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/086.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/087.pt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/088.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/089.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/090.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/091.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/101.html
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/102.html
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/103.html
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/120-en.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/120.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/121.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/122.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/123.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/124-en.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/124.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/125.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/126.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/127.pt
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/128-en.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/128.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/237.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/238.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/greeting.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/hello_world.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/hello_world.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/multinode-en.pt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/outputs/multinode.pt
+-rw-r--r--   0 runner    (1001) docker     (127)    10636 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/test_bools_plus_sniffing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/test_exc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7380 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/test_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/test_sniffing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25600 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/test_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/test_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5176 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13205 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 06:12:15.598334 Chameleon-4.5.3/src/chameleon/zpt/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/zpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/zpt/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28494 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/zpt/program.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17587 2024-04-05 06:12:13.000000 Chameleon-4.5.3/src/chameleon/zpt/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-05 06:12:13.000000 Chameleon-4.5.3/tox.ini
```

### Comparing `Chameleon-4.5.2/.readthedocs.yaml` & `Chameleon-4.5.3/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `Chameleon-4.5.2/CHANGES.rst` & `Chameleon-4.5.3/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 Changes
 =======
 
+4.5.3 (2024-04-05)
+------------------
+
+- Minor optimization when rendering translations with a static
+  message id (don't need to test if it's non-empty).
+
+- Fix a bug where a macro could not be used correctly to render a
+  translation name.
+  (`#419 <https://github.com/malthe/chameleon/issues/419>`_)
+
 4.5.2 (2024-01-29)
 ------------------
 
 - Fix a regression where a static symbol would not get correctly
   imported.
   (`#414 <https://github.com/malthe/chameleon/issues/414>`_)
```

### Comparing `Chameleon-4.5.2/LICENSE.txt` & `Chameleon-4.5.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Chameleon-4.5.2/Makefile` & `Chameleon-4.5.3/Makefile`

 * *Files identical despite different names*

### Comparing `Chameleon-4.5.2/PKG-INFO` & `Chameleon-4.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Chameleon
-Version: 4.5.2
+Version: 4.5.3
 Summary: Fast HTML/XML Template Compiler.
 Home-page: https://chameleon.readthedocs.io
 Author: Malthe Borch
 Author-email: mborch@gmail.com
 License: BSD-like (http://repoze.org/license.html)
 Project-URL: Documentation, https://chameleon.readthedocs.io
 Project-URL: Issue Tracker, https://github.com/malthe/chameleon/issues
@@ -21,16 +21,21 @@
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.9
 Provides-Extra: docs
 License-File: LICENSE.txt
 
-Overview
-========
+Chameleon
+=========
+
+.. image:: https://img.shields.io/pypi/pyversions/Chameleon
+   :alt: PyPI - Python Version
+.. image:: https://img.shields.io/github/actions/workflow/status/malthe/chameleon/main.yml
+   :alt: GitHub Actions Workflow Status
 
 Chameleon is an HTML/XML template engine for `Python
 <http://www.python.org>`_. It uses the *page templates* language.
 
 You can use it in any Python application with just about any
 version of Python (3.9+ and up, plus `pypy 3
 <http://pypy.org>`_).
@@ -51,14 +56,24 @@
 .. [1] This software is licensed under the `Repoze
        <http://repoze.org/license.html>`_ license.
 
 
 Changes
 =======
 
+4.5.3 (2024-04-05)
+------------------
+
+- Minor optimization when rendering translations with a static
+  message id (don't need to test if it's non-empty).
+
+- Fix a bug where a macro could not be used correctly to render a
+  translation name.
+  (`#419 <https://github.com/malthe/chameleon/issues/419>`_)
+
 4.5.2 (2024-01-29)
 ------------------
 
 - Fix a regression where a static symbol would not get correctly
   imported.
   (`#414 <https://github.com/malthe/chameleon/issues/414>`_)
```

### Comparing `Chameleon-4.5.2/README.rst` & `Chameleon-4.5.3/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,14 @@
-Overview
-========
+Chameleon
+=========
+
+.. image:: https://img.shields.io/pypi/pyversions/Chameleon
+   :alt: PyPI - Python Version
+.. image:: https://img.shields.io/github/actions/workflow/status/malthe/chameleon/main.yml
+   :alt: GitHub Actions Workflow Status
 
 Chameleon is an HTML/XML template engine for `Python
 <http://www.python.org>`_. It uses the *page templates* language.
 
 You can use it in any Python application with just about any
 version of Python (3.9+ and up, plus `pypy 3
 <http://pypy.org>`_).
```

### Comparing `Chameleon-4.5.2/benchmarks/bm_chameleon.py` & `Chameleon-4.5.3/benchmarks/bm_chameleon.py`

 * *Files identical despite different names*

### Comparing `Chameleon-4.5.2/benchmarks/bm_mako.py` & `Chameleon-4.5.3/benchmarks/bm_mako.py`

 * *Files identical despite different names*

### Comparing `Chameleon-4.5.2/benchmarks/util.py` & `Chameleon-4.5.3/benchmarks/util.py`

 * *Files identical despite different names*

### Comparing `Chameleon-4.5.2/docs/conf.py` & `Chameleon-4.5.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `Chameleon-4.5.2/docs/configuration.rst` & `Chameleon-4.5.3/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `Chameleon-4.5.2/docs/index.rst` & `Chameleon-4.5.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `Chameleon-4.5.2/docs/integration.rst` & `Chameleon-4.5.3/docs/integration.rst`

 * *Files identical despite different names*

### Comparing `Chameleon-4.5.2/docs/library.rst` & `Chameleon-4.5.3/docs/library.rst`

 * *Files identical despite different names*

### Comparing `Chameleon-4.5.2/docs/reference.rst` & `Chameleon-4.5.3/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `Chameleon-4.5.2/pyproject.toml` & `Chameleon-4.5.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 build-backend = "setuptools.build_meta"
 
 [tool.mypy]
 mypy_path = "$MYPY_CONFIG_FILE_DIR/src"
 # we may want to include tests eventually
 exclude = "/tests/"
 follow_imports = "silent"
+warn_redundant_casts = true
+warn_unused_configs = true
+warn_unused_ignores = true
+warn_return_any = true
 
 [[tool.mypy.overrides]]
 # strict config for fully typed modules and public API
 module = [
     "chameleon.exc.*",
     "chameleon.utils.*",
     "chameleon.zpt.loader.*",
@@ -19,12 +23,14 @@
 disallow_any_unimported = true
 disallow_any_generics = true
 disallow_subclassing_any = true
 disallow_untyped_calls = true
 disallow_untyped_defs = true
 disallow_incomplete_defs = true
 disallow_untyped_decorators = true
-warn_unused_ignores = true
+no_implicit_reexport = true
+strict_equality = true
+extra_checks = true
 
 [[tool.mypy.overrides]]
 module = ["zope.*"]
 ignore_missing_imports = true
```

### Comparing `Chameleon-4.5.2/setup.py` & `Chameleon-4.5.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '4.5.2'
+__version__ = '4.5.3'
 
 import os
 
 from setuptools import find_packages
 from setuptools import setup
 from setuptools.command.test import test
```

### Comparing `Chameleon-4.5.2/src/Chameleon.egg-info/PKG-INFO` & `Chameleon-4.5.3/src/Chameleon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Chameleon
-Version: 4.5.2
+Version: 4.5.3
 Summary: Fast HTML/XML Template Compiler.
 Home-page: https://chameleon.readthedocs.io
 Author: Malthe Borch
 Author-email: mborch@gmail.com
 License: BSD-like (http://repoze.org/license.html)
 Project-URL: Documentation, https://chameleon.readthedocs.io
 Project-URL: Issue Tracker, https://github.com/malthe/chameleon/issues
@@ -21,16 +21,21 @@
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.9
 Provides-Extra: docs
 License-File: LICENSE.txt
 
-Overview
-========
+Chameleon
+=========
+
+.. image:: https://img.shields.io/pypi/pyversions/Chameleon
+   :alt: PyPI - Python Version
+.. image:: https://img.shields.io/github/actions/workflow/status/malthe/chameleon/main.yml
+   :alt: GitHub Actions Workflow Status
 
 Chameleon is an HTML/XML template engine for `Python
 <http://www.python.org>`_. It uses the *page templates* language.
 
 You can use it in any Python application with just about any
 version of Python (3.9+ and up, plus `pypy 3
 <http://pypy.org>`_).
@@ -51,14 +56,24 @@
 .. [1] This software is licensed under the `Repoze
        <http://repoze.org/license.html>`_ license.
 
 
 Changes
 =======
 
+4.5.3 (2024-04-05)
+------------------
+
+- Minor optimization when rendering translations with a static
+  message id (don't need to test if it's non-empty).
+
+- Fix a bug where a macro could not be used correctly to render a
+  translation name.
+  (`#419 <https://github.com/malthe/chameleon/issues/419>`_)
+
 4.5.2 (2024-01-29)
 ------------------
 
 - Fix a regression where a static symbol would not get correctly
   imported.
   (`#414 <https://github.com/malthe/chameleon/issues/414>`_)
```

### Comparing `Chameleon-4.5.2/src/Chameleon.egg-info/SOURCES.txt` & `Chameleon-4.5.3/src/Chameleon.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -275,14 +275,15 @@
 src/chameleon/tests/inputs/121-translation-comment.pt
 src/chameleon/tests/inputs/122-translation-ignore.pt
 src/chameleon/tests/inputs/123-html5-data-attributes.pt
 src/chameleon/tests/inputs/124-translation-target.pt
 src/chameleon/tests/inputs/125-macro-translation-ordering.pt
 src/chameleon/tests/inputs/126-define-escaping.pt
 src/chameleon/tests/inputs/127-tags-and-attributes-special-chars.pt
+src/chameleon/tests/inputs/128-translation-macro-name.pt
 src/chameleon/tests/inputs/237-double-define.pt
 src/chameleon/tests/inputs/238-macroname.pt
 src/chameleon/tests/inputs/greeting.pt
 src/chameleon/tests/inputs/hello_world.pt
 src/chameleon/tests/inputs/hello_world.txt
 src/chameleon/tests/inputs/multinode-implicit-i18n.pt
 src/chameleon/tests/outputs/001.html
@@ -398,14 +399,16 @@
 src/chameleon/tests/outputs/122.pt
 src/chameleon/tests/outputs/123.pt
 src/chameleon/tests/outputs/124-en.pt
 src/chameleon/tests/outputs/124.pt
 src/chameleon/tests/outputs/125.pt
 src/chameleon/tests/outputs/126.pt
 src/chameleon/tests/outputs/127.pt
+src/chameleon/tests/outputs/128-en.pt
+src/chameleon/tests/outputs/128.pt
 src/chameleon/tests/outputs/237.pt
 src/chameleon/tests/outputs/238.pt
 src/chameleon/tests/outputs/greeting.pt
 src/chameleon/tests/outputs/hello_world.pt
 src/chameleon/tests/outputs/hello_world.txt
 src/chameleon/tests/outputs/multinode-en.pt
 src/chameleon/tests/outputs/multinode.pt
```

### Comparing `Chameleon-4.5.2/src/chameleon/astutil.py` & `Chameleon-4.5.3/src/chameleon/astutil.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,57 +1,66 @@
 """Support code for generating code from abstract syntax trees."""
 
 from __future__ import annotations
 
 import ast
 from copy import deepcopy
 from typing import TYPE_CHECKING
+from typing import Any
 from typing import ClassVar
 
 
 if TYPE_CHECKING:
     from collections.abc import Callable
-    from typing import Union
-    _NodeTransform = Callable[[ast.AST], Union[ast.AST, None]]
+    from collections.abc import Hashable
+    from typing import Optional
+
+    from chameleon.tokenize import Token
+
+    _NodeTransform = Callable[[ast.AST], Optional[ast.AST]]
 
 
 __docformat__ = 'restructuredtext en'
 
 
-def parse(source, mode='eval'):
+def parse(source, mode: str = 'eval') -> ast.AST:
     return compile(source, '', mode, ast.PyCF_ONLY_AST)
 
 
-def load(name):
+def load(name: str) -> ast.Name:
     return ast.Name(id=name, ctx=ast.Load())
 
 
-def store(name):
+def store(name: str) -> ast.Name:
     return ast.Name(id=name, ctx=ast.Store())
 
 
-def param(name):
+def param(name: str) -> ast.Name:
     return ast.Name(id=name, ctx=ast.Param())
 
 
-def subscript(name, value, ctx):
+def subscript(
+    name: str,
+    value: ast.expr,
+    ctx: ast.expr_context
+) -> ast.Subscript:
     return ast.Subscript(
         value=value,
         slice=ast.Index(value=ast.Str(s=name)),
         ctx=ctx,
     )
 
 
 class Node(ast.AST):
     """AST baseclass that gives us a convenient initialization
     method. We explicitly declare and use the ``_fields`` attribute."""
 
     _fields: ClassVar[tuple[str, ...]] = ()
 
-    def __init__(self, *args, **kwargs) -> None:
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
         assert isinstance(self._fields, tuple)
         self.__dict__.update(kwargs)
         for name, value in zip(self._fields, args):
             setattr(self, name, value)
 
     def __repr__(self) -> str:
         """Poor man's single-line pretty printer."""
@@ -73,40 +82,49 @@
     Used when a builtin is used internally by the compiler, to avoid
     clashing with a user assignment (e.g. ``help`` is a builtin, but
     also commonly assigned in templates).
     """
 
     _fields = "id", "ctx"
 
+    id: str
     ctx = ast.Load()
 
 
 class Symbol(Node):
     """Represents an importable symbol."""
 
     _fields = "value",
 
+    # Apart from a few builtins this should be type[Any]
+    value: type[Any] | Hashable
+
 
 class Static(Node):
     """Represents a static value."""
 
     _fields = "value", "name"
 
-    name = None
+    value: ast.expr
+    name: str | None = None
 
 
 class Comment(Node):
     _fields = "text",
 
+    text: str
+
 
 class TokenRef(Node):
     """Represents a source-code token reference."""
 
     _fields = "token",
 
+    token: Token
+
 
 class NodeTransformerBase(ast.NodeTransformer):
     def __init__(self, transform: _NodeTransform):
         self.transform = transform
 
     def apply_transform(self, node: ast.AST) -> ast.AST:
         result = self.transform(node)
@@ -116,46 +134,46 @@
 
 
 class NameLookupRewriteVisitor(NodeTransformerBase):
     def __init__(self, transform: _NodeTransform):
         self.scopes: list[set[str]] = [set()]
         super().__init__(transform)
 
-    def __call__(self, node) -> ast.AST:
+    def __call__(self, node: ast.AST) -> ast.AST:
         clone = deepcopy(node)
-        return self.visit(clone)
+        return self.visit(clone)  # type: ignore[no-any-return]
 
-    def visit_arg(self, node) -> ast.AST:
+    def visit_arg(self, node: ast.arg) -> ast.AST:
         scope = self.scopes[-1]
         scope.add(node.arg)
         return node
 
-    def visit_Name(self, node) -> ast.AST:
+    def visit_Name(self, node: ast.Name) -> ast.AST:
         scope = self.scopes[-1]
         if isinstance(node.ctx, ast.Param):
             scope.add(node.id)
             return node
         if node.id not in scope:
-            node = self.apply_transform(node)
+            return self.apply_transform(node)
         return node
 
-    def visit_FunctionDef(self, node) -> ast.AST:
+    def visit_FunctionDef(self, node: ast.FunctionDef) -> ast.AST:
         self.scopes[-1].add(node.name)
         return super().generic_visit(node)
 
-    def visit_alias(self, node) -> ast.AST:
+    def visit_alias(self, node: ast.alias) -> ast.AST:
         name = node.asname if node.asname is not None else node.name
         self.scopes[-1].add(name)
         return super().generic_visit(node)
 
-    def visit_Lambda(self, node) -> ast.AST:
+    def visit_Lambda(self, node: ast.Lambda) -> ast.AST:
         self.scopes.append(set())
         try:
             return super().generic_visit(node)
         finally:
             self.scopes.pop()
 
 
 class ItemLookupOnAttributeErrorVisitor(NodeTransformerBase):
-    def visit_Attribute(self, node) -> ast.AST:
-        node = self.apply_transform(node)
-        return self.generic_visit(node)
+    def visit_Attribute(self, node: ast.Attribute) -> ast.AST:
+        transformed = self.apply_transform(node)
+        return self.generic_visit(transformed)
```

### Comparing `Chameleon-4.5.2/src/chameleon/benchmark.py` & `Chameleon-4.5.3/src/chameleon/benchmark.py`

 * *Files identical despite different names*

### Comparing `Chameleon-4.5.2/src/chameleon/codegen.py` & `Chameleon-4.5.3/src/chameleon/codegen.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,24 +11,34 @@
 from ast import FunctionDef
 from ast import Import
 from ast import ImportFrom
 from ast import Module
 from ast import NodeTransformer
 from ast import alias
 from ast import unparse
+from typing import TYPE_CHECKING
+from typing import Any
 
 from chameleon.astutil import Builtin
 from chameleon.astutil import Symbol
 from chameleon.astutil import load
 from chameleon.astutil import parse
 from chameleon.astutil import store
 from chameleon.exc import CompilationError
 
 
-reverse_builtin_map = {}
+if TYPE_CHECKING:
+    import ast
+    from collections.abc import Hashable
+
+    from chameleon.astutil import Comment
+    from chameleon.astutil import Static
+
+
+reverse_builtin_map: dict[type[Any] | Hashable, str] = {}
 for name, value in builtins.__dict__.items():
     try:
         hash(value)
     except TypeError:
         continue
 
     reverse_builtin_map[value] = name
@@ -56,15 +66,15 @@
                     name=name,
                     args=node.args,
                     body=list(map(self.visit, node.body)),
                     decorator_list=getattr(node, "decorator_list", []),
                     lineno=None,
                 )
 
-            def visit_Name(self, node) -> AST:
+            def visit_Name(self, node: ast.Name) -> AST:
                 value = symbols.get(node.id, self)
                 if value is self:
                     if node.id == 'None' or \
                        getattr(builtins, node.id, None) is not None:
                         return Builtin(node.id)
                     return node
 
@@ -73,15 +83,15 @@
                     if name is not None:
                         return Builtin(name)
                     return Symbol(value)
 
                 if isinstance(value, str):
                     value = load(value)
 
-                return value
+                return value  # type: ignore[no-any-return]
 
         expr = parse(textwrap.dedent(source), mode=mode)
 
         Transformer().visit(expr)
         return expr.body
 
     assert isinstance(source, str)
@@ -99,14 +109,16 @@
     The syntax tree has been extended with internal nodes. We first
     transform the tree to process the internal nodes before generating
     the code string.
     """
 
     names = ()
 
+    imports: dict[type[Any] | Hashable, ast.Name]
+
     def __init__(self, tree):
         self.comments = []
         self.defines = {}
         self.imports = {}
 
         # Run transform.
         tree = self.visit(tree)
@@ -138,30 +150,30 @@
             self.defines[name] = node
         else:
             raise CompilationError(
                 "Duplicate symbol name for define.", name)
 
         return load(name)
 
-    def require(self, value):
+    def require(self, value: type[Any] | Hashable) -> ast.Name:
         node = self.imports.get(value)
         if node is None:
             # we come up with a unique symbol based on the class name
             name = (
                 "_%s"
                 % getattr(value, '__name__', str(value)).rsplit('.', 1)[-1]
             )
             node = load(name)
             self.imports[value] = store(node.id)
 
         return node
 
-    def visit_Module(self, module) -> AST:
+    def visit_Module(self, module: Module) -> AST:
         assert isinstance(module, Module)
-        module = super().generic_visit(module)
+        module = super().generic_visit(module)  # type: ignore[assignment]
         preamble: list[AST] = []
 
         for name, node in self.defines.items():
             assignment = Assign(targets=[store(name)], value=node, lineno=None)
             preamble.append(self.visit(assignment))
 
         imports: list[AST] = []
@@ -184,25 +196,25 @@
             else:
                 raise TypeError(value)
 
             imports.append(stmt)
 
         return Module(imports + preamble + module.body, ())
 
-    def visit_Comment(self, node) -> AST:
+    def visit_Comment(self, node: Comment) -> AST:
         self.comments.append(node.text)
         return Expr(Constant(...))
 
-    def visit_Builtin(self, node) -> AST:
+    def visit_Builtin(self, node: Builtin) -> AST:
         name = load(node.id)
-        return self.visit(name)
+        return self.visit(name)  # type: ignore[no-any-return]
 
-    def visit_Symbol(self, node) -> AST:
+    def visit_Symbol(self, node: Symbol) -> AST:
         return self.require(node.value)
 
-    def visit_Static(self, node) -> AST:
+    def visit_Static(self, node: Static) -> AST:
         if node.name is None:
             name = "_static_%s" % str(id(node.value)).replace('-', '_')
         else:
             name = node.name
         node = self.define(name, node.value)
-        return self.visit(node)
+        return self.visit(node)  # type: ignore[no-any-return]
```

### Comparing `Chameleon-4.5.2/src/chameleon/compiler.py` & `Chameleon-4.5.3/src/chameleon/compiler.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,32 +58,32 @@
     "rcontext",
 }
 
 RE_MANGLE = re.compile(r'[^\w_]')
 RE_NAME = re.compile('^%s$' % NAME)
 
 
-def identifier(prefix, suffix=None) -> str:
+def identifier(prefix: str, suffix: str | None = None) -> str:
     return "__{}_{}".format(prefix, mangle(suffix or id(prefix)))
 
 
-def mangle(string):
+def mangle(string: int | str) -> str:
     return RE_MANGLE.sub('_', str(string)).replace('\n', '').replace('-', '_')
 
 
 def load_econtext(name):
     return template("getname(KEY)", KEY=ast.Str(s=name), mode="eval")
 
 
-def store_econtext(name):
+def store_econtext(name: object) -> ast.Subscript:
     name = str(name)
     return subscript(name, load("econtext"), ast.Store())
 
 
-def store_rcontext(name):
+def store_rcontext(name: object) -> ast.Subscript:
     name = str(name)
     return subscript(name, load("rcontext"), ast.Store())
 
 
 def eval_token(token):
     try:
         line, column = token.location
@@ -97,15 +97,15 @@
         string=ast.Str(s=string),
         line=ast.Num(n=line),
         col=ast.Num(n=column),
         mode="eval"
     )
 
 
-def indent(s):
+def indent(s: str | None) -> str:
     return textwrap.indent(s, "    ") if s else ""
 
 
 emit_node_if_non_trivial = template(is_func=True, func_args=('node',),
                                     source=r"""
     if node is not None:
         __append(node)
@@ -1020,24 +1020,24 @@
 
         class Generator(TemplateCodeGenerator):
             scopes = [TranslationContext()]
             tokens = []
 
             def visit_EmitText(self, node) -> ast.AST:
                 append = load(self.scopes[-1].append or "__append")
-                node = ast.Expr(ast.Call(
+                expr = ast.Expr(ast.Call(
                     func=append,
                     args=[ast.Str(s=node.s)],
                     keywords=[],
                     starargs=None,
                     kwargs=None
                 ))
-                return self.visit(node)
+                return self.visit(expr)  # type: ignore[no-any-return]
 
-            def visit_Name(self, node) -> ast.AST:
+            def visit_Name(self, node: ast.Name) -> ast.AST:
                 if isinstance(node.ctx, ast.Load):
                     scope = self.scopes[-1]
                     for name in ("append", "stream"):
                         if node.id == f"__{name}":
                             identifier = getattr(scope, name, None)
                             if identifier:
                                 return load(identifier)
@@ -1045,15 +1045,15 @@
 
             def visit_TranslationContext(self, node) -> list[ast.AST]:
                 self.scopes.append(node)
                 stmts = list(map(self.visit, node.body))
                 self.scopes.pop()
                 return stmts
 
-            def visit_TokenRef(self, node) -> ast.AST:
+            def visit_TokenRef(self, node: TokenRef) -> ast.AST:
                 self.tokens.append((node.token.pos, len(node.token)))
                 return ast.Assign(
                     [store("__token")],
                     ast.Num(n=node.token.pos),
                     lineno=None,
                 )
 
@@ -1488,21 +1488,28 @@
             mapping = None
 
         # if this translation node has a name, use it as the message id
         if node.msgid:
             msgid = ast.Str(s=node.msgid)
 
         # emit the translation expression
-        body += template(
-            "if msgid: __append(translate("
+        translation = template(
+            "__append(translate("
             "msgid, mapping=mapping, default=default, domain=__i18n_domain, context=__i18n_context, target_language=target_language))",  # noqa:  E501 line too long
             msgid=msgid,
             default=default,
             mapping=mapping)
 
+        if not node.msgid:
+            translation = [ast.If(
+                test=load(msgid), body=translation, orelse=[]
+            )]
+
+        body += translation
+
         # pop away translation block reference
         self._translations.pop()
 
         return body
 
     def visit_Start(self, node):
         try:
@@ -1699,15 +1706,15 @@
         # prepare new stream
         stream, append = self._get_translation_identifiers(node.name)
         body += template("s = new_list", s=stream, new_list=self._new_list) + \
             template("a = s.append", a=append, s=stream)
 
         # generate code
         code = self.visit(node.node)
-        body.append(TranslationContext(code, append))
+        body.append(TranslationContext(code, append, stream))
 
         # output msgid
         text = Text('${%s}' % node.name)
         body += self.visit(text)
 
         # Concatenate stream
         body += template("stream = ''.join(stream)", stream=stream)
```

### Comparing `Chameleon-4.5.2/src/chameleon/config.py` & `Chameleon-4.5.3/src/chameleon/config.py`

 * *Files identical despite different names*

### Comparing `Chameleon-4.5.2/src/chameleon/exc.py` & `Chameleon-4.5.3/src/chameleon/exc.py`

 * *Files identical despite different names*

### Comparing `Chameleon-4.5.2/src/chameleon/i18n.py` & `Chameleon-4.5.3/src/chameleon/i18n.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,19 +65,19 @@
         default: str | None = None
     ) -> str | None:
 
         if msgid is None:
             return None
 
         if target_language is not None or context is not None:
-            result = translate(
+            result: str = translate(
                 msgid, domain=domain, mapping=mapping, context=context,
                 target_language=target_language, default=default)
             if result != msgid:
-                return result  # type: ignore[no-any-return]
+                return result
 
         if isinstance(msgid, Message):
             default = msgid.default
             mapping = msgid.mapping
 
         if default is None:
             default = str(msgid)
```

### Comparing `Chameleon-4.5.2/src/chameleon/loader.py` & `Chameleon-4.5.3/src/chameleon/loader.py`

 * *Files identical despite different names*

### Comparing `Chameleon-4.5.2/src/chameleon/metal.py` & `Chameleon-4.5.3/src/chameleon/metal.py`

 * *Files identical despite different names*

### Comparing `Chameleon-4.5.2/src/chameleon/nodes.py` & `Chameleon-4.5.3/src/chameleon/nodes.py`

 * *Files identical despite different names*

### Comparing `Chameleon-4.5.2/src/chameleon/parser.py` & `Chameleon-4.5.3/src/chameleon/parser.py`

 * *Files identical despite different names*

### Comparing `Chameleon-4.5.2/src/chameleon/program.py` & `Chameleon-4.5.3/src/chameleon/program.py`

 * *Files identical despite different names*

### Comparing `Chameleon-4.5.2/src/chameleon/tal.py` & `Chameleon-4.5.3/src/chameleon/tal.py`

 * *Files identical despite different names*

### Comparing `Chameleon-4.5.2/src/chameleon/tales.py` & `Chameleon-4.5.3/src/chameleon/tales.py`

 * *Files identical despite different names*

### Comparing `Chameleon-4.5.2/src/chameleon/template.py` & `Chameleon-4.5.3/src/chameleon/template.py`

 * *Files 1% similar despite different names*

```diff
@@ -338,15 +338,15 @@
             self.engine,
             module,
             str(self.filename),
             body,
             builtins=builtins,
             strict=self.strict
         )
-        return compiler.code
+        return compiler.code  # type: ignore[no-any-return]
 
 
 class BaseTemplateFile(BaseTemplate):
     """File-based template base class.
 
     Relative path names are supported only when a template loader is
     provided as the ``loader`` parameter.
```

### Comparing `Chameleon-4.5.2/src/chameleon/tests/inputs/004-attributes.pt` & `Chameleon-4.5.3/src/chameleon/tests/inputs/004-attributes.pt`

 * *Files identical despite different names*

### Comparing `Chameleon-4.5.2/src/chameleon/tests/inputs/012-translation.pt` & `Chameleon-4.5.3/src/chameleon/tests/inputs/012-translation.pt`

 * *Files identical despite different names*

### Comparing `Chameleon-4.5.2/src/chameleon/tests/inputs/022-switch.pt` & `Chameleon-4.5.3/src/chameleon/tests/inputs/022-switch.pt`

 * *Files identical despite different names*

### Comparing `Chameleon-4.5.2/src/chameleon/tests/inputs/026-repeat-variable.pt` & `Chameleon-4.5.3/src/chameleon/tests/inputs/026-repeat-variable.pt`

 * *Files identical despite different names*

### Comparing `Chameleon-4.5.2/src/chameleon/tests/inputs/032-master-template.pt` & `Chameleon-4.5.3/src/chameleon/tests/inputs/032-master-template.pt`

 * *Files identical despite different names*

### Comparing `Chameleon-4.5.2/src/chameleon/tests/inputs/040-macro-using-template-symbol.pt` & `Chameleon-4.5.3/src/chameleon/tests/inputs/040-macro-using-template-symbol.pt`

 * *Files identical despite different names*

### Comparing `Chameleon-4.5.2/src/chameleon/tests/inputs/045-namespaces.pt` & `Chameleon-4.5.3/src/chameleon/tests/inputs/045-namespaces.pt`

 * *Files identical despite different names*

### Comparing `Chameleon-4.5.2/src/chameleon/tests/inputs/071-html-attribute-defaults.pt` & `Chameleon-4.5.3/src/chameleon/tests/inputs/071-html-attribute-defaults.pt`

 * *Files identical despite different names*

### Comparing `Chameleon-4.5.2/src/chameleon/tests/inputs/078-tags-and-newlines.pt` & `Chameleon-4.5.3/src/chameleon/tests/inputs/078-tags-and-newlines.pt`

 * *Files identical despite different names*

### Comparing `Chameleon-4.5.2/src/chameleon/tests/inputs/079-implicit-i18n.pt` & `Chameleon-4.5.3/src/chameleon/tests/inputs/079-implicit-i18n.pt`

 * *Files identical despite different names*

### Comparing `Chameleon-4.5.2/src/chameleon/tests/outputs/004.pt` & `Chameleon-4.5.3/src/chameleon/tests/outputs/004.pt`

 * *Files identical despite different names*

### Comparing `Chameleon-4.5.2/src/chameleon/tests/outputs/079-en.pt` & `Chameleon-4.5.3/src/chameleon/tests/outputs/079-en.pt`

 * *Files identical despite different names*

### Comparing `Chameleon-4.5.2/src/chameleon/tests/test_bools_plus_sniffing.py` & `Chameleon-4.5.3/src/chameleon/tests/test_bools_plus_sniffing.py`

 * *Files identical despite different names*

### Comparing `Chameleon-4.5.2/src/chameleon/tests/test_exc.py` & `Chameleon-4.5.3/src/chameleon/tests/test_exc.py`

 * *Files identical despite different names*

### Comparing `Chameleon-4.5.2/src/chameleon/tests/test_imports.py` & `Chameleon-4.5.3/src/chameleon/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `Chameleon-4.5.2/src/chameleon/tests/test_loader.py` & `Chameleon-4.5.3/src/chameleon/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `Chameleon-4.5.2/src/chameleon/tests/test_parser.py` & `Chameleon-4.5.3/src/chameleon/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `Chameleon-4.5.2/src/chameleon/tests/test_sniffing.py` & `Chameleon-4.5.3/src/chameleon/tests/test_sniffing.py`

 * *Files identical despite different names*

### Comparing `Chameleon-4.5.2/src/chameleon/tests/test_templates.py` & `Chameleon-4.5.3/src/chameleon/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `Chameleon-4.5.2/src/chameleon/tests/test_tokenizer.py` & `Chameleon-4.5.3/src/chameleon/tests/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `Chameleon-4.5.2/src/chameleon/tests/test_utils.py` & `Chameleon-4.5.3/src/chameleon/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `Chameleon-4.5.2/src/chameleon/tokenize.py` & `Chameleon-4.5.3/src/chameleon/tokenize.py`

 * *Files identical despite different names*

### Comparing `Chameleon-4.5.2/src/chameleon/types.py` & `Chameleon-4.5.3/src/chameleon/types.py`

 * *Files identical despite different names*

### Comparing `Chameleon-4.5.2/src/chameleon/utils.py` & `Chameleon-4.5.3/src/chameleon/utils.py`

 * *Files identical despite different names*

### Comparing `Chameleon-4.5.2/src/chameleon/zpt/loader.py` & `Chameleon-4.5.3/src/chameleon/zpt/loader.py`

 * *Files identical despite different names*

### Comparing `Chameleon-4.5.2/src/chameleon/zpt/program.py` & `Chameleon-4.5.3/src/chameleon/zpt/program.py`

 * *Files identical despite different names*

### Comparing `Chameleon-4.5.2/src/chameleon/zpt/template.py` & `Chameleon-4.5.3/src/chameleon/zpt/template.py`

 * *Files identical despite different names*

### Comparing `Chameleon-4.5.2/tox.ini` & `Chameleon-4.5.3/tox.ini`

 * *Files 14% similar despite different names*

```diff
@@ -8,14 +8,17 @@
     py310
     py311
     py312
     pypy3
     docs
     coverage
     mypy
+    z3c.macro
+    z3c.pt
+
 [testenv]
 usedevelop = true
 deps =
     build
     wheel
     pytest
     setuptools
@@ -106,7 +109,29 @@
     mypy
     importlib_metadata
 commands =
     mypy -p chameleon --python-version 3.9
     mypy -p chameleon --python-version 3.10
     mypy -p chameleon --python-version 3.11
     mypy -p chameleon --python-version 3.12
+
+[testenv:z3c.macro]
+basepython = python3
+skip_install = true
+commands_pre =
+    pip install -e.
+usedevelop = true
+deps =
+    z3c.macro[test]
+commands =
+    zope-testrunner --path {env_site_packages_dir} --path . -s z3c.macro {posargs:-vc}
+
+[testenv:z3c.pt]
+basepython = python3
+skip_install = true
+commands_pre =
+    pip install -e.
+usedevelop = true
+deps =
+    z3c.pt[test]
+commands =
+    zope-testrunner --path {env_site_packages_dir} --path . -s z3c.pt {posargs:-vc}
```

