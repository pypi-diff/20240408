# Comparing `tmp/pyflyby-1.9.2.tar.gz` & `tmp/pyflyby-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyflyby-1.9.2.tar", last modified: Mon Mar 25 06:42:48 2024, max compression
+gzip compressed data, was "pyflyby-1.9.3.tar", last modified: Mon Apr  8 05:04:13 2024, max compression
```

## Comparing `pyflyby-1.9.2.tar` & `pyflyby-1.9.3.tar`

### file list

```diff
@@ -1,165 +1,165 @@
-drwxrwsr-x   0 dhamodha (25011) dhamodha (25011)        0 2024-03-25 06:42:48.127948 pyflyby-1.9.2/
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     2965 2024-01-31 12:57:01.000000 pyflyby-1.9.2/.pyflyby
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     1188 2024-01-31 12:57:01.000000 pyflyby-1.9.2/LICENSE.txt
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)      520 2024-01-31 12:57:01.000000 pyflyby-1.9.2/MANIFEST.in
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    14675 2024-03-25 06:42:48.127382 pyflyby-1.9.2/PKG-INFO
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    13778 2024-02-28 12:59:51.000000 pyflyby-1.9.2/README.rst
-drwxrwsr-x   0 dhamodha (25011) dhamodha (25011)        0 2024-03-25 06:42:47.506544 pyflyby-1.9.2/bin/
--rwxrwxr-x   0 dhamodha (25011) dhamodha (25011)     2338 2024-01-31 12:57:01.000000 pyflyby-1.9.2/bin/autoipython
--rwxrwxr-x   0 dhamodha (25011) dhamodha (25011)      207 2024-01-31 12:57:01.000000 pyflyby-1.9.2/bin/autopython
--rwxrwxr-x   0 dhamodha (25011) dhamodha (25011)     2863 2024-01-31 12:57:01.000000 pyflyby-1.9.2/bin/collect-exports
--rwxrwxr-x   0 dhamodha (25011) dhamodha (25011)     2141 2024-01-31 12:57:01.000000 pyflyby-1.9.2/bin/collect-imports
--rwxrwxr-x   0 dhamodha (25011) dhamodha (25011)      238 2024-01-31 12:57:01.000000 pyflyby-1.9.2/bin/create-imports
--rwxrwxr-x   0 dhamodha (25011) dhamodha (25011)      932 2024-01-31 12:57:01.000000 pyflyby-1.9.2/bin/find-import
--rwxrwxr-x   0 dhamodha (25011) dhamodha (25011)     1027 2024-01-31 12:57:01.000000 pyflyby-1.9.2/bin/list-bad-xrefs
--rwxrwxr-x   0 dhamodha (25011) dhamodha (25011)      861 2024-01-31 12:57:01.000000 pyflyby-1.9.2/bin/prune-broken-imports
--rwxrwxr-x   0 dhamodha (25011) dhamodha (25011)     1014 2024-01-31 12:57:01.000000 pyflyby-1.9.2/bin/py
-drwxrwsr-x   0 dhamodha (25011) dhamodha (25011)        0 2024-03-25 06:42:47.592103 pyflyby-1.9.2/bin/pyflyby/
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     2606 2024-01-31 12:57:02.000000 pyflyby-1.9.2/bin/pyflyby/__init__.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)      190 2024-01-31 12:57:02.000000 pyflyby-1.9.2/bin/pyflyby/__main__.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    81126 2024-03-25 06:42:42.000000 pyflyby-1.9.2/bin/pyflyby/_autoimp.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    20351 2024-03-25 06:42:42.000000 pyflyby-1.9.2/bin/pyflyby/_cmdline.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     8209 2024-02-28 12:59:57.000000 pyflyby-1.9.2/bin/pyflyby/_comms.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    45604 2024-02-28 12:59:52.000000 pyflyby-1.9.2/bin/pyflyby/_dbg.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    14117 2024-02-28 12:59:57.000000 pyflyby-1.9.2/bin/pyflyby/_docxref.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    23116 2024-03-25 06:42:42.000000 pyflyby-1.9.2/bin/pyflyby/_file.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     7196 2024-02-28 12:59:57.000000 pyflyby-1.9.2/bin/pyflyby/_flags.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     6893 2024-02-28 12:59:57.000000 pyflyby-1.9.2/bin/pyflyby/_format.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     6849 2024-02-28 12:59:57.000000 pyflyby-1.9.2/bin/pyflyby/_idents.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    21657 2024-03-15 06:45:07.000000 pyflyby-1.9.2/bin/pyflyby/_importclns.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    23574 2024-02-28 12:59:52.000000 pyflyby-1.9.2/bin/pyflyby/_importdb.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    25480 2024-03-25 06:42:42.000000 pyflyby-1.9.2/bin/pyflyby/_imports2s.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    20613 2024-03-15 06:45:07.000000 pyflyby-1.9.2/bin/pyflyby/_importstmt.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)   104036 2024-02-28 12:59:57.000000 pyflyby-1.9.2/bin/pyflyby/_interactive.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    29339 2024-02-28 12:59:57.000000 pyflyby-1.9.2/bin/pyflyby/_livepatch.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     6547 2024-01-31 12:57:02.000000 pyflyby-1.9.2/bin/pyflyby/_log.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    18395 2024-03-15 06:45:07.000000 pyflyby-1.9.2/bin/pyflyby/_modules.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    53005 2024-03-25 06:42:42.000000 pyflyby-1.9.2/bin/pyflyby/_parse.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    77210 2024-03-15 06:45:07.000000 pyflyby-1.9.2/bin/pyflyby/_py.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    13862 2024-03-15 06:45:07.000000 pyflyby-1.9.2/bin/pyflyby/_util.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)      160 2024-03-25 06:42:42.000000 pyflyby-1.9.2/bin/pyflyby/_version.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)      485 2024-01-31 12:57:02.000000 pyflyby-1.9.2/bin/pyflyby/autoimport.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)      494 2024-01-31 12:57:02.000000 pyflyby-1.9.2/bin/pyflyby/importdb.py
--rwxrwxr-x   0 dhamodha (25011) dhamodha (25011)      938 2024-01-31 12:57:02.000000 pyflyby-1.9.2/bin/pyflyby-diff
--rwxrwxr-x   0 dhamodha (25011) dhamodha (25011)      690 2024-01-31 12:57:01.000000 pyflyby-1.9.2/bin/reformat-imports
--rwxrwxr-x   0 dhamodha (25011) dhamodha (25011)      913 2024-01-31 12:57:01.000000 pyflyby-1.9.2/bin/replace-star-imports
--rwxrwxr-x   0 dhamodha (25011) dhamodha (25011)     6325 2024-03-25 06:42:41.000000 pyflyby-1.9.2/bin/tidy-imports
--rwxrwxr-x   0 dhamodha (25011) dhamodha (25011)     1450 2024-01-31 12:57:01.000000 pyflyby-1.9.2/bin/transform-imports
-drwxrwsr-x   0 dhamodha (25011) dhamodha (25011)        0 2024-03-25 06:42:47.652792 pyflyby-1.9.2/doc/
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     1188 2024-01-31 12:57:01.000000 pyflyby-1.9.2/doc/LICENSE.txt
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)      855 2024-01-31 12:57:01.000000 pyflyby-1.9.2/doc/Makefile
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     5622 2024-01-31 12:57:01.000000 pyflyby-1.9.2/doc/TODO.txt
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)        0 2024-01-31 12:57:01.000000 pyflyby-1.9.2/doc/__init__.py
-drwxrwsr-x   0 dhamodha (25011) dhamodha (25011)        0 2024-03-25 06:42:48.009108 pyflyby-1.9.2/doc/api/
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)      275 2024-01-31 12:57:01.000000 pyflyby-1.9.2/doc/api/api.rst
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)       78 2024-01-31 12:57:01.000000 pyflyby-1.9.2/doc/api/autoimp.rst
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)       78 2024-01-31 12:57:01.000000 pyflyby-1.9.2/doc/api/cmdline.rst
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)       72 2024-01-31 12:57:01.000000 pyflyby-1.9.2/doc/api/comms.rst
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)       66 2024-01-31 12:57:01.000000 pyflyby-1.9.2/doc/api/dbg.rst
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)       69 2024-01-31 12:57:01.000000 pyflyby-1.9.2/doc/api/file.rst
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)      123 2024-01-31 12:57:01.000000 pyflyby-1.9.2/doc/api/flags.rst
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)       75 2024-01-31 12:57:01.000000 pyflyby-1.9.2/doc/api/format.rst
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)      109 2024-01-31 12:57:01.000000 pyflyby-1.9.2/doc/api/idents.rst
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)       86 2024-01-31 12:57:01.000000 pyflyby-1.9.2/doc/api/importclns.rst
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)       80 2024-01-31 12:57:01.000000 pyflyby-1.9.2/doc/api/importdb.rst
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)       83 2024-01-31 12:57:01.000000 pyflyby-1.9.2/doc/api/imports2s.rst
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)       86 2024-01-31 12:57:01.000000 pyflyby-1.9.2/doc/api/importstmt.rst
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)       89 2024-01-31 12:57:01.000000 pyflyby-1.9.2/doc/api/interactive.rst
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)       83 2024-01-31 12:57:01.000000 pyflyby-1.9.2/doc/api/livepatch.rst
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)       65 2024-01-31 12:57:01.000000 pyflyby-1.9.2/doc/api/log.rst
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)       77 2024-01-31 12:57:01.000000 pyflyby-1.9.2/doc/api/modules.rst
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)       71 2024-01-31 12:57:01.000000 pyflyby-1.9.2/doc/api/parse.rst
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)       62 2024-01-31 12:57:01.000000 pyflyby-1.9.2/doc/api/py.rst
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)       68 2024-01-31 12:57:01.000000 pyflyby-1.9.2/doc/api/util.rst
-drwxrwsr-x   0 dhamodha (25011) dhamodha (25011)        0 2024-03-25 06:42:48.019263 pyflyby-1.9.2/doc/cli/
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)      102 2024-01-31 12:57:01.000000 pyflyby-1.9.2/doc/cli/autoipython.rst
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)      273 2024-01-31 12:57:01.000000 pyflyby-1.9.2/doc/cli/cli.rst
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)       85 2024-01-31 12:57:01.000000 pyflyby-1.9.2/doc/cli/collect_exports.rst
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)       85 2024-01-31 12:57:01.000000 pyflyby-1.9.2/doc/cli/collect_imports.rst
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)       73 2024-01-31 12:57:01.000000 pyflyby-1.9.2/doc/cli/find_import.rst
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)      100 2024-01-31 12:57:01.000000 pyflyby-1.9.2/doc/cli/prune_broken_imports.rst
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)       46 2024-01-31 12:57:02.000000 pyflyby-1.9.2/doc/cli/py.rst
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)       76 2024-01-31 12:57:02.000000 pyflyby-1.9.2/doc/cli/pyflyby_diff.rst
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)       84 2024-01-31 12:57:02.000000 pyflyby-1.9.2/doc/cli/reformat_imports.rst
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)      100 2024-01-31 12:57:02.000000 pyflyby-1.9.2/doc/cli/replace_star_imports.rst
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)       76 2024-01-31 12:57:02.000000 pyflyby-1.9.2/doc/cli/tidy_imports.rst
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)       91 2024-01-31 12:57:02.000000 pyflyby-1.9.2/doc/cli/transform_imports.rst
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     1057 2024-01-31 12:57:02.000000 pyflyby-1.9.2/doc/conf.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)      201 2024-01-31 12:57:02.000000 pyflyby-1.9.2/doc/index.rst
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)      760 2024-01-31 12:57:02.000000 pyflyby-1.9.2/doc/make.bat
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)      186 2024-01-31 12:57:02.000000 pyflyby-1.9.2/doc/testing.txt
-drwxrwsr-x   0 dhamodha (25011) dhamodha (25011)        0 2024-03-25 06:42:47.429611 pyflyby-1.9.2/etc/
-drwxrwsr-x   0 dhamodha (25011) dhamodha (25011)        0 2024-03-25 06:42:48.024651 pyflyby-1.9.2/etc/pyflyby/
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)      270 2024-01-31 12:57:02.000000 pyflyby-1.9.2/etc/pyflyby/canonical.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)      569 2024-01-31 12:57:02.000000 pyflyby-1.9.2/etc/pyflyby/common.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)      369 2024-01-31 12:57:02.000000 pyflyby-1.9.2/etc/pyflyby/forget.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)      352 2024-01-31 12:57:02.000000 pyflyby-1.9.2/etc/pyflyby/mandatory.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    10469 2024-01-31 12:57:02.000000 pyflyby-1.9.2/etc/pyflyby/numpy.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    17596 2024-02-28 12:59:57.000000 pyflyby-1.9.2/etc/pyflyby/std.py
-drwxrwsr-x   0 dhamodha (25011) dhamodha (25011)        0 2024-03-25 06:42:47.430982 pyflyby-1.9.2/lib/
-drwxrwsr-x   0 dhamodha (25011) dhamodha (25011)        0 2024-03-25 06:42:48.026005 pyflyby-1.9.2/lib/emacs/
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     4122 2024-01-31 12:57:02.000000 pyflyby-1.9.2/lib/emacs/pyflyby.el
-drwxrwsr-x   0 dhamodha (25011) dhamodha (25011)        0 2024-03-25 06:42:47.431786 pyflyby-1.9.2/lib/python/
-drwxrwsr-x   0 dhamodha (25011) dhamodha (25011)        0 2024-03-25 06:42:48.066456 pyflyby-1.9.2/lib/python/pyflyby/
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     2606 2024-01-31 12:57:02.000000 pyflyby-1.9.2/lib/python/pyflyby/__init__.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)      190 2024-01-31 12:57:02.000000 pyflyby-1.9.2/lib/python/pyflyby/__main__.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    81126 2024-03-25 06:42:42.000000 pyflyby-1.9.2/lib/python/pyflyby/_autoimp.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    20351 2024-03-25 06:42:42.000000 pyflyby-1.9.2/lib/python/pyflyby/_cmdline.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     8209 2024-02-28 12:59:57.000000 pyflyby-1.9.2/lib/python/pyflyby/_comms.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    45604 2024-02-28 12:59:52.000000 pyflyby-1.9.2/lib/python/pyflyby/_dbg.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    14117 2024-02-28 12:59:57.000000 pyflyby-1.9.2/lib/python/pyflyby/_docxref.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    23116 2024-03-25 06:42:42.000000 pyflyby-1.9.2/lib/python/pyflyby/_file.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     7196 2024-02-28 12:59:57.000000 pyflyby-1.9.2/lib/python/pyflyby/_flags.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     6893 2024-02-28 12:59:57.000000 pyflyby-1.9.2/lib/python/pyflyby/_format.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     6849 2024-02-28 12:59:57.000000 pyflyby-1.9.2/lib/python/pyflyby/_idents.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    21657 2024-03-15 06:45:07.000000 pyflyby-1.9.2/lib/python/pyflyby/_importclns.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    23574 2024-02-28 12:59:52.000000 pyflyby-1.9.2/lib/python/pyflyby/_importdb.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    25480 2024-03-25 06:42:42.000000 pyflyby-1.9.2/lib/python/pyflyby/_imports2s.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    20613 2024-03-15 06:45:07.000000 pyflyby-1.9.2/lib/python/pyflyby/_importstmt.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)   104036 2024-02-28 12:59:57.000000 pyflyby-1.9.2/lib/python/pyflyby/_interactive.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    29339 2024-02-28 12:59:57.000000 pyflyby-1.9.2/lib/python/pyflyby/_livepatch.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     6547 2024-01-31 12:57:02.000000 pyflyby-1.9.2/lib/python/pyflyby/_log.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    18395 2024-03-15 06:45:07.000000 pyflyby-1.9.2/lib/python/pyflyby/_modules.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    53005 2024-03-25 06:42:42.000000 pyflyby-1.9.2/lib/python/pyflyby/_parse.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    77210 2024-03-15 06:45:07.000000 pyflyby-1.9.2/lib/python/pyflyby/_py.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    13862 2024-03-15 06:45:07.000000 pyflyby-1.9.2/lib/python/pyflyby/_util.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)      160 2024-03-25 06:42:42.000000 pyflyby-1.9.2/lib/python/pyflyby/_version.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)      485 2024-01-31 12:57:02.000000 pyflyby-1.9.2/lib/python/pyflyby/autoimport.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)      494 2024-01-31 12:57:02.000000 pyflyby-1.9.2/lib/python/pyflyby/importdb.py
-drwxrwsr-x   0 dhamodha (25011) dhamodha (25011)        0 2024-03-25 06:42:48.071741 pyflyby-1.9.2/lib/python/pyflyby.egg-info/
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    14675 2024-03-25 06:42:46.000000 pyflyby-1.9.2/lib/python/pyflyby.egg-info/PKG-INFO
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     3431 2024-03-25 06:42:47.000000 pyflyby-1.9.2/lib/python/pyflyby.egg-info/SOURCES.txt
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)        1 2024-03-25 06:42:46.000000 pyflyby-1.9.2/lib/python/pyflyby.egg-info/dependency_links.txt
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)       69 2024-03-25 06:42:46.000000 pyflyby-1.9.2/lib/python/pyflyby.egg-info/entry_points.txt
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)       21 2024-03-25 06:42:46.000000 pyflyby-1.9.2/lib/python/pyflyby.egg-info/requires.txt
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)        8 2024-03-25 06:42:46.000000 pyflyby-1.9.2/lib/python/pyflyby.egg-info/top_level.txt
-drwxrwsr-x   0 dhamodha (25011) dhamodha (25011)        0 2024-03-25 06:42:47.432498 pyflyby-1.9.2/libexec/
-drwxrwsr-x   0 dhamodha (25011) dhamodha (25011)        0 2024-03-25 06:42:48.096975 pyflyby-1.9.2/libexec/pyflyby/
--rwxrwxr-x   0 dhamodha (25011) dhamodha (25011)      938 2024-01-31 12:57:02.000000 pyflyby-1.9.2/libexec/pyflyby/colordiff
--rwxrwxr-x   0 dhamodha (25011) dhamodha (25011)     5578 2024-01-31 12:57:02.000000 pyflyby-1.9.2/libexec/pyflyby/diff-colorize
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)       38 2024-03-25 06:42:48.128039 pyflyby-1.9.2/setup.cfg
--rwxrwxr-x   0 dhamodha (25011) dhamodha (25011)     7714 2024-02-28 12:59:52.000000 pyflyby-1.9.2/setup.py
-drwxrwsr-x   0 dhamodha (25011) dhamodha (25011)        0 2024-03-25 06:42:48.126649 pyflyby-1.9.2/tests/
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)        1 2024-01-31 12:57:02.000000 pyflyby-1.9.2/tests/__init__.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     2036 2024-01-31 12:57:02.000000 pyflyby-1.9.2/tests/test_0testconfig.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    58324 2024-02-28 12:59:58.000000 pyflyby-1.9.2/tests/test_autoimp.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    24292 2024-02-28 12:59:58.000000 pyflyby-1.9.2/tests/test_cmdline.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     2278 2024-01-31 12:57:02.000000 pyflyby-1.9.2/tests/test_docxref.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    10444 2024-01-31 12:57:02.000000 pyflyby-1.9.2/tests/test_file.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     4457 2024-01-31 12:57:02.000000 pyflyby-1.9.2/tests/test_flags.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     4132 2024-01-31 12:57:02.000000 pyflyby-1.9.2/tests/test_format.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     2631 2024-01-31 12:57:02.000000 pyflyby-1.9.2/tests/test_idents.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     7900 2024-01-31 12:57:02.000000 pyflyby-1.9.2/tests/test_importclns.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     7150 2024-01-31 12:57:02.000000 pyflyby-1.9.2/tests/test_importdb.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    30781 2024-03-25 06:42:42.000000 pyflyby-1.9.2/tests/test_imports2s.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     9887 2024-03-15 06:45:07.000000 pyflyby-1.9.2/tests/test_importstmt.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)   142012 2024-03-15 06:45:07.000000 pyflyby-1.9.2/tests/test_interactive.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     1893 2024-01-31 12:57:02.000000 pyflyby-1.9.2/tests/test_jupyterlab_pyflyby.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    71327 2024-01-31 12:57:02.000000 pyflyby-1.9.2/tests/test_livepatch.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     3172 2024-03-15 06:45:07.000000 pyflyby-1.9.2/tests/test_modules.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    41344 2024-02-28 12:59:58.000000 pyflyby-1.9.2/tests/test_parse.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    73341 2024-02-28 12:59:52.000000 pyflyby-1.9.2/tests/test_py.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)      751 2024-01-31 12:57:02.000000 pyflyby-1.9.2/tests/test_util.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     2447 2024-02-28 12:59:52.000000 pyflyby-1.9.2/tests/tests_sorts.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     1745 2024-01-31 12:57:02.000000 pyflyby-1.9.2/tests/xrefs.py
--rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     1890 2024-01-31 12:57:02.000000 pyflyby-1.9.2/tox.ini
+drwxrwsr-x   0 dhamodha (25011) dhamodha (25011)        0 2024-04-08 05:04:13.918460 pyflyby-1.9.3/
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     2965 2024-04-08 04:25:37.000000 pyflyby-1.9.3/.pyflyby
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     1188 2024-04-08 04:25:37.000000 pyflyby-1.9.3/LICENSE.txt
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)      520 2024-04-08 04:25:37.000000 pyflyby-1.9.3/MANIFEST.in
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    14675 2024-04-08 05:04:13.917038 pyflyby-1.9.3/PKG-INFO
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    13778 2024-04-08 04:25:37.000000 pyflyby-1.9.3/README.rst
+drwxrwsr-x   0 dhamodha (25011) dhamodha (25011)        0 2024-04-08 05:04:12.863607 pyflyby-1.9.3/bin/
+-rwxrwxr-x   0 dhamodha (25011) dhamodha (25011)     2338 2024-04-08 04:25:37.000000 pyflyby-1.9.3/bin/autoipython
+-rwxrwxr-x   0 dhamodha (25011) dhamodha (25011)      207 2024-04-08 04:25:37.000000 pyflyby-1.9.3/bin/autopython
+-rwxrwxr-x   0 dhamodha (25011) dhamodha (25011)     2863 2024-04-08 04:25:37.000000 pyflyby-1.9.3/bin/collect-exports
+-rwxrwxr-x   0 dhamodha (25011) dhamodha (25011)     2141 2024-04-08 04:25:37.000000 pyflyby-1.9.3/bin/collect-imports
+-rwxrwxr-x   0 dhamodha (25011) dhamodha (25011)      238 2024-04-08 04:25:37.000000 pyflyby-1.9.3/bin/create-imports
+-rwxrwxr-x   0 dhamodha (25011) dhamodha (25011)      932 2024-04-08 04:25:37.000000 pyflyby-1.9.3/bin/find-import
+-rwxrwxr-x   0 dhamodha (25011) dhamodha (25011)     1027 2024-04-08 04:25:37.000000 pyflyby-1.9.3/bin/list-bad-xrefs
+-rwxrwxr-x   0 dhamodha (25011) dhamodha (25011)      861 2024-04-08 04:25:37.000000 pyflyby-1.9.3/bin/prune-broken-imports
+-rwxrwxr-x   0 dhamodha (25011) dhamodha (25011)     1014 2024-04-08 04:25:37.000000 pyflyby-1.9.3/bin/py
+drwxrwsr-x   0 dhamodha (25011) dhamodha (25011)        0 2024-04-08 05:04:13.138617 pyflyby-1.9.3/bin/pyflyby/
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     2606 2024-04-08 04:25:38.000000 pyflyby-1.9.3/bin/pyflyby/__init__.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)      190 2024-04-08 04:25:38.000000 pyflyby-1.9.3/bin/pyflyby/__main__.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    81126 2024-04-08 04:25:38.000000 pyflyby-1.9.3/bin/pyflyby/_autoimp.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    20351 2024-04-08 04:25:38.000000 pyflyby-1.9.3/bin/pyflyby/_cmdline.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     8184 2024-04-08 04:25:38.000000 pyflyby-1.9.3/bin/pyflyby/_comms.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    45604 2024-04-08 04:25:38.000000 pyflyby-1.9.3/bin/pyflyby/_dbg.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    14117 2024-04-08 04:25:38.000000 pyflyby-1.9.3/bin/pyflyby/_docxref.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    23116 2024-04-08 04:25:38.000000 pyflyby-1.9.3/bin/pyflyby/_file.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     7196 2024-04-08 04:25:38.000000 pyflyby-1.9.3/bin/pyflyby/_flags.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     6893 2024-04-08 04:25:38.000000 pyflyby-1.9.3/bin/pyflyby/_format.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     6849 2024-04-08 04:25:38.000000 pyflyby-1.9.3/bin/pyflyby/_idents.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    21645 2024-04-08 04:25:38.000000 pyflyby-1.9.3/bin/pyflyby/_importclns.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    23556 2024-04-08 04:25:38.000000 pyflyby-1.9.3/bin/pyflyby/_importdb.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    25480 2024-04-08 04:25:38.000000 pyflyby-1.9.3/bin/pyflyby/_imports2s.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    20613 2024-04-08 04:25:38.000000 pyflyby-1.9.3/bin/pyflyby/_importstmt.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)   104052 2024-04-08 04:25:38.000000 pyflyby-1.9.3/bin/pyflyby/_interactive.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    29349 2024-04-08 04:25:38.000000 pyflyby-1.9.3/bin/pyflyby/_livepatch.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     6515 2024-04-08 04:25:38.000000 pyflyby-1.9.3/bin/pyflyby/_log.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    18395 2024-04-08 04:25:38.000000 pyflyby-1.9.3/bin/pyflyby/_modules.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    53005 2024-04-08 04:25:38.000000 pyflyby-1.9.3/bin/pyflyby/_parse.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    77210 2024-04-08 04:25:38.000000 pyflyby-1.9.3/bin/pyflyby/_py.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    13862 2024-04-08 04:25:38.000000 pyflyby-1.9.3/bin/pyflyby/_util.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)      160 2024-04-08 05:03:58.000000 pyflyby-1.9.3/bin/pyflyby/_version.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)      485 2024-04-08 04:25:38.000000 pyflyby-1.9.3/bin/pyflyby/autoimport.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)      494 2024-04-08 04:25:38.000000 pyflyby-1.9.3/bin/pyflyby/importdb.py
+-rwxrwxr-x   0 dhamodha (25011) dhamodha (25011)      938 2024-04-08 04:25:38.000000 pyflyby-1.9.3/bin/pyflyby-diff
+-rwxrwxr-x   0 dhamodha (25011) dhamodha (25011)      690 2024-04-08 04:25:37.000000 pyflyby-1.9.3/bin/reformat-imports
+-rwxrwxr-x   0 dhamodha (25011) dhamodha (25011)      913 2024-04-08 04:25:37.000000 pyflyby-1.9.3/bin/replace-star-imports
+-rwxrwxr-x   0 dhamodha (25011) dhamodha (25011)     6218 2024-04-08 05:03:58.000000 pyflyby-1.9.3/bin/tidy-imports
+-rwxrwxr-x   0 dhamodha (25011) dhamodha (25011)     1450 2024-04-08 04:25:37.000000 pyflyby-1.9.3/bin/transform-imports
+drwxrwsr-x   0 dhamodha (25011) dhamodha (25011)        0 2024-04-08 05:04:13.192013 pyflyby-1.9.3/doc/
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     1188 2024-04-08 04:25:37.000000 pyflyby-1.9.3/doc/LICENSE.txt
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)      855 2024-04-08 04:25:37.000000 pyflyby-1.9.3/doc/Makefile
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     5622 2024-04-08 04:25:37.000000 pyflyby-1.9.3/doc/TODO.txt
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)        0 2024-04-08 04:25:37.000000 pyflyby-1.9.3/doc/__init__.py
+drwxrwsr-x   0 dhamodha (25011) dhamodha (25011)        0 2024-04-08 05:04:13.323957 pyflyby-1.9.3/doc/api/
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)      275 2024-04-08 04:25:37.000000 pyflyby-1.9.3/doc/api/api.rst
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)       78 2024-04-08 04:25:37.000000 pyflyby-1.9.3/doc/api/autoimp.rst
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)       78 2024-04-08 04:25:37.000000 pyflyby-1.9.3/doc/api/cmdline.rst
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)       72 2024-04-08 04:25:37.000000 pyflyby-1.9.3/doc/api/comms.rst
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)       66 2024-04-08 04:25:37.000000 pyflyby-1.9.3/doc/api/dbg.rst
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)       69 2024-04-08 04:25:37.000000 pyflyby-1.9.3/doc/api/file.rst
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)      123 2024-04-08 04:25:37.000000 pyflyby-1.9.3/doc/api/flags.rst
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)       75 2024-04-08 04:25:37.000000 pyflyby-1.9.3/doc/api/format.rst
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)      109 2024-04-08 04:25:37.000000 pyflyby-1.9.3/doc/api/idents.rst
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)       86 2024-04-08 04:25:37.000000 pyflyby-1.9.3/doc/api/importclns.rst
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)       80 2024-04-08 04:25:37.000000 pyflyby-1.9.3/doc/api/importdb.rst
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)       83 2024-04-08 04:25:37.000000 pyflyby-1.9.3/doc/api/imports2s.rst
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)       86 2024-04-08 04:25:37.000000 pyflyby-1.9.3/doc/api/importstmt.rst
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)       89 2024-04-08 04:25:37.000000 pyflyby-1.9.3/doc/api/interactive.rst
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)       83 2024-04-08 04:25:37.000000 pyflyby-1.9.3/doc/api/livepatch.rst
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)       65 2024-04-08 04:25:37.000000 pyflyby-1.9.3/doc/api/log.rst
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)       77 2024-04-08 04:25:37.000000 pyflyby-1.9.3/doc/api/modules.rst
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)       71 2024-04-08 04:25:37.000000 pyflyby-1.9.3/doc/api/parse.rst
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)       62 2024-04-08 04:25:37.000000 pyflyby-1.9.3/doc/api/py.rst
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)       68 2024-04-08 04:25:37.000000 pyflyby-1.9.3/doc/api/util.rst
+drwxrwsr-x   0 dhamodha (25011) dhamodha (25011)        0 2024-04-08 05:04:13.414278 pyflyby-1.9.3/doc/cli/
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)      102 2024-04-08 04:25:37.000000 pyflyby-1.9.3/doc/cli/autoipython.rst
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)      273 2024-04-08 04:25:37.000000 pyflyby-1.9.3/doc/cli/cli.rst
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)       85 2024-04-08 04:25:37.000000 pyflyby-1.9.3/doc/cli/collect_exports.rst
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)       85 2024-04-08 04:25:37.000000 pyflyby-1.9.3/doc/cli/collect_imports.rst
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)       73 2024-04-08 04:25:37.000000 pyflyby-1.9.3/doc/cli/find_import.rst
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)      100 2024-04-08 04:25:37.000000 pyflyby-1.9.3/doc/cli/prune_broken_imports.rst
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)       46 2024-04-08 04:25:38.000000 pyflyby-1.9.3/doc/cli/py.rst
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)       76 2024-04-08 04:25:38.000000 pyflyby-1.9.3/doc/cli/pyflyby_diff.rst
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)       84 2024-04-08 04:25:38.000000 pyflyby-1.9.3/doc/cli/reformat_imports.rst
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)      100 2024-04-08 04:25:38.000000 pyflyby-1.9.3/doc/cli/replace_star_imports.rst
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)       76 2024-04-08 04:25:38.000000 pyflyby-1.9.3/doc/cli/tidy_imports.rst
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)       91 2024-04-08 04:25:38.000000 pyflyby-1.9.3/doc/cli/transform_imports.rst
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     1057 2024-04-08 04:25:38.000000 pyflyby-1.9.3/doc/conf.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)      201 2024-04-08 04:25:38.000000 pyflyby-1.9.3/doc/index.rst
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)      760 2024-04-08 04:25:38.000000 pyflyby-1.9.3/doc/make.bat
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)      186 2024-04-08 04:25:38.000000 pyflyby-1.9.3/doc/testing.txt
+drwxrwsr-x   0 dhamodha (25011) dhamodha (25011)        0 2024-04-08 05:04:12.673085 pyflyby-1.9.3/etc/
+drwxrwsr-x   0 dhamodha (25011) dhamodha (25011)        0 2024-04-08 05:04:13.462524 pyflyby-1.9.3/etc/pyflyby/
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)      270 2024-04-08 04:25:38.000000 pyflyby-1.9.3/etc/pyflyby/canonical.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)      569 2024-04-08 04:25:38.000000 pyflyby-1.9.3/etc/pyflyby/common.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)      369 2024-04-08 04:25:38.000000 pyflyby-1.9.3/etc/pyflyby/forget.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)      352 2024-04-08 04:25:38.000000 pyflyby-1.9.3/etc/pyflyby/mandatory.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    10469 2024-04-08 04:25:38.000000 pyflyby-1.9.3/etc/pyflyby/numpy.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    17596 2024-04-08 04:25:38.000000 pyflyby-1.9.3/etc/pyflyby/std.py
+drwxrwsr-x   0 dhamodha (25011) dhamodha (25011)        0 2024-04-08 05:04:12.680134 pyflyby-1.9.3/lib/
+drwxrwsr-x   0 dhamodha (25011) dhamodha (25011)        0 2024-04-08 05:04:13.469714 pyflyby-1.9.3/lib/emacs/
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     4122 2024-04-08 04:25:38.000000 pyflyby-1.9.3/lib/emacs/pyflyby.el
+drwxrwsr-x   0 dhamodha (25011) dhamodha (25011)        0 2024-04-08 05:04:12.684632 pyflyby-1.9.3/lib/python/
+drwxrwsr-x   0 dhamodha (25011) dhamodha (25011)        0 2024-04-08 05:04:13.661105 pyflyby-1.9.3/lib/python/pyflyby/
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     2606 2024-04-08 04:25:38.000000 pyflyby-1.9.3/lib/python/pyflyby/__init__.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)      190 2024-04-08 04:25:38.000000 pyflyby-1.9.3/lib/python/pyflyby/__main__.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    81126 2024-04-08 04:25:38.000000 pyflyby-1.9.3/lib/python/pyflyby/_autoimp.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    20351 2024-04-08 04:25:38.000000 pyflyby-1.9.3/lib/python/pyflyby/_cmdline.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     8184 2024-04-08 04:25:38.000000 pyflyby-1.9.3/lib/python/pyflyby/_comms.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    45604 2024-04-08 04:25:38.000000 pyflyby-1.9.3/lib/python/pyflyby/_dbg.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    14117 2024-04-08 04:25:38.000000 pyflyby-1.9.3/lib/python/pyflyby/_docxref.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    23116 2024-04-08 04:25:38.000000 pyflyby-1.9.3/lib/python/pyflyby/_file.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     7196 2024-04-08 04:25:38.000000 pyflyby-1.9.3/lib/python/pyflyby/_flags.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     6893 2024-04-08 04:25:38.000000 pyflyby-1.9.3/lib/python/pyflyby/_format.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     6849 2024-04-08 04:25:38.000000 pyflyby-1.9.3/lib/python/pyflyby/_idents.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    21645 2024-04-08 04:25:38.000000 pyflyby-1.9.3/lib/python/pyflyby/_importclns.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    23556 2024-04-08 04:25:38.000000 pyflyby-1.9.3/lib/python/pyflyby/_importdb.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    25480 2024-04-08 04:25:38.000000 pyflyby-1.9.3/lib/python/pyflyby/_imports2s.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    20613 2024-04-08 04:25:38.000000 pyflyby-1.9.3/lib/python/pyflyby/_importstmt.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)   104052 2024-04-08 04:25:38.000000 pyflyby-1.9.3/lib/python/pyflyby/_interactive.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    29349 2024-04-08 04:25:38.000000 pyflyby-1.9.3/lib/python/pyflyby/_livepatch.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     6515 2024-04-08 04:25:38.000000 pyflyby-1.9.3/lib/python/pyflyby/_log.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    18395 2024-04-08 04:25:38.000000 pyflyby-1.9.3/lib/python/pyflyby/_modules.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    53005 2024-04-08 04:25:38.000000 pyflyby-1.9.3/lib/python/pyflyby/_parse.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    77210 2024-04-08 04:25:38.000000 pyflyby-1.9.3/lib/python/pyflyby/_py.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    13862 2024-04-08 04:25:38.000000 pyflyby-1.9.3/lib/python/pyflyby/_util.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)      160 2024-04-08 05:03:58.000000 pyflyby-1.9.3/lib/python/pyflyby/_version.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)      485 2024-04-08 04:25:38.000000 pyflyby-1.9.3/lib/python/pyflyby/autoimport.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)      494 2024-04-08 04:25:38.000000 pyflyby-1.9.3/lib/python/pyflyby/importdb.py
+drwxrwsr-x   0 dhamodha (25011) dhamodha (25011)        0 2024-04-08 05:04:13.706584 pyflyby-1.9.3/lib/python/pyflyby.egg-info/
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    14675 2024-04-08 05:04:12.000000 pyflyby-1.9.3/lib/python/pyflyby.egg-info/PKG-INFO
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     3431 2024-04-08 05:04:12.000000 pyflyby-1.9.3/lib/python/pyflyby.egg-info/SOURCES.txt
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)        1 2024-04-08 05:04:12.000000 pyflyby-1.9.3/lib/python/pyflyby.egg-info/dependency_links.txt
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)       69 2024-04-08 05:04:12.000000 pyflyby-1.9.3/lib/python/pyflyby.egg-info/entry_points.txt
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)       21 2024-04-08 05:04:12.000000 pyflyby-1.9.3/lib/python/pyflyby.egg-info/requires.txt
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)        8 2024-04-08 05:04:12.000000 pyflyby-1.9.3/lib/python/pyflyby.egg-info/top_level.txt
+drwxrwsr-x   0 dhamodha (25011) dhamodha (25011)        0 2024-04-08 05:04:12.689199 pyflyby-1.9.3/libexec/
+drwxrwsr-x   0 dhamodha (25011) dhamodha (25011)        0 2024-04-08 05:04:13.723467 pyflyby-1.9.3/libexec/pyflyby/
+-rwxrwxr-x   0 dhamodha (25011) dhamodha (25011)      938 2024-04-08 04:25:38.000000 pyflyby-1.9.3/libexec/pyflyby/colordiff
+-rwxrwxr-x   0 dhamodha (25011) dhamodha (25011)     5578 2024-04-08 04:25:38.000000 pyflyby-1.9.3/libexec/pyflyby/diff-colorize
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)       38 2024-04-08 05:04:13.920445 pyflyby-1.9.3/setup.cfg
+-rwxrwxr-x   0 dhamodha (25011) dhamodha (25011)     7714 2024-04-08 04:25:38.000000 pyflyby-1.9.3/setup.py
+drwxrwsr-x   0 dhamodha (25011) dhamodha (25011)        0 2024-04-08 05:04:13.907952 pyflyby-1.9.3/tests/
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)        1 2024-04-08 04:25:38.000000 pyflyby-1.9.3/tests/__init__.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     2036 2024-04-08 04:25:38.000000 pyflyby-1.9.3/tests/test_0testconfig.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    58324 2024-04-08 04:25:38.000000 pyflyby-1.9.3/tests/test_autoimp.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    24292 2024-04-08 04:25:38.000000 pyflyby-1.9.3/tests/test_cmdline.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     2278 2024-04-08 04:25:38.000000 pyflyby-1.9.3/tests/test_docxref.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    10444 2024-04-08 04:25:38.000000 pyflyby-1.9.3/tests/test_file.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     4457 2024-04-08 04:25:38.000000 pyflyby-1.9.3/tests/test_flags.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     4132 2024-04-08 04:25:38.000000 pyflyby-1.9.3/tests/test_format.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     2631 2024-04-08 04:25:38.000000 pyflyby-1.9.3/tests/test_idents.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     7900 2024-04-08 04:25:38.000000 pyflyby-1.9.3/tests/test_importclns.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     7150 2024-04-08 04:25:38.000000 pyflyby-1.9.3/tests/test_importdb.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    30781 2024-04-08 04:25:38.000000 pyflyby-1.9.3/tests/test_imports2s.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     9887 2024-04-08 04:25:38.000000 pyflyby-1.9.3/tests/test_importstmt.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)   142012 2024-04-08 04:25:38.000000 pyflyby-1.9.3/tests/test_interactive.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     1893 2024-04-08 04:25:38.000000 pyflyby-1.9.3/tests/test_jupyterlab_pyflyby.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    71327 2024-04-08 04:25:38.000000 pyflyby-1.9.3/tests/test_livepatch.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     3172 2024-04-08 04:25:38.000000 pyflyby-1.9.3/tests/test_modules.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    41344 2024-04-08 04:25:38.000000 pyflyby-1.9.3/tests/test_parse.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)    73341 2024-04-08 04:25:38.000000 pyflyby-1.9.3/tests/test_py.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)      751 2024-04-08 04:25:38.000000 pyflyby-1.9.3/tests/test_util.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     2447 2024-04-08 04:25:38.000000 pyflyby-1.9.3/tests/tests_sorts.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     1745 2024-04-08 04:25:39.000000 pyflyby-1.9.3/tests/xrefs.py
+-rw-rw-r--   0 dhamodha (25011) dhamodha (25011)     1890 2024-04-08 04:25:39.000000 pyflyby-1.9.3/tox.ini
```

### Comparing `pyflyby-1.9.2/.pyflyby` & `pyflyby-1.9.3/.pyflyby`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/LICENSE.txt` & `pyflyby-1.9.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/MANIFEST.in` & `pyflyby-1.9.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/PKG-INFO` & `pyflyby-1.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyflyby
-Version: 1.9.2
+Version: 1.9.3
 Summary: pyflyby - Python development productivity tools, in particular automatic import management
 Home-page: https://pypi.org/project/pyflyby/
 Author: Karl Chen
 Author-email: quarl@8166.clguba.z.quarl.org
 License: MIT
 Project-URL: Documentation, https://deshaw.github.io/pyflyby/
 Project-URL: Source, https://github.com/deshaw/pyflyby
```

