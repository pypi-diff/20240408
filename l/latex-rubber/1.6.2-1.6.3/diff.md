# Comparing `tmp/latex-rubber-1.6.2.tar.gz` & `tmp/latex_rubber-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latex-rubber-1.6.2.tar", last modified: Tue Apr  2 23:40:48 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `latex-rubber-1.6.2.tar` & `latex_rubber-1.6.3.tar`

### file list

```diff
@@ -1,88 +1,72 @@
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2024-04-02 23:40:48.360086 latex-rubber-1.6.2/
--rw-r--r--   0 sping     (1000) sping     (1000)    35149 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/COPYING
--rw-r--r--   0 sping     (1000) sping     (1000)       38 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/MANIFEST.in
--rw-r--r--   0 sping     (1000) sping     (1000)    14527 2024-04-02 23:30:39.000000 latex-rubber-1.6.2/NEWS
--rw-r--r--   0 sping     (1000) sping     (1000)      894 2024-04-02 23:40:48.360086 latex-rubber-1.6.2/PKG-INFO
--rw-r--r--   0 sping     (1000) sping     (1000)     6574 2024-04-02 23:30:39.000000 latex-rubber-1.6.2/README
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2024-04-02 23:40:48.348085 latex-rubber-1.6.2/bin/
--rwxr-xr-x   0 sping     (1000) sping     (1000)      785 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/bin/rubber
--rwxr-xr-x   0 sping     (1000) sping     (1000)      784 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/bin/rubber-info
--rwxr-xr-x   0 sping     (1000) sping     (1000)      756 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/bin/rubber-lsmod
--rwxr-xr-x   0 sping     (1000) sping     (1000)      784 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/bin/rubber-pipe
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2024-04-02 23:40:48.347086 latex-rubber-1.6.2/doc/
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2024-04-02 23:40:48.347086 latex-rubber-1.6.2/doc/man-en/
--rw-r--r--   0 sping     (1000) sping     (1000)     2535 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/doc/man-en/rubber-info.1.in
--rw-r--r--   0 sping     (1000) sping     (1000)    18437 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/doc/man-en/rubber.1.in
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2024-04-02 23:40:48.347086 latex-rubber-1.6.2/doc/man-fr/
--rw-r--r--   0 sping     (1000) sping     (1000)     2930 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/doc/man-fr/rubber-info.1.in
--rw-r--r--   0 sping     (1000) sping     (1000)    20999 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/doc/man-fr/rubber.1.in
--rw-r--r--   0 sping     (1000) sping     (1000)    42055 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/doc/rubber.texi.in
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2024-04-02 23:40:48.360086 latex-rubber-1.6.2/latex_rubber.egg-info/
--rw-r--r--   0 sping     (1000) sping     (1000)      894 2024-04-02 23:40:48.000000 latex-rubber-1.6.2/latex_rubber.egg-info/PKG-INFO
--rw-r--r--   0 sping     (1000) sping     (1000)     2059 2024-04-02 23:40:48.000000 latex-rubber-1.6.2/latex_rubber.egg-info/SOURCES.txt
--rw-r--r--   0 sping     (1000) sping     (1000)        1 2024-04-02 23:40:48.000000 latex-rubber-1.6.2/latex_rubber.egg-info/dependency_links.txt
--rw-r--r--   0 sping     (1000) sping     (1000)        7 2024-04-02 23:40:48.000000 latex-rubber-1.6.2/latex_rubber.egg-info/top_level.txt
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2024-04-02 23:40:48.352086 latex-rubber-1.6.2/rubber/
--rw-r--r--   0 sping     (1000) sping     (1000)      305 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/__init__.py
--rw-r--r--   0 sping     (1000) sping     (1000)     6688 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/biblio.py
--rw-r--r--   0 sping     (1000) sping     (1000)    26003 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/cmdline.py
--rw-r--r--   0 sping     (1000) sping     (1000)     4265 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/contents.py
--rw-r--r--   0 sping     (1000) sping     (1000)     9270 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/convert.py
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2024-04-02 23:40:48.353086 latex-rubber-1.6.2/rubber/converters/
--rw-r--r--   0 sping     (1000) sping     (1000)        0 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/converters/__init__.py
--rw-r--r--   0 sping     (1000) sping     (1000)      887 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/converters/compressor.py
--rw-r--r--   0 sping     (1000) sping     (1000)     1840 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/converters/eps_gz.py
--rw-r--r--   0 sping     (1000) sping     (1000)     2115 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/converters/fig2dev.py
--rw-r--r--   0 sping     (1000) sping     (1000)    48052 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/converters/latex.py
--rw-r--r--   0 sping     (1000) sping     (1000)     1025 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/converters/literate.py
--rw-r--r--   0 sping     (1000) sping     (1000)     7804 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/converters/mpost.py
--rw-r--r--   0 sping     (1000) sping     (1000)      761 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/converters/shell.py
--rw-r--r--   0 sping     (1000) sping     (1000)    11277 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/depend.py
--rw-r--r--   0 sping     (1000) sping     (1000)     1926 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/dvip_tool.py
--rw-r--r--   0 sping     (1000) sping     (1000)     4782 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/environment.py
--rw-r--r--   0 sping     (1000) sping     (1000)     4272 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/index.py
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2024-04-02 23:40:48.360086 latex-rubber-1.6.2/rubber/latex_modules/
--rw-r--r--   0 sping     (1000) sping     (1000)        0 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/__init__.py
--rw-r--r--   0 sping     (1000) sping     (1000)      233 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/aleph.py
--rw-r--r--   0 sping     (1000) sping     (1000)     4204 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/asymptote.py
--rw-r--r--   0 sping     (1000) sping     (1000)      283 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/backref.py
--rw-r--r--   0 sping     (1000) sping     (1000)      570 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/beamer.py
--rw-r--r--   0 sping     (1000) sping     (1000)     4274 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/biblatex.py
--rw-r--r--   0 sping     (1000) sping     (1000)      863 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/bibtex.py
--rw-r--r--   0 sping     (1000) sping     (1000)     2362 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/bibtopic.py
--rw-r--r--   0 sping     (1000) sping     (1000)     1665 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/combine.py
--rw-r--r--   0 sping     (1000) sping     (1000)      264 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/dvipdfm.py
--rw-r--r--   0 sping     (1000) sping     (1000)      262 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/dvips.py
--rw-r--r--   0 sping     (1000) sping     (1000)     1298 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/epsfig.py
--rw-r--r--   0 sping     (1000) sping     (1000)      588 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/glossaries.py
--rw-r--r--   0 sping     (1000) sping     (1000)      212 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/gnuplottex.py
--rw-r--r--   0 sping     (1000) sping     (1000)     7513 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/graphics.py
--rw-r--r--   0 sping     (1000) sping     (1000)     7513 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/graphicx.py
--rw-r--r--   0 sping     (1000) sping     (1000)      370 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/hyperref.py
--rw-r--r--   0 sping     (1000) sping     (1000)     3602 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/index.py
--rw-r--r--   0 sping     (1000) sping     (1000)      866 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/listings.py
--rw-r--r--   0 sping     (1000) sping     (1000)      620 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/ltxtable.py
--rw-r--r--   0 sping     (1000) sping     (1000)      317 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/lualatex.py
--rw-r--r--   0 sping     (1000) sping     (1000)      288 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/makeidx.py
--rw-r--r--   0 sping     (1000) sping     (1000)     1654 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/minitoc-hyper.py
--rw-r--r--   0 sping     (1000) sping     (1000)     1654 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/minitoc.py
--rw-r--r--   0 sping     (1000) sping     (1000)     1044 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/moreverb.py
--rw-r--r--   0 sping     (1000) sping     (1000)     2544 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/multibib.py
--rw-r--r--   0 sping     (1000) sping     (1000)      492 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/nomencl.py
--rw-r--r--   0 sping     (1000) sping     (1000)      283 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/ntheorem.py
--rw-r--r--   0 sping     (1000) sping     (1000)      234 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/omega.py
--rw-r--r--   0 sping     (1000) sping     (1000)     1069 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/pdftex.py
--rw-r--r--   0 sping     (1000) sping     (1000)      692 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/ps2pdf.py
--rw-r--r--   0 sping     (1000) sping     (1000)     1431 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/pythontex.py
--rw-r--r--   0 sping     (1000) sping     (1000)      669 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/verbatim.py
--rw-r--r--   0 sping     (1000) sping     (1000)      907 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/vtex.py
--rw-r--r--   0 sping     (1000) sping     (1000)      315 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/xelatex.py
--rw-r--r--   0 sping     (1000) sping     (1000)     1021 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/latex_modules/xr.py
--rw-r--r--   0 sping     (1000) sping     (1000)     3831 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/module_interface.py
--rw-r--r--   0 sping     (1000) sping     (1000)     2158 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/rules.ini
--rw-r--r--   0 sping     (1000) sping     (1000)    14742 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/tex.py
--rw-r--r--   0 sping     (1000) sping     (1000)    10336 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/util.py
--rw-r--r--   0 sping     (1000) sping     (1000)       18 2024-04-02 23:40:16.000000 latex-rubber-1.6.2/rubber/version.py
--rw-r--r--   0 sping     (1000) sping     (1000)       22 2024-03-30 14:41:12.000000 latex-rubber-1.6.2/rubber/version.py.in
--rw-r--r--   0 sping     (1000) sping     (1000)       38 2024-04-02 23:40:48.360086 latex-rubber-1.6.2/setup.cfg
--rw-r--r--   0 sping     (1000) sping     (1000)    10152 2024-04-02 23:30:39.000000 latex-rubber-1.6.2/setup.py
+-rw-r--r--   0        0        0    74904 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/doc/rubber.html
+-rw-r--r--   0        0        0    48721 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/doc/rubber.info
+-rw-r--r--   0        0        0   178373 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/doc/rubber.pdf
+-rw-r--r--   0        0        0    42055 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/doc/rubber.texi
+-rw-r--r--   0        0        0    42677 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/doc/rubber.txt
+-rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/doc/man-en/rubber-info.1
+-rw-r--r--   0        0        0    18467 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/doc/man-en/rubber.1
+-rw-r--r--   0        0        0     2960 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/doc/man-fr/rubber-info.1
+-rw-r--r--   0        0        0    21029 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/doc/man-fr/rubber.1
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/__init__.py
+-rw-r--r--   0        0        0     6688 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/biblio.py
+-rw-r--r--   0        0        0    26287 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/cmdline.py
+-rw-r--r--   0        0        0     4265 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/contents.py
+-rw-r--r--   0        0        0     9270 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/convert.py
+-rw-r--r--   0        0        0    11277 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/depend.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/dvip_tool.py
+-rw-r--r--   0        0        0     4782 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/environment.py
+-rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/index.py
+-rw-r--r--   0        0        0     3831 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/module_interface.py
+-rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/rules.ini
+-rw-r--r--   0        0        0    14742 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/tex.py
+-rw-r--r--   0        0        0    10336 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/util.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/converters/__init__.py
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/converters/compressor.py
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/converters/eps_gz.py
+-rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/converters/fig2dev.py
+-rw-r--r--   0        0        0    48052 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/converters/latex.py
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/converters/literate.py
+-rw-r--r--   0        0        0     7804 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/converters/mpost.py
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/converters/shell.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/__init__.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/aleph.py
+-rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/asymptote.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/backref.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/beamer.py
+-rw-r--r--   0        0        0     4274 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/biblatex.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/bibtex.py
+-rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/bibtopic.py
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/combine.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/dvipdfm.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/dvips.py
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/epsfig.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/glossaries.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/gnuplottex.py
+-rw-r--r--   0        0        0     7513 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/graphics.py
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/graphicx.py -> graphics.py
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/hyperref.py
+-rw-r--r--   0        0        0     3602 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/index.py
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/listings.py
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/ltxtable.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/lualatex.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/makeidx.py
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/minitoc-hyper.py -> minitoc.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/minitoc.py
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/moreverb.py
+-rw-r--r--   0        0        0     2544 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/multibib.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/nomencl.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/ntheorem.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/omega.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/pdftex.py
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/ps2pdf.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/pythontex.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/verbatim.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/vtex.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/xelatex.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/rubber/latex_modules/xr.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/COPYING
+-rw-r--r--   0        0        0     8269 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/hatch_build.py
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/pyproject.toml
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 latex_rubber-1.6.3/PKG-INFO
```

### Comparing `latex-rubber-1.6.2/COPYING` & `latex_rubber-1.6.3/COPYING`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.2/doc/man-en/rubber-info.1.in` & `latex_rubber-1.6.3/doc/man-en/rubber-info.1`

 * *Files 4% similar despite different names*

```diff
@@ -62,17 +62,17 @@
 Stupidly enumerate all LaTeX warnings, i.e. all the lines in the log file that
 contain the string "Warning".
 .PP
 
 .SH BUGS
 There are surely a some...
 
-This page documents Rubber version @version@.
-The program and this man-page are maintained by @maintainer@ <@maintainer_email@>.
-The homepage for Rubber can be found at @url@.
+This page documents Rubber version 1.6.3.
+The program and this man-page are maintained by Florian Schmaus <flo@geekplace.eu>.
+The homepage for Rubber can be found at https://gitlab.com/latex-rubber/rubber.
 
 .SH SEE ALSO
 The full documentation for
 .B rubber
 is maintained as a Texinfo manual.  If the
 .B info
 and
```

### Comparing `latex-rubber-1.6.2/doc/man-en/rubber.1.in` & `latex_rubber-1.6.3/doc/man-en/rubber.1`

 * *Files 1% similar despite different names*

```diff
@@ -636,17 +636,17 @@
 module, which may be used to specify the list of bibliographies the command
 applies to.
 .PP
 .
 .SH BUGS
 There are surely a some...
 .PP
-This page documents Rubber version @version@.
-The program and this man-page are maintained by @maintainer@ <@maintainer_email@>.
-The homepage for Rubber can be found at @url@.
+This page documents Rubber version 1.6.3.
+The program and this man-page are maintained by Florian Schmaus <flo@geekplace.eu>.
+The homepage for Rubber can be found at https://gitlab.com/latex-rubber/rubber.
 .
 .SH SEE ALSO
 The full documentation for
 .B rubber
 is maintained as a Texinfo manual.  If the
 .B info
 and
```