### Comparing `pyflyby-1.9.2/README.rst` & `pyflyby-1.9.3/README.rst`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/bin/autoipython` & `pyflyby-1.9.3/bin/autoipython`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/bin/collect-exports` & `pyflyby-1.9.3/bin/collect-exports`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/bin/collect-imports` & `pyflyby-1.9.3/bin/collect-imports`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/bin/find-import` & `pyflyby-1.9.3/bin/find-import`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/bin/list-bad-xrefs` & `pyflyby-1.9.3/bin/list-bad-xrefs`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/bin/prune-broken-imports` & `pyflyby-1.9.3/bin/prune-broken-imports`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/bin/py` & `pyflyby-1.9.3/bin/py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/bin/pyflyby/__init__.py` & `pyflyby-1.9.3/bin/pyflyby/__init__.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/bin/pyflyby/_autoimp.py` & `pyflyby-1.9.3/bin/pyflyby/_autoimp.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/bin/pyflyby/_cmdline.py` & `pyflyby-1.9.3/bin/pyflyby/_cmdline.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/bin/pyflyby/_comms.py` & `pyflyby-1.9.3/bin/pyflyby/_comms.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from   pyflyby._imports2s       import (SourceToSourceFileImportsTransformation,
                                         SourceToSourceImportBlockTransformation,
                                         fix_unused_and_missing_imports,
                                         replace_star_imports,
                                         reformat_import_statements)
 from   pyflyby._importstmt      import Import
 from   pyflyby._log             import logger
-import six
 
 # These are comm targets that the frontend (lab/notebook) is expected to
 # open. At this point, we handle only missing imports and
 # formatting imports
 
 MISSING_IMPORTS = "pyflyby.missing_imports"
 FORMATTING_IMPORTS = "pyflyby.format_imports"
@@ -63,15 +62,15 @@
         comm = Comm(target_name=INIT_COMMS)
         msg = {"type": INIT_COMMS}
         logger.debug("Requesting frontend to (re-)initialize comms")
         comm.send(msg)
 
 
 def remove_comms():
-    for target_name, comm in six.iteritems(comms):
+    for target_name, comm in comms.items():
         comm.close()
         logger.debug("Closing comm for " + target_name)
 
 def send_comm_message(target_name, msg):
     if in_jupyter():
         try:
             comm = comms[target_name]
@@ -83,15 +82,15 @@
             msg["type"] = target_name
             comm.send(msg)
             logger.debug("Sending comm message for target " + target_name)
 
 
 def comm_close_handler(comm, message):
     comm_id = message["comm_id"]
-    for target, comm in six.iterkeys(comms):
+    for target, comm in comms.keys():
         if comm.comm_id == comm_id:
             comms.pop(target)
 
 
 def _reformat_helper(input_code, imports):
     if PYFLYBY_START_MSG in input_code:
         before, bmarker, middle = input_code.partition(PYFLYBY_START_MSG)