### Comparing `latex-rubber-1.6.2/doc/man-fr/rubber-info.1.in` & `latex_rubber-1.6.3/doc/man-fr/rubber-info.1`

 * *Files 4% similar despite different names*

```diff
@@ -68,17 +68,17 @@
 Affiche stupidement la liste de tous les avertissements de LaTeX, c'est-à-dire
 toutes les lignes du fichier log qui contiennent « Warning ».
 .PP
 
 .SH BUGS
 Il y en a surement quelques uns...
 
-Cette page se rapporte à la version @version@ de Rubber. Le programme et cette
-documentation sont maintenus par @maintainer@ <@maintainer_email@>.
-La page web du programme se trouve à l'adresse @url@.
+Cette page se rapporte à la version 1.6.3 de Rubber. Le programme et cette
+documentation sont maintenus par Florian Schmaus <flo@geekplace.eu>.
+La page web du programme se trouve à l'adresse https://gitlab.com/latex-rubber/rubber.
 
 .SH VOIR AUSSI
 La documentation complète de
 .B rubber
 est maintenue en tant que manuel en Texinfo. Si les programmes
 .B info
 et
```

### Comparing `latex-rubber-1.6.2/doc/man-fr/rubber.1.in` & `latex_rubber-1.6.3/doc/man-fr/rubber.1`

 * *Files 2% similar despite different names*