```

### Comparing `pyflyby-1.9.2/bin/pyflyby/_dbg.py` & `pyflyby-1.9.3/bin/pyflyby/_dbg.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/bin/pyflyby/_docxref.py` & `pyflyby-1.9.3/bin/pyflyby/_docxref.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/bin/pyflyby/_file.py` & `pyflyby-1.9.3/bin/pyflyby/_file.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/bin/pyflyby/_flags.py` & `pyflyby-1.9.3/bin/pyflyby/_flags.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # License: MIT http://opensource.org/licenses/MIT
 
 
 
 import __future__
 import ast
 import operator
-from   six.moves                import reduce
+from   functools                import reduce
 import warnings
 
 from   pyflyby._util            import cached_attribute
 from typing import Tuple
 
 # Initialize mappings from compiler_flag to feature name and vice versa.
 _FLAG2NAME = {}
```

### Comparing `pyflyby-1.9.2/bin/pyflyby/_format.py` & `pyflyby-1.9.3/bin/pyflyby/_format.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/bin/pyflyby/_idents.py` & `pyflyby-1.9.3/bin/pyflyby/_idents.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/bin/pyflyby/_importclns.py` & `pyflyby-1.9.3/bin/pyflyby/_importclns.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # Copyright (C) 2011, 2012, 2013, 2014 Karl Chen.
 # License: MIT http://opensource.org/licenses/MIT
 
 
 
 from   collections              import defaultdict
 from   functools                import total_ordering
-import six
 
 from   pyflyby._flags           import CompilerFlags
 from   pyflyby._idents          import dotted_prefixes, is_identifier
 from   pyflyby._importstmt      import (Import, ImportFormatParams,
                                         ImportStatement,
                                         NonImportStatementError)
 from   pyflyby._parse           import PythonBlock
@@ -563,15 +562,15 @@
     def items(self):
         return self._data.items()
 
     def iteritems(self):
         return self._data.items()
 
     def iterkeys(self):
-        return six.iterkeys(self._data)
+        return iter(self._data.keys())
 
     def keys(self):
         return self._data.keys()
 
     def values(self):
         return self._data.values()
```

### Comparing `pyflyby-1.9.2/bin/pyflyby/_importdb.py` & `pyflyby-1.9.3/bin/pyflyby/_importdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # License: MIT http://opensource.org/licenses/MIT
 
 
 
 from   collections              import defaultdict
 import os
 import re
-import six
 
 from pyflyby._file import Filename, expand_py_files_from_args, UnsafeFilenameError
 from   pyflyby._idents          import dotted_prefixes
 from   pyflyby._importclns      import ImportMap, ImportSet
 from   pyflyby._importstmt      import Import, ImportStatement
 from   pyflyby._log             import logger
 from   pyflyby._parse           import PythonBlock