```diff
@@ -657,17 +657,17 @@
 qui permet de spécifier la liste des bibliographies auxquelles s’applique la
 commande.
 .PP
 .
 .SH BUGS
 Il y en a surement quelques uns...
 .PP
-Cette page se rapporte à la version @version@ de Rubber. Le programme et cette
-documentation sont maintenus par @maintainer@ <@maintainer_email@>.
-La page web du programme se trouve à l’adresse @url@.
+Cette page se rapporte à la version 1.6.3 de Rubber. Le programme et cette
+documentation sont maintenus par Florian Schmaus <flo@geekplace.eu>.
+La page web du programme se trouve à l’adresse https://gitlab.com/latex-rubber/rubber.
 .
 .SH VOIR AUSSI
 La documentation complète de
 .B rubber
 est maintenue en tant que manuel en Texinfo.
 Si les programmes
 .B info
```

### Comparing `latex-rubber-1.6.2/doc/rubber.texi.in` & `latex_rubber-1.6.3/doc/rubber.texi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 \input texinfo
 @c %**start of header
 @setfilename rubber.info
-@settitle Rubber Manual @version@
+@settitle Rubber Manual 1.6.3
 @c %**end of header
 
 @copying
 Permission is granted to make and distribute verbatim
 copies of this manual provided the copyright notice and
 this permission notice are preserved on all copies.
 