@@ -556,15 +555,15 @@
             # We don't include an entry labeled "quux" because the user has
             # implied he doesn't want to pollute the global namespace with
             # "quux", only "QUUX".
             d[imp.import_as].add(imp)
             for prefix in dotted_prefixes(imp.fullname)[:-1]:
                 d[prefix].add(Import.from_parts(prefix, prefix))
         return dict( (k, tuple(sorted(v - set(self.forget_imports.imports))))
-                     for k, v in six.iteritems(d))
+                     for k, v in d.items())
 
     def __repr__(self):
         printed = self.pretty_print()
         lines = "".join("  "+line for line in printed.splitlines(True))
         return "%s('''\n%s''')" % (type(self).__name__, lines)
 
     def pretty_print(self):
```

### Comparing `pyflyby-1.9.2/bin/pyflyby/_imports2s.py` & `pyflyby-1.9.3/bin/pyflyby/_imports2s.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/bin/pyflyby/_importstmt.py` & `pyflyby-1.9.3/bin/pyflyby/_importstmt.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/bin/pyflyby/_interactive.py` & `pyflyby-1.9.3/bin/pyflyby/_interactive.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # pyflyby/_interactive.py.
 # Copyright (C) 2011, 2012, 2013, 2014, 2015, 2018 Karl Chen.
 # License: MIT http://opensource.org/licenses/MIT
 
 
 
 import ast
+import builtins
 from   contextlib               import contextmanager
 import errno
 import inspect
 import os
+import operator
 import re
 import subprocess
 import sys
 
-import six
-from   six.moves                import builtins
 
 from   pyflyby._autoimp         import (LoadSymbolError, ScopeStack, auto_eval,
                                         auto_import,
                                         clear_failed_imports_cache,
                                         load_symbol)
 from   pyflyby._comms           import (initialize_comms, remove_comms,
                                         send_comm_message, MISSING_IMPORTS)
@@ -33,14 +33,16 @@
                                         indent)
 
 
 if False:
     __original__ = None # for pyflakes
 
 
+get_method_self = operator.attrgetter('__self__')
+
 # TODO: also support arbitrary code (in the form of a lambda and/or
 # assignment) as new way to do "lazy" creations, e.g. foo = a.b.c(d.e+f.g())
 
 
 class NoIPythonPackageError(Exception):
     """
     Exception raised when the IPython package is not installed in the system.
@@ -2094,15 +2096,15 @@
         """
         Enable a hook so that %prun will autoimport.
         """
         if hasattr(ip, 'magics_manager'):
             # Tested with IPython 1.0, 1.1, 1.2, 2.0, 2.1, 2.2, 2.3, 2.4, 3.0,
             # 3.1, 3.2, 4.0.
             line_magics = ip.magics_manager.magics['line']
-            execmgr = six.get_method_self(line_magics['prun'])#.im_self
+            execmgr = get_method_self(line_magics['prun'])#.im_self
             if hasattr(execmgr, "_run_with_profiler"):
                 @self._advise(execmgr._run_with_profiler)
                 def run_with_profiler_with_autoimport(code, opts, namespace):
                     logger.debug("run_with_profiler_with_autoimport()")
                     self.auto_import(code, [namespace])
                     return __original__(code, opts, namespace)
                 return True
@@ -2299,15 +2301,15 @@
             ok = False
         if hasattr(ip, 'magics_manager'):
             # Hook ExecutionMagics._run_with_debugger().  This implements auto
             # importing for "%debug <statement>".
             # Tested with IPython 1.0, 1.1, 1.2, 2.0, 2.1, 2.2, 2.3, 2.4, 3.0,
             # 3.1, 3.2, 4.0, 5.8.
             line_magics = ip.magics_manager.magics['line']
-            execmgr = six.get_method_self(line_magics['debug'])
+            execmgr = get_method_self(line_magics['debug'])
             if hasattr(execmgr, "_run_with_debugger"):
                 @self._advise(execmgr._run_with_debugger)
                 def run_with_debugger_with_autoimport(code, code_ns,
                                                       filename=None,
                                                       *args, **kwargs):
                     db = ImportDB.get_default(filename or ".")
                     auto_import(code, namespaces=[code_ns], db=db)
```

### Comparing `pyflyby-1.9.2/bin/pyflyby/_livepatch.py` & `pyflyby-1.9.3/bin/pyflyby/_livepatch.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,15 +134,15 @@
 import ast
 import os
 import re
 import sys
 import time
 import types
 
-from   six.moves                import reload_module
+from   importlib                import reload as reload_module
 
 import inspect
 from   pyflyby._log             import logger
 
 
 # Keep track of when the process was started.
 if os.uname()[0] == 'Linux':
```

### Comparing `pyflyby-1.9.2/bin/pyflyby/_log.py` & `pyflyby-1.9.3/bin/pyflyby/_log.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # pyflyby/_log.py.
 # Copyright (C) 2011, 2012, 2013, 2014, 2015, 2018 Karl Chen.
 # License: MIT http://opensource.org/licenses/MIT
 
 
 
+import builtins
 from   contextlib               import contextmanager
 import logging
 from   logging                  import Handler, Logger
 import os
-from   six.moves                import builtins
 import sys
 
 
 class _PyflybyHandler(Handler):
 
     _pre_log_function = None
     _logged_anything_during_context = False
```

### Comparing `pyflyby-1.9.2/bin/pyflyby/_modules.py` & `pyflyby-1.9.3/bin/pyflyby/_modules.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/bin/pyflyby/_parse.py` & `pyflyby-1.9.3/bin/pyflyby/_parse.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/bin/pyflyby/_py.py` & `pyflyby-1.9.3/bin/pyflyby/_py.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/bin/pyflyby/_util.py` & `pyflyby-1.9.3/bin/pyflyby/_util.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/bin/pyflyby-diff` & `pyflyby-1.9.3/bin/pyflyby-diff`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/bin/reformat-imports` & `pyflyby-1.9.3/bin/reformat-imports`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/bin/replace-star-imports` & `pyflyby-1.9.3/bin/replace-star-imports`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/bin/tidy-imports` & `pyflyby-1.9.3/bin/tidy-imports`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 import os
 
 from   pyflyby._cmdline         import hfmt, parse_args, process_actions
 from pyflyby._imports2s import (canonicalize_imports,
                                 fix_unused_and_missing_imports,
                                 replace_star_imports,
-                                transform_imports, sort_imports)
+                                transform_imports)
 
 import toml
 TOML_AVAIL = True
 
 
 def _get_pyproj_toml_config():
     """