@@ -27,16 +27,16 @@
 Copyright @copyright{} 2002--2006 Emmanuel Beffara.
 
 Copyright @copyright{} 2006--2015 Sebastian Kapfer.
 @end copying
 
 @titlepage
 @title Rubber
-@subtitle Documentation for version @version@
-@author @author@
+@subtitle Documentation for version 1.6.3
+@author Sebastian Kapfer
 @page
 @vskip 0pt plus 1fill
 @insertcopying
 @end titlepage
 
 @iftex
 @contents
```

### Comparing `latex-rubber-1.6.2/rubber/biblio.py` & `latex_rubber-1.6.3/rubber/biblio.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.2/rubber/cmdline.py` & `latex_rubber-1.6.3/rubber/cmdline.py`

 * *Files 2% similar despite different names*

```diff
@@ -673,7 +673,25 @@
                 msg.info(_("There is no undefined reference."))
         else:
             assert act == "warnings"
             for err in log.get_warnings():
                 display(short, **err)
             else:
                 msg.info(_("There is no warning."))
+
+
+def main_rubber_plain():
+    main(RUBBER_PLAIN)
+
+
+def main_rubber_info():
+    main(RUBBER_INFO)
+
+
+def main_rubber_pipe():
+    main(RUBBER_PIPE)
+
+
+def main_rubber_lsmod():
+    from rubber.util import iter_rubber_modules
+    for module in iter_rubber_modules():
+        print(module)
```

### Comparing `latex-rubber-1.6.2/rubber/contents.py` & `latex_rubber-1.6.3/rubber/contents.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.2/rubber/convert.py` & `latex_rubber-1.6.3/rubber/convert.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.2/rubber/converters/compressor.py` & `latex_rubber-1.6.3/rubber/converters/compressor.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.2/rubber/converters/eps_gz.py` & `latex_rubber-1.6.3/rubber/converters/eps_gz.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.2/rubber/converters/fig2dev.py` & `latex_rubber-1.6.3/rubber/converters/fig2dev.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.2/rubber/converters/latex.py` & `latex_rubber-1.6.3/rubber/converters/latex.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.2/rubber/converters/literate.py` & `latex_rubber-1.6.3/rubber/converters/literate.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.2/rubber/converters/mpost.py` & `latex_rubber-1.6.3/rubber/converters/mpost.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.2/rubber/converters/shell.py` & `latex_rubber-1.6.3/rubber/converters/shell.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.2/rubber/depend.py` & `latex_rubber-1.6.3/rubber/depend.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.2/rubber/dvip_tool.py` & `latex_rubber-1.6.3/rubber/dvip_tool.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.2/rubber/environment.py` & `latex_rubber-1.6.3/rubber/environment.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.2/rubber/index.py` & `latex_rubber-1.6.3/rubber/index.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.2/rubber/latex_modules/asymptote.py` & `latex_rubber-1.6.3/rubber/latex_modules/asymptote.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.2/rubber/latex_modules/beamer.py` & `latex_rubber-1.6.3/rubber/latex_modules/beamer.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.2/rubber/latex_modules/biblatex.py` & `latex_rubber-1.6.3/rubber/latex_modules/biblatex.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.2/rubber/latex_modules/bibtex.py` & `latex_rubber-1.6.3/rubber/latex_modules/bibtex.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.2/rubber/latex_modules/bibtopic.py` & `latex_rubber-1.6.3/rubber/latex_modules/bibtopic.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.2/rubber/latex_modules/combine.py` & `latex_rubber-1.6.3/rubber/latex_modules/combine.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.2/rubber/latex_modules/epsfig.py` & `latex_rubber-1.6.3/rubber/latex_modules/epsfig.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.2/rubber/latex_modules/glossaries.py` & `latex_rubber-1.6.3/rubber/latex_modules/glossaries.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.2/rubber/latex_modules/graphics.py` & `latex_rubber-1.6.3/rubber/latex_modules/graphics.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.2/rubber/latex_modules/index.py` & `latex_rubber-1.6.3/rubber/latex_modules/index.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.2/rubber/latex_modules/listings.py` & `latex_rubber-1.6.3/rubber/latex_modules/listings.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.2/rubber/latex_modules/ltxtable.py` & `latex_rubber-1.6.3/rubber/latex_modules/ltxtable.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.2/rubber/latex_modules/minitoc-hyper.py` & `latex_rubber-1.6.3/rubber/latex_modules/minitoc.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.2/rubber/latex_modules/moreverb.py` & `latex_rubber-1.6.3/rubber/latex_modules/moreverb.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.2/rubber/latex_modules/multibib.py` & `latex_rubber-1.6.3/rubber/latex_modules/multibib.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.2/rubber/latex_modules/pdftex.py` & `latex_rubber-1.6.3/rubber/latex_modules/pdftex.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.2/rubber/latex_modules/ps2pdf.py` & `latex_rubber-1.6.3/rubber/latex_modules/ps2pdf.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.2/rubber/latex_modules/pythontex.py` & `latex_rubber-1.6.3/rubber/latex_modules/pythontex.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.2/rubber/latex_modules/verbatim.py` & `latex_rubber-1.6.3/rubber/latex_modules/verbatim.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.2/rubber/latex_modules/vtex.py` & `latex_rubber-1.6.3/rubber/latex_modules/vtex.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.2/rubber/latex_modules/xr.py` & `latex_rubber-1.6.3/rubber/latex_modules/xr.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.2/rubber/module_interface.py` & `latex_rubber-1.6.3/rubber/module_interface.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.2/rubber/rules.ini` & `latex_rubber-1.6.3/rubber/rules.ini`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.2/rubber/tex.py` & `latex_rubber-1.6.3/rubber/tex.py`

 * *Files identical despite different names*

### Comparing `latex-rubber-1.6.2/rubber/util.py` & `latex_rubber-1.6.3/rubber/util.py`

 * *Files identical despite different names*