@@ -152,19 +152,17 @@
             x, params=options.params,
             add_missing=options.add_missing,
             remove_unused=options.remove_unused,
             add_mandatory=options.add_mandatory,
             )
         # TODO: disable sorting until we figure out #287
         # https://github.com/deshaw/pyflyby/issues/287
-        # sorted_imports = sort_imports(x)
-        sorted_imports = x
+        # from pyflyby._imports2s import sort_imports
+        # x = sort_imports(x)
         if options.canonicalize:
-            cannonical_imports = canonicalize_imports(sorted_imports, params=options.params)
-        else:
-            cannonical_imports = sort_imports
-        return cannonical_imports
+            x = canonicalize_imports(x, params=options.params)
+        return x
     process_actions(args, options.actions, modify)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `pyflyby-1.9.2/bin/transform-imports` & `pyflyby-1.9.3/bin/transform-imports`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/doc/LICENSE.txt` & `pyflyby-1.9.3/doc/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/doc/Makefile` & `pyflyby-1.9.3/doc/Makefile`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/doc/TODO.txt` & `pyflyby-1.9.3/doc/TODO.txt`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/doc/conf.py` & `pyflyby-1.9.3/doc/conf.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/doc/make.bat` & `pyflyby-1.9.3/doc/make.bat`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/etc/pyflyby/common.py` & `pyflyby-1.9.3/etc/pyflyby/common.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/etc/pyflyby/numpy.py` & `pyflyby-1.9.3/etc/pyflyby/numpy.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/etc/pyflyby/std.py` & `pyflyby-1.9.3/etc/pyflyby/std.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,15 @@
 import six
 from   io                       import StringIO
 from   six.moves                import (builtins, cPickle, configparser,
                                         copyreg, email_mime_base,
                                         email_mime_image, email_mime_multipart,
                                         email_mime_text, http_client, map,
                                         queue, zip)
-from   six.moves.urllib.parse   import urlencode
+from   urllib.parse             import urlencode
 from   six.moves.urllib.request import urlopen
 import smtplib
 from   smtplib                  import (SMTP, SMTPAuthenticationError,
                                         SMTPConnectError, SMTPDataError,
                                         SMTPException, SMTPHeloError,
                                         SMTPRecipientsRefused,
                                         SMTPResponseException,
```

### Comparing `pyflyby-1.9.2/lib/emacs/pyflyby.el` & `pyflyby-1.9.3/lib/emacs/pyflyby.el`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/lib/python/pyflyby/__init__.py` & `pyflyby-1.9.3/lib/python/pyflyby/__init__.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/lib/python/pyflyby/_autoimp.py` & `pyflyby-1.9.3/lib/python/pyflyby/_autoimp.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/lib/python/pyflyby/_cmdline.py` & `pyflyby-1.9.3/lib/python/pyflyby/_cmdline.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/lib/python/pyflyby/_comms.py` & `pyflyby-1.9.3/lib/python/pyflyby/_comms.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from   pyflyby._imports2s       import (SourceToSourceFileImportsTransformation,
                                         SourceToSourceImportBlockTransformation,
                                         fix_unused_and_missing_imports,
                                         replace_star_imports,
                                         reformat_import_statements)
 from   pyflyby._importstmt      import Import
 from   pyflyby._log             import logger
-import six
 
 # These are comm targets that the frontend (lab/notebook) is expected to
 # open. At this point, we handle only missing imports and
 # formatting imports
 
 MISSING_IMPORTS = "pyflyby.missing_imports"
 FORMATTING_IMPORTS = "pyflyby.format_imports"
@@ -63,15 +62,15 @@
         comm = Comm(target_name=INIT_COMMS)
         msg = {"type": INIT_COMMS}
         logger.debug("Requesting frontend to (re-)initialize comms")
         comm.send(msg)
 
 
 def remove_comms():
-    for target_name, comm in six.iteritems(comms):
+    for target_name, comm in comms.items():
         comm.close()
         logger.debug("Closing comm for " + target_name)
 
 def send_comm_message(target_name, msg):
     if in_jupyter():
         try:
             comm = comms[target_name]
@@ -83,15 +82,15 @@
             msg["type"] = target_name
             comm.send(msg)
             logger.debug("Sending comm message for target " + target_name)
 
 
 def comm_close_handler(comm, message):
     comm_id = message["comm_id"]
-    for target, comm in six.iterkeys(comms):
+    for target, comm in comms.keys():
         if comm.comm_id == comm_id:
             comms.pop(target)
 
 
 def _reformat_helper(input_code, imports):
     if PYFLYBY_START_MSG in input_code:
         before, bmarker, middle = input_code.partition(PYFLYBY_START_MSG)
```

### Comparing `pyflyby-1.9.2/lib/python/pyflyby/_dbg.py` & `pyflyby-1.9.3/lib/python/pyflyby/_dbg.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/lib/python/pyflyby/_docxref.py` & `pyflyby-1.9.3/lib/python/pyflyby/_docxref.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/lib/python/pyflyby/_file.py` & `pyflyby-1.9.3/lib/python/pyflyby/_file.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/lib/python/pyflyby/_flags.py` & `pyflyby-1.9.3/lib/python/pyflyby/_flags.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # License: MIT http://opensource.org/licenses/MIT
 
 
 
 import __future__
 import ast
 import operator
-from   six.moves                import reduce
+from   functools                import reduce
 import warnings
 
 from   pyflyby._util            import cached_attribute
 from typing import Tuple
 
 # Initialize mappings from compiler_flag to feature name and vice versa.
 _FLAG2NAME = {}
```

### Comparing `pyflyby-1.9.2/lib/python/pyflyby/_format.py` & `pyflyby-1.9.3/lib/python/pyflyby/_format.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/lib/python/pyflyby/_idents.py` & `pyflyby-1.9.3/lib/python/pyflyby/_idents.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/lib/python/pyflyby/_importclns.py` & `pyflyby-1.9.3/lib/python/pyflyby/_importclns.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # Copyright (C) 2011, 2012, 2013, 2014 Karl Chen.
 # License: MIT http://opensource.org/licenses/MIT
 
 
 
 from   collections              import defaultdict
 from   functools                import total_ordering
-import six
 
 from   pyflyby._flags           import CompilerFlags
 from   pyflyby._idents          import dotted_prefixes, is_identifier
 from   pyflyby._importstmt      import (Import, ImportFormatParams,
                                         ImportStatement,
                                         NonImportStatementError)
 from   pyflyby._parse           import PythonBlock
@@ -563,15 +562,15 @@
     def items(self):
         return self._data.items()
 
     def iteritems(self):
         return self._data.items()
 
     def iterkeys(self):
-        return six.iterkeys(self._data)
+        return iter(self._data.keys())
 
     def keys(self):
         return self._data.keys()
 
     def values(self):
         return self._data.values()
```

### Comparing `pyflyby-1.9.2/lib/python/pyflyby/_importdb.py` & `pyflyby-1.9.3/lib/python/pyflyby/_importdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # License: MIT http://opensource.org/licenses/MIT
 
 
 
 from   collections              import defaultdict
 import os
 import re
-import six
 
 from pyflyby._file import Filename, expand_py_files_from_args, UnsafeFilenameError
 from   pyflyby._idents          import dotted_prefixes
 from   pyflyby._importclns      import ImportMap, ImportSet
 from   pyflyby._importstmt      import Import, ImportStatement
 from   pyflyby._log             import logger
 from   pyflyby._parse           import PythonBlock
@@ -556,15 +555,15 @@
             # We don't include an entry labeled "quux" because the user has
             # implied he doesn't want to pollute the global namespace with
             # "quux", only "QUUX".
             d[imp.import_as].add(imp)
             for prefix in dotted_prefixes(imp.fullname)[:-1]:
                 d[prefix].add(Import.from_parts(prefix, prefix))
         return dict( (k, tuple(sorted(v - set(self.forget_imports.imports))))
-                     for k, v in six.iteritems(d))
+                     for k, v in d.items())
 
     def __repr__(self):
         printed = self.pretty_print()
         lines = "".join("  "+line for line in printed.splitlines(True))
         return "%s('''\n%s''')" % (type(self).__name__, lines)
 
     def pretty_print(self):
```

### Comparing `pyflyby-1.9.2/lib/python/pyflyby/_imports2s.py` & `pyflyby-1.9.3/lib/python/pyflyby/_imports2s.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/lib/python/pyflyby/_importstmt.py` & `pyflyby-1.9.3/lib/python/pyflyby/_importstmt.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/lib/python/pyflyby/_interactive.py` & `pyflyby-1.9.3/lib/python/pyflyby/_interactive.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # pyflyby/_interactive.py.
 # Copyright (C) 2011, 2012, 2013, 2014, 2015, 2018 Karl Chen.
 # License: MIT http://opensource.org/licenses/MIT
 
 
 
 import ast
+import builtins
 from   contextlib               import contextmanager
 import errno
 import inspect
 import os
+import operator
 import re
 import subprocess
 import sys
 
-import six
-from   six.moves                import builtins
 
 from   pyflyby._autoimp         import (LoadSymbolError, ScopeStack, auto_eval,
                                         auto_import,
                                         clear_failed_imports_cache,
                                         load_symbol)
 from   pyflyby._comms           import (initialize_comms, remove_comms,
                                         send_comm_message, MISSING_IMPORTS)
@@ -33,14 +33,16 @@
                                         indent)
 
 
 if False:
     __original__ = None # for pyflakes
 
 
+get_method_self = operator.attrgetter('__self__')
+
 # TODO: also support arbitrary code (in the form of a lambda and/or
 # assignment) as new way to do "lazy" creations, e.g. foo = a.b.c(d.e+f.g())
 
 
 class NoIPythonPackageError(Exception):
     """
     Exception raised when the IPython package is not installed in the system.
@@ -2094,15 +2096,15 @@
         """
         Enable a hook so that %prun will autoimport.
         """
         if hasattr(ip, 'magics_manager'):
             # Tested with IPython 1.0, 1.1, 1.2, 2.0, 2.1, 2.2, 2.3, 2.4, 3.0,
             # 3.1, 3.2, 4.0.
             line_magics = ip.magics_manager.magics['line']
-            execmgr = six.get_method_self(line_magics['prun'])#.im_self
+            execmgr = get_method_self(line_magics['prun'])#.im_self
             if hasattr(execmgr, "_run_with_profiler"):
                 @self._advise(execmgr._run_with_profiler)
                 def run_with_profiler_with_autoimport(code, opts, namespace):
                     logger.debug("run_with_profiler_with_autoimport()")
                     self.auto_import(code, [namespace])
                     return __original__(code, opts, namespace)
                 return True
@@ -2299,15 +2301,15 @@
             ok = False
         if hasattr(ip, 'magics_manager'):
             # Hook ExecutionMagics._run_with_debugger().  This implements auto
             # importing for "%debug <statement>".
             # Tested with IPython 1.0, 1.1, 1.2, 2.0, 2.1, 2.2, 2.3, 2.4, 3.0,
             # 3.1, 3.2, 4.0, 5.8.
             line_magics = ip.magics_manager.magics['line']
-            execmgr = six.get_method_self(line_magics['debug'])
+            execmgr = get_method_self(line_magics['debug'])
             if hasattr(execmgr, "_run_with_debugger"):
                 @self._advise(execmgr._run_with_debugger)
                 def run_with_debugger_with_autoimport(code, code_ns,
                                                       filename=None,
                                                       *args, **kwargs):
                     db = ImportDB.get_default(filename or ".")
                     auto_import(code, namespaces=[code_ns], db=db)
```

### Comparing `pyflyby-1.9.2/lib/python/pyflyby/_livepatch.py` & `pyflyby-1.9.3/lib/python/pyflyby/_livepatch.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,15 +134,15 @@
 import ast
 import os
 import re
 import sys
 import time
 import types
 
-from   six.moves                import reload_module
+from   importlib                import reload as reload_module
 
 import inspect
 from   pyflyby._log             import logger
 
 
 # Keep track of when the process was started.
 if os.uname()[0] == 'Linux':
```

### Comparing `pyflyby-1.9.2/lib/python/pyflyby/_log.py` & `pyflyby-1.9.3/lib/python/pyflyby/_log.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # pyflyby/_log.py.
 # Copyright (C) 2011, 2012, 2013, 2014, 2015, 2018 Karl Chen.
 # License: MIT http://opensource.org/licenses/MIT
 
 
 
+import builtins
 from   contextlib               import contextmanager
 import logging
 from   logging                  import Handler, Logger
 import os
-from   six.moves                import builtins
 import sys
 
 
 class _PyflybyHandler(Handler):
 
     _pre_log_function = None
     _logged_anything_during_context = False
```

### Comparing `pyflyby-1.9.2/lib/python/pyflyby/_modules.py` & `pyflyby-1.9.3/lib/python/pyflyby/_modules.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/lib/python/pyflyby/_parse.py` & `pyflyby-1.9.3/lib/python/pyflyby/_parse.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/lib/python/pyflyby/_py.py` & `pyflyby-1.9.3/lib/python/pyflyby/_py.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/lib/python/pyflyby/_util.py` & `pyflyby-1.9.3/lib/python/pyflyby/_util.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/lib/python/pyflyby.egg-info/PKG-INFO` & `pyflyby-1.9.3/lib/python/pyflyby.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyflyby
-Version: 1.9.2
+Version: 1.9.3
 Summary: pyflyby - Python development productivity tools, in particular automatic import management
 Home-page: https://pypi.org/project/pyflyby/
 Author: Karl Chen
 Author-email: quarl@8166.clguba.z.quarl.org
 License: MIT
 Project-URL: Documentation, https://deshaw.github.io/pyflyby/
 Project-URL: Source, https://github.com/deshaw/pyflyby
```

### Comparing `pyflyby-1.9.2/lib/python/pyflyby.egg-info/SOURCES.txt` & `pyflyby-1.9.3/lib/python/pyflyby.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/libexec/pyflyby/colordiff` & `pyflyby-1.9.3/libexec/pyflyby/colordiff`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/libexec/pyflyby/diff-colorize` & `pyflyby-1.9.3/libexec/pyflyby/diff-colorize`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/setup.py` & `pyflyby-1.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/tests/test_0testconfig.py` & `pyflyby-1.9.3/tests/test_0testconfig.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/tests/test_autoimp.py` & `pyflyby-1.9.3/tests/test_autoimp.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/tests/test_cmdline.py` & `pyflyby-1.9.3/tests/test_cmdline.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/tests/test_docxref.py` & `pyflyby-1.9.3/tests/test_docxref.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/tests/test_file.py` & `pyflyby-1.9.3/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/tests/test_flags.py` & `pyflyby-1.9.3/tests/test_flags.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/tests/test_format.py` & `pyflyby-1.9.3/tests/test_format.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/tests/test_idents.py` & `pyflyby-1.9.3/tests/test_idents.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/tests/test_importclns.py` & `pyflyby-1.9.3/tests/test_importclns.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/tests/test_importdb.py` & `pyflyby-1.9.3/tests/test_importdb.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/tests/test_imports2s.py` & `pyflyby-1.9.3/tests/test_imports2s.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/tests/test_importstmt.py` & `pyflyby-1.9.3/tests/test_importstmt.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/tests/test_interactive.py` & `pyflyby-1.9.3/tests/test_interactive.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/tests/test_jupyterlab_pyflyby.py` & `pyflyby-1.9.3/tests/test_jupyterlab_pyflyby.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/tests/test_livepatch.py` & `pyflyby-1.9.3/tests/test_livepatch.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/tests/test_modules.py` & `pyflyby-1.9.3/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/tests/test_parse.py` & `pyflyby-1.9.3/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/tests/test_py.py` & `pyflyby-1.9.3/tests/test_py.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/tests/test_util.py` & `pyflyby-1.9.3/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/tests/tests_sorts.py` & `pyflyby-1.9.3/tests/tests_sorts.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/tests/xrefs.py` & `pyflyby-1.9.3/tests/xrefs.py`

 * *Files identical despite different names*

### Comparing `pyflyby-1.9.2/tox.ini` & `pyflyby-1.9.3/tox.ini`

 * *Files identical despite different names*

