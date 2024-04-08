# Comparing `tmp/jpylyzer-2.2.0b1.tar.gz` & `tmp/jpylyzer-2.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jpylyzer-2.2.0b1.tar", last modified: Mon Oct 30 13:12:23 2023, max compression
+gzip compressed data, was "dist/jpylyzer-2.2.0rc1.tar", last modified: Mon Nov  6 17:51:28 2023, max compression
```

## Comparing `jpylyzer-2.2.0b1.tar` & `jpylyzer-2.2.0rc1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-30 13:12:23.000000 jpylyzer-2.2.0b1/
--rw-rw-r--   0 root         (0) root         (0)     5200 2023-09-11 16:39:20.000000 jpylyzer-2.2.0b1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-30 13:12:23.000000 jpylyzer-2.2.0b1/example_files/
--rw-rw-r--   0 root         (0) root         (0)   670264 2019-02-15 11:04:54.000000 jpylyzer-2.2.0b1/example_files/balloon_trunc1.jp2
--rw-rw-r--   0 root         (0) root         (0)     5000 2019-02-15 11:04:54.000000 jpylyzer-2.2.0b1/example_files/balloon_trunc2.jp2
--rw-rw-r--   0 root         (0) root         (0)   645179 2019-02-15 11:04:54.000000 jpylyzer-2.2.0b1/example_files/balloon_trunc3.jp2
--rw-rw-r--   0 root         (0) root         (0)      606 2019-02-15 11:04:54.000000 jpylyzer-2.2.0b1/example_files/readme.txt
--rw-rw-r--   0 root         (0) root         (0)   670265 2019-02-15 11:04:54.000000 jpylyzer-2.2.0b1/example_files/balloon.jp2
--rwxrwxr-x   0 root         (0) root         (0)     2084 2023-09-07 14:37:02.000000 jpylyzer-2.2.0b1/setup.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-10-30 13:12:23.000000 jpylyzer-2.2.0b1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-30 13:12:23.000000 jpylyzer-2.2.0b1/jpylyzer/
--rw-rw-r--   0 root         (0) root         (0)      173 2022-08-03 13:21:05.000000 jpylyzer-2.2.0b1/jpylyzer/__init__.pyc
--rwxrwxr-x   0 root         (0) root         (0)    15443 2023-10-05 17:24:33.000000 jpylyzer-2.2.0b1/jpylyzer/mix.py
--rw-rw-r--   0 root         (0) root         (0)      708 2023-09-07 15:06:46.000000 jpylyzer-2.2.0b1/jpylyzer/config.pyc
--rw-rw-r--   0 root         (0) root         (0)     4602 2023-10-05 17:24:21.000000 jpylyzer-2.2.0b1/jpylyzer/etpatch.py
--rw-rw-r--   0 root         (0) root         (0)     1442 2022-08-03 13:21:05.000000 jpylyzer-2.2.0b1/jpylyzer/shared.pyc
--rw-rw-r--   0 root         (0) root         (0)     4075 2023-09-07 14:57:21.000000 jpylyzer-2.2.0b1/jpylyzer/etpatch.pyc
--rw-rw-r--   0 root         (0) root         (0)    10294 2022-08-03 13:21:05.000000 jpylyzer-2.2.0b1/jpylyzer/mix.pyc
--rw-rw-r--   0 root         (0) root         (0)    57623 2023-09-07 14:57:21.000000 jpylyzer-2.2.0b1/jpylyzer/boxvalidator.pyc
--rw-rw-r--   0 root         (0) root         (0)      138 2023-09-07 14:50:19.000000 jpylyzer-2.2.0b1/jpylyzer/__main__.py
--rw-rw-r--   0 root         (0) root         (0)     4795 2023-09-07 14:57:21.000000 jpylyzer-2.2.0b1/jpylyzer/byteconv.pyc
--rw-rw-r--   0 root         (0) root         (0)     4175 2023-10-05 17:24:08.000000 jpylyzer-2.2.0b1/jpylyzer/byteconv.py
--rw-rw-r--   0 root         (0) root         (0)    19676 2023-09-07 15:10:26.000000 jpylyzer-2.2.0b1/jpylyzer/jpylyzer.pyc
--rwxrwxr-x   0 root         (0) root         (0)    28410 2023-10-30 13:04:28.000000 jpylyzer-2.2.0b1/jpylyzer/jpylyzer.py
--rw-rw-r--   0 root         (0) root         (0)     1492 2019-11-22 12:41:22.000000 jpylyzer-2.2.0b1/jpylyzer/shared.py
--rw-rw-r--   0 root         (0) root         (0)     1046 2023-10-19 17:06:06.000000 jpylyzer-2.2.0b1/jpylyzer/config.py
--rw-rw-r--   0 root         (0) root         (0)   151525 2023-10-25 16:08:16.000000 jpylyzer-2.2.0b1/jpylyzer/boxvalidator.py
--rw-rw-r--   0 root         (0) root         (0)       29 2019-11-22 12:41:22.000000 jpylyzer-2.2.0b1/jpylyzer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-30 13:12:23.000000 jpylyzer-2.2.0b1/doc/
--rw-rw-r--   0 root         (0) root         (0)   489743 2022-08-04 16:33:49.000000 jpylyzer-2.2.0b1/doc/jpylyzerUserManual.html
--rw-rw-r--   0 root         (0) root         (0)   167623 2022-08-04 16:33:49.000000 jpylyzer-2.2.0b1/doc/userManual.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-30 13:12:23.000000 jpylyzer-2.2.0b1/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-30 13:12:23.000000 jpylyzer-2.2.0b1/tests/unit/
--rw-rw-r--   0 root         (0) root         (0)    11598 2023-10-26 15:32:04.000000 jpylyzer-2.2.0b1/tests/unit/test_testfiles.py
--rw-rw-r--   0 root         (0) root         (0)     1903 2022-08-08 14:56:55.000000 jpylyzer-2.2.0b1/tests/unit/test_jpylyzer.py
--rw-rw-r--   0 root         (0) root         (0)     2966 2023-09-07 15:52:06.000000 jpylyzer-2.2.0b1/tests/unit/notest_openjpeg.py
--rw-rw-r--   0 root         (0) root         (0)        0 2019-11-22 12:41:22.000000 jpylyzer-2.2.0b1/tests/unit/__init__.py
--rw-rw-r--   0 root         (0) root         (0)        0 2019-11-22 12:41:22.000000 jpylyzer-2.2.0b1/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5845 2023-10-30 13:12:23.000000 jpylyzer-2.2.0b1/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     2273 2019-02-15 11:04:54.000000 jpylyzer-2.2.0b1/LICENSE
--rw-rw-r--   0 root         (0) root         (0)       63 2019-02-15 11:04:54.000000 jpylyzer-2.2.0b1/MANIFEST.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-30 13:12:23.000000 jpylyzer-2.2.0b1/jpylyzer.egg-info/
--rw-r--r--   0 root         (0) root         (0)       15 2023-10-30 13:12:23.000000 jpylyzer-2.2.0b1/jpylyzer.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-10-30 13:12:23.000000 jpylyzer-2.2.0b1/jpylyzer.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      911 2023-10-30 13:12:23.000000 jpylyzer-2.2.0b1/jpylyzer.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-30 13:12:23.000000 jpylyzer-2.2.0b1/jpylyzer.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     5845 2023-10-30 13:12:23.000000 jpylyzer-2.2.0b1/jpylyzer.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      101 2023-10-30 13:12:23.000000 jpylyzer-2.2.0b1/jpylyzer.egg-info/requires.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-06 17:51:28.000000 jpylyzer-2.2.0rc1/
+-rw-rw-r--   0 root         (0) root         (0)     5568 2023-11-03 19:06:15.000000 jpylyzer-2.2.0rc1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-06 17:51:28.000000 jpylyzer-2.2.0rc1/example_files/
+-rw-rw-r--   0 root         (0) root         (0)   670264 2019-02-15 11:04:54.000000 jpylyzer-2.2.0rc1/example_files/balloon_trunc1.jp2
+-rw-rw-r--   0 root         (0) root         (0)     5000 2019-02-15 11:04:54.000000 jpylyzer-2.2.0rc1/example_files/balloon_trunc2.jp2
+-rw-rw-r--   0 root         (0) root         (0)   645179 2019-02-15 11:04:54.000000 jpylyzer-2.2.0rc1/example_files/balloon_trunc3.jp2
+-rw-rw-r--   0 root         (0) root         (0)      606 2019-02-15 11:04:54.000000 jpylyzer-2.2.0rc1/example_files/readme.txt
+-rw-rw-r--   0 root         (0) root         (0)   670265 2019-02-15 11:04:54.000000 jpylyzer-2.2.0rc1/example_files/balloon.jp2
+-rwxrwxr-x   0 root         (0) root         (0)     2084 2023-09-07 14:37:02.000000 jpylyzer-2.2.0rc1/setup.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-11-06 17:51:28.000000 jpylyzer-2.2.0rc1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-06 17:51:28.000000 jpylyzer-2.2.0rc1/jpylyzer/
+-rw-rw-r--   0 root         (0) root         (0)      173 2022-08-03 13:21:05.000000 jpylyzer-2.2.0rc1/jpylyzer/__init__.pyc
+-rwxrwxr-x   0 root         (0) root         (0)    15443 2023-10-05 17:24:33.000000 jpylyzer-2.2.0rc1/jpylyzer/mix.py
+-rw-rw-r--   0 root         (0) root         (0)      708 2023-09-07 15:06:46.000000 jpylyzer-2.2.0rc1/jpylyzer/config.pyc
+-rw-rw-r--   0 root         (0) root         (0)     4602 2023-10-05 17:24:21.000000 jpylyzer-2.2.0rc1/jpylyzer/etpatch.py
+-rw-rw-r--   0 root         (0) root         (0)     1442 2022-08-03 13:21:05.000000 jpylyzer-2.2.0rc1/jpylyzer/shared.pyc
+-rw-rw-r--   0 root         (0) root         (0)     4075 2023-09-07 14:57:21.000000 jpylyzer-2.2.0rc1/jpylyzer/etpatch.pyc
+-rw-rw-r--   0 root         (0) root         (0)    10294 2022-08-03 13:21:05.000000 jpylyzer-2.2.0rc1/jpylyzer/mix.pyc
+-rw-rw-r--   0 root         (0) root         (0)    57623 2023-09-07 14:57:21.000000 jpylyzer-2.2.0rc1/jpylyzer/boxvalidator.pyc
+-rw-rw-r--   0 root         (0) root         (0)      138 2023-09-07 14:50:19.000000 jpylyzer-2.2.0rc1/jpylyzer/__main__.py
+-rw-rw-r--   0 root         (0) root         (0)     4795 2023-09-07 14:57:21.000000 jpylyzer-2.2.0rc1/jpylyzer/byteconv.pyc
+-rw-rw-r--   0 root         (0) root         (0)     4175 2023-10-05 17:24:08.000000 jpylyzer-2.2.0rc1/jpylyzer/byteconv.py
+-rw-rw-r--   0 root         (0) root         (0)    19676 2023-09-07 15:10:26.000000 jpylyzer-2.2.0rc1/jpylyzer/jpylyzer.pyc
+-rwxrwxr-x   0 root         (0) root         (0)    28355 2023-11-06 17:47:04.000000 jpylyzer-2.2.0rc1/jpylyzer/jpylyzer.py
+-rw-rw-r--   0 root         (0) root         (0)     1492 2019-11-22 12:41:22.000000 jpylyzer-2.2.0rc1/jpylyzer/shared.py
+-rw-rw-r--   0 root         (0) root         (0)     1046 2023-10-19 17:06:06.000000 jpylyzer-2.2.0rc1/jpylyzer/config.py
+-rw-rw-r--   0 root         (0) root         (0)   151525 2023-10-25 16:08:16.000000 jpylyzer-2.2.0rc1/jpylyzer/boxvalidator.py
+-rw-rw-r--   0 root         (0) root         (0)       29 2019-11-22 12:41:22.000000 jpylyzer-2.2.0rc1/jpylyzer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-06 17:51:28.000000 jpylyzer-2.2.0rc1/doc/
+-rw-rw-r--   0 root         (0) root         (0)   508528 2023-11-03 19:06:38.000000 jpylyzer-2.2.0rc1/doc/jpylyzerUserManual.html
+-rw-rw-r--   0 root         (0) root         (0)   178266 2023-11-03 19:06:37.000000 jpylyzer-2.2.0rc1/doc/userManual.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-06 17:51:28.000000 jpylyzer-2.2.0rc1/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-06 17:51:28.000000 jpylyzer-2.2.0rc1/tests/unit/
+-rw-rw-r--   0 root         (0) root         (0)    12006 2023-11-01 11:49:30.000000 jpylyzer-2.2.0rc1/tests/unit/test_testfiles.py
+-rw-rw-r--   0 root         (0) root         (0)     1903 2022-08-08 14:56:55.000000 jpylyzer-2.2.0rc1/tests/unit/test_jpylyzer.py
+-rw-rw-r--   0 root         (0) root         (0)     2966 2023-09-07 15:52:06.000000 jpylyzer-2.2.0rc1/tests/unit/notest_openjpeg.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2019-11-22 12:41:22.000000 jpylyzer-2.2.0rc1/tests/unit/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2019-11-22 12:41:22.000000 jpylyzer-2.2.0rc1/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6215 2023-11-06 17:51:28.000000 jpylyzer-2.2.0rc1/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     2273 2019-02-15 11:04:54.000000 jpylyzer-2.2.0rc1/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)       63 2019-02-15 11:04:54.000000 jpylyzer-2.2.0rc1/MANIFEST.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-06 17:51:28.000000 jpylyzer-2.2.0rc1/jpylyzer.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       15 2023-11-06 17:51:28.000000 jpylyzer-2.2.0rc1/jpylyzer.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-11-06 17:51:28.000000 jpylyzer-2.2.0rc1/jpylyzer.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      911 2023-11-06 17:51:28.000000 jpylyzer-2.2.0rc1/jpylyzer.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-11-06 17:51:28.000000 jpylyzer-2.2.0rc1/jpylyzer.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     6215 2023-11-06 17:51:28.000000 jpylyzer-2.2.0rc1/jpylyzer.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      101 2023-11-06 17:51:28.000000 jpylyzer-2.2.0rc1/jpylyzer.egg-info/requires.txt
```

### Comparing `jpylyzer-2.2.0b1/README.md` & `jpylyzer-2.2.0rc1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -17,47 +17,71 @@
 - [![Build Status](https://jenkins.openpreservation.org/buildStatus/icon?job=jpylyzer%2Fjpylyzer)](https://jenkins.openpreservation.org/job/jpylyzer/job/jpylyzer/) OPF Jenkins
 <!-- Start of text to be copied to usage.md of jpylyzer website -->
 
 ## Using jpylyzer from the command line
 
 Calling *jpylyzer* in a command window without any arguments results in the following helper message:
 
-    usage: jpylyzer [-h] [--format FMT] [--mix {1,2}] [--nopretty]
-              [--nullxml] [--recurse] [--packetmarkers] [--verbose]
-              [--version] jp2In [jp2In ...]
+```
+usage: jpylyzer [-h] [--format FMT] [--mix {1,2}] [--nopretty]
+            [--nullxml] [--recurse] [--packetmarkers] [--verbose]
+            [--version] jp2In [jp2In ...]
+```
 
 ### Positional arguments
 
 |Argument|Description|
 |:--|:--|
-|`jp2In`|input JP2 image(s), may be one or more (whitespace-separated) path expressions; prefix wildcard (\*) with backslash (\\) in Linux|
+|`jp2In`|input image(s), may be one or more (whitespace-separated) path expressions; prefix wildcard (\*) with backslash (\\) in Linux|
 
 ### Optional arguments
 
 |Argument|Description|
 |:--|:--|
 |`[-h, --help]`|show help message and exit|
-|`[--format FMT]`|validation format; allowed values are `jp2` (used by default) and `j2c` (which activates raw codestream validation)|
+|`[--format FMT]`|validation format; allowed values are `jp2` (JPEG 2000 Part 1, used by default), `j2c` (Part 1 codestream), `jph` (JPEG 2000 Part 15 / High Throughput JPEG 2000) and `jhc` (Part 15 codestream)|
 |`[--mix {1,2}]`|report additional output in NISO MIX format (version 1.0 or 2.0)|
 |`[--nopretty]`|suppress pretty-printing of XML output|
 |`[--nullxml]`|extract null-terminated XML content from XML and UUID boxes(doesn't affect validation)|
 |`[--recurse, -r]`|when analysing a directory, recurse into subdirectories|
 |`[--packetmarkers]`|Report packet-level codestream markers (plm, ppm, plt, ppt)|
 |`[--verbose]`|report test results in verbose format|
 |`[-v, --version]`|show program's version number and exit|
 
 ## Output
 
 Output is directed to the standard output device (*stdout*).
 
-### Example
+## Examples
+
+Validate JP2 image:
+
+```
+jpylyzer rubbish.jp2 > rubbish-jp2.xml`
+```
+
+Validate JPEG 2000 Part 1 codestream:
+
+```
+jpylyzer --format j2c rubbish.j2c > rubbish-j2c.xml`
+```
+
+Validate JPH (High Throughput) image:
 
-`jpylyzer rubbish.jp2 > rubbish.xml`
+```
+jpylyzer --format jph rubbish.jph > rubbish-jph.xml`
+```
 
-In the above example, output is redirected to the file &#8216;rubbish.xml&#8217;. By default *jpylyzer*&#8217;s XML is pretty-printed, so you should be able to view the file using your favourite text editor. Alternatively use a dedicated XML editor, or open the file in your web browser.
+Validate JPEG 2000 Part 15 (High Throughput) codestream:
+
+```
+jpylyzer --format jhc rubbish.jhc > rubbish-jhc.xml`
+```
+
+In the above examples, output is redirected to the output files &#8216;rubbish-???.xml&#8217;. By default *jpylyzer*&#8217;s XML is pretty-printed, so you should be able to view the file using your favourite text editor. Alternatively use a dedicated XML editor, or open the file in your web browser.
 
 ## Output format
 
 The output file contains the following top-level elements:
 
 1. One *toolInfo* element, which contains information about *jpylyzer* (its name and version number)
 
@@ -76,14 +100,16 @@
 4. *tests*: outcome of the individual tests that are part of the
 validation process (organised by box)
 
 5. *properties*: image properties (organised by box)
 
 6. *propertiesExtension*: wrapper element for NISO *MIX* output (only if the `--mix` option is used)
 
+7. *warnings*: reported warnings
+
 ## Using jpylyzer as a Python module
 
 Instead of using *jpylyzer* from the command-line, you can also import
 it as a module in your own Python programs. To do so, install jpylyzer
 with *pip*. Then import *jpylyzer* into your code by adding:
 
 ```python
@@ -106,16 +132,15 @@
 
 # Return image height value
 imageHeight = myResult.findtext('./properties/jp2HeaderBox/imageHeaderBox/height')
 print(imageHeight)
 ```
 
 Here, *myResult* is an *Element* object that can either be used directly,
-or converted to XML using the *ElementTree* module[^3]. The structure of the
-element object follows the XML output that described in [Chapter 5](#output-format).
+or converted to XML using the *ElementTree* module[^3].
 
 For validation a raw JPEG 2000 codestreams, call the *checkOneFile* function with the additional
 *validationFormat* argument, and set it to `j2c`:
 
 ```python
 # Define Codestream
 myFile = "/home/johan/jpylyzer-test-files/rubbish.j2c"
```

### Comparing `jpylyzer-2.2.0b1/example_files/balloon_trunc1.jp2` & `jpylyzer-2.2.0rc1/example_files/balloon_trunc1.jp2`

 * *Files identical despite different names*

### Comparing `jpylyzer-2.2.0b1/example_files/balloon_trunc2.jp2` & `jpylyzer-2.2.0rc1/example_files/balloon_trunc2.jp2`

 * *Files identical despite different names*

### Comparing `jpylyzer-2.2.0b1/example_files/balloon_trunc3.jp2` & `jpylyzer-2.2.0rc1/example_files/balloon_trunc3.jp2`

 * *Files identical despite different names*

### Comparing `jpylyzer-2.2.0b1/example_files/readme.txt` & `jpylyzer-2.2.0rc1/example_files/readme.txt`

 * *Files identical despite different names*

### Comparing `jpylyzer-2.2.0b1/example_files/balloon.jp2` & `jpylyzer-2.2.0rc1/example_files/balloon.jp2`

 * *Files identical despite different names*

### Comparing `jpylyzer-2.2.0b1/setup.py` & `jpylyzer-2.2.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `jpylyzer-2.2.0b1/jpylyzer/mix.py` & `jpylyzer-2.2.0rc1/jpylyzer/mix.py`

 * *Files identical despite different names*

### Comparing `jpylyzer-2.2.0b1/jpylyzer/config.pyc` & `jpylyzer-2.2.0rc1/jpylyzer/config.pyc`

 * *Files identical despite different names*

### Comparing `jpylyzer-2.2.0b1/jpylyzer/etpatch.py` & `jpylyzer-2.2.0rc1/jpylyzer/etpatch.py`

 * *Files identical despite different names*

### Comparing `jpylyzer-2.2.0b1/jpylyzer/shared.pyc` & `jpylyzer-2.2.0rc1/jpylyzer/shared.pyc`

 * *Files identical despite different names*

### Comparing `jpylyzer-2.2.0b1/jpylyzer/etpatch.pyc` & `jpylyzer-2.2.0rc1/jpylyzer/etpatch.pyc`

 * *Files identical despite different names*

### Comparing `jpylyzer-2.2.0b1/jpylyzer/mix.pyc` & `jpylyzer-2.2.0rc1/jpylyzer/mix.pyc`

 * *Files identical despite different names*

### Comparing `jpylyzer-2.2.0b1/jpylyzer/boxvalidator.pyc` & `jpylyzer-2.2.0rc1/jpylyzer/boxvalidator.pyc`

 * *Files identical despite different names*

### Comparing `jpylyzer-2.2.0b1/jpylyzer/byteconv.pyc` & `jpylyzer-2.2.0rc1/jpylyzer/byteconv.pyc`

 * *Files identical despite different names*

### Comparing `jpylyzer-2.2.0b1/jpylyzer/byteconv.py` & `jpylyzer-2.2.0rc1/jpylyzer/byteconv.py`

 * *Files identical despite different names*

### Comparing `jpylyzer-2.2.0b1/jpylyzer/jpylyzer.pyc` & `jpylyzer-2.2.0rc1/jpylyzer/jpylyzer.pyc`

 * *Files identical despite different names*

### Comparing `jpylyzer-2.2.0b1/jpylyzer/jpylyzer.py` & `jpylyzer-2.2.0rc1/jpylyzer/jpylyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
 SCRIPT_PATH, SCRIPT_NAME = os.path.split(sys.argv[0])
 
 # SCRIPT_NAME is empty when called from Java/Jython, so this needs a fix
 if not SCRIPT_NAME:
     SCRIPT_NAME = 'jpylyzer'
 
-__version__ = "2.2.0b1"
+__version__ = "2.2.0rc1"
 
 # Create PARSER
 PARSER = argparse.ArgumentParser(
     description="JP2 image validator and properties extractor")
 
 # list of existing files to be analysed
 EXISTING_FILES = []
@@ -432,17 +432,14 @@
             failureMessage = "I/O error (cannot open file)"
         elif exceptionType == RuntimeError:
             failureMessage = "runtime error, please report to developers by creating " + \
                              "an issue at https://github.com/openpreserve/jpylyzer/issues"
         else:
             failureMessage = "unknown error, please report to developers by creating " + \
                              "an issue at https://github.com/openpreserve/jpylyzer/issues"
-            # TEST
-            raise
-            # TEST
 
         tests = ET.Element("tests")
         characteristics = ET.Element("properties")
         warnings = ET.Element("warnings")
         warnings.appendChildTagWithText("warning", failureMessage)
         shared.printWarning(failureMessage)
```

### Comparing `jpylyzer-2.2.0b1/jpylyzer/shared.py` & `jpylyzer-2.2.0rc1/jpylyzer/shared.py`

 * *Files identical despite different names*

### Comparing `jpylyzer-2.2.0b1/jpylyzer/config.py` & `jpylyzer-2.2.0rc1/jpylyzer/config.py`

 * *Files identical despite different names*

### Comparing `jpylyzer-2.2.0b1/jpylyzer/boxvalidator.py` & `jpylyzer-2.2.0rc1/jpylyzer/boxvalidator.py`

 * *Files identical despite different names*

### Comparing `jpylyzer-2.2.0b1/doc/jpylyzerUserManual.html` & `jpylyzer-2.2.0rc1/doc/jpylyzerUserManual.html`

 * *Files 4% similar despite different names*

```diff
@@ -63,14 +63,15 @@
 <li><a href="#file-element">file element</a></li>
 <li><a href="#fileinfo-element">fileInfo element</a></li>
 <li><a href="#statusinfo-element">statusInfo element</a></li>
 <li><a href="#isvalid-element">isValid element</a></li>
 <li><a href="#tests-element">tests element</a></li>
 <li><a href="#properties-element">properties element</a></li>
 <li><a href="#propertiesExtension-element">propertiesExtension element</a></li>
+<li><a href="#warnings-element">warnings element</a></li>
 </ul></li>
 <li><a href="#jp2-box-by-box">JP2: box by box</a>
 <ul>
 <li><a href="#about-properties-tests-trees">About the properties and tests trees</a></li>
 <li><a href="#jpeg2000-signature-box">JPEG 2000 Signature box</a></li>
 <li><a href="#file-type-box">File Type box</a></li>
 <li><a href="#jp2-header-box">JP2 Header box (superbox)</a></li>
@@ -104,14 +105,17 @@
 <li><a href="#coc-marker">Coding style component (COC) marker segment</a></li>
 <li><a href="#rgn-marker">Region-of-interest (RGN) marker segment</a></li>
 <li><a href="#qcd-marker">Quantization default (QCD) marker segment</a></li>
 <li><a href="#qcc-marker">Quantization component (QCC) marker segment</a></li>
 <li><a href="#poc-marker">Progression order change (POC) marker segment</a></li>
 <li><a href="#crg-marker">Component registration (CRG) marker segment</a></li>
 <li><a href="#com-marker">Comment (COM) marker segment</a></li>
+<li><a href="#cap-marker">Extended capabilities (CAP) marker segment</a></li>
+<li><a href="#prf-marker">Profile (PRF) marker segment</a></li>
+<li><a href="#cpf-marker">Corresponding profile (CPF) marker segment</a></li>
 <li><a href="#tile-part">Tile part (child of Contiguous Codestream box)</a></li>
 <li><a href="#sot-marker">Start of tile part (SOT) marker segment (child of tile part)</a></li>
 <li><a href="#tlm-marker">Tile-part lengths (TLM) marker segment</a></li>
 <li><a href="#plm-marker">Packet length, main header (PLM) marker segment</a></li>
 <li><a href="#ppm-marker">Packed packet headers, main header (PPM) marker segment</a></li>
 <li><a href="#plt-marker">Packet length, tile-part header (PLT) marker segment</a></li>
 <li><a href="#ppt-marker">Packed packet headers, tile-part header (PPT) marker segment</a></li>
@@ -122,14 +126,15 @@
 <h1 id="introduction">Introduction</h1>
 <h2 id="about-jpylyzer">About jpylyzer</h2>
 <p>This User Manual documents <em>jpylyzer</em>, a validator and feature extractor for JP2 images. JP2 is the still image format that is defined by JPEG 2000 Part 1 (ISO/IEC 15444-1). <em>Jpylyzer</em> was specifically created to answer the following questions that you might have about any JP2 file:</p>
 <ol type="1">
 <li><p>Is this really a JP2 and does it really conform to the format’s specifications (validation)?</p></li>
 <li><p>What are the technical characteristics of this image (feature extraction)?</p></li>
 </ol>
+<p>Starting with version 2.2, <em>jpylyzer</em> also supports Part 15 of the standard (ISO/IEC 15444-15, High Throughput JPEG 2000), and its JPH image format.</p>
 <h2 id="validation-scope-and-restrictions">Validation: scope and restrictions</h2>
 <p>Since the word ‘validation’ means different things to different people, a few words about the overall scope of <em>jpylyzer</em>. First of all, it is important to stress that <em>jpylyzer</em> is not a ‘one stop solution’ that will tell you that an image is 100% perfect. What <em>jpylyzer</em> does is this: based on the JP2 format specification (ISO/IEC 15444-1), it parses a file. It then subjects the file’s contents to a large number of tests, each of which is based on the requirements and restrictions that are defined by the standard. If a file fails one or more tests, this implies that it does not conform to the standard, and is no valid JP2. Importantly, this presumes that <em>jpylyzer</em>’s tests accurately reflect the format specification, without producing false positives.</p>
 <h3 id="valid-means-probably-valid">‘Valid’ means ‘probably valid’</h3>
 <p>If a file passes all tests, this is an indication that it is <em>probably</em> valid JP2. This (intentionally) implies a certain degree of remaining uncertainty, which is related to the following.</p>
 <p>First of all, <em>jpylyzer</em> (or any other format validator for that matter) ‘validates’ a file by trying to prove that it does <em>not</em> conform to the standard. It cannot prove that that a file <em>does</em> conform to the standard.</p>
 <p>Related to this, even though <em>jpylyzer</em>’s validation process is very comprehensive, it is not complete. For instance, the validation of JPEG 2000 codestreams at this moment is still somewhat limited. These limitations are discussed in detail <a href="#limitations-codestream-validation">here</a>. Some of these limitations (e.g. optional codestream segment markers that are only minimally supported at this stage) may be taken away in upcoming versions of the tool.</p>
 <h3 id="no-check-on-compressed-bitstreams">No check on compressed bitstreams</h3>
@@ -137,16 +142,14 @@
 <h3 id="recommendations-for-use-in-quality-assurance-workflows">Recommendations for use in quality assurance workflows</h3>
 <p>Because of the foregoing, a thorough JP2 quality assurance workflow should not rely on <em>jpylyzer</em> (or any other format validator) alone, but it should include other tests as well. Some obvious examples are:</p>
 <ul>
 <li><p>A rendering test that checks if a file renders at all</p></li>
 <li><p>Format migration workflows (e.g. TIFF to JP2) should ideally also include some comparison between source and destination images (e.g. a pixel-wise comparison)</p></li>
 </ul>
 <p>Conversely, an image that successfully passes a rendering test or pixel-wise comparison may still contain problematic features (e.g. incorrect colour space information), so validation, rendering tests and pixel-wise comparisons are really complementary to each other.</p>
-<h3 id="note-on-icc-profile-support">Note on ICC profile support</h3>
-<p>The support of ICC profiles in JP2 was recently extended through an <a href="https://www.itu.int/rec/T-REC-T.800-201303-P!Amd6/en">amendment</a> to the standard. These changes are taken into account by <em>jpylyzer</em>, which is in line with the most recent version of the (updated) standard.</p>
 <h2 id="outline">Outline of this User Manual</h2>
 <p>We start by describing the <a href="#installation">installation process</a> of <em>jpylyzer</em> for Windows and Unix-based systems. We then explain its <a href="#using-jpylyzer">basic usage</a>, either as a command-line tool, or as an importable Python module. This is followed by a brief overview of <a href="#structure-jp2">the structure of the JP2 format</a> and its ‘box’ structure, and an explanation of <em>Jpylyzer</em>’s <a href="#output-format">output format</a>. The final sections give a detailed description of the tests that <em>jpylyzer</em> performs for validation, and the properties that are reported in the output. The <a href="#jp2-box-by-box">penultimate section</a> does this for all ‘boxes’, except the ‘Contiguous Codestream’ box, which is given a <a href="#contiguous-codestream-box-chapter">section of its own</a>.</p>
 <h2 id="funding">Funding</h2>
 <p>The development of <em>jpylyzer</em> was funded by the EU FP 7 project SCAPE (SCAlable Preservation Environments). More information about this project can be found here:</p>
 <p><a href="https://www.scape-project.eu/">https://www.scape-project.eu/</a></p>
 <h2 id="license">License</h2>
 <p><em>Jpylyzer</em> is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more details. You should have received a copy of the GNU Lesser General Public License along with this program. If not, see:</p>
@@ -155,15 +158,15 @@
 <pre><code>/usr/share/common-licenses/LGPL-3</code></pre>
 <h1 id="installation">Installation and set-up</h1>
 <h2 id="obtaining-the-software">Obtaining the software</h2>
 <p>To obtain the latest version of the software please use the download links at the <em>jpylyzer</em> homepage:</p>
 <p><a href="https://jpylyzer.openpreservation.org/" class="uri">https://jpylyzer.openpreservation.org/</a></p>
 <p>You have three options:</p>
 <ol type="1">
-<li><p>Install the software with the <em>Pip</em> package manager. This works on all platforms (Windows, Linux, Mac, etc.), but you need to have the Python interpreter available on your system. Jpylyzer is compatible with Python 2.7, and Python 3.2 and more recent (Python 3.0 and 3.1 are not supported).</p></li>
+<li><p>Install the software with the <em>Pip</em> package manager. This works on all platforms (Windows, Linux, Mac, etc.), but you need to have the Python interpreter available on your system. Jpylyzer is compatible with Python 3.2 and more recent.</p></li>
 <li><p>Alternatively, for Windows users there is also a set of stand-alone binaries<a href="#fn1" class="footnote-ref" id="fnref1" role="doc-noteref"><sup>1</sup></a>. These allow you to run <em>jpylyzer</em> as an executable Windows application, without any need for installing Python. This option is particularly useful for Windows users who cannot (or don’t want to) install software on their system.</p></li>
 <li><p>For Linux users Debian packages are available.</p></li>
 </ol>
 <p>These options are described in the following sub-sections.</p>
 <h2 id="installation-pip">Installation with Pip (Linux/Unix, Windows, Mac OS X)</h2>
 <h3 id="general-installation-procedure">General installation procedure</h3>
 <p>First make sure you have a recent version of <em>pip</em>. Then install <em>jpylyzer</em> with the following command:</p>
@@ -179,18 +182,17 @@
 <pre><code># set PATH so it includes the user&#39;s .local bin if it exists
 if [ -d &quot;$HOME/.local/bin&quot; ] ; then
     PATH=&quot;$HOME/.local/bin:$PATH&quot;
 fi</code></pre>
 <p>Save the file, log out of your session and then log in again. Open a command terminal and type:</p>
 <pre><code>jpylyzer</code></pre>
 <p>If all went well you now see this:</p>
-<pre><code>usage: jpylyzer [-h] [--format FMT] [--legacyout] [--mix {1,2}] [--nopretty]
+<pre><code>usage: jpylyzer [-h] [--format FMT] [--mix {1,2}] [--nopretty]
           [--nullxml] [--recurse] [--packetmarkers] [--verbose]
-          [--version] [--wrapper]
-          jp2In [jp2In ...]
+          [--version] jp2In [jp2In ...]
 jpylyzer: error: the following arguments are required: jp2In</code></pre>
 <p>Which means that the installation was successful!</p>
 <h3 id="global-installation-linux">Global installation (Linux)</h3>
 <p>Simply enter:</p>
 <pre><code>sudo -H pip install jpylyzer</code></pre>
 <p>No further configuration is needed in this case.</p>
 <h3 id="note-on-pre-releases">Note on pre-releases</h3>
@@ -200,24 +202,23 @@
 <p>Download the binary using the link on the <em>jpylyzer</em> homepage. Unzip the contents of this file to an empty folder on your PC. <em>Jpylyzer</em> should now be ready for use.</p>
 <h3 id="testing-the-installation">Testing the installation</h3>
 <p>To test your installation, open a Command Prompt (‘DOS prompt’) and type:</p>
 <pre><code>%jpylyzerPath%\jpylyzer</code></pre>
 <p>In the above command, replace <em>%jpylyzerPath%</em> with the full path to the <em>jpylyzer</em> installation directory (i.e. the directory that contains ‘jpylyzer.exe’ and its associated files). For example, if you extracted the files to directory <code>c:\tools\jpylyzer</code>, the command would become:</p>
 <pre><code>c:\tools\jpylyzer\jpylyzer</code></pre>
 <p>Executing this command should result in the following screen output:</p>
-<pre><code>usage: jpylyzer [-h] [--format FMT] [--legacyout] [--mix {1,2}] [--nopretty]
+<pre><code>usage: jpylyzer [-h] [--format FMT] [--mix {1,2}] [--nopretty]
           [--nullxml] [--recurse] [--packetmarkers] [--verbose]
-          [--version] [--wrapper]
-          jp2In [jp2In ...]
+          [--version] jp2In [jp2In ...]
 jpylyzer: error: the following arguments are required: jp2In</code></pre>
 <h3 id="running-jpylyzer-without-typing-the-full-path">Running jpylyzer without typing the full path</h3>
 <p>Optionally, you may also want to add the full path of the <em>jpylyzer</em> installation directory to the Windows ’Path’ environment variable. Doing so allows you to run <em>jpylyzer</em> from any directory on your PC without having to type the full path. In Windows 7 you can do this by selecting ‘settings’ from the ‘Start’ menu; then go to ‘control panel’/’system’ and go to the ‘advanced’ tab. Click on the ‘environment variables’ button. Finally, locate the ‘Path’ variable in the ‘system variables’ window, click on ‘Edit’ and add the full <em>jpylyzer</em> path (this requires local Administrator privileges). The settings take effect on any newly opened command prompt.</p>
 <h2 id="installation-debian">Installation of Debian packages (Ubuntu/Linux)</h2>
 <p>For Linux, Debian packages of <em>jpylyzer</em> exist. To install, simply download the <em>.deb</em> file, double-click on it and select <em>Install Package</em>. Alternatively you can also do this in the command terminal by typing:</p>
-<pre><code>sudo dpkg -i opf-jpylyzer_2.0.0_all.deb</code></pre>
+<pre><code>sudo dpkg -i opf-jpylyzer_2.2.0_all.deb</code></pre>
 <p>In both cases you need to have administrative privileges.</p>
 <p>For <em>Ubuntu</em> and <em>Debian</em> alternative packages are available in the official release channels. To install simply run the following commands:</p>
 <pre><code>sudo apt-get update
 sudo apt-get install python-jpylyzer</code></pre>
 <h1 id="using-jpylyzer">Using <em>jpylyzer</em></h1>
 <h2 id="using-overview">Overview</h2>
 <p>This section describes the general use of <em>jpylyzer</em>. The first sub-sections cover the use of <em>jpylyzer</em> as a command-line tool and as an importable Python module.</p>
@@ -240,30 +241,29 @@
 <td style="text-align: left;"><code>c:\tools\jpylyzer\jpylyzer</code></td>
 </tr>
 </tbody>
 </table>
 <p>Furthermore, command line arguments that are given between square brackets (example: <code>[-h]</code>) are optional.</p>
 <h3 id="synopsis">Synopsis</h3>
 <p><em>Jpylyzer</em> can be invoked using the following command-line arguments:</p>
-<pre><code>usage: jpylyzer [-h] [--format FMT] [--legacyout] [--mix {1,2}] [--nopretty]
+<pre><code>usage: jpylyzer [-h] [--format FMT] [--mix {1,2}] [--nopretty]
           [--nullxml] [--recurse] [--packetmarkers] [--verbose]
-          [--version] [--wrapper]
-          jp2In [jp2In ...]</code></pre>
+          [--version] jp2In [jp2In ...]</code></pre>
 <h4 id="positional-arguments">Positional arguments</h4>
 <table>
 <thead>
 <tr class="header">
 <th style="text-align: left;">Argument</th>
 <th style="text-align: left;">Description</th>
 </tr>
 </thead>
 <tbody>
 <tr class="odd">
 <td style="text-align: left;"><code>jp2In</code></td>
-<td style="text-align: left;">input JP2 image(s), may be one or more (whitespace-separated) path expressions; prefix wildcard (*) with backslash (\) in Linux</td>
+<td style="text-align: left;">input image(s), may be one or more (whitespace-separated) path expressions; prefix wildcard (*) with backslash (\) in Linux</td>
 </tr>
 </tbody>
 </table>
 <h4 id="optional-arguments">Optional arguments</h4>
 <table>
 <thead>
 <tr class="header">
@@ -274,52 +274,44 @@
 <tbody>
 <tr class="odd">
 <td style="text-align: left;"><code>[-h, --help]</code></td>
 <td style="text-align: left;">show help message and exit</td>
 </tr>
 <tr class="even">
 <td style="text-align: left;"><code>[--format FMT]</code></td>
-<td style="text-align: left;">validation format; allowed values are <code>jp2</code> (used by default) and <code>j2c</code> (which activates raw codestream validation)</td>
+<td style="text-align: left;">validation format; allowed values are <code>jp2</code> (JPEG 2000 Part 1, used by default), <code>j2c</code> (Part 1 codestream), <code>jph</code> (JPEG 2000 Part 15 / High Throughput JPEG 2000) and <code>jhc</code> (Part 15 codestream)</td>
 </tr>
 <tr class="odd">
 <td style="text-align: left;"><code>[--mix {1,2}]</code></td>
 <td style="text-align: left;">report additional output in NISO MIX format (version 1.0 or 2.0)</td>
 </tr>
 <tr class="even">
-<td style="text-align: left;"><code>[--legacyout]</code></td>
-<td style="text-align: left;">report output in jpylyzer 1.x format (provided for backward compatibility only)</td>
-</tr>
-<tr class="odd">
 <td style="text-align: left;"><code>[--nopretty]</code></td>
 <td style="text-align: left;">suppress pretty-printing of XML output</td>
 </tr>
-<tr class="even">
+<tr class="odd">
 <td style="text-align: left;"><code>[--nullxml]</code></td>
 <td style="text-align: left;">extract null-terminated XML content from XML and UUID boxes(doesn’t affect validation)</td>
 </tr>
-<tr class="odd">
+<tr class="even">
 <td style="text-align: left;"><code>[--recurse, -r]</code></td>
-<td style="text-align: left;">when analysing a directory, recurse into subdirectories (implies <code>--wrapper</code> if <code>--legacyout</code> is used)</td>
+<td style="text-align: left;">when analysing a directory, recurse into subdirectories</td>
 </tr>
-<tr class="even">
+<tr class="odd">
 <td style="text-align: left;"><code>[--packetmarkers]</code></td>
 <td style="text-align: left;">Report packet-level codestream markers (plm, ppm, plt, ppt)</td>
 </tr>
-<tr class="odd">
+<tr class="even">
 <td style="text-align: left;"><code>[--verbose]</code></td>
 <td style="text-align: left;">report test results in verbose format</td>
 </tr>
-<tr class="even">
+<tr class="odd">
 <td style="text-align: left;"><code>[-v, --version]</code></td>
 <td style="text-align: left;">show program’s version number and exit</td>
 </tr>
-<tr class="odd">
-<td style="text-align: left;"><code>[--wrapper, -w]</code></td>
-<td style="text-align: left;">wrap output for individual image(s) in ‘results’ XML element (deprecated from jpylyzer 2.x onward, only takes effect if <code>--legacyout</code> is used)</td>
-</tr>
 </tbody>
 </table>
 <p>Note that the input can either be a single image, a space-separated sequence of images, a pathname expression that includes multiple images, or any combination of the above. For example, the following command will process one single image:</p>
 <pre><code>jpylyzer rubbish.jp2</code></pre>
 <p>The next example shows how to process all files with a ‘jp2’ extension in the current directory:</p>
 <pre><code>jpylyzer *.jp2</code></pre>
 <p>Note that on Unix/Linux based systems pathname expressions may not work properly unless you wrap them in quotation marks:</p>
@@ -329,44 +321,39 @@
 <pre><code>jpylyzer jp2In &gt; outputFile</code></pre>
 <p>E.g. the following command will run <em>jpylyzer</em> on image ‘rubbish.jp2’ and redirects the output to file ‘rubbish.xml’:</p>
 <pre><code>jpylyzer rubbish.jp2 &gt; rubbish.xml</code></pre>
 <p>The format of the XML output is described <a href="#output-format">here</a>.</p>
 <h3 id="format-option">‘format’ option</h3>
 <p>By default, <em>jpylyzer</em> validates against the <em>JP2</em> format specification. Starting with version 2.0, <em>jpylyzer</em> can also validate raw JPEG 2000 codestreams that are not wrapped inside a <em>JP2</em> container. For codestream validation, use the <code>--format</code> option with value <code>j2c</code>, e.g.:</p>
 <pre><code>jpylyzer --format j2c rubbish.j2c &gt; rubbish.xml</code></pre>
+<p>Starting with version 2.2, <em>jpylyzer</em> also supports JPEG 2000 Part 15 (High Throughput JPEG 2000) and its <em>JPH</em> container format. To validate a <em>JPH</em> file, use the <code>--format</code> option with value <code>jph</code>:</p>
+<pre><code>jpylyzer --format jph rubbish.jph &gt; rubbish.xml</code></pre>
+<p>And use <code>--format</code> with value <code>jhc</code> to validate a raw High Throughput codestream:</p>
+<pre><code>jpylyzer --format jhc rubbish.jhc &gt; rubbish.xml</code></pre>
 <h3 id="mix-option">‘mix’ option</h3>
 <p>When this option is used, <em>jpylyzer</em> reports additional output in <a href="https://www.loc.gov/standards/mix/"><em>NISO MIX</em></a> format. This option takes one argument that defines whether <em>MIX</em> 1.0 or <em>MIX</em> 2.0 is used. For example, the following command will result in <em>MIX</em> 2.0 output:</p>
 <pre><code>jpylyzer --mix 2 rubbish.jp2 &gt; rubbish.xml</code></pre>
-<p>The <em>MIX</em> output is wrapped inside a <em>file/propertiesExtension</em> element. Note that <em>MIX</em> output is <em>only</em> written for files that are valid JP2 (files that are not valid result in an empty <em>propertiesExtension</em> element). Also, the <code>--mix</code> option is ignored if <code>--format</code> is set to <code>j2c</code>, or if <code>--legacyout</code> (see below) is used.</p>
-<h3 id="legacyout-option">‘legacyout’ option</h3>
-<p>The output format of <em>jpylyzer</em> has changed in version 2.0, which may break existing workflows that expect output in 1.x format. For backward compatibility the <code>--legacyout</code> option results in output that follows the old 1.x format. Note that codestream validation is disabled if you use this option.</p>
+<p>The <em>MIX</em> output is wrapped inside a <em>file/propertiesExtension</em> element. Note that <em>MIX</em> output is <em>only</em> written for files that are valid JP2 or JPH (files that are not valid result in an empty <em>propertiesExtension</em> element). Also, the <code>--mix</code> option is ignored if <code>--format</code> is set to <code>j2c</code>.</p>
 <h3 id="recurse-option">‘recurse’ option</h3>
 <p>If the <code>--recurse</code> option is used, <em>jpylyzer</em> will recursively traverse all subdirectories of a filepath expression. E.g:</p>
 <pre><code>jpylyzer /home/myJP2s/*.jp2 &gt; rubbish.xml</code></pre>
 <p>In this case <em>jpylyzer</em> analyses all files that have a <em>.jp2</em> extension in directory <em>/home/myJP2s</em> and all its subdirectories.</p>
 <h3 id="packetmarkers-option">‘packetmarkers’ option</h3>
 <p>When this option is enabled, jpylyzer will report the properties of the following packet-level codestream markers:</p>
 <ul>
 <li>PLM (packet length, main header) marker</li>
 <li>PPM (packed packet headers, main header) marker</li>
 <li>PLT (packet length, tile-part header) marker</li>
 <li>PPT (packed packet headers, tile-part header) marker</li>
 </ul>
 <p>By default these are excluded from the output, in order to prevent excessive output size.</p>
-<h3 id="wrapper-option-deprecated">‘wrapper’ option (deprecated)</h3>
-<p>This deprecated option is included for backward-compatibility, and only takes effect if <code>--legacyout</code> (see above) is used.By default, the <em>jpylyzer</em> 1.x releases would create a separate XML tree for each analysed image, without any overarching hierarchy. For multiple-image pathname expressions this resulted in output that was <strong>not</strong> well-formed XML. The <code>--legacyout</code> option still results in this is behaviour. For example:</p>
-<pre><code>jpylyzer --legacyout rubbish.jp2 garbage.jp2 &gt; rubbish.xml</code></pre>
-<p>In this case, the file ‘rubbish.xml’ contains a succession of two XML trees, which by itself is not well-formed XML. The <code>--wrapper</code> option is provided to create valid XML instead:</p>
-<pre><code>jpylyzer --legacyout --wrapper rubbish.jp2 garbage.jp2 &gt; rubbish.xml</code></pre>
-<p>In the above case the XML trees of the individual images are wrapped inside a ‘results’ element. When the <code>--recurse</code> option is used, jpylyzer will automatically wrap the output in a ‘results’ element, so there’s no need to specify <code>--wrapper</code> in that case.</p>
-<p>Starting with version 2.0, <em>jpylyzer</em> <em>always</em> generates well-formed XML (unless the <code>--legacyout</code> option is used), which makes the <code>--wrapper</code> option largely obsolete, apart from cases where the ‘old’ behaviour is needed for backward-compatibility reasons.</p>
 <h3 id="nullxml-option">‘nullxml’ option</h3>
 <p>The <em>nullxml</em> option was added to enable extraction of XML content that is terminated by a null-byte. By default <em>jpylyzer</em> doesn’t report the XML in that case, because it throws an exception in the XML parser. Apparently some old versions of the Kakadu demo applications would erroneously add a null-byte to embedded XML, so this option can be used to force extraction for images that are affected by this.</p>
 <h3 id="user-warnings">User warnings</h3>
-<p>Under the following conditions <em>jpylyzer</em> will print a user warning to the standard error device (typically the console screen):</p>
+<p>Under the following conditions <em>jpylyzer</em> will report a user warning:</p>
 <h4 id="no-images-to-check">No images to check</h4>
 <p>If there are no input images to check (typically because the value of jp2In refers to a non-existent file), the following warning message is shown:</p>
 <pre><code>User warning: no images to check!</code></pre>
 <h4 id="unsupported-box">Unsupported box</h4>
 <p>In some cases you will see the following warning message:</p>
 <pre><code>User warning: ignoring &#39;boxName&#39; (validator function not yet implemented)</code></pre>
 <p>The reason for this: a JP2 file is made up of units that are called ‘boxes’. This is explained in more detail <a href="#structure-jp2">here</a>. Each ‘box’ has its own dedicated validator function. At this stage validator functions are still missing for a small number of (optional) boxes. <em>Jpylyzer</em> will display the above warning message if it encounters a (yet) unsupported box. Any unsupported boxes are simply ignored, and the remainder of the file will be analyzed (and validated) normally.</p>
@@ -382,40 +369,49 @@
 <pre><code>User warning: unknown error (please report to developers)</code></pre>
 <p>If you ever run into either of these two errors, please get in touch with the jpylyzer developers. The easiest way to do this is to create a new issue at:</p>
 <p><a href="https://github.com/openpreserve/jpylyzer/issues" class="uri">https://github.com/openpreserve/jpylyzer/issues</a></p>
 <h4 id="unknown-box">Unknown box</h4>
 <p>Occasionally, you may see this warning message:</p>
 <pre><code>User warning: ignoring unknown box</code></pre>
 <p>This happens if <em>jpylyzer</em> encounters a box that is not defined by JPEG 2000 Part 1. It should be noted that, to a large extent, JPEG 2000 Part 1 permits the presence of boxes that are defined outside the standard. Again, <em>jpylyzer</em> will simply ignore these and process all other boxes normally.</p>
+<p>All user warnings are printed to the standard error device (typically the console screen). File-level warnings are also written to the <em>warnings</em> output element.</p>
 <h2 id="using-as-python-module">Using <em>jpylyzer</em> as a Python module</h2>
 <p>Instead of using <em>jpylyzer</em> from the command-line, you can also import it as a module in your own Python programs. To do so, install jpylyzer with <em>pip</em>. Then import <em>jpylyzer</em> into your code by adding:</p>
 <pre><code>from jpylyzer import jpylyzer</code></pre>
 <p>Subsequently you can call any function that is defined in <em>jpylyzer.py</em>. In practice you will most likely only need the <em>checkOneFile</em> function. The following minimal script shows how this works:</p>
-<pre><code>#! /usr/bin/env python
+<pre><code>#! /usr/bin/env python3
 
 from jpylyzer import jpylyzer
 
 # Define JP2
 myFile = &quot;/home/johan/jpylyzer-test-files/aware.jp2&quot;
 
 # Analyse with jpylyzer, result to Element object
 myResult = jpylyzer.checkOneFile(myFile)
 
 # Return image height value
 imageHeight = myResult.findtext(&#39;./properties/jp2HeaderBox/imageHeaderBox/height&#39;)
 print(imageHeight)</code></pre>
 <p>Here, <em>myResult</em> is an <em>Element</em> object that can either be used directly, or converted to XML using the <em>ElementTree</em> module<a href="#fn2" class="footnote-ref" id="fnref2" role="doc-noteref"><sup>2</sup></a>. The structure of the element object follows the XML output that described <a href="#output-format">here</a>.</p>
-<p>For validation a raw JPEG 2000 codestreams, call the <em>checkOneFile</em> function with the additional <em>validationFormat</em> argument, and set it to <code>j2c</code>:</p>
+<p>You may use the following optional arguments (which correspond to the command-line options explained above):</p>
+<ul>
+<li>validationFormat - sets the validation format. Values: ‘jp2’ (default), ‘jph’, ‘j2c’ or ‘jhc’.</li>
+<li>verboseFlag - report test results in verbose format. Values: False (default) or True.</li>
+<li>packetmarkersFlag - report packet-level codestream markers. Values: False (default) or True.</li>
+<li>nullxmlFlag - extract null-terminated XML content from XML and UUID boxes. Values: False (default) or True.</li>
+<li>mixFlag - report additional output in NISO MIX format (version 1.0 or 2.0). Values: 0 (default), 1 or 2.</li>
+</ul>
+<p>As an example, for validating a raw JPEG 2000 codestream, call the <em>checkOneFile</em> function with the additional <em>validationFormat</em> argument, and set it to <code>j2c</code>:</p>
 <pre><code># Define Codestream
 myFile = &quot;/home/johan/jpylyzer-test-files/rubbish.j2c&quot;
 
 # Analyse with jpylyzer, result to Element object
 myResult = jpylyzer.checkOneFile(myFile, &#39;j2c&#39;)</code></pre>
 <h2 id="java-integration">Java integration</h2>
-<p>It is possible to integrate <em>jpylyzer</em> into Java applications. A test class that shows how this works is included in the source repo <a href="https://github.com/openpreserve/jpylyzer/tree/master/jpylyzer/java_demo/CallJpylyzer.java">here</a>. This requires <a href="https://www.jython.org/">Jython</a>. Note that you may run into performance issues with (very) large images in this case, as Jython does not support <a href="https://docs.python.org/3/library/mmap.html">memory mapping</a>, so make sure you’ve got plenty of RAM available.</p>
+<p>It is possible to integrate <em>jpylyzer</em> into Java applications<a href="#fn3" class="footnote-ref" id="fnref3" role="doc-noteref"><sup>3</sup></a>. A test class that shows how this works is included in the source repo <a href="https://github.com/openpreserve/jpylyzer/tree/master/jpylyzer/java_demo/CallJpylyzer.java">here</a>. This requires <a href="https://www.jython.org/">Jython</a>. Note that you may run into performance issues with (very) large images in this case, as Jython does not support <a href="https://docs.python.org/3/library/mmap.html">memory mapping</a>, so make sure you’ve got plenty of RAM available.</p>
 <h1 id="structure-jp2">Structure of a JP2 file</h1>
 <h2 id="structure-scope">Scope of this section</h2>
 <p>This section gives a brief overview of the JP2 file format. A basic understanding of the general structure of JP2 is helpful for appreciating how <em>jpylyzer</em> performs its validation. It will also make it easier to understand <em>jpylyzer</em>‘s extracted properties, as these are reported as a hierarchical tree that corresponds to the internal structure of JP2.</p>
 <p>For an exhaustive description of every detail of the format you are advised to consult Annex I (‘JP2 file format syntax’) and Annex A (‘Codestream syntax’) of ISO/IEC 15444-1.</p>
 <h2 id="general-format-structure">General format structure</h2>
 <p>At the highest level, a JP2 file is made up of a collection of <em>boxes</em>. A <em>box</em> can be thought of as the fundamental building block of the format. Some boxes (‘superboxes’) are containers for other boxes. The Figure below gives an overview of the top-level boxes in a JP2 file.</p>
 <figure>
@@ -568,17 +564,17 @@
 </tr>
 </tbody>
 </table>
 <p>A JP2 file may contain boxes that are not defined by the standard. Such boxes are simply skipped and ignored by conforming reader applications.</p>
 <h1 id="output-format">Output format</h1>
 <p>This section explains <em>jpylyzer</em>’s output format.</p>
 <h2 id="output-format-overview">Overview</h2>
-<p><em>Jpylyzer</em> generates its output in XML format, which is defined by <a href="https://jpylyzer.openpreservation.org/jpylyzer-v-2-1.xsd">the schema that can be found here</a>. The following Figure shows the output structure:</p>
+<p><em>Jpylyzer</em> generates its output in XML format, which is defined by <a href="https://jpylyzer.openpreservation.org/jpylyzer-v-2-2.xsd">the schema that can be found here</a>. The following Figure shows the output structure:</p>
 <figure>
-<img src="data:image/png;base64,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ErC3t39pGxnRoUOHLNehlEIplekEmZCQkKV2M+r5d1m8eHEsLS0BKFeu3Cu3u3PnDrGxseke5xo1ahAUFMSqVavo27fvS+tJTU3l6tWrPH36FFtbW/Lly6cTm1IKCwsLQkNDSU5OpmLFihgYGBAbG0toaChlypShYMGCOnUqpbhx4wapqanY2tq+9slJbiIJXYj/CA8PRymFh4eHvkPJFlu2bHmt7Xx9fZk/fz7R0dG4uLjg6+vLli1bSE5Oxt/fP035kJAQPDw8iI+Pp2DBgly7do0ZM2YwePDgdOufPHkyp0+fxt7ent27d/P48WMAfv/9d2rWrImLiwsPHjxg+vTprFy5kpCQEPbs2UOfPn3Imzcv5ubm3Lp1i+nTpzN06NDX2keAChUqpEkWmRUaGsr169dxc3PDzMwsw9vdunWLS5cuZantjJg2bRqLFi0iNjYWFxcX5syZw5o1a8ibNy+rV69OU/7UqVN4enqSmJhIgQIFuH79OnPmzKF///5aGSsrK7799lvGjh1LmzZtKFy4cLptBwUF4eHhQXJyMlZWVly7do2ZM2cyZMgQAD777DMiIiKAZ4/CvXnzJvXr12fcuHEMGDAAAwMDwsLC2LRpE23atAEgMDCQPn36YGFhgYmJCffv32fZsmW0a9cuuw/du0XlAFOnTlWAOn36tL5DEUK1adNGWVhY6DuMbGNubq5at279Wtt+++23ysHBQfvco0cP5enpqZRS6tdff1UGBgZKKaWSk5PVBx98oPr166eSk5OVUkpt27ZNGRkZqbNnzyqllNq6dasCVHh4uFJKqUmTJikzMzO1YMECpZRSSUlJqlatWuqjjz7S2itevLi2PioqShUoUECNHTtWW79q1SplaGiotZEZCxYsUIDat29fprf9r3HjxilAXb16NVPbzZ8/XwFq//79WY7hVb7++mvl5OSkfe7atavq1auXUkqp9evXqzx58iillEpMTFS2trZq4MCBKiUlRSml1ObNm5WxsbG6ePGiUkqpadOmqfr166uUlBRVp04d1adPH63epUuXKnt7e+2zu7u78vT0VKmpqUoppZYvX65MTEzUw4cPlVJKffrppypv3rwqICBAKaXUwYMHFaCaNGmiYmNjlVJKdenSRTVt2lQppdSjR4+UlZWV+vrrr7U25s6dqywtLdWDBw+y8YildeTIEQWoOXPm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lpbedLsNaceOHbq0ezO+//57bQ790qVLZGRkEBUVxfbt24mMjOTHH3/E29u7zjne3t6cPn2akydP4uLiQmBgIK+++irTp09n0aJFtGnTRo9baXB5eXksWrTI4utUVVXx7bffMm7cONLT07nnnnswmUxkZ2eTkJDABx98QFhYGC1btiQnJ0c7rlOnTtjZ2bF7927Gjh3LBx98QOfOnSWhC9Ec/bby/cKFC3WSnK2tbZ39zs7OnD9/vs62c+fOAWgFc3Dl6YBf//vixYs4OTlhNBoB+PLLLwkICKhznV+39dt2b6RVq1YYjUbKysrq7bs6D9ujRw8KCgooLS1l7dq1zJs3jzVr1tRJpHPnzr3pNpurFi1aMG7cOObOncvy5cuJjIy87mfCxsZG+yxdvHiRFStWEBISwrJlyxgzZkydL4p/VqtXr2b16tUWX6ddu3acO3eOBx54ALPZTMuWLVm1ahVHjhyhc+fOmM1m3NzcyM7O5pdffqFjx46YzWbatGnDhg0bOHv2LPfeey9msxlfX19J6EI0R3v27Knz+sCBAzes6g8KCqKwsLDOtqKiIry8vOok9D179hAYGAhAWVkZNTU1+Pv74+/vj52dHSUlJXTp0kU7fv/+/b/7NMH1HrsLCgrif//7HydOnKBDhw7a9uLiYkJDQzl58iT79++nW7duBAQEMGXKFKKionjwwQc5deqUdnxKSgrh4eE3jOH3LFmyhBUrVpCZmXlLi76sXbuW999/36K2b5czZ85w9OhR3NzcgOt/Jvz8/LQvZtOnT8fR0ZGvvvqKiIgIkpKSmD59+m2PvaElJCQ0SGHlmTNncHV1JTIyEicnJ4YPH05RUREA4eHhuLi48MQTT7B7925atGjBvffei7u7OyNGjGDgwIE4ODgQHByMp6cno0aNkoQuRHNUXFxMWloaffv25auvvmLHjh1aNfq1TJw4kUceeYT33nuPAQMGUFxczLx583j11VfrHPf+++9z11134e7uTmJiIh06dKB79+5YW1vz3HPPkZiYiKurK8HBwWRlZfHyyy/z+eef06NHj2u2azQaqaioYOvWrfj7+9fZ16NHDyIiInjqqaeYO3cuRqORjIwMli1bxrfffssvv/xC7969SUpKol+/ftTU1JCRkUFISIg2YgAQERFBdHS0Be8mfPXVVwB069YNPz+/mz6vpKTEonYb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" alt="Jpylyzer’s XML output structure. ‘box’ elements under ‘tests’ and ‘properties’ contain further sub-elements." /><figcaption aria-hidden="true">Jpylyzer’s XML output structure. ‘box’ elements under ‘tests’ and ‘properties’ contain further sub-elements.</figcaption>
+<img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAhMAAALFCAYAAAB5xGEWAAAABHNCSVQICAgIfAhkiAAAAAlwSFlzAAAK6wAACusBgosNWgAAABl0RVh0U29mdHdhcmUAd3d3Lmlua3NjYXBlLm9yZ5vuPBoAACAASURBVHic7N13VBTX/z7wZ6lKl46CSLErKljQGLuCBRUjxthIbKhRYyQJlmjQGEsSDWKIFSxBxRI19hoVYsGKiAhREEQErKCCIOX+/uDHfN2ABlhw4ePzOsdz2Jk7975nFuRh5s6sTAghQERERFROKsougIiIiKo3hgkiIiJSCMMEERERKYRhgoiIiBTCMEFEREQKYZggIiIihTBMEBERkUIYJoiIiEghDBNERESkEIYJIiIiUgjDBBERESmEYYKIiIgUwjBBRERECmGYICIiIoUwTBAREZFCGCaIiIhIIQwTREREpBCGCSIiIlIIwwQREREphGGCiIiIFMIwQURERAphmCAiIiKFMEwQERGRQhgmiIiISCEME0RERKQQhgkiIiJSCMMEERERKYRhgoiIiBTCMEFEREQKYZggIiIihTBMEBERkUIYJoiIiEghDBNERESkEIYJIiIiUgjDBBERESmEYYKIiIgUwjBBRERECmGYICIiIoUwTBAREZFCGCaIiIhIIQwTREREpBCGCSIiIlIIwwQREREphGGCiIiIFMIwQURERAphmCAiIiKFMEwQERGRQhgmiIiISCEME0RERKQQhgkiIiJSCMMEERERKYRhgoiIiBTCMEFEREQKYZggIiIihTBMEBERkUIYJoiIiEghDBNERESkEIYJIiIiUgjDBBERESmEYYKIiIgUwjBBRERECmGYICIiIoUwTBAREZFCGCaIiIhIIQwTREREpBCGCSIiIlIIwwQREREphGGCiIiIFMIwQURERAphmCAiIiKFMEwQERGRQtRK0ygmJgaxsbGVXUu1Y2ZmBmdnZ2WXUaKEhARERkYqu4wqR19fH507d1bK2OfPn8eDBw+UMjaVTc+ePVGzZk1ll0FUbZQqTAQHB+OHH36o7FqqHVdXVxw6dEjZZZRo//79mDJlirLLqHJatmyJq1evKmXs7777DkePHlXK2FQ2CQkJsLa2VnYZRNVGqcJEkfXr16NWrVqVVUu18tlnnym7hFJZunQpbG1tlV1GlTB9+nRllwBDQ0MEBgYq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abIsAFSvXh1jxowp9HyJ/ksl/j2OSEQF9OnTBxEREXj69KnSpciyevVq9OvXDwcPHoSvr+8bH/f111/jyJEj2L9/f5HVMnHiRBw9ehSxsbFF1ia9H23atMGJEydw+/ZtpUuhEoRjXERERCQLL3MQ0Sv5+PigbNmyRd7mm77TgohKPoYJInqlTp06FXmbnTt3LvI2iUg5vMxBREREsjBMEBERkSwME0RERCQLwwQRERHJwjBBREREsjBMEBERkSwME0RERCQLwwQRERHJwodWEZUyqampuHDhgtJl0Afq368yJ3qBYYKolOnTp4/SJdAH7sXbWIleYJggKiXq16+PefPmKV3GB2f79u1ITEzEt99+C11dXaXLKRHKlCmjdAlUwjBMEJUS7u7ucHd3V7qMD05KSgoSExMxduxY6OvrK10OUYnECZhEREQkC8MEERERycIwQURERLIwTBAREZEsDBNEREQkC8MEERERycIwQURERLIwTBAREZEsDBNEREQkC8MEERERycIwQURERLIwTBAREZEsDBNEREQkC8MEERERycIwQURERLIwTBAREZEsDBNEREQki57SBRAR0eu1aNFC6RLoDVSqVAmrV69Wuoz3jmGCiKiEE0Jg//79KFOmDGxsbJQuhwpx584dODo6Kl2GIhgmiIg+EN26dcPKlSuVLoMK0aRJE9y9e1fpMhTBORNEREQkC8MEERERycIwQURERLIwTBAREZEsDBNERFSs8vLyMHHiRKSlpSldChUThgkiIipWGo0GV65cwZMnT5QuhYoJbw0lIqJiZWxsjM2bNytdBhUjjkwQEdFbuXXrFrp27YpLly6hW7duaNCgAcaOHYu8vDzMnTsXDRs2RPv27XHmzBkAQG5uLrp27YqkpCScPXsW3bp1w507d6T2tmzZgqFDhyI/P1+pUyKZODJBRPQGunfvjqysLKXLKBGePHmCLVu2IDc3FyNGjEBOTg569OiBI0eOoEOHDli0aBFmzZqFQYMG4ciRI8jPz8eWLVswevRoNGzYEM+ePcOIESMQGRmJ27dvY/DgwQgPD4eeHr+SPlT8yRERvYG0tDRkZmYqXUaJoKurCwDo168f/P39AQANGzZEfn4+xo8fDwAYMmQIgoKCIIQocHxYWBhq1aqF6OhorFu3Dh06dEDnzp3f3wkUs5kzZ+LmzZuy28nJyUFM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goiIiGRhmCAiIiJZGCaIiIhIFk7AJCIqAbKysvjK7RIqJydH6RJKPIYJIqIS4N9PkyT60DBMEBEpyM/PDxqNRuky6A1UqVJF6RJKLN4aSkREsuXk5KBixYoYOnQoZs+erXQ59J7xAh0REcm2Y8cO6OnpIS8vT+lSSAEcmSAioiIxatQoTJs2TeslYVQ6cGSCiIhk27RpE37++Wf4+PgoXQopgCMTREQkW3Z2NjZs2IDAwEA4ODgoXQ69ZxyZICIi2e7du4fx48djypQpSpdCCmCYICIi2VJSUlC7dm3Ur19f6VJIAQwTREQk26effgpjY2O4uLgoXQopgA+tIiIi2cLDw7Fv3z5kZ2fD399f6XLoPWOYICIi2QYMGAA9PT107dpV6VJIAbzMQUREsiUmJmLEiBHo0qWL0qWQAjgyQUREspmZmaFbt24ME6UURyaIiEg2d3d3HDhwAKmpqUqXQgpgmCAiItlWrlyJq1evIi4uTulSSAG8zEFERLINHDgQWVlZ+PLLL5UuhRTAx2kTEZFs0dHR6N69O9zd3fHXX38pXQ69ZwwTREQk2+3bt7Fu3Tq0bt0aHh4eSpdD7xnnTBARkWzm5uaYNWsWIiIilC6FFMAwQUREskVHR8PU1BQc7C6deJmDiIiIZOHIBBEREcnCMEFERESyMEwQERGRLAwTREREJAvDBBEREcnCMEFERESyMEwQERGRLAwTREREJAvDBBEREcnCMEFERESyMEwQERGRLAwTREREJAvDBBEREcnCMEFERESyMEwQERGRLAwTREREJAvDBBEREcnCMEFERESyMEwQERGRLAwTREREJAvDBBEREcnCMEFERESyMEwQERGRLAwTREREJAvDBBEREcnCMEFERESyMEwQERGRLAwTREREJAvDBBEREcnCMEFERESyMEwQERGRLAwTREREJAvDBBEREcnCMEFERESyMEwQERGRLAwTREREJAvDBBEREcnCMEFERESyMEwQERGRLAwTREREJAvDBBEREcnCMEFERESyMEwQERGRLAwTREREJAvDBBEREcnCMEFERESyMEwQERGRLAwTREREJAvDBBEREcnCMEFERESyMEwQERGRLAwTREREJAvDBBEREcnCMEFERESyMEwQERGRLP8P3HvksW+2aj0AAAAASUVORK5CYII=" alt="Jpylyzer’s XML output structure. ‘box’ elements under ‘tests’ and ‘properties’ contain further sub-elements." /><figcaption aria-hidden="true">Jpylyzer’s XML output structure. ‘box’ elements under ‘tests’ and ‘properties’ contain further sub-elements.</figcaption>
 </figure>
 <p>The root element (<em>jpylyzer</em>) contains the following child elements:</p>
 <ol type="1">
 <li><p>one <em>toolInfo</em> element, which contains information about <em>jpylyzer</em></p></li>
 <li><p>one or more <em>file</em> elements, each of which contain information about about the analysed files</p></li>
 </ol>
 <p>The XML output is pretty-printed. You can use the <code>--nopretty</code> switch to disable pretty-printing (this produces smaller files and may give a slightly better performance).</p>
@@ -593,14 +589,15 @@
 <ol type="1">
 <li><p><em>fileInfo</em>: general information about the analysed file</p></li>
 <li><p><em>statusInfo</em>: information about the status of <em>jpylyzer</em>’s validation attempt</p></li>
 <li><p><em>isValid</em>: outcome of the validation</p></li>
 <li><p><em>tests</em>: outcome of the individual tests that are part of the validation process (organised by box)</p></li>
 <li><p><em>properties</em>: image properties (organised by box)</p></li>
 <li><p><em>propertiesExtension</em>: wrapper element for NISO <em>MIX</em> output (only if the <code>--mix</code> option is used)</p></li>
+<li><p><em>warnings</em>: reported warnings</p></li>
 </ol>
 <h2 id="fileinfo-element">fileInfo element</h2>
 <p>This element holds general information about the analysed file. Currently it contains the following sub-elements:</p>
 <ul>
 <li><p><em>filename</em>: name of the analysed file without its path (e.g. “rubbish.jp2”)</p></li>
 <li><p><em>filePath</em>: name of the analysed file, including its full absolute path (e.g. “d:\data\images\rubbish.jp2”)</p></li>
 <li><p><em>fileSizeInBytes</em>: file size in bytes</p></li>
@@ -627,19 +624,26 @@
 <p>This element is reserved to hold the outcomes of all the individual tests that <em>jpylyzer</em> performs to assess whether a file is valid JP2. The results are organised in a hierarchical tree that corresponds to JP2’s box structure. Each individual test can have two values:</p>
 <ul>
 <li><p>“True” if a file passed the test.</p></li>
 <li><p>“False” if a file failed the test.</p></li>
 </ul>
 <p>If a file passed <em>all</em> tests, this is an indication that it is most likely valid JP2. In that case, the <a href="#isvalid-element"><em>isValid</em> element</a> has a value of “True” (and “False” in all other cases). These tests are all explained <a href="#jp2-box-by-box">here</a> and <a href="#contiguous-codestream-box-chapter">here</a>.</p>
 <h3 id="default-and-verbose-reporting-of-test-results">Default and verbose reporting of test results</h3>
-<p>By default, <em>jpylyzer</em> only reports any tests that failed (i.e. returned “False”), including the corresponding part of the box structure. For a valid JP2 the tests element will be empty. If the –verbose flag is used, the results of <em>all</em> tests are included (including those that returned “True”)<a href="#fn3" class="footnote-ref" id="fnref3" role="doc-noteref"><sup>3</sup></a>.</p>
+<p>By default, <em>jpylyzer</em> only reports any tests that failed (i.e. returned “False”), including the corresponding part of the box structure. For a valid JP2 the tests element will be empty. If the –verbose flag is used, the results of <em>all</em> tests are included (including those that returned “True”)<a href="#fn4" class="footnote-ref" id="fnref4" role="doc-noteref"><sup>4</sup></a>.</p>
 <h2 id="properties-element">properties element</h2>
 <p>This element contains the extracted image properties, which are organised in a hierarchical tree that corresponds to JP2’s box structure. See <a href="#jp2-box-by-box">here</a> and <a href="#contiguous-codestream-box-chapter">here</a> for a description of the reported properties.</p>
 <h2 id="propertiesExtension-element">propertiesExtension element</h2>
 <p>This optional element is reserved for output in alternative formats. Currently it is used to wrap output in NISO <em>MIX</em> format if the <code>--mix</code> option is used. See the <a href="https://www.loc.gov/standards/mix/"><em>MIX</em> documentation</a> for a description of the reported elements.</p>
+<h2 id="warnings-element">warnings element</h2>
+<p>This element is reserved for reporting any warnings that are not directly related to the validation process. Examples are:</p>
+<ul>
+<li>Jpylyzer encountered an unknown box type while parsing a file.</li>
+<li>Reading of a file failed because of system limitations.</li>
+</ul>
+<p>Each warning is wrapped in a ‘warning’ element. The results are organised in a hierarchical tree that corresponds to JP2’s box structure.</p>
 <h1 id="jp2-box-by-box">JP2: box by box</h1>
 <p>The following two sections provide a detailed explanation of <em>jpylyzer</em>’s functionality and its output. In particular, the following two aspects are addressed:</p>
 <ol type="1">
 <li><p>The reported properties</p></li>
 <li><p>The tests that <em>jpylyzer</em> performs to establish the validity of a file.</p></li>
 </ol>
 <h2 id="about-properties-tests-trees">About the properties and tests trees</h2>
@@ -709,23 +713,23 @@
 <tbody>
 <tr class="odd">
 <td style="text-align: left;">boxLengthIsValid</td>
 <td style="text-align: left;">(Size of box – 8) /4 is a whole number (integer)</td>
 </tr>
 <tr class="even">
 <td style="text-align: left;">brandIsValid</td>
-<td style="text-align: left;"><em>br</em> equals 0x6a703220 (“jp2”)</td>
+<td style="text-align: left;"><em>br</em> equals 0x6a703220 (“jp2”) for JP2, or 0x6a706820 (“jph”)for JPH</td>
 </tr>
 <tr class="odd">
 <td style="text-align: left;">minorVersionIsValid</td>
 <td style="text-align: left;"><em>minV</em> equals 0</td>
 </tr>
 <tr class="even">
 <td style="text-align: left;">compatibilityListIsValid</td>
-<td style="text-align: left;">Sequence of compatibility (<em>cL</em>) fields includes one entry that equals 0x6a703220 (“jp2”)</td>
+<td style="text-align: left;">Sequence of compatibility (<em>cL</em>) fields includes one entry that equals 0x6a703220 (“jp2”) for JP2, or 0x6a706820 (“jph”)for JPH</td>
 </tr>
 </tbody>
 </table>
 <h2 id="jp2-header-box">JP2 Header box (superbox)</h2>
 <p>This box is a superbox that holds a series of boxes that contain header-type information about the file.</p>
 <h3 id="element-name-2">Element name</h3>
 <p>jp2HeaderBox</p>
@@ -822,14 +826,18 @@
 <td style="text-align: left;">colourSpecificationBoxesAreContiguous</td>
 <td style="text-align: left;">In case of multiple Colour Specification boxes, they appear contiguously in the JP2 Header box</td>
 </tr>
 <tr class="even">
 <td style="text-align: left;">paletteAndComponentMappingBoxesOnlyTogether</td>
 <td style="text-align: left;">Box contains a Palette box (only if Component Mapping box is present); box contains a Component Mapping box (only if Palette box is present)</td>
 </tr>
+<tr class="odd">
+<td style="text-align: left;">noZeroCTypesIfNoColourBox</td>
+<td style="text-align: left;">If file does not contain a Colour Specification Box, no cTyp values (from Channel definition box) shall be equal to 0 (JPH)</td>
+</tr>
 </tbody>
 </table>
 <h2 id="image-header-box">Image Header box (child of JP2 Header box)</h2>
 <p>This box specifies the size of the image and other related fields.</p>
 <h3 id="element-name-3">Element name</h3>
 <p>imageHeaderBox</p>
 <h3 id="reported-properties-3">Reported properties</h3>
@@ -967,32 +975,48 @@
 <th style="text-align: left;">Property</th>
 <th style="text-align: left;">Description</th>
 </tr>
 </thead>
 <tbody>
 <tr class="odd">
 <td style="text-align: left;">meth</td>
-<td style="text-align: left;">Specification method. Indicates whether colourspace of this image is defined as an enumerated colourspace or using a (restricted) ICC profile.</td>
+<td style="text-align: left;">Specification method. Indicates how the colourspace is defined (enumerated colourspace, or restricted ICC profile for JP2, with additional Any ICC and Parameterized Colourspace methods for JPH.</td>
 </tr>
 <tr class="even">
 <td style="text-align: left;">prec</td>
 <td style="text-align: left;">Precedence</td>
 </tr>
 <tr class="odd">
 <td style="text-align: left;">approx</td>
 <td style="text-align: left;">Colourspace approximation</td>
 </tr>
 <tr class="even">
 <td style="text-align: left;">enumCS (if meth equals “Enumerated”)</td>
 <td style="text-align: left;">Enumerated colourspace (as descriptive text string)</td>
 </tr>
 <tr class="odd">
-<td style="text-align: left;">icc (if meth equals “Restricted ICC” or “Any ICC”<a href="#fn4" class="footnote-ref" id="fnref4" role="doc-noteref"><sup>4</sup></a>)</td>
+<td style="text-align: left;">icc (if meth equals “Restricted ICC” or “Any ICC”)</td>
 <td style="text-align: left;">Properties of ICC profile as child element (see below)</td>
 </tr>
+<tr class="even">
+<td style="text-align: left;">colPrims (if meth equals “Parameterized Colourspace”)</td>
+<td style="text-align: left;">ColourPrimaries value (JPH)<a href="#fn5" class="footnote-ref" id="fnref5" role="doc-noteref"><sup>5</sup></a>.</td>
+</tr>
+<tr class="odd">
+<td style="text-align: left;">transfC (if meth equals “Parameterized Colourspace”)</td>
+<td style="text-align: left;">TransferCharacteristics value (JPH)<a href="#fn6" class="footnote-ref" id="fnref6" role="doc-noteref"><sup>6</sup></a></td>
+</tr>
+<tr class="even">
+<td style="text-align: left;">matCoeffs (if meth equals “Parameterized Colourspace”)</td>
+<td style="text-align: left;">MatrixCoefficients value (JPH)<a href="#fn7" class="footnote-ref" id="fnref7" role="doc-noteref"><sup>7</sup></a></td>
+</tr>
+<tr class="odd">
+<td style="text-align: left;">vidFRng (if meth equals “Parameterized Colourspace”)</td>
+<td style="text-align: left;">VideoFullRangeFlag (“yes”/”no”) (JPH)<a href="#fn8" class="footnote-ref" id="fnref8" role="doc-noteref"><sup>8</sup></a></td>
+</tr>
 </tbody>
 </table>
 <h3 id="reported-properties-of-icc-profiles">Reported properties of ICC profiles</h3>
 <p>If the colour specification box contains an embedded ICC profile, <em>jpylyzer</em> will also report the following properties (which are all grouped in an “icc” sub-element in the properties tree). An exhaustive explanation of these properties is given in the ICC specification (ISO 15076-1 / ICC.1:2004-10). Note that <em>jpylyzer</em> does <em>not</em> validate embedded ICC profiles (even though it does check if a specific ICC profile is allowed in JP2)!</p>
 <table>
 <thead>
 <tr class="header">
@@ -1130,20 +1154,32 @@
 </tr>
 <tr class="odd">
 <td style="text-align: left;">iccSizeIsValid (if meth equals “Restricted ICC”)</td>
 <td style="text-align: left;">Actual size of embedded ICC profile equals value of profileSize field in ICC header</td>
 </tr>
 <tr class="even">
 <td style="text-align: left;">iccPermittedProfileClass (if meth equals “Restricted ICC”)</td>
-<td style="text-align: left;">ICC profile class is “input device” or “display device”<a href="#fn5" class="footnote-ref" id="fnref5" role="doc-noteref"><sup>5</sup></a></td>
+<td style="text-align: left;">ICC profile class is “input device” or “display device”<a href="#fn9" class="footnote-ref" id="fnref9" role="doc-noteref"><sup>9</sup></a></td>
 </tr>
 <tr class="odd">
 <td style="text-align: left;">iccNoLUTBasedProfile (if meth equals “Restricted ICC”)</td>
 <td style="text-align: left;">ICC profile type is not N-component LUT based (which is not allowed in JP2)</td>
 </tr>
+<tr class="even">
+<td style="text-align: left;">colPrimsIsValid</td>
+<td style="text-align: left;"><em>colPrims</em> value is defined by ITU-T H.273 / ISO/IEC 23001-8 (JPH)</td>
+</tr>
+<tr class="odd">
+<td style="text-align: left;">transfCIsValid</td>
+<td style="text-align: left;"><em>transfC</em> value is defined by ITU-T H.273 / ISO/IEC 23001-8 (JPH)</td>
+</tr>
+<tr class="even">
+<td style="text-align: left;">matCoeffsIsValid</td>
+<td style="text-align: left;"><em>matCoeffs</em> value is defined by ITU-T H.273 / ISO/IEC 23001-8 (JPH)</td>
+</tr>
 </tbody>
 </table>
 <h2 id="palette-box">Palette box (child of JP2 Header box)</h2>
 <p>This (optional) box specifies the palette which maps a single component in index space to a multiple-component image.</p>
 <h3 id="element-name-6">Element name</h3>
 <p>paletteBox</p>
 <h3 id="reported-properties-6">Reported properties</h3>
@@ -1300,20 +1336,28 @@
 </tr>
 <tr class="odd">
 <td style="text-align: left;">cNIsValid<sup>*</sup></td>
 <td style="text-align: left;"><em>cN</em> is within range [0, 65535] (repeated for all channels)</td>
 </tr>
 <tr class="even">
 <td style="text-align: left;">cTypIsValid<sup>*</sup></td>
-<td style="text-align: left;"><em>cType</em> is within range [0, 65535] (repeated for all channels)</td>
+<td style="text-align: left;"><em>cType</em> is one of the values defined in Table I.16 (repeated for all channels)<a href="#fn10" class="footnote-ref" id="fnref10" role="doc-noteref"><sup>10</sup></a></td>
 </tr>
 <tr class="odd">
 <td style="text-align: left;">cAssocIsValid<sup>*</sup></td>
 <td style="text-align: left;"><em>cAssoc</em> is within range [0, 65535] (repeated for all channels)</td>
 </tr>
+<tr class="even">
+<td style="text-align: left;">noMoreThanOneAlphaChannel</td>
+<td style="text-align: left;">At most one <em>cTyp</em> field is equal to 1 or 2 (JPH)</td>
+</tr>
+<tr class="odd">
+<td style="text-align: left;">cAssocAlphaChannelIsZero</td>
+<td style="text-align: left;">If <em>cTyp</em> is 1 or 2, the corresponding <em>cAssoc</em> value equals 0 (JPH)</td>
+</tr>
 </tbody>
 </table>
 <h2 id="resolution-box">Resolution box (child of JP2 Header box, superbox)</h2>
 <p>This (optional) box contains the grid resolution.</p>
 <h3 id="element-name-9">Element name</h3>
 <p>resolutionBox</p>
 <h3 id="reported-properties-9">Reported properties</h3>
@@ -1395,27 +1439,27 @@
 </tr>
 <tr class="even">
 <td style="text-align: left;">hRcE</td>
 <td style="text-align: left;">Horizontal grid resolution exponent</td>
 </tr>
 <tr class="odd">
 <td style="text-align: left;">vRescInPixelsPerMeter</td>
-<td style="text-align: left;">Vertical grid resolution, expressed in pixels per meter<a href="#fn6" class="footnote-ref" id="fnref6" role="doc-noteref"><sup>6</sup></a></td>
+<td style="text-align: left;">Vertical grid resolution, expressed in pixels per meter<a href="#fn11" class="footnote-ref" id="fnref11" role="doc-noteref"><sup>11</sup></a></td>
 </tr>
 <tr class="even">
 <td style="text-align: left;">hRescInPixelsPerMeter</td>
-<td style="text-align: left;">Horizontal grid resolution, expressed in pixels per meter<a href="#fn7" class="footnote-ref" id="fnref7" role="doc-noteref"><sup>7</sup></a></td>
+<td style="text-align: left;">Horizontal grid resolution, expressed in pixels per meter<a href="#fn12" class="footnote-ref" id="fnref12" role="doc-noteref"><sup>12</sup></a></td>
 </tr>
 <tr class="odd">
 <td style="text-align: left;">vRescInPixelsPerInch</td>
-<td style="text-align: left;">Vertical grid resolution, expressed in pixels per inch<a href="#fn8" class="footnote-ref" id="fnref8" role="doc-noteref"><sup>8</sup></a></td>
+<td style="text-align: left;">Vertical grid resolution, expressed in pixels per inch<a href="#fn13" class="footnote-ref" id="fnref13" role="doc-noteref"><sup>13</sup></a></td>
 </tr>
 <tr class="even">
 <td style="text-align: left;">hRescInPixelsPerInch</td>
-<td style="text-align: left;">Horizontal grid resolution, expressed in pixels per inch<a href="#fn9" class="footnote-ref" id="fnref9" role="doc-noteref"><sup>9</sup></a></td>
+<td style="text-align: left;">Horizontal grid resolution, expressed in pixels per inch<a href="#fn14" class="footnote-ref" id="fnref14" role="doc-noteref"><sup>14</sup></a></td>
 </tr>
 </tbody>
 </table>
 <h3 id="tests-10">Tests</h3>
 <table>
 <thead>
 <tr class="header">
@@ -1490,27 +1534,27 @@
 </tr>
 <tr class="even">
 <td style="text-align: left;">hRdE</td>
 <td style="text-align: left;">Horizontal grid resolution exponent</td>
 </tr>
 <tr class="odd">
 <td style="text-align: left;">vResdInPixelsPerMeter</td>
-<td style="text-align: left;">Vertical grid resolution, expressed in pixels per meter<a href="#fn10" class="footnote-ref" id="fnref10" role="doc-noteref"><sup>10</sup></a></td>
+<td style="text-align: left;">Vertical grid resolution, expressed in pixels per meter<a href="#fn15" class="footnote-ref" id="fnref15" role="doc-noteref"><sup>15</sup></a></td>
 </tr>
 <tr class="even">
 <td style="text-align: left;">hResdInPixelsPerMeter</td>
-<td style="text-align: left;">Horizontal grid resolution, expressed in pixels per meter<a href="#fn11" class="footnote-ref" id="fnref11" role="doc-noteref"><sup>11</sup></a></td>
+<td style="text-align: left;">Horizontal grid resolution, expressed in pixels per meter<a href="#fn16" class="footnote-ref" id="fnref16" role="doc-noteref"><sup>16</sup></a></td>
 </tr>
 <tr class="odd">
 <td style="text-align: left;">vResdInPixelsPerInch</td>
-<td style="text-align: left;">Vertical grid resolution, expressed in pixels per inch<a href="#fn12" class="footnote-ref" id="fnref12" role="doc-noteref"><sup>12</sup></a></td>
+<td style="text-align: left;">Vertical grid resolution, expressed in pixels per inch<a href="#fn17" class="footnote-ref" id="fnref17" role="doc-noteref"><sup>17</sup></a></td>
 </tr>
 <tr class="even">
 <td style="text-align: left;">hResdInPixelsPerInch</td>
-<td style="text-align: left;">Horizontal grid resolution, expressed in pixels per inch<a href="#fn13" class="footnote-ref" id="fnref13" role="doc-noteref"><sup>13</sup></a></td>
+<td style="text-align: left;">Horizontal grid resolution, expressed in pixels per inch<a href="#fn18" class="footnote-ref" id="fnref18" role="doc-noteref"><sup>18</sup></a></td>
 </tr>
 </tbody>
 </table>
 <h3 id="tests-11">Tests</h3>
 <table>
 <thead>
 <tr class="header">
@@ -1572,15 +1616,15 @@
 <td style="text-align: left;">containsWellformedXML</td>
 <td style="text-align: left;">Contents of box are parsable, well-formed XML</td>
 </tr>
 </tbody>
 </table>
 <p>Note that <em>jpylyzer</em> does not check whether the XML is <em>valid</em>, as this is not required by the standard. Besides, doing so would make <em>jpylyzer</em> significantly slower for XML that contains references to external schemas and DTDs.</p>
 <h2 id="uuid-box">UUID box</h2>
-<p>This (optional) box contains additional (binary) information, which may be vendor-specific. Some applications (e.g. Kakadu and ExifTool) also use this box for storing XMP metadata (see Section 1.1.4 in Part 3 of the XMP specification<a href="#fn14" class="footnote-ref" id="fnref14" role="doc-noteref"><sup>14</sup></a>).</p>
+<p>This (optional) box contains additional (binary) information, which may be vendor-specific. Some applications (e.g. Kakadu and ExifTool) also use this box for storing XMP metadata (see Section 1.1.4 in Part 3 of the XMP specification<a href="#fn19" class="footnote-ref" id="fnref19" role="doc-noteref"><sup>19</sup></a>).</p>
 <h3 id="element-name-13">Element name</h3>
 <p>uuidBox</p>
 <h3 id="reported-properties-13">Reported properties</h3>
 <p>If the value of <em>uuid</em> indicates the presence of XMP metadata and the contents of this box are well-formed XML, (see ‘tests’ below), the ‘uuidBox’ element in the properties tree will contain the XMP data. Note that, depending on the character encoding of the original XML, it may contain characters that are not allowed in the encoding that is used for <em>jpylyzer</em>’s output. Any such characters will be represented by numerical entity references in the output. In all other cases, the ‘uuidBox’ element will contain a standard string representation the of UUID.</p>
 <table>
 <thead>
 <tr class="header">
@@ -1992,15 +2036,15 @@
 <p>In addition the following optional marker segments may also occur:</p>
 <ul>
 <li><p>Packet length, tile-part header (PLT) marker segment (optional) <sup>*</sup></p></li>
 <li><p>Packed packet headers, tile-part header (PPT) marker segment (optional) <sup>*</sup></p></li>
 </ul>
 <p>The optional markers that are marked with an asterisk above are only minimally supported at this stage: if <em>jpylyzer</em> encounters them, it will include the corresponding element in the <em>properties</em> element of the output. However, <em>jpylyzer</em> does not analyse the contents of these marker segments, which means that the respective elements in the output will be empty.</p>
 <h3 id="bit-streams">Bit streams</h3>
-<p>In addition to the above limitations, <em>jpylyzer</em> can <em>not</em> be used to establish whether the data in the bitstream are correct (this would require decoding the compressed image data, which is completely out of <em>jpylyzer</em>’s scope)<a href="#fn15" class="footnote-ref" id="fnref15" role="doc-noteref"><sup>15</sup></a>. As a result, if <em>jpylyzer</em> is used as part of a quality assurance workflow, it is recommended to also include an additional check on the image contents<a href="#fn16" class="footnote-ref" id="fnref16" role="doc-noteref"><sup>16</sup></a>. Also, <em>jpylyzer</em> does not perform any checks on marker segments within the bit-stream: start-of packet (SOP) and end-of-packet (EPH) markers.</p>
+<p>In addition to the above limitations, <em>jpylyzer</em> can <em>not</em> be used to establish whether the data in the bitstream are correct (this would require decoding the compressed image data, which is completely out of <em>jpylyzer</em>’s scope)<a href="#fn20" class="footnote-ref" id="fnref20" role="doc-noteref"><sup>20</sup></a>. As a result, if <em>jpylyzer</em> is used as part of a quality assurance workflow, it is recommended to also include an additional check on the image contents<a href="#fn21" class="footnote-ref" id="fnref21" role="doc-noteref"><sup>21</sup></a>. Also, <em>jpylyzer</em> does not perform any checks on marker segments within the bit-stream: start-of packet (SOP) and end-of-packet (EPH) markers.</p>
 <h3 id="detection-of-incomplete-or-truncated-codestreams">Detection of incomplete or truncated codestreams</h3>
 <p>A JP2’s tile part header contains information that makes it possible to detect incomplete and truncated codestreams in most cases. Depending on the encoder software used, this method may fail for images that only contain one single tile part (i.e. images that do not contain tiling).</p>
 <h3 id="current-limitations-of-comment-extraction">Current limitations of comment extraction</h3>
 <p>Both the codestream header and the tile part header can contain comment marker segments, which are used for embedding arbitrary binary data or text. <em>Jpylyzer</em> will extract the contents of any comments that are text.</p>
 <h2 id="structure-reported-output">Structure of reported output</h2>
 <p>The Figure below illustrates the structure of <em>jpylyzer</em>’s codestream-level output.</p>
 <figure>
@@ -2103,38 +2147,50 @@
 <td style="text-align: left;">First 2 bytes in codestream constitute a start of codestream (SOC) marker segment</td>
 </tr>
 <tr class="even">
 <td style="text-align: left;">foundSIZMarker</td>
 <td style="text-align: left;">Second marker segment in codestream is image and tile size (SIZ) marker segment</td>
 </tr>
 <tr class="odd">
+<td style="text-align: left;">foundCAPMarker</td>
+<td style="text-align: left;">Codestream main header contains Extended Capabilities (CAP) marker segment if second most significant bit of <em>rsiz</em> equals 1</td>
+</tr>
+<tr class="even">
 <td style="text-align: left;">foundCODMarker</td>
 <td style="text-align: left;">Codestream main header contains coding style default (COD) marker segment</td>
 </tr>
-<tr class="even">
+<tr class="odd">
 <td style="text-align: left;">foundQCDMarker</td>
 <td style="text-align: left;">Codestream main header contains quantization default (QCD) marker segment</td>
 </tr>
+<tr class="even">
+<td style="text-align: left;">CPFnumConsistentWithPRFnum</td>
+<td style="text-align: left;">Value of <em>CPFnum</em> in CPF marker segment is consistent with <em>PRFnum</em> value in PRF marker segment</td>
+</tr>
 <tr class="odd">
+<td style="text-align: left;">CPFnumConsistentWithRsiz</td>
+<td style="text-align: left;">Value of <em>CPFnum</em> in CPF marker segment is consistent with *rsiz^ value in SIZ marker segment</td>
+</tr>
+<tr class="even">
 <td style="text-align: left;">foundExpectedNumberOfTiles</td>
 <td style="text-align: left;">Number of encountered tiles is consistent with expected number of tiles (as calculated from <a href="#siz-marker">SIZ marker</a>)</td>
 </tr>
-<tr class="even">
+<tr class="odd">
 <td style="text-align: left;">foundExpectedNumberOfTileParts</td>
 <td style="text-align: left;">For all tiles, number of encountered tile parts is consistent with expected number of tile parts (values of <em>tnsot</em> from <a href="#sot-marker">SOT marker</a>)</td>
 </tr>
-<tr class="odd">
-<td style="text-align: left;">maxOneCcocPerComponent</td>
-<td style="text-align: left;">No more than one <em>ccoc</em> value for each component (only reported if codestream contains any COC marker segments)</td>
-</tr>
 <tr class="even">
-<td style="text-align: left;">maxOneCqccPerComponent</td>
-<td style="text-align: left;">No more than one <em>cqcc</em> value for each component (only reported if codestream contains any QCC marker segments)</td>
+<td style="text-align: left;">maxOneCcocPerComponentMain</td>
+<td style="text-align: left;">No more than one <em>ccoc</em> value for each component in main header (only reported if codestream contains any COC marker segments)</td>
 </tr>
 <tr class="odd">
+<td style="text-align: left;">maxOneCqccPerComponentMain</td>
+<td style="text-align: left;">No more than one <em>cqcc</em> value for each component in main header (only reported if codestream contains any QCC marker segments)</td>
+</tr>
+<tr class="even">
 <td style="text-align: left;">foundEOCMarker</td>
 <td style="text-align: left;">Last 2 bytes in codestream constitute an end of codestream (EOC) marker segment</td>
 </tr>
 </tbody>
 </table>
 <h2 id="siz-marker">Image and tile size (SIZ) marker segment (child of Contiguous Codestream box)</h2>
 <h3 id="element-name-20">Element name</h3>
@@ -2150,69 +2206,73 @@
 <tbody>
 <tr class="odd">
 <td style="text-align: left;">lsiz</td>
 <td style="text-align: left;">Length of SIZ marker segment in bytes</td>
 </tr>
 <tr class="even">
 <td style="text-align: left;">rsiz</td>
-<td style="text-align: left;">Decoder capabilities</td>
+<td style="text-align: left;">Numerical value of <em>rsiz</em> (capabilities) field</td>
 </tr>
 <tr class="odd">
+<td style="text-align: left;">capability</td>
+<td style="text-align: left;">Capabilities (profile) encoded by <em>rsiz</em> value</td>
+</tr>
+<tr class="even">
 <td style="text-align: left;">xsiz</td>
 <td style="text-align: left;">Width of reference grid</td>
 </tr>
-<tr class="even">
+<tr class="odd">
 <td style="text-align: left;">ysiz</td>
 <td style="text-align: left;">Height of reference grid</td>
 </tr>
-<tr class="odd">
+<tr class="even">
 <td style="text-align: left;">xOsiz</td>
 <td style="text-align: left;">Horizontal offset from origin of reference grid to left of image area</td>
 </tr>
-<tr class="even">
+<tr class="odd">
 <td style="text-align: left;">yOsiz</td>
 <td style="text-align: left;">Vertical offset from origin of reference grid to top of image area</td>
 </tr>
-<tr class="odd">
+<tr class="even">
 <td style="text-align: left;">xTsiz</td>
 <td style="text-align: left;">Width of one reference tile with respect to the reference grid</td>
 </tr>
-<tr class="even">
+<tr class="odd">
 <td style="text-align: left;">yTsiz</td>
 <td style="text-align: left;">Height of one reference tile with respect to the reference grid</td>
 </tr>
-<tr class="odd">
+<tr class="even">
 <td style="text-align: left;">xTOsiz</td>
 <td style="text-align: left;">Horizontal offset from origin of reference grid to left side of first tile</td>
 </tr>
-<tr class="even">
+<tr class="odd">
 <td style="text-align: left;">yTOsiz</td>
 <td style="text-align: left;">Vertical offset from origin of reference grid to top side of first tile</td>
 </tr>
-<tr class="odd">
+<tr class="even">
 <td style="text-align: left;">numberOfTiles</td>
-<td style="text-align: left;">Number of tiles<a href="#fn17" class="footnote-ref" id="fnref17" role="doc-noteref"><sup>17</sup></a></td>
+<td style="text-align: left;">Number of tiles<a href="#fn22" class="footnote-ref" id="fnref22" role="doc-noteref"><sup>22</sup></a></td>
 </tr>
-<tr class="even">
+<tr class="odd">
 <td style="text-align: left;">csiz</td>
 <td style="text-align: left;">Number of components</td>
 </tr>
-<tr class="odd">
+<tr class="even">
 <td style="text-align: left;">ssizSign<sup>*</sup></td>
 <td style="text-align: left;">Indicates whether image component is signed or unsigned (repeated for all components)</td>
 </tr>
-<tr class="even">
+<tr class="odd">
 <td style="text-align: left;">ssizDepth<sup>*</sup></td>
 <td style="text-align: left;">Number of bits for this component (repeated for all components)</td>
 </tr>
-<tr class="odd">
+<tr class="even">
 <td style="text-align: left;">xRsiz<sup>*</sup></td>
 <td style="text-align: left;">Horizontal separation of sample of this component with respect to reference grid (repeated for all components)</td>
 </tr>
-<tr class="even">
+<tr class="odd">
 <td style="text-align: left;">yRsiz<sup>*</sup></td>
 <td style="text-align: left;">Vertical separation of sample of this component with respect to reference grid (repeated for all components)</td>
 </tr>
 </tbody>
 </table>
 <h3 id="tests-19">Tests</h3>
 <table>
@@ -2225,15 +2285,15 @@
 <tbody>
 <tr class="odd">
 <td style="text-align: left;">lsizIsValid</td>
 <td style="text-align: left;"><em>lsiz</em> is within range [41,49190]</td>
 </tr>
 <tr class="even">
 <td style="text-align: left;">rsizIsValid</td>
-<td style="text-align: left;"><em>rsiz</em> equals 0 (“ISO/IEC 15444-1”), 1 (“Profile 0”) or 2 (“Profile 1”)</td>
+<td style="text-align: left;">Four most significant bits of <em>rsiz</em> are 0 (JP2, J2C); second most significant bit of <em>rsiz</em> equals 1 (JPH, JHC)</td>
 </tr>
 <tr class="odd">
 <td style="text-align: left;">xsizIsValid</td>
 <td style="text-align: left;"><em>xsiz</em> is within range [1,2<sup>32</sup> - 1]</td>
 </tr>
 <tr class="even">
 <td style="text-align: left;">ysizIsValid</td>
@@ -2339,31 +2399,31 @@
 </tr>
 <tr class="odd">
 <td style="text-align: left;">codingBypass</td>
 <td style="text-align: left;">Indicates use of coding bypass (“yes”/“no”)</td>
 </tr>
 <tr class="even">
 <td style="text-align: left;">resetOnBoundaries</td>
-<td style="text-align: left;">Indicates reset of context probabilities on coding pass boundaries (“yes”/“no”)</td>
+<td style="text-align: left;">Indicates reset of context probabilities on coding pass boundaries (“yes”/“no”) (does not apply to High Throughput code blocks)</td>
 </tr>
 <tr class="odd">
 <td style="text-align: left;">termOnEachPass</td>
 <td style="text-align: left;">Indicates termination on each coding pass (“yes”/“no”)</td>
 </tr>
 <tr class="even">
 <td style="text-align: left;">vertCausalContext</td>
 <td style="text-align: left;">Indicates vertically causal context (“yes”/“no”)</td>
 </tr>
 <tr class="odd">
 <td style="text-align: left;">predTermination</td>
-<td style="text-align: left;">Indicates predictable termination (“yes”/“no”)</td>
+<td style="text-align: left;">Indicates predictable termination (“yes”/“no”) (does not apply to High Throughput code blocks)</td>
 </tr>
 <tr class="even">
 <td style="text-align: left;">segmentationSymbols</td>
-<td style="text-align: left;">Indicates use of segmentation symbols (“yes”/“no”)</td>
+<td style="text-align: left;">Indicates use of segmentation symbols (“yes”/“no”) (does not apply to High Throughput code blocks)</td>
 </tr>
 <tr class="odd">
 <td style="text-align: left;">transformation</td>
 <td style="text-align: left;">Wavelet transformation: “9-7 irreversible” or “5-3 reversible”</td>
 </tr>
 <tr class="even">
 <td style="text-align: left;">precinctSizeX<sup>*</sup></td>
@@ -2600,15 +2660,15 @@
 </tr>
 <tr class="odd">
 <td style="text-align: left;">roiStyleIsValid</td>
 <td style="text-align: left;"><em>roiStyle</em> equals 0 (“Implicit ROI (maximum shift)”)</td>
 </tr>
 <tr class="even">
 <td style="text-align: left;">roiShiftIsValid</td>
-<td style="text-align: left;"><em>roiShift</em> is within range [0,255]</td>
+<td style="text-align: left;"><em>roiShift</em> is within range [0,255] (JP2, J2C) or [0,37] (JPH, JHC)</td>
 </tr>
 </tbody>
 </table>
 <h2 id="qcd-marker">Quantization default (QCD) marker segment</h2>
 <h3 id="element-name-24">Element name</h3>
 <p>qcd</p>
 <h3 id="reported-properties-24">Reported properties</h3>
@@ -2893,19 +2953,171 @@
 </tr>
 <tr class="odd">
 <td style="text-align: left;">commentIsValid</td>
 <td style="text-align: left;">Comment is valid ISO/IEC8859-15 and does not contain control characters, other than tab, newline or carriage return</td>
 </tr>
 </tbody>
 </table>
+<h2 id="cap-marker">Extended capabilities (CAP) marker segment</h2>
+<p>This marker segment is defined in ISO/IEC 15444-2, and is used by ISO/IEC 15444-15 (as well as other parts of the standard).</p>
+<h3 id="element-name-29">Element name</h3>
+<p>cap</p>
+<h3 id="reported-properties-29">Reported properties</h3>
+<table>
+<thead>
+<tr class="header">
+<th style="text-align: left;">Property</th>
+<th style="text-align: left;">Description</th>
+</tr>
+</thead>
+<tbody>
+<tr class="odd">
+<td style="text-align: left;">lcap</td>
+<td style="text-align: left;">Length of CAP marker segment in bytes</td>
+</tr>
+<tr class="even">
+<td style="text-align: left;">pcapPart</td>
+<td style="text-align: left;">Indicates the use of capabilities from Part <em>pcapPart</em> of the ISO/IEC 15444 standard (repeated for all referenced parts)</td>
+</tr>
+<tr class="odd">
+<td style="text-align: left;">htCodeBlocks</td>
+<td style="text-align: left;">See section 8.2 of ISO/IEC 15444-15 (JPH, JHC)</td>
+</tr>
+<tr class="even">
+<td style="text-align: left;">htSets</td>
+<td style="text-align: left;">See section 8.3 of ISO/IEC 15444-15 (JPH, JHC)</td>
+</tr>
+<tr class="odd">
+<td style="text-align: left;">htRegion</td>
+<td style="text-align: left;">See section 8.4 of ISO/IEC 15444-15 (JPH, JHC)</td>
+</tr>
+<tr class="even">
+<td style="text-align: left;">htHomogeneous</td>
+<td style="text-align: left;">See section 8.5 of ISO/IEC 15444-15 (JPH, JHC)</td>
+</tr>
+<tr class="odd">
+<td style="text-align: left;">htReversible</td>
+<td style="text-align: left;">See section 8.7.2 of ISO/IEC 15444-15 (JPH, JHC)</td>
+</tr>
+<tr class="even">
+<td style="text-align: left;">htB</td>
+<td style="text-align: left;">Parameter <em>B</em> as used in <em>MAGBP</em> sets, see sections A.3.7 and 8.7.3 of ISO/IEC 15444-15 (JPH, JHC)</td>
+</tr>
+</tbody>
+</table>
+<h3 id="tests-28">Tests</h3>
+<table>
+<thead>
+<tr class="header">
+<th style="text-align: left;">Test name</th>
+<th style="text-align: left;">True if</th>
+</tr>
+</thead>
+<tbody>
+<tr class="odd">
+<td style="text-align: left;">lcapIsValid</td>
+<td style="text-align: left;">Number of <em>pcapPart</em> entries equals (<em>lcap</em> - 6)/2</td>
+</tr>
+<tr class="even">
+<td style="text-align: left;">pcap15IsValid</td>
+<td style="text-align: left;">15th most significant bit of <em>pcap</em> equals 1 (JPH, JHC)</td>
+</tr>
+</tbody>
+</table>
+<h2 id="prf-marker">Profile (PRF) marker segment</h2>
+<h3 id="element-name-30">Element name</h3>
+<p>prf</p>
+<h3 id="reported-properties-30">Reported properties</h3>
+<table>
+<thead>
+<tr class="header">
+<th style="text-align: left;">Property</th>
+<th style="text-align: left;">Description</th>
+</tr>
+</thead>
+<tbody>
+<tr class="odd">
+<td style="text-align: left;">lprf</td>
+<td style="text-align: left;">Length of PRF marker segment in bytes</td>
+</tr>
+<tr class="even">
+<td style="text-align: left;">PRFnum</td>
+<td style="text-align: left;">Profile number</td>
+</tr>
+</tbody>
+</table>
+<h3 id="tests-29">Tests</h3>
+<table>
+<thead>
+<tr class="header">
+<th style="text-align: left;">Test name</th>
+<th style="text-align: left;">True if</th>
+</tr>
+</thead>
+<tbody>
+<tr class="odd">
+<td style="text-align: left;">lprfIsValid</td>
+<td style="text-align: left;"><em>lprf</em> is within range [4,65534]</td>
+</tr>
+<tr class="even">
+<td style="text-align: left;">pprfIsValid</td>
+<td style="text-align: left;">last <em>pprf</em> value is not zero</td>
+</tr>
+<tr class="odd">
+<td style="text-align: left;">PRFnumIsValid</td>
+<td style="text-align: left;"><em>PRFnum</em> &gt; 4095</td>
+</tr>
+</tbody>
+</table>
+<h2 id="cpf-marker">Corresponding profile (CPF) marker segment</h2>
+<h3 id="element-name-31">Element name</h3>
+<p>cpf</p>
+<h3 id="reported-properties-31">Reported properties</h3>
+<table>
+<thead>
+<tr class="header">
+<th style="text-align: left;">Property</th>
+<th style="text-align: left;">Description</th>
+</tr>
+</thead>
+<tbody>
+<tr class="odd">
+<td style="text-align: left;">lcpf</td>
+<td style="text-align: left;">Length of CPF marker segment in bytes</td>
+</tr>
+<tr class="even">
+<td style="text-align: left;">CPFnum</td>
+<td style="text-align: left;">Profile number</td>
+</tr>
+</tbody>
+</table>
+<h3 id="tests-30">Tests</h3>
+<table>
+<thead>
+<tr class="header">
+<th style="text-align: left;">Test name</th>
+<th style="text-align: left;">True if</th>
+</tr>
+</thead>
+<tbody>
+<tr class="odd">
+<td style="text-align: left;">lcpfIsValid</td>
+<td style="text-align: left;"><em>lcpf</em> is within range [4,65534] (JPH, JHC)</td>
+</tr>
+<tr class="even">
+<td style="text-align: left;">pcpfIsValid</td>
+<td style="text-align: left;">last <em>pcpf</em> value is not zero (JPH, JHC)</td>
+</tr>
+</tbody>
+</table>
 <h2 id="tile-part">Tile part (child of Contiguous Codestream box)</h2>
 <p>Tile-part level properties and tests. This is not a box or a marker segment!</p>
-<h3 id="element-name-29">Element name</h3>
+<h3 id="element-name-32">Element name</h3>
 <p>tilePart (child of tileParts)</p>
-<h3 id="reported-properties-29">Reported properties</h3>
+<h3 id="reported-properties-32">Reported properties</h3>
 <p>Each tile part element can contain a number of child elements:</p>
 <table>
 <thead>
 <tr class="header">
 <th style="text-align: left;">Child element</th>
 <th style="text-align: left;">Description</th>
 </tr>
@@ -2968,37 +3180,65 @@
 </tr>
 <tr class="even">
 <td style="text-align: left;">pptCount</td>
 <td style="text-align: left;">Number of PPT markers in tile part header</td>
 </tr>
 </tbody>
 </table>
-<h3 id="tests-28">Tests</h3>
+<h3 id="tests-31">Tests</h3>
 <table>
 <thead>
 <tr class="header">
 <th style="text-align: left;">Test name</th>
 <th style="text-align: left;">True if</th>
 </tr>
 </thead>
 <tbody>
 <tr class="odd">
+<td style="text-align: left;">CODAllowed</td>
+<td style="text-align: left;">COD marker is allowed in this tile part (only allowed in first tile-part of a tile)</td>
+</tr>
+<tr class="even">
+<td style="text-align: left;">COCAllowed</td>
+<td style="text-align: left;">COC marker is allowed in this tile part (only allowed in first tile-part of a tile)</td>
+</tr>
+<tr class="odd">
+<td style="text-align: left;">QCDAllowed</td>
+<td style="text-align: left;">QCD marker is allowed in this tile part (only allowed in first tile-part of a tile)</td>
+</tr>
+<tr class="even">
+<td style="text-align: left;">QCCAllowed</td>
+<td style="text-align: left;">QCC marker is allowed in this tile part (only allowed in first tile-part of a tile)</td>
+</tr>
+<tr class="odd">
+<td style="text-align: left;">RGNAllowed</td>
+<td style="text-align: left;">RGN marker is allowed in this tile part (only allowed in first tile-part of a tile)</td>
+</tr>
+<tr class="even">
+<td style="text-align: left;">maxOneCcocPerComponentTP</td>
+<td style="text-align: left;">No more than one <em>ccoc</em> value for each component in tile-part header (only reported if codestream contains any COC marker segments)</td>
+</tr>
+<tr class="odd">
+<td style="text-align: left;">maxOneCqccPerComponentTP</td>
+<td style="text-align: left;">No more than one <em>cqcc</em> value for each component in tile-part header (only reported if codestream contains any QCC marker segments)</td>
+</tr>
+<tr class="even">
 <td style="text-align: left;">foundNextTilePartOrEOC</td>
 <td style="text-align: left;">Tile part start offset + <em>tilePartLength</em> points to either start of new tile or EOC marker (useful for detecting within-codestream byte corruption)</td>
 </tr>
-<tr class="even">
+<tr class="odd">
 <td style="text-align: left;">foundSODMarker</td>
 <td style="text-align: left;">Last marker segment of tile part is a start-of-data (SOD) marker</td>
 </tr>
 </tbody>
 </table>
 <h2 id="sot-marker">Start of tile part (SOT) marker segment (child of tile part)</h2>
-<h3 id="element-name-30">Element name</h3>
+<h3 id="element-name-33">Element name</h3>
 <p>sot</p>
-<h3 id="reported-properties-30">Reported properties</h3>
+<h3 id="reported-properties-33">Reported properties</h3>
 <table>
 <thead>
 <tr class="header">
 <th style="text-align: left;">Property</th>
 <th style="text-align: left;">Description</th>
 </tr>
 </thead>
@@ -3021,15 +3261,15 @@
 </tr>
 <tr class="odd">
 <td style="text-align: left;">tnsot</td>
 <td style="text-align: left;">Number of tile-parts of a tile in the codestream (value of 0 indicates that number of tile-parts of tile in the codestream is not defined in current header)</td>
 </tr>
 </tbody>
 </table>
-<h3 id="tests-29">Tests</h3>
+<h3 id="tests-32">Tests</h3>
 <table>
 <thead>
 <tr class="header">
 <th style="text-align: left;">Test name</th>
 <th style="text-align: left;">True if</th>
 </tr>
 </thead>
@@ -3051,17 +3291,17 @@
 <td style="text-align: left;"><em>tpsot</em> is within range [0,254]</td>
 </tr>
 </tbody>
 </table>
 <p><br></p>
 <p>The following marker segments are only minimally supported: <em>jpylyzer</em> will report their presence in the <em>properties</em> element, but it does not perform any further tests or analyses. This may change in upcoming versions of the software.</p>
 <h2 id="tlm-marker">Tile-part lengths (TLM) marker segment</h2>
-<h3 id="element-name-31">Element name</h3>
+<h3 id="element-name-34">Element name</h3>
 <p>tlm</p>
-<h3 id="reported-properties-31">Reported properties</h3>
+<h3 id="reported-properties-34">Reported properties</h3>
 <table>
 <thead>
 <tr class="header">
 <th style="text-align: left;">Property</th>
 <th style="text-align: left;">Description</th>
 </tr>
 </thead>
@@ -3072,15 +3312,15 @@
 </tr>
 <tr class="even">
 <td style="text-align: left;"></td>
 <td style="text-align: left;"></td>
 </tr>
 </tbody>
 </table>
-<h3 id="tests-30">Tests</h3>
+<h3 id="tests-33">Tests</h3>
 <table>
 <thead>
 <tr class="header">
 <th style="text-align: left;">Test name</th>
 <th style="text-align: left;">True if</th>
 </tr>
 </thead>
@@ -3092,17 +3332,17 @@
 <tr class="even">
 <td style="text-align: left;"></td>
 <td style="text-align: left;"></td>
 </tr>
 </tbody>
 </table>
 <h2 id="plm-marker">Packet length, main header (PLM) marker segment</h2>
-<h3 id="element-name-32">Element name</h3>
+<h3 id="element-name-35">Element name</h3>
 <p>plm</p>
-<h3 id="reported-properties20">Reported properties<a href="#fn18" class="footnote-ref" id="fnref18" role="doc-noteref"><sup>18</sup></a></h3>
+<h3 id="reported-properties20">Reported properties<a href="#fn23" class="footnote-ref" id="fnref23" role="doc-noteref"><sup>23</sup></a></h3>
 <table>
 <thead>
 <tr class="header">
 <th style="text-align: left;">Property</th>
 <th style="text-align: left;">Description</th>
 </tr>
 </thead>
@@ -3121,15 +3361,15 @@
 </tr>
 <tr class="even">
 <td style="text-align: left;">iplm</td>
 <td style="text-align: left;">Comma separated list of packet length values (as hexadecimal strings)</td>
 </tr>
 </tbody>
 </table>
-<h3 id="tests-31">Tests</h3>
+<h3 id="tests-34">Tests</h3>
 <table>
 <thead>
 <tr class="header">
 <th style="text-align: left;">Test name</th>
 <th style="text-align: left;">True if</th>
 </tr>
 </thead>
@@ -3141,17 +3381,17 @@
 <tr class="even">
 <td style="text-align: left;"></td>
 <td style="text-align: left;"></td>
 </tr>
 </tbody>
 </table>
 <h2 id="ppm-marker">Packed packet headers, main header (PPM) marker segment</h2>
-<h3 id="element-name-33">Element name</h3>
+<h3 id="element-name-36">Element name</h3>
 <p>ppm</p>
-<h3 id="reported-properties20-1">Reported properties<a href="#fn19" class="footnote-ref" id="fnref19" role="doc-noteref"><sup>19</sup></a></h3>
+<h3 id="reported-properties20-1">Reported properties<a href="#fn24" class="footnote-ref" id="fnref24" role="doc-noteref"><sup>24</sup></a></h3>
 <table>
 <thead>
 <tr class="header">
 <th style="text-align: left;">Property</th>
 <th style="text-align: left;">Description</th>
 </tr>
 </thead>
@@ -3162,15 +3402,15 @@
 </tr>
 <tr class="even">
 <td style="text-align: left;"></td>
 <td style="text-align: left;"></td>
 </tr>
 </tbody>
 </table>
-<h3 id="tests-32">Tests</h3>
+<h3 id="tests-35">Tests</h3>
 <table>
 <thead>
 <tr class="header">
 <th style="text-align: left;">Test name</th>
 <th style="text-align: left;">True if</th>
 </tr>
 </thead>
@@ -3182,17 +3422,17 @@
 <tr class="even">
 <td style="text-align: left;"></td>
 <td style="text-align: left;"></td>
 </tr>
 </tbody>
 </table>
 <h2 id="plt-marker">Packet length, tile-part header (PLT) marker segment</h2>
-<h3 id="element-name-34">Element name</h3>
+<h3 id="element-name-37">Element name</h3>
 <p>plt</p>
-<h3 id="reported-properties20-2">Reported properties<a href="#fn20" class="footnote-ref" id="fnref20" role="doc-noteref"><sup>20</sup></a></h3>
+<h3 id="reported-properties20-2">Reported properties<a href="#fn25" class="footnote-ref" id="fnref25" role="doc-noteref"><sup>25</sup></a></h3>
 <table>
 <thead>
 <tr class="header">
 <th style="text-align: left;">Property</th>
 <th style="text-align: left;">Description</th>
 </tr>
 </thead>
@@ -3211,15 +3451,15 @@
 </tr>
 <tr class="even">
 <td style="text-align: left;">iplt</td>
 <td style="text-align: left;">Comma separated list of packet length values (as hexadecimal strings)</td>
 </tr>
 </tbody>
 </table>
-<h3 id="tests-33">Tests</h3>
+<h3 id="tests-36">Tests</h3>
 <table>
 <thead>
 <tr class="header">
 <th style="text-align: left;">Test name</th>
 <th style="text-align: left;">True if</th>
 </tr>
 </thead>
@@ -3231,17 +3471,17 @@
 <tr class="even">
 <td style="text-align: left;"></td>
 <td style="text-align: left;"></td>
 </tr>
 </tbody>
 </table>
 <h2 id="ppt-marker">Packed packet headers, tile-part header (PPT) marker segment</h2>
-<h3 id="element-name-35">Element name</h3>
+<h3 id="element-name-38">Element name</h3>
 <p>ppt</p>
-<h3 id="reported-properties20-3">Reported properties<a href="#fn21" class="footnote-ref" id="fnref21" role="doc-noteref"><sup>21</sup></a></h3>
+<h3 id="reported-properties20-3">Reported properties<a href="#fn26" class="footnote-ref" id="fnref26" role="doc-noteref"><sup>26</sup></a></h3>
 <table>
 <thead>
 <tr class="header">
 <th style="text-align: left;">Property</th>
 <th style="text-align: left;">Description</th>
 </tr>
 </thead>
@@ -3252,15 +3492,15 @@
 </tr>
 <tr class="even">
 <td style="text-align: left;"></td>
 <td style="text-align: left;"></td>
 </tr>
 </tbody>
 </table>
-<h3 id="tests-34">Tests</h3>
+<h3 id="tests-37">Tests</h3>
 <table>
 <thead>
 <tr class="header">
 <th style="text-align: left;">Test name</th>
 <th style="text-align: left;">True if</th>
 </tr>
 </thead>
@@ -3281,30 +3521,35 @@
 <p>ISO/IEC. Information technology — JPEG 2000 image coding system: Extensions. ISO/IEC 15444-2, First edition. Geneva: ISO/IEC, 2004b. <a href="https://www.jpeg.org/public/15444-2annexm.pdf">https://www.jpeg.org/public/15444-2annexm.pdf</a> (“Annex M: JPX extended file format syntax” only).</p>
 <p>Leach, P., Mealling, M. &amp; Salz, R. A Universally Unique IDentifier (UUID) URN namespace. Memo, IETF. <a href="https://tools.ietf.org/html/rfc4122.html">https://tools.ietf.org/html/rfc4122.html</a>.</p>
 <section class="footnotes" role="doc-endnotes">
 <hr />
 <ol>
 <li id="fn1" role="doc-endnote"><p>The <em>jpylyzer</em> binaries were created using the <em>PyInstaller</em> package: <a href="https://www.pyinstaller.org/">https://www.pyinstaller.org/</a><a href="#fnref1" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
 <li id="fn2" role="doc-endnote"><p>Note that <em>jpylyzer</em> versions 1.8 and earlier returned a formatted XML string instead of an element object!<a href="#fnref2" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
-<li id="fn3" role="doc-endnote"><p>Note that <em>jpylyzer</em> versions 1.4 and earlier used the verbose output format by default. This behaviour has changed in version 1.5 onwards, as the lengthy output turned out to be slightly confusing to some users.<a href="#fnref3" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
-<li id="fn4" role="doc-endnote"><p>The “Any ICC” method is defined in ISO/IEC 15444-2 (the JPX format), and is not allowed in JP2. However, <em>jpylyzer</em> offers limited support for JPX here by also reporting the properties of ICC profiles that were embedded using this method. Note that any file that uses this method will fail the “methIsValid” test (and thereby the validation).<a href="#fnref4" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
-<li id="fn5" role="doc-endnote"><p>Originally ISO/IEC 15444-1 only allowed “input device” profiles. Support of “display device” profiles was added through an <a href="http://www.itu.int/rec/T-REC-T.800-201303-P!Amd6/en">amendment</a> to the standard in 2013. The behaviour of <em>jpylyzer</em> is consistent with this amendment.<a href="#fnref5" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
-<li id="fn6" role="doc-endnote"><p>Calculated as: <math xmlns="http://www.w3.org/1998/Math/MathML"> <mrow> <mfrac> <mrow> <mi>vRcN</mi> </mrow> <mrow> <mi>vRcD</mi> </mrow> </mfrac> <mo>•</mo> <msup> <mn>10</mn> <mi>vRcE</mi> </msup> </mrow> </math><a href="#fnref6" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
-<li id="fn7" role="doc-endnote"><p>Calculated as: <math xmlns="http://www.w3.org/1998/Math/MathML"> <mrow> <mfrac> <mrow> <mi>hRcN</mi> </mrow> <mrow> <mi>hRcD</mi> </mrow> </mfrac> <mo>•</mo> <msup> <mn>10</mn> <mi>hRcE</mi> </msup> </mrow> </math><a href="#fnref7" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
-<li id="fn8" role="doc-endnote"><p>Calculated as: <math xmlns="http://www.w3.org/1998/Math/MathML"> <mrow> <mi>vRescInPixelsPerMeter</mi> <mo>•</mo> <mn>25.4</mn> <mo>•</mo> <msup> <mn>10</mn> <mi>-3</mi> </msup> </mrow> </math><a href="#fnref8" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
-<li id="fn9" role="doc-endnote"><p>Calculated as: <math xmlns="http://www.w3.org/1998/Math/MathML"> <mrow> <mi>hRescInPixelsPerMeter</mi> <mo>•</mo> <mn>25.4</mn> <mo>•</mo> <msup> <mn>10</mn> <mi>-3</mi> </msup> </mrow> </math><a href="#fnref9" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
-<li id="fn10" role="doc-endnote"><p>Calculated as: <math xmlns="http://www.w3.org/1998/Math/MathML"> <mrow> <mfrac> <mrow> <mi>vRdN</mi> </mrow> <mrow> <mi>vRdD</mi> </mrow> </mfrac> <mo>•</mo> <msup> <mn>10</mn> <mi>vRdE</mi> </msup> </mrow> </math><a href="#fnref10" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
-<li id="fn11" role="doc-endnote"><p>Calculated as: <math xmlns="http://www.w3.org/1998/Math/MathML"> <mrow> <mfrac> <mrow> <mi>hRdN</mi> </mrow> <mrow> <mi>hRdD</mi> </mrow> </mfrac> <mo>•</mo> <msup> <mn>10</mn> <mi>hRdE</mi> </msup> </mrow> </math><a href="#fnref11" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
-<li id="fn12" role="doc-endnote"><p>Calculated as: <math xmlns="http://www.w3.org/1998/Math/MathML"> <mrow> <mi>vResdInPixelsPerMeter</mi> <mo>•</mo> <mn>25.4</mn> <mo>•</mo> <msup> <mn>10</mn> <mi>-3</mi> </msup> </mrow> </math><a href="#fnref12" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
-<li id="fn13" role="doc-endnote"><p>Calculated as: <math xmlns="http://www.w3.org/1998/Math/MathML"> <mrow> <mi>hResdInPixelsPerMeter</mi> <mo>•</mo> <mn>25.4</mn> <mo>•</mo> <msup> <mn>10</mn> <mi>-3</mi> </msup> </mrow> </math><a href="#fnref13" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
-<li id="fn14" role="doc-endnote"><p>Link: <a href="https://wwwimages.adobe.com/www.adobe.com/content/dam/Adobe/en/devnet/xmp/pdfs/cs6/XMPSpecificationPart3.pdf">https://wwwimages.adobe.com/www.adobe.com/content/dam/Adobe/en/devnet/xmp/pdfs/cs6/XMPSpecificationPart3.pdf</a><a href="#fnref14" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
-<li id="fn15" role="doc-endnote"><p>However, support for start of packet (SOP) and end of packet (EPH) markers may be included in future versions.<a href="#fnref15" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
-<li id="fn16" role="doc-endnote"><p>For example, in a TIFF to JP2 conversion workflow one could include a pixel-by-pixel comparison of the values in the TIFF and the JP2.<a href="#fnref16" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
-<li id="fn17" role="doc-endnote"><p>Calculated as: <math xmlns="http://www.w3.org/1998/Math/MathML"> <mrow> <mi>numberOfTiles</mi> <mo>=</mo> <mo>[</mo> <mfrac> <mrow> <mi>xsiz</mi> <mo>-</mo> <mi>xOsiz</mi> </mrow> <mrow> <mi>xTsiz</mi> </mrow> </mfrac> <mo>]</mo> <mo>•</mo> <mo>[</mo> <mfrac> <mrow> <mi>ysiz</mi> <mo>-</mo> <mi>yOsiz</mi> </mrow> <mrow> <mi>yTsiz</mi> </mrow> </mfrac> <mo>]</mo> </mrow> </math><a href="#fnref17" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
-<li id="fn18" role="doc-endnote"><p>Only reported if the <code>--packetmarkers</code> option is used.<a href="#fnref18" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
-<li id="fn19" role="doc-endnote"><p>Only reported if the <code>--packetmarkers</code> option is used.<a href="#fnref19" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
-<li id="fn20" role="doc-endnote"><p>Only reported if the <code>--packetmarkers</code> option is used.<a href="#fnref20" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
-<li id="fn21" role="doc-endnote"><p>Only reported if the <code>--packetmarkers</code> option is used.<a href="#fnref21" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
+<li id="fn3" role="doc-endnote"><p>Jpylyzer 2.2 and more recent only work with Python &gt; 3.2. Since Jython still hasn’t been upgraded to support Python 3, Java integration with Jython currently doesn’t work.<a href="#fnref3" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
+<li id="fn4" role="doc-endnote"><p>Note that <em>jpylyzer</em> versions 1.4 and earlier used the verbose output format by default. This behaviour has changed in version 1.5 onwards, as the lengthy output turned out to be slightly confusing to some users.<a href="#fnref4" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
+<li id="fn5" role="doc-endnote"><p>Meaning of values defined in Table 2 of Rec. ITU-T H.273 / ISO/IEC 23001-8 <a href="https://www.itu.int/rec/dologin_pub.asp?lang=e&amp;id=T-REC-H.273-202107-I!!PDF-E&amp;type=items">“Coding-independent code points for video signal type identification”</a><a href="#fnref5" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
+<li id="fn6" role="doc-endnote"><p>Meaning of values defined in Table 3 of Rec. ITU-T H.273 / ISO/IEC 23001-8 <a href="https://www.itu.int/rec/dologin_pub.asp?lang=e&amp;id=T-REC-H.273-202107-I!!PDF-E&amp;type=items">“Coding-independent code points for video signal type identification”</a><a href="#fnref6" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
+<li id="fn7" role="doc-endnote"><p>Meaning of values defined in Table 4 of Rec. ITU-T H.273 / ISO/IEC 23001-8 <a href="https://www.itu.int/rec/dologin_pub.asp?lang=e&amp;id=T-REC-H.273-202107-I!!PDF-E&amp;type=items">“Coding-independent code points for video signal type identification”</a><a href="#fnref7" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
+<li id="fn8" role="doc-endnote"><p>Meaning defined in Rec. ITU-T H.273 / ISO/IEC 23001-8 <a href="https://www.itu.int/rec/dologin_pub.asp?lang=e&amp;id=T-REC-H.273-202107-I!!PDF-E&amp;type=items">“Coding-independent code points for video signal type identification”</a><a href="#fnref8" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
+<li id="fn9" role="doc-endnote"><p>Originally ISO/IEC 15444-1 only allowed “input device” profiles. Support of “display device” profiles was added through an <a href="http://www.itu.int/rec/T-REC-T.800-201303-P!Amd6/en">amendment</a> to the standard in 2013. The behaviour of <em>jpylyzer</em> is consistent with this amendment.<a href="#fnref9" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
+<li id="fn10" role="doc-endnote"><p>For JPH, an addition “application-defined” value is allowed (ISO/IEC 15444-15, Table D.4)<a href="#fnref10" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
+<li id="fn11" role="doc-endnote"><p>Calculated as: <math xmlns="http://www.w3.org/1998/Math/MathML"> <mrow> <mfrac> <mrow> <mi>vRcN</mi> </mrow> <mrow> <mi>vRcD</mi> </mrow> </mfrac> <mo>•</mo> <msup> <mn>10</mn> <mi>vRcE</mi> </msup> </mrow> </math><a href="#fnref11" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
+<li id="fn12" role="doc-endnote"><p>Calculated as: <math xmlns="http://www.w3.org/1998/Math/MathML"> <mrow> <mfrac> <mrow> <mi>hRcN</mi> </mrow> <mrow> <mi>hRcD</mi> </mrow> </mfrac> <mo>•</mo> <msup> <mn>10</mn> <mi>hRcE</mi> </msup> </mrow> </math><a href="#fnref12" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
+<li id="fn13" role="doc-endnote"><p>Calculated as: <math xmlns="http://www.w3.org/1998/Math/MathML"> <mrow> <mi>vRescInPixelsPerMeter</mi> <mo>•</mo> <mn>25.4</mn> <mo>•</mo> <msup> <mn>10</mn> <mi>-3</mi> </msup> </mrow> </math><a href="#fnref13" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
+<li id="fn14" role="doc-endnote"><p>Calculated as: <math xmlns="http://www.w3.org/1998/Math/MathML"> <mrow> <mi>hRescInPixelsPerMeter</mi> <mo>•</mo> <mn>25.4</mn> <mo>•</mo> <msup> <mn>10</mn> <mi>-3</mi> </msup> </mrow> </math><a href="#fnref14" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
+<li id="fn15" role="doc-endnote"><p>Calculated as: <math xmlns="http://www.w3.org/1998/Math/MathML"> <mrow> <mfrac> <mrow> <mi>vRdN</mi> </mrow> <mrow> <mi>vRdD</mi> </mrow> </mfrac> <mo>•</mo> <msup> <mn>10</mn> <mi>vRdE</mi> </msup> </mrow> </math><a href="#fnref15" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
+<li id="fn16" role="doc-endnote"><p>Calculated as: <math xmlns="http://www.w3.org/1998/Math/MathML"> <mrow> <mfrac> <mrow> <mi>hRdN</mi> </mrow> <mrow> <mi>hRdD</mi> </mrow> </mfrac> <mo>•</mo> <msup> <mn>10</mn> <mi>hRdE</mi> </msup> </mrow> </math><a href="#fnref16" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
+<li id="fn17" role="doc-endnote"><p>Calculated as: <math xmlns="http://www.w3.org/1998/Math/MathML"> <mrow> <mi>vResdInPixelsPerMeter</mi> <mo>•</mo> <mn>25.4</mn> <mo>•</mo> <msup> <mn>10</mn> <mi>-3</mi> </msup> </mrow> </math><a href="#fnref17" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
+<li id="fn18" role="doc-endnote"><p>Calculated as: <math xmlns="http://www.w3.org/1998/Math/MathML"> <mrow> <mi>hResdInPixelsPerMeter</mi> <mo>•</mo> <mn>25.4</mn> <mo>•</mo> <msup> <mn>10</mn> <mi>-3</mi> </msup> </mrow> </math><a href="#fnref18" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
+<li id="fn19" role="doc-endnote"><p>Link: <a href="https://wwwimages.adobe.com/www.adobe.com/content/dam/Adobe/en/devnet/xmp/pdfs/cs6/XMPSpecificationPart3.pdf">https://wwwimages.adobe.com/www.adobe.com/content/dam/Adobe/en/devnet/xmp/pdfs/cs6/XMPSpecificationPart3.pdf</a><a href="#fnref19" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
+<li id="fn20" role="doc-endnote"><p>However, support for start of packet (SOP) and end of packet (EPH) markers may be included in future versions.<a href="#fnref20" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
+<li id="fn21" role="doc-endnote"><p>For example, in a TIFF to JP2 conversion workflow one could include a pixel-by-pixel comparison of the values in the TIFF and the JP2.<a href="#fnref21" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
+<li id="fn22" role="doc-endnote"><p>Calculated as: <math xmlns="http://www.w3.org/1998/Math/MathML"> <mrow> <mi>numberOfTiles</mi> <mo>=</mo> <mo>[</mo> <mfrac> <mrow> <mi>xsiz</mi> <mo>-</mo> <mi>xOsiz</mi> </mrow> <mrow> <mi>xTsiz</mi> </mrow> </mfrac> <mo>]</mo> <mo>•</mo> <mo>[</mo> <mfrac> <mrow> <mi>ysiz</mi> <mo>-</mo> <mi>yOsiz</mi> </mrow> <mrow> <mi>yTsiz</mi> </mrow> </mfrac> <mo>]</mo> </mrow> </math><a href="#fnref22" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
+<li id="fn23" role="doc-endnote"><p>Only reported if the <code>--packetmarkers</code> option is used.<a href="#fnref23" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
+<li id="fn24" role="doc-endnote"><p>Only reported if the <code>--packetmarkers</code> option is used.<a href="#fnref24" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
+<li id="fn25" role="doc-endnote"><p>Only reported if the <code>--packetmarkers</code> option is used.<a href="#fnref25" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
+<li id="fn26" role="doc-endnote"><p>Only reported if the <code>--packetmarkers</code> option is used.<a href="#fnref26" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
 </ol>
 </section>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -26,14 +26,15 @@
           o _f_i_l_e_ _e_l_e_m_e_n_t
           o _f_i_l_e_I_n_f_o_ _e_l_e_m_e_n_t
           o _s_t_a_t_u_s_I_n_f_o_ _e_l_e_m_e_n_t
           o _i_s_V_a_l_i_d_ _e_l_e_m_e_n_t
           o _t_e_s_t_s_ _e_l_e_m_e_n_t
           o _p_r_o_p_e_r_t_i_e_s_ _e_l_e_m_e_n_t
           o _p_r_o_p_e_r_t_i_e_s_E_x_t_e_n_s_i_o_n_ _e_l_e_m_e_n_t
+          o _w_a_r_n_i_n_g_s_ _e_l_e_m_e_n_t
     * _J_P_2_:_ _b_o_x_ _b_y_ _b_o_x
           o _A_b_o_u_t_ _t_h_e_ _p_r_o_p_e_r_t_i_e_s_ _a_n_d_ _t_e_s_t_s_ _t_r_e_e_s
           o _J_P_E_G_ _2_0_0_0_ _S_i_g_n_a_t_u_r_e_ _b_o_x
           o _F_i_l_e_ _T_y_p_e_ _b_o_x
           o _J_P_2_ _H_e_a_d_e_r_ _b_o_x_ _(_s_u_p_e_r_b_o_x_)
           o _I_m_a_g_e_ _H_e_a_d_e_r_ _b_o_x_ _(_c_h_i_l_d_ _o_f_ _J_P_2_ _H_e_a_d_e_r_ _b_o_x_)
           o _B_i_t_s_ _P_e_r_ _C_o_m_p_o_n_e_n_t_ _b_o_x_ _(_c_h_i_l_d_ _o_f_ _J_P_2_ _H_e_a_d_e_r_ _b_o_x_)
@@ -64,14 +65,17 @@
           o _C_o_d_i_n_g_ _s_t_y_l_e_ _c_o_m_p_o_n_e_n_t_ _(_C_O_C_)_ _m_a_r_k_e_r_ _s_e_g_m_e_n_t
           o _R_e_g_i_o_n_-_o_f_-_i_n_t_e_r_e_s_t_ _(_R_G_N_)_ _m_a_r_k_e_r_ _s_e_g_m_e_n_t
           o _Q_u_a_n_t_i_z_a_t_i_o_n_ _d_e_f_a_u_l_t_ _(_Q_C_D_)_ _m_a_r_k_e_r_ _s_e_g_m_e_n_t
           o _Q_u_a_n_t_i_z_a_t_i_o_n_ _c_o_m_p_o_n_e_n_t_ _(_Q_C_C_)_ _m_a_r_k_e_r_ _s_e_g_m_e_n_t
           o _P_r_o_g_r_e_s_s_i_o_n_ _o_r_d_e_r_ _c_h_a_n_g_e_ _(_P_O_C_)_ _m_a_r_k_e_r_ _s_e_g_m_e_n_t
           o _C_o_m_p_o_n_e_n_t_ _r_e_g_i_s_t_r_a_t_i_o_n_ _(_C_R_G_)_ _m_a_r_k_e_r_ _s_e_g_m_e_n_t
           o _C_o_m_m_e_n_t_ _(_C_O_M_)_ _m_a_r_k_e_r_ _s_e_g_m_e_n_t
+          o _E_x_t_e_n_d_e_d_ _c_a_p_a_b_i_l_i_t_i_e_s_ _(_C_A_P_)_ _m_a_r_k_e_r_ _s_e_g_m_e_n_t
+          o _P_r_o_f_i_l_e_ _(_P_R_F_)_ _m_a_r_k_e_r_ _s_e_g_m_e_n_t
+          o _C_o_r_r_e_s_p_o_n_d_i_n_g_ _p_r_o_f_i_l_e_ _(_C_P_F_)_ _m_a_r_k_e_r_ _s_e_g_m_e_n_t
           o _T_i_l_e_ _p_a_r_t_ _(_c_h_i_l_d_ _o_f_ _C_o_n_t_i_g_u_o_u_s_ _C_o_d_e_s_t_r_e_a_m_ _b_o_x_)
           o _S_t_a_r_t_ _o_f_ _t_i_l_e_ _p_a_r_t_ _(_S_O_T_)_ _m_a_r_k_e_r_ _s_e_g_m_e_n_t_ _(_c_h_i_l_d_ _o_f_ _t_i_l_e_ _p_a_r_t_)
           o _T_i_l_e_-_p_a_r_t_ _l_e_n_g_t_h_s_ _(_T_L_M_)_ _m_a_r_k_e_r_ _s_e_g_m_e_n_t
           o _P_a_c_k_e_t_ _l_e_n_g_t_h_,_ _m_a_i_n_ _h_e_a_d_e_r_ _(_P_L_M_)_ _m_a_r_k_e_r_ _s_e_g_m_e_n_t
           o _P_a_c_k_e_d_ _p_a_c_k_e_t_ _h_e_a_d_e_r_s_,_ _m_a_i_n_ _h_e_a_d_e_r_ _(_P_P_M_)_ _m_a_r_k_e_r_ _s_e_g_m_e_n_t
           o _P_a_c_k_e_t_ _l_e_n_g_t_h_,_ _t_i_l_e_-_p_a_r_t_ _h_e_a_d_e_r_ _(_P_L_T_)_ _m_a_r_k_e_r_ _s_e_g_m_e_n_t
           o _P_a_c_k_e_d_ _p_a_c_k_e_t_ _h_e_a_d_e_r_s_,_ _t_i_l_e_-_p_a_r_t_ _h_e_a_d_e_r_ _(_P_P_T_)_ _m_a_r_k_e_r_ _s_e_g_m_e_n_t
@@ -82,14 +86,16 @@
 images. JP2 is the still image format that is defined by JPEG 2000 Part 1 (ISO/
 IEC 15444-1). JJppyyllyyzzeerr was specifically created to answer the following
 questions that you might have about any JP2 file:
    1. Is this really a JP2 and does it really conform to the format’s
       specifications (validation)?
    2. What are the technical characteristics of this image (feature
       extraction)?
+Starting with version 2.2, jjppyyllyyzzeerr also supports Part 15 of the standard (ISO/
+IEC 15444-15, High Throughput JPEG 2000), and its JPH image format.
 ********** VVaalliiddaattiioonn:: ssccooppee aanndd rreessttrriiccttiioonnss **********
 Since the word ‘validation’ means different things to different people, a few
 words about the overall scope of jjppyyllyyzzeerr. First of all, it is important to
 stress that jjppyyllyyzzeerr is not a ‘one stop solution’ that will tell you that an
 image is 100% perfect. What jjppyyllyyzzeerr does is this: based on the JP2 format
 specification (ISO/IEC 15444-1), it parses a file. It then subjects the file’s
 contents to a large number of tests, each of which is based on the requirements
@@ -125,18 +131,14 @@
     * Format migration workflows (e.g. TIFF to JP2) should ideally also include
       some comparison between source and destination images (e.g. a pixel-wise
       comparison)
 Conversely, an image that successfully passes a rendering test or pixel-wise
 comparison may still contain problematic features (e.g. incorrect colour space
 information), so validation, rendering tests and pixel-wise comparisons are
 really complementary to each other.
-******** NNoottee oonn IICCCC pprrooffiillee ssuuppppoorrtt ********
-The support of ICC profiles in JP2 was recently extended through an _a_m_e_n_d_m_e_n_t
-to the standard. These changes are taken into account by jjppyyllyyzzeerr, which is in
-line with the most recent version of the (updated) standard.
 ********** OOuuttlliinnee ooff tthhiiss UUsseerr MMaannuuaall **********
 We start by describing the _i_n_s_t_a_l_l_a_t_i_o_n_ _p_r_o_c_e_s_s of jjppyyllyyzzeerr for Windows and
 Unix-based systems. We then explain its _b_a_s_i_c_ _u_s_a_g_e, either as a command-line
 tool, or as an importable Python module. This is followed by a brief overview
 of _t_h_e_ _s_t_r_u_c_t_u_r_e_ _o_f_ _t_h_e_ _J_P_2_ _f_o_r_m_a_t and its ‘box’ structure, and an explanation
 of JJppyyllyyzzeerr’s _o_u_t_p_u_t_ _f_o_r_m_a_t. The final sections give a detailed description of
 the tests that jjppyyllyyzzeerr performs for validation, and the properties that are
@@ -165,16 +167,15 @@
 To obtain the latest version of the software please use the download links at
 the jjppyyllyyzzeerr homepage:
 _h_t_t_p_s_:_/_/_j_p_y_l_y_z_e_r_._o_p_e_n_p_r_e_s_e_r_v_a_t_i_o_n_._o_r_g_/
 You have three options:
    1. Install the software with the PPiipp package manager. This works on all
       platforms (Windows, Linux, Mac, etc.), but you need to have the Python
       interpreter available on your system. Jpylyzer is compatible with Python
-      2.7, and Python 3.2 and more recent (Python 3.0 and 3.1 are not
-      supported).
+      3.2 and more recent.
    2. Alternatively, for Windows users there is also a set of stand-alone
       binaries_1. These allow you to run jjppyyllyyzzeerr as an executable Windows
       application, without any need for installing Python. This option is
       particularly useful for Windows users who cannot (or don’t want to)
       install software on their system.
    3. For Linux users Debian packages are available.
 These options are described in the following sub-sections.
@@ -201,18 +202,17 @@
 if [ -d "$HOME/.local/bin" ] ; then
     PATH="$HOME/.local/bin:$PATH"
 fi
 Save the file, log out of your session and then log in again. Open a command
 terminal and type:
 jpylyzer
 If all went well you now see this:
-usage: jpylyzer [-h] [--format FMT] [--legacyout] [--mix {1,2}] [--nopretty]
+usage: jpylyzer [-h] [--format FMT] [--mix {1,2}] [--nopretty]
           [--nullxml] [--recurse] [--packetmarkers] [--verbose]
-          [--version] [--wrapper]
-          jp2In [jp2In ...]
+          [--version] jp2In [jp2In ...]
 jpylyzer: error: the following arguments are required: jp2In
 Which means that the installation was successful!
 ******** GGlloobbaall iinnssttaallllaattiioonn ((LLiinnuuxx)) ********
 Simply enter:
 sudo -H pip install jpylyzer
 No further configuration is needed in this case.
 ******** NNoottee oonn pprree--rreelleeaasseess ********
@@ -228,18 +228,17 @@
 %jpylyzerPath%\jpylyzer
 In the above command, replace %%jjppyyllyyzzeerrPPaatthh%% with the full path to the jjppyyllyyzzeerr
 installation directory (i.e. the directory that contains ‘jpylyzer.exe’ and its
 associated files). For example, if you extracted the files to directory c:
 \tools\jpylyzer, the command would become:
 c:\tools\jpylyzer\jpylyzer
 Executing this command should result in the following screen output:
-usage: jpylyzer [-h] [--format FMT] [--legacyout] [--mix {1,2}] [--nopretty]
+usage: jpylyzer [-h] [--format FMT] [--mix {1,2}] [--nopretty]
           [--nullxml] [--recurse] [--packetmarkers] [--verbose]
-          [--version] [--wrapper]
-          jp2In [jp2In ...]
+          [--version] jp2In [jp2In ...]
 jpylyzer: error: the following arguments are required: jp2In
 ******** RRuunnnniinngg jjppyyllyyzzeerr wwiitthhoouutt ttyyppiinngg tthhee ffuullll ppaatthh ********
 Optionally, you may also want to add the full path of the jjppyyllyyzzeerr installation
 directory to the Windows ’Path’ environment variable. Doing so allows you to
 run jjppyyllyyzzeerr from any directory on your PC without having to type the full
 path. In Windows 7 you can do this by selecting ‘settings’ from the ‘Start’
 menu; then go to ‘control panel’/’system’ and go to the ‘advanced’ tab. Click
@@ -247,15 +246,15 @@
 the ‘system variables’ window, click on ‘Edit’ and add the full jjppyyllyyzzeerr path
 (this requires local Administrator privileges). The settings take effect on any
 newly opened command prompt.
 ********** IInnssttaallllaattiioonn ooff DDeebbiiaann ppaacckkaaggeess ((UUbbuunnttuu//LLiinnuuxx)) **********
 For Linux, Debian packages of jjppyyllyyzzeerr exist. To install, simply download the
 ..ddeebb file, double-click on it and select IInnssttaallll PPaacckkaaggee. Alternatively you can
 also do this in the command terminal by typing:
-sudo dpkg -i opf-jpylyzer_2.0.0_all.deb
+sudo dpkg -i opf-jpylyzer_2.2.0_all.deb
 In both cases you need to have administrative privileges.
 For UUbbuunnttuu and DDeebbiiaann alternative packages are available in the official
 release channels. To install simply run the following commands:
 sudo apt-get update
 sudo apt-get install python-jpylyzer
 ************ UUssiinngg jjppyyllyyzzeerr ************
 ********** OOvveerrvviieeww **********
@@ -271,42 +270,37 @@
 TThhiiss UUsseerr MMaannuuaall                      jjppyyllyyzzeerr
 Substitution example Linux            /home/jpylyzer/jpylyzer
 Substitution example Windows binaries c:\tools\jpylyzer\jpylyzer
 Furthermore, command line arguments that are given between square brackets
 (example: [-h]) are optional.
 ******** SSyynnooppssiiss ********
 JJppyyllyyzzeerr can be invoked using the following command-line arguments:
-usage: jpylyzer [-h] [--format FMT] [--legacyout] [--mix {1,2}] [--nopretty]
+usage: jpylyzer [-h] [--format FMT] [--mix {1,2}] [--nopretty]
           [--nullxml] [--recurse] [--packetmarkers] [--verbose]
-          [--version] [--wrapper]
-          jp2In [jp2In ...]
+          [--version] jp2In [jp2In ...]
 ****** PPoossiittiioonnaall aarrgguummeennttss ******
 AArrgguummeenntt DDeessccrriippttiioonn
-jp2In    input JP2 image(s), may be one or more (whitespace-separated) path
+jp2In    input image(s), may be one or more (whitespace-separated) path
          expressions; prefix wildcard (*) with backslash (\) in Linux
 ****** OOppttiioonnaall aarrgguummeennttss ******
 AArrgguummeenntt          DDeessccrriippttiioonn
 [-h, --help]      show help message and exit
-[--format FMT]    validation format; allowed values are jp2 (used by default)
-                  and j2c (which activates raw codestream validation)
+                  validation format; allowed values are jp2 (JPEG 2000 Part 1,
+[--format FMT]    used by default), j2c (Part 1 codestream), jph (JPEG 2000
+                  Part 15 / High Throughput JPEG 2000) and jhc (Part 15
+                  codestream)
 [--mix {1,2}]     report additional output in NISO MIX format (version 1.0 or
                   2.0)
-[--legacyout]     report output in jpylyzer 1.x format (provided for backward
-                  compatibility only)
 [--nopretty]      suppress pretty-printing of XML output
 [--nullxml]       extract null-terminated XML content from XML and UUID boxes
                   (doesn’t affect validation)
 [--recurse, -r]   when analysing a directory, recurse into subdirectories
-                  (implies --wrapper if --legacyout is used)
 [--packetmarkers] Report packet-level codestream markers (plm, ppm, plt, ppt)
 [--verbose]       report test results in verbose format
 [-v, --version]   show program’s version number and exit
-                  wrap output for individual image(s) in ‘results’ XML element
-[--wrapper, -w]   (deprecated from jpylyzer 2.x onward, only takes effect if --
-                  legacyout is used)
 Note that the input can either be a single image, a space-separated sequence of
 images, a pathname expression that includes multiple images, or any combination
 of the above. For example, the following command will process one single image:
 jpylyzer rubbish.jp2
 The next example shows how to process all files with a ‘jp2’ extension in the
 current directory:
 jpylyzer *.jp2
@@ -327,28 +321,29 @@
 The format of the XML output is described _h_e_r_e.
 ******** ?‘ffoorrmmaatt?’ ooppttiioonn ********
 By default, jjppyyllyyzzeerr validates against the JJPP22 format specification. Starting
 with version 2.0, jjppyyllyyzzeerr can also validate raw JPEG 2000 codestreams that are
 not wrapped inside a JJPP22 container. For codestream validation, use the --format
 option with value j2c, e.g.:
 jpylyzer --format j2c rubbish.j2c > rubbish.xml
+Starting with version 2.2, jjppyyllyyzzeerr also supports JPEG 2000 Part 15 (High
+Throughput JPEG 2000) and its JJPPHH container format. To validate a JJPPHH file, use
+the --format option with value jph:
+jpylyzer --format jph rubbish.jph > rubbish.xml
+And use --format with value jhc to validate a raw High Throughput codestream:
+jpylyzer --format jhc rubbish.jhc > rubbish.xml
 ******** ?‘mmiixx?’ ooppttiioonn ********
 When this option is used, jjppyyllyyzzeerr reports additional output in _NN_II_SS_OO_ _MM_II_XX
 format. This option takes one argument that defines whether MMIIXX 1.0 or MMIIXX 2.0
 is used. For example, the following command will result in MMIIXX 2.0 output:
 jpylyzer --mix 2 rubbish.jp2 > rubbish.xml
 The MMIIXX output is wrapped inside a ffiillee//pprrooppeerrttiieessEExxtteennssiioonn element. Note that
-MMIIXX output is oonnllyy written for files that are valid JP2 (files that are not
-valid result in an empty pprrooppeerrttiieessEExxtteennssiioonn element). Also, the --mix option
-is ignored if --format is set to j2c, or if --legacyout (see below) is used.
-******** ?‘lleeggaaccyyoouutt?’ ooppttiioonn ********
-The output format of jjppyyllyyzzeerr has changed in version 2.0, which may break
-existing workflows that expect output in 1.x format. For backward compatibility
-the --legacyout option results in output that follows the old 1.x format. Note
-that codestream validation is disabled if you use this option.
+MMIIXX output is oonnllyy written for files that are valid JP2 or JPH (files that are
+not valid result in an empty pprrooppeerrttiieessEExxtteennssiioonn element). Also, the --mix
+option is ignored if --format is set to j2c.
 ******** ?‘rreeccuurrssee?’ ooppttiioonn ********
 If the --recurse option is used, jjppyyllyyzzeerr will recursively traverse all
 subdirectories of a filepath expression. E.g:
 jpylyzer /home/myJP2s/*.jp2 > rubbish.xml
 In this case jjppyyllyyzzeerr analyses all files that have a ..jjpp22 extension in
 directory //hhoommee//mmyyJJPP22ss and all its subdirectories.
 ******** ?‘ppaacckkeettmmaarrkkeerrss?’ ooppttiioonn ********
@@ -356,44 +351,23 @@
 following packet-level codestream markers:
     * PLM (packet length, main header) marker
     * PPM (packed packet headers, main header) marker
     * PLT (packet length, tile-part header) marker
     * PPT (packed packet headers, tile-part header) marker
 By default these are excluded from the output, in order to prevent excessive
 output size.
-******** ?‘wwrraappppeerr?’ ooppttiioonn ((ddeepprreeccaatteedd)) ********
-This deprecated option is included for backward-compatibility, and only takes
-effect if --legacyout (see above) is used.By default, the jjppyyllyyzzeerr 1.x releases
-would create a separate XML tree for each analysed image, without any
-overarching hierarchy. For multiple-image pathname expressions this resulted in
-output that was nnoott well-formed XML. The --legacyout option still results in
-this is behaviour. For example:
-jpylyzer --legacyout rubbish.jp2 garbage.jp2 > rubbish.xml
-In this case, the file ‘rubbish.xml’ contains a succession of two XML trees,
-which by itself is not well-formed XML. The --wrapper option is provided to
-create valid XML instead:
-jpylyzer --legacyout --wrapper rubbish.jp2 garbage.jp2 > rubbish.xml
-In the above case the XML trees of the individual images are wrapped inside a
-‘results’ element. When the --recurse option is used, jpylyzer will
-automatically wrap the output in a ‘results’ element, so there’s no need to
-specify --wrapper in that case.
-Starting with version 2.0, jjppyyllyyzzeerr aallwwaayyss generates well-formed XML (unless
-the --legacyout option is used), which makes the --wrapper option largely
-obsolete, apart from cases where the ‘old’ behaviour is needed for backward-
-compatibility reasons.
 ******** ?‘nnuullllxxmmll?’ ooppttiioonn ********
 The nnuullllxxmmll option was added to enable extraction of XML content that is
 terminated by a null-byte. By default jjppyyllyyzzeerr doesn’t report the XML in that
 case, because it throws an exception in the XML parser. Apparently some old
 versions of the Kakadu demo applications would erroneously add a null-byte to
 embedded XML, so this option can be used to force extraction for images that
 are affected by this.
 ******** UUsseerr wwaarrnniinnggss ********
-Under the following conditions jjppyyllyyzzeerr will print a user warning to the
-standard error device (typically the console screen):
+Under the following conditions jjppyyllyyzzeerr will report a user warning:
 ****** NNoo iimmaaggeess ttoo cchheecckk ******
 If there are no input images to check (typically because the value of jp2In
 refers to a non-existent file), the following warning message is shown:
 User warning: no images to check!
 ****** UUnnssuuppppoorrtteedd bbooxx ******
 In some cases you will see the following warning message:
 User warning: ignoring 'boxName' (validator function not yet implemented)
@@ -423,23 +397,26 @@
 ****** UUnnkknnoowwnn bbooxx ******
 Occasionally, you may see this warning message:
 User warning: ignoring unknown box
 This happens if jjppyyllyyzzeerr encounters a box that is not defined by JPEG 2000 Part
 1. It should be noted that, to a large extent, JPEG 2000 Part 1 permits the
 presence of boxes that are defined outside the standard. Again, jjppyyllyyzzeerr will
 simply ignore these and process all other boxes normally.
+All user warnings are printed to the standard error device (typically the
+console screen). File-level warnings are also written to the wwaarrnniinnggss output
+element.
 ********** UUssiinngg jjppyyllyyzzeerr aass aa PPyytthhoonn mmoodduullee **********
 Instead of using jjppyyllyyzzeerr from the command-line, you can also import it as a
 module in your own Python programs. To do so, install jpylyzer with ppiipp. Then
 import jjppyyllyyzzeerr into your code by adding:
 from jpylyzer import jpylyzer
 Subsequently you can call any function that is defined in jjppyyllyyzzeerr..ppyy. In
 practice you will most likely only need the cchheecckkOOnneeFFiillee function. The
 following minimal script shows how this works:
-#! /usr/bin/env python
+#! /usr/bin/env python3
 
 from jpylyzer import jpylyzer
 
 # Define JP2
 myFile = "/home/johan/jpylyzer-test-files/aware.jp2"
 
 # Analyse with jpylyzer, result to Element object
@@ -448,23 +425,35 @@
 # Return image height value
 imageHeight = myResult.findtext('./properties/jp2HeaderBox/imageHeaderBox/
 height')
 print(imageHeight)
 Here, mmyyRReessuulltt is an EElleemmeenntt object that can either be used directly, or
 converted to XML using the EElleemmeennttTTrreeee module_2. The structure of the element
 object follows the XML output that described _h_e_r_e.
-For validation a raw JPEG 2000 codestreams, call the cchheecckkOOnneeFFiillee function with
-the additional vvaalliiddaattiioonnFFoorrmmaatt argument, and set it to j2c:
+You may use the following optional arguments (which correspond to the command-
+line options explained above):
+    * validationFormat - sets the validation format. Values: ‘jp2’ (default),
+      ‘jph’, ‘j2c’ or ‘jhc’.
+    * verboseFlag - report test results in verbose format. Values: False
+      (default) or True.
+    * packetmarkersFlag - report packet-level codestream markers. Values: False
+      (default) or True.
+    * nullxmlFlag - extract null-terminated XML content from XML and UUID
+      boxes. Values: False (default) or True.
+    * mixFlag - report additional output in NISO MIX format (version 1.0 or
+      2.0). Values: 0 (default), 1 or 2.
+As an example, for validating a raw JPEG 2000 codestream, call the cchheecckkOOnneeFFiillee
+function with the additional vvaalliiddaattiioonnFFoorrmmaatt argument, and set it to j2c:
 # Define Codestream
 myFile = "/home/johan/jpylyzer-test-files/rubbish.j2c"
 
 # Analyse with jpylyzer, result to Element object
 myResult = jpylyzer.checkOneFile(myFile, 'j2c')
 ********** JJaavvaa iinntteeggrraattiioonn **********
-It is possible to integrate jjppyyllyyzzeerr into Java applications. A test class that
+It is possible to integrate jjppyyllyyzzeerr into Java applications_3. A test class that
 shows how this works is included in the source repo _h_e_r_e. This requires _J_y_t_h_o_n.
 Note that you may run into performance issues with (very) large images in this
 case, as Jython does not support _m_e_m_o_r_y_ _m_a_p_p_i_n_g, so make sure you’ve got plenty
 of RAM available.
 ************ SSttrruuccttuurree ooff aa JJPP22 ffiillee ************
 ********** SSccooppee ooff tthhiiss sseeccttiioonn **********
 This section gives a brief overview of the JP2 file format. A basic
@@ -602,14 +591,15 @@
    2. ssttaattuussIInnffoo: information about the status of jjppyyllyyzzeerr’s validation attempt
    3. iissVVaalliidd: outcome of the validation
    4. tteessttss: outcome of the individual tests that are part of the validation
       process (organised by box)
    5. pprrooppeerrttiieess: image properties (organised by box)
    6. pprrooppeerrttiieessEExxtteennssiioonn: wrapper element for NISO MMIIXX output (only if the --
       mix option is used)
+   7. wwaarrnniinnggss: reported warnings
 ********** ffiilleeIInnffoo eelleemmeenntt **********
 This element holds general information about the analysed file. Currently it
 contains the following sub-elements:
     * ffiilleennaammee: name of the analysed file without its path (e.g. “rubbish.jp2”)
     * ffiilleePPaatthh: name of the analysed file, including its full absolute path
       (e.g. “d:\data\images\rubbish.jp2”)
     * ffiilleeSSiizzeeIInnBByytteess: file size in bytes
@@ -648,23 +638,30 @@
 If a file passed aallll tests, this is an indication that it is most likely valid
 JP2. In that case, the _ii_ss_VV_aa_ll_ii_dd_ _e_l_e_m_e_n_t has a value of “True” (and “False” in
 all other cases). These tests are all explained _h_e_r_e and _h_e_r_e.
 ******** DDeeffaauulltt aanndd vveerrbboossee rreeppoorrttiinngg ooff tteesstt rreessuullttss ********
 By default, jjppyyllyyzzeerr only reports any tests that failed (i.e. returned
 “False”), including the corresponding part of the box structure. For a valid
 JP2 the tests element will be empty. If the –verbose flag is used, the results
-of aallll tests are included (including those that returned “True”)_3.
+of aallll tests are included (including those that returned “True”)_4.
 ********** pprrooppeerrttiieess eelleemmeenntt **********
 This element contains the extracted image properties, which are organised in a
 hierarchical tree that corresponds to JP2’s box structure. See _h_e_r_e and _h_e_r_e
 for a description of the reported properties.
 ********** pprrooppeerrttiieessEExxtteennssiioonn eelleemmeenntt **********
 This optional element is reserved for output in alternative formats. Currently
 it is used to wrap output in NISO MMIIXX format if the --mix option is used. See
 the _MM_II_XX_ _d_o_c_u_m_e_n_t_a_t_i_o_n for a description of the reported elements.
+********** wwaarrnniinnggss eelleemmeenntt **********
+This element is reserved for reporting any warnings that are not directly
+related to the validation process. Examples are:
+    * Jpylyzer encountered an unknown box type while parsing a file.
+    * Reading of a file failed because of system limitations.
+Each warning is wrapped in a ‘warning’ element. The results are organised in a
+hierarchical tree that corresponds to JP2’s box structure.
 ************ JJPP22:: bbooxx bbyy bbooxx ************
 The following two sections provide a detailed explanation of jjppyyllyyzzeerr’s
 functionality and its output. In particular, the following two aspects are
 addressed:
    1. The reported properties
    2. The tests that jjppyyllyyzzeerr performs to establish the validity of a file.
 ********** AAbboouutt tthhee pprrooppeerrttiieess aanndd tteessttss ttrreeeess **********
@@ -715,18 +712,20 @@
 PPrrooppeerrttyy DDeessccrriippttiioonn
 br       Brand
 minV     Minor version
 cL*      Compatibility field (repeatable)
 ******** TTeessttss ********
 TTeesstt nnaammee                TTrruuee iiff
 boxLengthIsValid         (Size of box – 8) /4 is a whole number (integer)
-brandIsValid             bbrr equals 0x6a703220 (“jp2”)
+brandIsValid             bbrr equals 0x6a703220 (“jp2”) for JP2, or 0x6a706820
+                         (“jph”)for JPH
 minorVersionIsValid      mmiinnVV equals 0
-compatibilityListIsValid Sequence of compatibility (ccLL) fields includes one
-                         entry that equals 0x6a703220 (“jp2”)
+                         Sequence of compatibility (ccLL) fields includes one
+compatibilityListIsValid entry that equals 0x6a703220 (“jp2”) for JP2, or
+                         0x6a706820 (“jph”)for JPH
 ********** JJPP22 HHeeaaddeerr bbooxx ((ssuuppeerrbbooxx)) **********
 This box is a superbox that holds a series of boxes that contain header-type
 information about the file.
 ******** EElleemmeenntt nnaammee ********
 jp2HeaderBox
 ******** RReeppoorrtteedd pprrooppeerrttiieess ********
 Since this is a superbox, it contains a number of child boxes. These are
@@ -767,14 +766,18 @@
 colourSpecificationBoxesAreContiguous       Specification boxes, they appear
                                             contiguously in the JP2 Header box
                                             Box contains a Palette box (only if
                                             Component Mapping box is present);
 paletteAndComponentMappingBoxesOnlyTogether box contains a Component Mapping
                                             box (only if Palette box is
                                             present)
+                                            If file does not contain a Colour
+noZeroCTypesIfNoColourBox                   Specification Box, no cTyp values
+                                            (from Channel definition box) shall
+                                            be equal to 0 (JPH)
 ********** IImmaaggee HHeeaaddeerr bbooxx ((cchhiilldd ooff JJPP22 HHeeaaddeerr bbooxx)) **********
 This box specifies the size of the image and other related fields.
 ******** EElleemmeenntt nnaammee ********
 imageHeaderBox
 ******** RReeppoorrtteedd pprrooppeerrttiieess ********
 PPrrooppeerrttyy DDeessccrriippttiioonn
 height   Image height in pixels
@@ -813,24 +816,34 @@
 bPCIsValid* bbPPCCDDeepptthh is within range [1,38] (repeated for all components)
 ********** CCoolloouurr SSppeecciiffiiccaattiioonn bbooxx ((cchhiilldd ooff JJPP22 HHeeaaddeerr bbooxx)) **********
 This box specifies the colourspace of the image.
 ******** EElleemmeenntt nnaammee ********
 colourSpecificationBox
 ******** RReeppoorrtteedd pprrooppeerrttiieess ********
 PPrrooppeerrttyy                                DDeessccrriippttiioonn
-                                        Specification method. Indicates whether
-meth                                    colourspace of this image is defined as
-                                        an enumerated colourspace or using a
-                                        (restricted) ICC profile.
+                                        Specification method. Indicates how the
+                                        colourspace is defined (enumerated
+meth                                    colourspace, or restricted ICC profile
+                                        for JP2, with additional Any ICC and
+                                        Parameterized Colourspace methods for
+                                        JPH.
 prec                                    Precedence
 approx                                  Colourspace approximation
 enumCS (if meth equals “Enumerated”)    Enumerated colourspace (as descriptive
                                         text string)
 icc (if meth equals “Restricted ICC” or Properties of ICC profile as child
-“Any ICC”_4)                             element (see below)
+“Any ICC”)                              element (see below)
+colPrims (if meth equals “Parameterized ColourPrimaries value (JPH)_5.
+Colourspace”)
+transfC (if meth equals “Parameterized  TransferCharacteristics value (JPH)_6
+Colourspace”)
+matCoeffs (if meth equals               MatrixCoefficients value (JPH)_7
+“Parameterized Colourspace”)
+vidFRng (if meth equals “Parameterized  VideoFullRangeFlag (“yes”/”no”) (JPH)_8
+Colourspace”)
 ******** RReeppoorrtteedd pprrooppeerrttiieess ooff IICCCC pprrooffiilleess ********
 If the colour specification box contains an embedded ICC profile, jjppyyllyyzzeerr will
 also report the following properties (which are all grouped in an “icc” sub-
 element in the properties tree). An exhaustive explanation of these properties
 is given in the ICC specification (ISO 15076-1 / ICC.1:2004-10). Note that
 jjppyyllyyzzeerr does nnoott validate embedded ICC profiles (even though it does check if
 a specific ICC profile is allowed in JP2)!
@@ -879,17 +892,23 @@
 approxIsValid                        aapppprrooxx equals 0
 enumCSIsValid (if meth equals        eennuummCCSS equals 16 (“sRGB”), 17
 “Enumerated”)                        (“greyscale”) or 18 (“sYCC”)
 iccSizeIsValid (if meth equals       Actual size of embedded ICC profile
 “Restricted ICC”)                    equals value of profileSize field in ICC
                                      header
 iccPermittedProfileClass (if meth    ICC profile class is “input device” or
-equals “Restricted ICC”)             “display device”_5
+equals “Restricted ICC”)             “display device”_9
 iccNoLUTBasedProfile (if meth equals ICC profile type is not N-component LUT
 “Restricted ICC”)                    based (which is not allowed in JP2)
+colPrimsIsValid                      ccoollPPrriimmss value is defined by ITU-T H.273
+                                     / ISO/IEC 23001-8 (JPH)
+transfCIsValid                       ttrraannssffCC value is defined by ITU-T H.273
+                                     / ISO/IEC 23001-8 (JPH)
+matCoeffsIsValid                     mmaattCCooeeffffss value is defined by ITU-
+                                     T H.273 / ISO/IEC 23001-8 (JPH)
 ********** PPaalleettttee bbooxx ((cchhiilldd ooff JJPP22 HHeeaaddeerr bbooxx)) **********
 This (optional) box specifies the palette which maps a single component in
 index space to a multiple-component image.
 ******** EElleemmeenntt nnaammee ********
 paletteBox
 ******** RReeppoorrtteedd pprrooppeerrttiieess ********
 PPrrooppeerrttyy DDeessccrriippttiioonn
@@ -930,20 +949,26 @@
 ******** RReeppoorrtteedd pprrooppeerrttiieess ********
 PPrrooppeerrttyy DDeessccrriippttiioonn
 n        Number of channel descriptions
 cN*      Channel index (repeated for all channels)
 cTyp*    Channel type (repeated for all channels)
 cAssoc*  Channel association (repeated for all channels)
 ******** TTeessttss ********
-TTeesstt nnaammee        TTrruuee iiff
-nIsValid         nn is within range [1, 65535]
-boxLengthIsValid (Size of box – 2) / equals 6*nn
-cNIsValid*       ccNN is within range [0, 65535] (repeated for all channels)
-cTypIsValid*     ccTTyyppee is within range [0, 65535] (repeated for all channels)
-cAssocIsValid*   ccAAssssoocc is within range [0, 65535] (repeated for all channels)
+TTeesstt nnaammee                 TTrruuee iiff
+nIsValid                  nn is within range [1, 65535]
+boxLengthIsValid          (Size of box – 2) / equals 6*nn
+cNIsValid*                ccNN is within range [0, 65535] (repeated for all
+                          channels)
+cTypIsValid*              ccTTyyppee is one of the values defined in Table I.16
+                          (repeated for all channels)_1_0
+cAssocIsValid*            ccAAssssoocc is within range [0, 65535] (repeated for all
+                          channels)
+noMoreThanOneAlphaChannel At most one ccTTyypp field is equal to 1 or 2 (JPH)
+cAssocAlphaChannelIsZero  If ccTTyypp is 1 or 2, the corresponding ccAAssssoocc value
+                          equals 0 (JPH)
 ********** RReessoolluuttiioonn bbooxx ((cchhiilldd ooff JJPP22 HHeeaaddeerr bbooxx,, ssuuppeerrbbooxx)) **********
 This (optional) box contains the grid resolution.
 ******** EElleemmeenntt nnaammee ********
 resolutionBox
 ******** RReeppoorrtteedd pprrooppeerrttiieess ********
 Since this is a superbox, it contains one or two child boxes. These are
 represented as child elements in the properties tree:
@@ -972,19 +997,20 @@
 PPrrooppeerrttyy              DDeessccrriippttiioonn
 vRcN                  Vertical grid resolution numerator
 vRcD                  Vertical grid resolution denominator
 hRcN                  Horizontal grid resolution numerator
 hRcD                  Horizontal grid resolution denominator
 vRcE                  Vertical grid resolution exponent
 hRcE                  Horizontal grid resolution exponent
-vRescInPixelsPerMeter Vertical grid resolution, expressed in pixels per meter_6
+vRescInPixelsPerMeter Vertical grid resolution, expressed in pixels per meter_1_1
 hRescInPixelsPerMeter Horizontal grid resolution, expressed in pixels per
-                      meter_7
-vRescInPixelsPerInch  Vertical grid resolution, expressed in pixels per inch_8
-hRescInPixelsPerInch  Horizontal grid resolution, expressed in pixels per inch_9
+                      meter_1_2
+vRescInPixelsPerInch  Vertical grid resolution, expressed in pixels per inch_1_3
+hRescInPixelsPerInch  Horizontal grid resolution, expressed in pixels per
+                      inch_1_4
 ******** TTeessttss ********
 TTeesstt nnaammee        TTrruuee iiff
 boxLengthIsValid Size of box contents equals 10 bytes
 vRcNIsValid      vvRRccNN is within range [1,65535]
 vRcDIsValid      vvRRccDD is within range [1,65535]
 hRcNIsValid      hhRRccNN is within range [1,65535]
 hRcDIsValid      hhRRccDD is within range [1,65535]
@@ -1003,20 +1029,20 @@
 PPrrooppeerrttyy              DDeessccrriippttiioonn
 vRdN                  Vertical grid resolution numerator
 vRdD                  Vertical grid resolution denominator
 hRdN                  Horizontal grid resolution numerator
 hRdD                  Horizontal grid resolution denominator
 vRdE                  Vertical grid resolution exponent
 hRdE                  Horizontal grid resolution exponent
-vResdInPixelsPerMeter Vertical grid resolution, expressed in pixels per meter_1_0
+vResdInPixelsPerMeter Vertical grid resolution, expressed in pixels per meter_1_5
 hResdInPixelsPerMeter Horizontal grid resolution, expressed in pixels per
-                      meter_1_1
-vResdInPixelsPerInch  Vertical grid resolution, expressed in pixels per inch_1_2
+                      meter_1_6
+vResdInPixelsPerInch  Vertical grid resolution, expressed in pixels per inch_1_7
 hResdInPixelsPerInch  Horizontal grid resolution, expressed in pixels per
-                      inch_1_3
+                      inch_1_8
 ******** TTeessttss ********
 TTeesstt nnaammee        TTrruuee iiff
 boxLengthIsValid Size of box contents equals 10 bytes
 vRdNIsValid      vvRRddNN is within range [1,65535]
 vRdDIsValid      vvRRddDD is within range [1,65535]
 hRdNIsValid      hhRRddNN is within range [1,65535]
 hRdDIsValid      hhRRddDD is within range [1,65535]
@@ -1049,15 +1075,15 @@
 Note that jjppyyllyyzzeerr does not check whether the XML is vvaalliidd, as this is not
 required by the standard. Besides, doing so would make jjppyyllyyzzeerr significantly
 slower for XML that contains references to external schemas and DTDs.
 ********** UUUUIIDD bbooxx **********
 This (optional) box contains additional (binary) information, which may be
 vendor-specific. Some applications (e.g. Kakadu and ExifTool) also use this box
 for storing XMP metadata (see Section 1.1.4 in Part 3 of the XMP
-specification_1_4).
+specification_1_9).
 ******** EElleemmeenntt nnaammee ********
 uuidBox
 ******** RReeppoorrtteedd pprrooppeerrttiieess ********
 If the value of uuuuiidd indicates the presence of XMP metadata and the contents of
 this box are well-formed XML, (see ‘tests’ below), the ‘uuidBox’ element in the
 properties tree will contain the XMP data. Note that, depending on the
 character encoding of the original XML, it may contain characters that are not
@@ -1294,17 +1320,17 @@
 supported at this stage: if jjppyyllyyzzeerr encounters them, it will include the
 corresponding element in the pprrooppeerrttiieess element of the output. However,
 jjppyyllyyzzeerr does not analyse the contents of these marker segments, which means
 that the respective elements in the output will be empty.
 ******** BBiitt ssttrreeaammss ********
 In addition to the above limitations, jjppyyllyyzzeerr can nnoott be used to establish
 whether the data in the bitstream are correct (this would require decoding the
-compressed image data, which is completely out of jjppyyllyyzzeerr’s scope)_1_5. As a
+compressed image data, which is completely out of jjppyyllyyzzeerr’s scope)_2_0. As a
 result, if jjppyyllyyzzeerr is used as part of a quality assurance workflow, it is
-recommended to also include an additional check on the image contents_1_6. Also,
+recommended to also include an additional check on the image contents_2_1. Also,
 jjppyyllyyzzeerr does not perform any checks on marker segments within the bit-stream:
 start-of packet (SOP) and end-of-packet (EPH) markers.
 ******** DDeetteeccttiioonn ooff iinnccoommpplleettee oorr ttrruunnccaatteedd ccooddeessttrreeaammss ********
 A JP2’s tile part header contains information that makes it possible to detect
 incomplete and truncated codestreams in most cases. Depending on the encoder
 software used, this method may fail for images that only contain one single
 tile part (i.e. images that do not contain tiling).
@@ -1360,66 +1386,76 @@
 ppmCount Number of PPM markers in main header
 ******** TTeessttss ********
 TTeesstt nnaammee                      TTrruuee iiff
 codestreamStartsWithSOCMarker  First 2 bytes in codestream constitute a start
                                of codestream (SOC) marker segment
 foundSIZMarker                 Second marker segment in codestream is image and
                                tile size (SIZ) marker segment
+                               Codestream main header contains Extended
+foundCAPMarker                 Capabilities (CAP) marker segment if second most
+                               significant bit of rrssiizz equals 1
 foundCODMarker                 Codestream main header contains coding style
                                default (COD) marker segment
 foundQCDMarker                 Codestream main header contains quantization
                                default (QCD) marker segment
+                               Value of CCPPFFnnuumm in CPF marker segment is
+CPFnumConsistentWithPRFnum     consistent with PPRRFFnnuumm value in PRF marker
+                               segment
+                               Value of CCPPFFnnuumm in CPF marker segment is
+CPFnumConsistentWithRsiz       consistent with *rsiz^ value in SIZ marker
+                               segment
                                Number of encountered tiles is consistent with
 foundExpectedNumberOfTiles     expected number of tiles (as calculated from _S_I_Z
                                _m_a_r_k_e_r)
                                For all tiles, number of encountered tile parts
 foundExpectedNumberOfTileParts is consistent with expected number of tile parts
                                (values of ttnnssoott from _S_O_T_ _m_a_r_k_e_r)
                                No more than one ccccoocc value for each component
-maxOneCcocPerComponent         (only reported if codestream contains any COC
-                               marker segments)
+maxOneCcocPerComponentMain     in main header (only reported if codestream
+                               contains any COC marker segments)
                                No more than one ccqqcccc value for each component
-maxOneCqccPerComponent         (only reported if codestream contains any QCC
-                               marker segments)
+maxOneCqccPerComponentMain     in main header (only reported if codestream
+                               contains any QCC marker segments)
 foundEOCMarker                 Last 2 bytes in codestream constitute an end of
                                codestream (EOC) marker segment
 ********** IImmaaggee aanndd ttiillee ssiizzee ((SSIIZZ)) mmaarrkkeerr sseeggmmeenntt ((cchhiilldd ooff CCoonnttiigguuoouuss CCooddeessttrreeaamm
 bbooxx)) **********
 ******** EElleemmeenntt nnaammee ********
 siz
 ******** RReeppoorrtteedd pprrooppeerrttiieess ********
 PPrrooppeerrttyy      DDeessccrriippttiioonn
 lsiz          Length of SIZ marker segment in bytes
-rsiz          Decoder capabilities
+rsiz          Numerical value of rrssiizz (capabilities) field
+capability    Capabilities (profile) encoded by rrssiizz value
 xsiz          Width of reference grid
 ysiz          Height of reference grid
 xOsiz         Horizontal offset from origin of reference grid to left of image
               area
 yOsiz         Vertical offset from origin of reference grid to top of image
               area
 xTsiz         Width of one reference tile with respect to the reference grid
 yTsiz         Height of one reference tile with respect to the reference grid
 xTOsiz        Horizontal offset from origin of reference grid to left side of
               first tile
 yTOsiz        Vertical offset from origin of reference grid to top side of
               first tile
-numberOfTiles Number of tiles_1_7
+numberOfTiles Number of tiles_2_2
 csiz          Number of components
 ssizSign*     Indicates whether image component is signed or unsigned (repeated
               for all components)
 ssizDepth*    Number of bits for this component (repeated for all components)
 xRsiz*        Horizontal separation of sample of this component with respect to
               reference grid (repeated for all components)
 yRsiz*        Vertical separation of sample of this component with respect to
               reference grid (repeated for all components)
 ******** TTeessttss ********
 TTeesstt nnaammee              TTrruuee iiff
 lsizIsValid            llssiizz is within range [41,49190]
-rsizIsValid            rrssiizz equals 0 (“ISO/IEC 15444-1”), 1 (“Profile 0”) or 2
-                       (“Profile 1”)
+rsizIsValid            Four most significant bits of rrssiizz are 0 (JP2, J2C);
+                       second most significant bit of rrssiizz equals 1 (JPH, JHC)
 xsizIsValid            xxssiizz is within range [1,232 - 1]
 ysizIsValid            yyssiizz is within range [1,232 - 1]
 xOsizIsValid           xxOOssiizz is within range [0,232 - 2]
 yOsizIsValid           yyOOssiizz is within range [0,232 - 2]
 xTsizIsValid           xxTTssiizz is within range [1,232 - 1]
 yTsizIsValid           yyTTssiizz is within range [1,232 - 1]
 xTOsizIsValid          xxTTOOssiizz is within range [0,232 - 2]
@@ -1448,23 +1484,26 @@
 layers                          Number of layers
 multipleComponentTransformation Indicates use of multiple component
                                 transformation (“yes”/“no”)
 levels                          Number of decomposition levels
 codeBlockWidth                  Code block width
 codeBlockHeight                 Code block height
 codingBypass                    Indicates use of coding bypass (“yes”/“no”)
-resetOnBoundaries               Indicates reset of context probabilities on
-                                coding pass boundaries (“yes”/“no”)
+                                Indicates reset of context probabilities on
+resetOnBoundaries               coding pass boundaries (“yes”/“no”) (does not
+                                apply to High Throughput code blocks)
 termOnEachPass                  Indicates termination on each coding pass
                                 (“yes”/“no”)
 vertCausalContext               Indicates vertically causal context (“yes”/
                                 “no”)
 predTermination                 Indicates predictable termination (“yes”/“no”)
-segmentationSymbols             Indicates use of segmentation symbols (“yes”/
-                                “no”)
+                                (does not apply to High Throughput code blocks)
+                                Indicates use of segmentation symbols (“yes”/
+segmentationSymbols             “no”) (does not apply to High Throughput code
+                                blocks)
 transformation                  Wavelet transformation: “9-7 irreversible” or
                                 “5-3 reversible”
                                 Precinct width (repeated for all resolution
 precinctSizeX*                  levels; order: low to high). Equals 32768 if
                                 pprreecciinnccttss is “default”
                                 Precinct height (repeated for all resolution
 precinctSizeY*                  levels; order: low to high). Equals 32768 if
@@ -1547,15 +1586,16 @@
 roiShift Implicit ROI shift
 ******** TTeessttss ********
 TTeesstt nnaammee       TTrruuee iiff
 lrgnIsValid     llrrggnn is within range [5,6]
 crgnIsValid     ccrrggnn is within range [0,255] (ccssiizz < 257) or [0,16383] (ccssiizz >=
                 257)
 roiStyleIsValid rrooiiSSttyyllee equals 0 (“Implicit ROI (maximum shift)”)
-roiShiftIsValid rrooiiSShhiifftt is within range [0,255]
+roiShiftIsValid rrooiiSShhiifftt is within range [0,255] (JP2, J2C) or [0,37] (JPH,
+                JHC)
 ********** QQuuaannttiizzaattiioonn ddeeffaauulltt ((QQCCDD)) mmaarrkkeerr sseeggmmeenntt **********
 ******** EElleemmeenntt nnaammee ********
 qcd
 ******** RReeppoorrtteedd pprrooppeerrttiieess ********
 PPrrooppeerrttyy  DDeessccrriippttiioonn
 lqcd      Length of QCD marker segment in bytes
 qStyle    Quantization style for all components
@@ -1664,14 +1704,58 @@
 comment  Embedded comment as text (only if rrccoomm = 1 )
 ******** TTeessttss ********
 TTeesstt nnaammee      TTrruuee iiff
 lcomIsValid    llqqccdd is within range [5,65535]
 rcomIsValid    rrccoomm equals 0 (“binary”) or 1 (“ISO/IEC 8859-15 (Latin”))
 commentIsValid Comment is valid ISO/IEC8859-15 and does not contain control
                characters, other than tab, newline or carriage return
+********** EExxtteennddeedd ccaappaabbiilliittiieess ((CCAAPP)) mmaarrkkeerr sseeggmmeenntt **********
+This marker segment is defined in ISO/IEC 15444-2, and is used by ISO/IEC
+15444-15 (as well as other parts of the standard).
+******** EElleemmeenntt nnaammee ********
+cap
+******** RReeppoorrtteedd pprrooppeerrttiieess ********
+PPrrooppeerrttyy      DDeessccrriippttiioonn
+lcap          Length of CAP marker segment in bytes
+pcapPart      Indicates the use of capabilities from Part ppccaappPPaarrtt of the ISO/
+              IEC 15444 standard (repeated for all referenced parts)
+htCodeBlocks  See section 8.2 of ISO/IEC 15444-15 (JPH, JHC)
+htSets        See section 8.3 of ISO/IEC 15444-15 (JPH, JHC)
+htRegion      See section 8.4 of ISO/IEC 15444-15 (JPH, JHC)
+htHomogeneous See section 8.5 of ISO/IEC 15444-15 (JPH, JHC)
+htReversible  See section 8.7.2 of ISO/IEC 15444-15 (JPH, JHC)
+htB           Parameter BB as used in MMAAGGBBPP sets, see sections A.3.7 and 8.7.3
+              of ISO/IEC 15444-15 (JPH, JHC)
+******** TTeessttss ********
+TTeesstt nnaammee     TTrruuee iiff
+lcapIsValid   Number of ppccaappPPaarrtt entries equals (llccaapp - 6)/2
+pcap15IsValid 15th most significant bit of ppccaapp equals 1 (JPH, JHC)
+********** PPrrooffiillee ((PPRRFF)) mmaarrkkeerr sseeggmmeenntt **********
+******** EElleemmeenntt nnaammee ********
+prf
+******** RReeppoorrtteedd pprrooppeerrttiieess ********
+PPrrooppeerrttyy DDeessccrriippttiioonn
+lprf     Length of PRF marker segment in bytes
+PRFnum   Profile number
+******** TTeessttss ********
+TTeesstt nnaammee     TTrruuee iiff
+lprfIsValid   llpprrff is within range [4,65534]
+pprfIsValid   last pppprrff value is not zero
+PRFnumIsValid PPRRFFnnuumm > 4095
+********** CCoorrrreessppoonnddiinngg pprrooffiillee ((CCPPFF)) mmaarrkkeerr sseeggmmeenntt **********
+******** EElleemmeenntt nnaammee ********
+cpf
+******** RReeppoorrtteedd pprrooppeerrttiieess ********
+PPrrooppeerrttyy DDeessccrriippttiioonn
+lcpf     Length of CPF marker segment in bytes
+CPFnum   Profile number
+******** TTeessttss ********
+TTeesstt nnaammee   TTrruuee iiff
+lcpfIsValid llccppff is within range [4,65534] (JPH, JHC)
+pcpfIsValid last ppccppff value is not zero (JPH, JHC)
 ********** TTiillee ppaarrtt ((cchhiilldd ooff CCoonnttiigguuoouuss CCooddeessttrreeaamm bbooxx)) **********
 Tile-part level properties and tests. This is not a box or a marker segment!
 ******** EElleemmeenntt nnaammee ********
 tilePart (child of tileParts)
 ******** RReeppoorrtteedd pprrooppeerrttiieess ********
 Each tile part element can contain a number of child elements:
 CChhiilldd eelleemmeenntt DDeessccrriippttiioonn
@@ -1698,20 +1782,36 @@
 option is used. The number of PLT and PPT markers is given by the following 2
 derived properties (these are always reported, irrespective of --
 packetmarkers):
 PPrrooppeerrttyy DDeessccrriippttiioonn
 pltCount Number of PLT markers in tile part header
 pptCount Number of PPT markers in tile part header
 ******** TTeessttss ********
-TTeesstt nnaammee              TTrruuee iiff
-                       Tile part start offset + ttiilleePPaarrttLLeennggtthh points to either
-foundNextTilePartOrEOC start of new tile or EOC marker (useful for detecting
-                       within-codestream byte corruption)
-foundSODMarker         Last marker segment of tile part is a start-of-data
-                       (SOD) marker
+TTeesstt nnaammee                TTrruuee iiff
+CODAllowed               COD marker is allowed in this tile part (only allowed
+                         in first tile-part of a tile)
+COCAllowed               COC marker is allowed in this tile part (only allowed
+                         in first tile-part of a tile)
+QCDAllowed               QCD marker is allowed in this tile part (only allowed
+                         in first tile-part of a tile)
+QCCAllowed               QCC marker is allowed in this tile part (only allowed
+                         in first tile-part of a tile)
+RGNAllowed               RGN marker is allowed in this tile part (only allowed
+                         in first tile-part of a tile)
+                         No more than one ccccoocc value for each component in
+maxOneCcocPerComponentTP tile-part header (only reported if codestream contains
+                         any COC marker segments)
+                         No more than one ccqqcccc value for each component in
+maxOneCqccPerComponentTP tile-part header (only reported if codestream contains
+                         any QCC marker segments)
+                         Tile part start offset + ttiilleePPaarrttLLeennggtthh points to
+foundNextTilePartOrEOC   either start of new tile or EOC marker (useful for
+                         detecting within-codestream byte corruption)
+foundSODMarker           Last marker segment of tile part is a start-of-data
+                         (SOD) marker
 ********** SSttaarrtt ooff ttiillee ppaarrtt ((SSOOTT)) mmaarrkkeerr sseeggmmeenntt ((cchhiilldd ooff ttiillee ppaarrtt)) **********
 ******** EElleemmeenntt nnaammee ********
 sot
 ******** RReeppoorrtteedd pprrooppeerrttiieess ********
 PPrrooppeerrttyy DDeessccrriippttiioonn
 lsot     Length of SOT marker segment in bytes
 isot     Tile index
@@ -1737,44 +1837,44 @@
 ******** RReeppoorrtteedd pprrooppeerrttiieess ********
 PPrrooppeerrttyy DDeessccrriippttiioonn
 ******** TTeessttss ********
 TTeesstt nnaammee TTrruuee iiff
 ********** PPaacckkeett lleennggtthh,, mmaaiinn hheeaaddeerr ((PPLLMM)) mmaarrkkeerr sseeggmmeenntt **********
 ******** EElleemmeenntt nnaammee ********
 plm
-******** RReeppoorrtteedd pprrooppeerrttiieess_11_88 ********
+******** RReeppoorrtteedd pprrooppeerrttiieess_22_33 ********
 PPrrooppeerrttyy DDeessccrriippttiioonn
 lplm     Length of PLM marker segment in bytes
 zplm     PLM marker segment index
 nplm     Number of bytes of Iplm information for the ith tile-part
 iplm     Comma separated list of packet length values (as hexadecimal strings)
 ******** TTeessttss ********
 TTeesstt nnaammee TTrruuee iiff
 ********** PPaacckkeedd ppaacckkeett hheeaaddeerrss,, mmaaiinn hheeaaddeerr ((PPPPMM)) mmaarrkkeerr sseeggmmeenntt **********
 ******** EElleemmeenntt nnaammee ********
 ppm
-******** RReeppoorrtteedd pprrooppeerrttiieess_11_99 ********
+******** RReeppoorrtteedd pprrooppeerrttiieess_22_44 ********
 PPrrooppeerrttyy DDeessccrriippttiioonn
 ******** TTeessttss ********
 TTeesstt nnaammee TTrruuee iiff
 ********** PPaacckkeett lleennggtthh,, ttiillee--ppaarrtt hheeaaddeerr ((PPLLTT)) mmaarrkkeerr sseeggmmeenntt **********
 ******** EElleemmeenntt nnaammee ********
 plt
-******** RReeppoorrtteedd pprrooppeerrttiieess_22_00 ********
+******** RReeppoorrtteedd pprrooppeerrttiieess_22_55 ********
 PPrrooppeerrttyy DDeessccrriippttiioonn
 lplt     Length of PLT marker segment in bytes
 zplt     PLT marker segment index
 nplm     Number of bytes of Iplm information for the ith tile-part
 iplt     Comma separated list of packet length values (as hexadecimal strings)
 ******** TTeessttss ********
 TTeesstt nnaammee TTrruuee iiff
 ********** PPaacckkeedd ppaacckkeett hheeaaddeerrss,, ttiillee--ppaarrtt hheeaaddeerr ((PPPPTT)) mmaarrkkeerr sseeggmmeenntt **********
 ******** EElleemmeenntt nnaammee ********
 ppt
-******** RReeppoorrtteedd pprrooppeerrttiieess_22_11 ********
+******** RReeppoorrtteedd pprrooppeerrttiieess_22_66 ********
 PPrrooppeerrttyy DDeessccrriippttiioonn
 ******** TTeessttss ********
 TTeesstt nnaammee TTrruuee iiff
 ************ RReeffeerreenncceess ************
 ICC. Specification ICC.1:1998-09 – File Format for Color Profiles.
 International Color Consortium, 1998. _h_t_t_p_s_:_/_/_w_w_w_._c_o_l_o_r_._o_r_g_/_I_C_C_-_1___1_9_9_8_-_0_9_._p_d_f.
 ISO/IEC. Information technology — JPEG 2000 image coding system: Core coding
@@ -1786,39 +1886,47 @@
 Leach, P., Mealling, M. & Salz, R. A Universally Unique IDentifier (UUID) URN
 namespace. Memo, IETF. _h_t_t_p_s_:_/_/_t_o_o_l_s_._i_e_t_f_._o_r_g_/_h_t_m_l_/_r_f_c_4_1_2_2_._h_t_m_l.
 ===============================================================================
    1. The jjppyyllyyzzeerr binaries were created using the PPyyIInnssttaalllleerr package: _h_t_t_p_s_:_/
       _/_w_w_w_._p_y_i_n_s_t_a_l_l_e_r_._o_r_g_/_↩_︎
    2. Note that jjppyyllyyzzeerr versions 1.8 and earlier returned a formatted XML
       string instead of an element object!_↩_︎
-   3. Note that jjppyyllyyzzeerr versions 1.4 and earlier used the verbose output
+   3. Jpylyzer 2.2 and more recent only work with Python > 3.2. Since Jython
+      still hasn’t been upgraded to support Python 3, Java integration with
+      Jython currently doesn’t work._↩_︎
+   4. Note that jjppyyllyyzzeerr versions 1.4 and earlier used the verbose output
       format by default. This behaviour has changed in version 1.5 onwards, as
       the lengthy output turned out to be slightly confusing to some users._↩_︎
-   4. The “Any ICC” method is defined in ISO/IEC 15444-2 (the JPX format), and
-      is not allowed in JP2. However, jjppyyllyyzzeerr offers limited support for JPX
-      here by also reporting the properties of ICC profiles that were embedded
-      using this method. Note that any file that uses this method will fail the
-      “methIsValid” test (and thereby the validation)._↩_︎
-   5. Originally ISO/IEC 15444-1 only allowed “input device” profiles. Support
+   5. Meaning of values defined in Table 2 of Rec. ITU-T H.273 / ISO/IEC 23001-
+      8 _“_C_o_d_i_n_g_-_i_n_d_e_p_e_n_d_e_n_t_ _c_o_d_e_ _p_o_i_n_t_s_ _f_o_r_ _v_i_d_e_o_ _s_i_g_n_a_l_ _t_y_p_e_ _i_d_e_n_t_i_f_i_c_a_t_i_o_n_”_↩_︎
+   6. Meaning of values defined in Table 3 of Rec. ITU-T H.273 / ISO/IEC 23001-
+      8 _“_C_o_d_i_n_g_-_i_n_d_e_p_e_n_d_e_n_t_ _c_o_d_e_ _p_o_i_n_t_s_ _f_o_r_ _v_i_d_e_o_ _s_i_g_n_a_l_ _t_y_p_e_ _i_d_e_n_t_i_f_i_c_a_t_i_o_n_”_↩_︎
+   7. Meaning of values defined in Table 4 of Rec. ITU-T H.273 / ISO/IEC 23001-
+      8 _“_C_o_d_i_n_g_-_i_n_d_e_p_e_n_d_e_n_t_ _c_o_d_e_ _p_o_i_n_t_s_ _f_o_r_ _v_i_d_e_o_ _s_i_g_n_a_l_ _t_y_p_e_ _i_d_e_n_t_i_f_i_c_a_t_i_o_n_”_↩_︎
+   8. Meaning defined in Rec. ITU-T H.273 / ISO/IEC 23001-8 _“_C_o_d_i_n_g_-_i_n_d_e_p_e_n_d_e_n_t
+      _c_o_d_e_ _p_o_i_n_t_s_ _f_o_r_ _v_i_d_e_o_ _s_i_g_n_a_l_ _t_y_p_e_ _i_d_e_n_t_i_f_i_c_a_t_i_o_n_”_↩_︎
+   9. Originally ISO/IEC 15444-1 only allowed “input device” profiles. Support
       of “display device” profiles was added through an _a_m_e_n_d_m_e_n_t to the
       standard in 2013. The behaviour of jjppyyllyyzzeerr is consistent with this
       amendment._↩_︎
-   6. Calculated as: vRcN vRcD • 10 vRcE _↩_︎
-   7. Calculated as: hRcN hRcD • 10 hRcE _↩_︎
-   8. Calculated as: vRescInPixelsPerMeter • 25.4 • 10 -3 _↩_︎
-   9. Calculated as: hRescInPixelsPerMeter • 25.4 • 10 -3 _↩_︎
-  10. Calculated as: vRdN vRdD • 10 vRdE _↩_︎
-  11. Calculated as: hRdN hRdD • 10 hRdE _↩_︎
-  12. Calculated as: vResdInPixelsPerMeter • 25.4 • 10 -3 _↩_︎
-  13. Calculated as: hResdInPixelsPerMeter • 25.4 • 10 -3 _↩_︎
-  14. Link: _h_t_t_p_s_:_/_/_w_w_w_i_m_a_g_e_s_._a_d_o_b_e_._c_o_m_/_w_w_w_._a_d_o_b_e_._c_o_m_/_c_o_n_t_e_n_t_/_d_a_m_/_A_d_o_b_e_/_e_n_/
+  10. For JPH, an addition “application-defined” value is allowed (ISO/IEC
+      15444-15, Table D.4)_↩_︎
+  11. Calculated as: vRcN vRcD • 10 vRcE _↩_︎
+  12. Calculated as: hRcN hRcD • 10 hRcE _↩_︎
+  13. Calculated as: vRescInPixelsPerMeter • 25.4 • 10 -3 _↩_︎
+  14. Calculated as: hRescInPixelsPerMeter • 25.4 • 10 -3 _↩_︎
+  15. Calculated as: vRdN vRdD • 10 vRdE _↩_︎
+  16. Calculated as: hRdN hRdD • 10 hRdE _↩_︎
+  17. Calculated as: vResdInPixelsPerMeter • 25.4 • 10 -3 _↩_︎
+  18. Calculated as: hResdInPixelsPerMeter • 25.4 • 10 -3 _↩_︎
+  19. Link: _h_t_t_p_s_:_/_/_w_w_w_i_m_a_g_e_s_._a_d_o_b_e_._c_o_m_/_w_w_w_._a_d_o_b_e_._c_o_m_/_c_o_n_t_e_n_t_/_d_a_m_/_A_d_o_b_e_/_e_n_/
       _d_e_v_n_e_t_/_x_m_p_/_p_d_f_s_/_c_s_6_/_X_M_P_S_p_e_c_i_f_i_c_a_t_i_o_n_P_a_r_t_3_._p_d_f_↩_︎
-  15. However, support for start of packet (SOP) and end of packet (EPH)
+  20. However, support for start of packet (SOP) and end of packet (EPH)
       markers may be included in future versions._↩_︎
-  16. For example, in a TIFF to JP2 conversion workflow one could include a
+  21. For example, in a TIFF to JP2 conversion workflow one could include a
       pixel-by-pixel comparison of the values in the TIFF and the JP2._↩_︎
-  17. Calculated as: numberOfTiles = [ xsiz - xOsiz xTsiz ] • [ ysiz - yOsiz
+  22. Calculated as: numberOfTiles = [ xsiz - xOsiz xTsiz ] • [ ysiz - yOsiz
       yTsiz ] _↩_︎
-  18. Only reported if the --packetmarkers option is used._↩_︎
-  19. Only reported if the --packetmarkers option is used._↩_︎
-  20. Only reported if the --packetmarkers option is used._↩_︎
-  21. Only reported if the --packetmarkers option is used._↩_︎
+  23. Only reported if the --packetmarkers option is used._↩_︎
+  24. Only reported if the --packetmarkers option is used._↩_︎
+  25. Only reported if the --packetmarkers option is used._↩_︎
+  26. Only reported if the --packetmarkers option is used._↩_︎
```

### Comparing `jpylyzer-2.2.0b1/doc/userManual.html` & `jpylyzer-2.2.0rc1/doc/userManual.html`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 <li><a href="#file-element">file element</a></li>
 <li><a href="#fileinfo-element">fileInfo element</a></li>
 <li><a href="#statusinfo-element">statusInfo element</a></li>
 <li><a href="#isvalid-element">isValid element</a></li>
 <li><a href="#tests-element">tests element</a></li>
 <li><a href="#properties-element">properties element</a></li>
 <li><a href="#propertiesExtension-element">propertiesExtension element</a></li>
+<li><a href="#warnings-element">warnings element</a></li>
 </ul></li>
 <li><a href="#jp2-box-by-box">JP2: box by box</a>
 <ul>
 <li><a href="#about-properties-tests-trees">About the properties and tests trees</a></li>
 <li><a href="#jpeg2000-signature-box">JPEG 2000 Signature box</a></li>
 <li><a href="#file-type-box">File Type box</a></li>
 <li><a href="#jp2-header-box">JP2 Header box (superbox)</a></li>
@@ -90,14 +91,17 @@
 <li><a href="#coc-marker">Coding style component (COC) marker segment</a></li>
 <li><a href="#rgn-marker">Region-of-interest (RGN) marker segment</a></li>
 <li><a href="#qcd-marker">Quantization default (QCD) marker segment</a></li>
 <li><a href="#qcc-marker">Quantization component (QCC) marker segment</a></li>
 <li><a href="#poc-marker">Progression order change (POC) marker segment</a></li>
 <li><a href="#crg-marker">Component registration (CRG) marker segment</a></li>
 <li><a href="#com-marker">Comment (COM) marker segment</a></li>
+<li><a href="#cap-marker">Extended capabilities (CAP) marker segment</a></li>
+<li><a href="#prf-marker">Profile (PRF) marker segment</a></li>
+<li><a href="#cpf-marker">Corresponding profile (CPF) marker segment</a></li>
 <li><a href="#tile-part">Tile part (child of Contiguous Codestream box)</a></li>
 <li><a href="#sot-marker">Start of tile part (SOT) marker segment (child of tile part)</a></li>
 <li><a href="#tlm-marker">Tile-part lengths (TLM) marker segment</a></li>
 <li><a href="#plm-marker">Packet length, main header (PLM) marker segment</a></li>
 <li><a href="#ppm-marker">Packed packet headers, main header (PPM) marker segment</a></li>
 <li><a href="#plt-marker">Packet length, tile-part header (PLT) marker segment</a></li>
 <li><a href="#ppt-marker">Packed packet headers, tile-part header (PPT) marker segment</a></li>
@@ -118,14 +122,17 @@
 
 <ol type="1">
 <li><p>Is this really a JP2 and does it really conform to the format’s specifications (validation)?</p></li>
 <li><p>What are the technical characteristics of this image (feature extraction)?</p></li>
 </ol>
 
 
+<p>Starting with version 2.2, <em>jpylyzer</em> also supports Part 15 of the standard (ISO/IEC 15444-15, High Throughput JPEG 2000), and its JPH image format.</p>
+
+
 <h2 id="validation-scope-and-restrictions">Validation: scope and restrictions</h2>
 
 
 <p>Since the word ‘validation’ means different things to different people, a few words about the overall scope of <em>jpylyzer</em>. First of all, it is important to stress that <em>jpylyzer</em> is not a ‘one stop solution’ that will tell you that an image is 100% perfect. What <em>jpylyzer</em> does is this: based on the JP2 format specification (ISO/IEC 15444-1), it parses a file. It then subjects the file’s contents to a large number of tests, each of which is based on the requirements and restrictions that are defined by the standard. If a file fails one or more tests, this implies that it does not conform to the standard, and is no valid JP2. Importantly, this presumes that <em>jpylyzer</em>’s tests accurately reflect the format specification, without producing false positives.</p>
 
 
 <h3 id="valid-means-probably-valid">‘Valid’ means ‘probably valid’</h3>
@@ -157,20 +164,14 @@
 <li><p>Format migration workflows (e.g. TIFF to JP2) should ideally also include some comparison between source and destination images (e.g. a pixel-wise comparison)</p></li>
 </ul>
 
 
 <p>Conversely, an image that successfully passes a rendering test or pixel-wise comparison may still contain problematic features (e.g. incorrect colour space information), so validation, rendering tests and pixel-wise comparisons are really complementary to each other.</p>
 
 
-<h3 id="note-on-icc-profile-support">Note on ICC profile support</h3>
-
-
-<p>The support of ICC profiles in JP2 was recently extended through an <a href="https://www.itu.int/rec/T-REC-T.800-201303-P!Amd6/en">amendment</a> to the standard. These changes are taken into account by <em>jpylyzer</em>, which is in line with the most recent version of the (updated) standard.</p>
-
-
 <h2 id="outline">Outline of this User Manual</h2>
 
 
 <p>We start by describing the <a href="#installation">installation process</a> of <em>jpylyzer</em> for Windows and Unix-based systems. We then explain its <a href="#using-jpylyzer">basic usage</a>, either as a command-line tool, or as an importable Python module. This is followed by a brief overview of <a href="#structure-jp2">the structure of the JP2 format</a> and its ‘box’ structure, and an explanation of <em>Jpylyzer</em>’s <a href="#output-format">output format</a>. The final sections give a detailed description of the tests that <em>jpylyzer</em> performs for validation, and the properties that are reported in the output. The <a href="#jp2-box-by-box">penultimate section</a> does this for all ‘boxes’, except the ‘Contiguous Codestream’ box, which is given a <a href="#contiguous-codestream-box-chapter">section of its own</a>.</p>
 
 
 <h2 id="funding">Funding</h2>
@@ -209,15 +210,15 @@
 <p><a href="https://jpylyzer.openpreservation.org/" class="uri">https://jpylyzer.openpreservation.org/</a></p>
 
 
 <p>You have three options:</p>
 
 
 <ol type="1">
-<li><p>Install the software with the <em>Pip</em> package manager. This works on all platforms (Windows, Linux, Mac, etc.), but you need to have the Python interpreter available on your system. Jpylyzer is compatible with Python 2.7, and Python 3.2 and more recent (Python 3.0 and 3.1 are not supported).</p></li>
+<li><p>Install the software with the <em>Pip</em> package manager. This works on all platforms (Windows, Linux, Mac, etc.), but you need to have the Python interpreter available on your system. Jpylyzer is compatible with Python 3.2 and more recent.</p></li>
 <li><p>Alternatively, for Windows users there is also a set of stand-alone binaries<a href="#fn1" class="footnote-ref" id="fnref1" role="doc-noteref"><sup>1</sup></a>. These allow you to run <em>jpylyzer</em> as an executable Windows application, without any need for installing Python. This option is particularly useful for Windows users who cannot (or don’t want to) install software on their system.</p></li>
 <li><p>For Linux users Debian packages are available.</p></li>
 </ol>
 
 
 <p>These options are described in the following sub-sections.</p>
 
@@ -269,18 +270,17 @@
 
 <pre><code>jpylyzer</code></pre>
 
 
 <p>If all went well you now see this:</p>
 
 
-<pre><code>usage: jpylyzer [-h] [--format FMT] [--legacyout] [--mix {1,2}] [--nopretty]
+<pre><code>usage: jpylyzer [-h] [--format FMT] [--mix {1,2}] [--nopretty]
           [--nullxml] [--recurse] [--packetmarkers] [--verbose]
-          [--version] [--wrapper]
-          jp2In [jp2In ...]
+          [--version] jp2In [jp2In ...]
 jpylyzer: error: the following arguments are required: jp2In</code></pre>
 
 
 <p>Which means that the installation was successful!</p>
 
 
 <h3 id="global-installation-linux">Global installation (Linux)</h3>
@@ -324,18 +324,17 @@
 
 <pre><code>c:\tools\jpylyzer\jpylyzer</code></pre>
 
 
 <p>Executing this command should result in the following screen output:</p>
 
 
-<pre><code>usage: jpylyzer [-h] [--format FMT] [--legacyout] [--mix {1,2}] [--nopretty]
+<pre><code>usage: jpylyzer [-h] [--format FMT] [--mix {1,2}] [--nopretty]
           [--nullxml] [--recurse] [--packetmarkers] [--verbose]
-          [--version] [--wrapper]
-          jp2In [jp2In ...]
+          [--version] jp2In [jp2In ...]
 jpylyzer: error: the following arguments are required: jp2In</code></pre>
 
 
 <h3 id="running-jpylyzer-without-typing-the-full-path">Running jpylyzer without typing the full path</h3>
 
 
 <p>Optionally, you may also want to add the full path of the <em>jpylyzer</em> installation directory to the Windows ’Path’ environment variable. Doing so allows you to run <em>jpylyzer</em> from any directory on your PC without having to type the full path. In Windows 7 you can do this by selecting ‘settings’ from the ‘Start’ menu; then go to ‘control panel’/’system’ and go to the ‘advanced’ tab. Click on the ‘environment variables’ button. Finally, locate the ‘Path’ variable in the ‘system variables’ window, click on ‘Edit’ and add the full <em>jpylyzer</em> path (this requires local Administrator privileges). The settings take effect on any newly opened command prompt.</p>
@@ -343,15 +342,15 @@
 
 <h2 id="installation-debian">Installation of Debian packages (Ubuntu/Linux)</h2>
 
 
 <p>For Linux, Debian packages of <em>jpylyzer</em> exist. To install, simply download the <em>.deb</em> file, double-click on it and select <em>Install Package</em>. Alternatively you can also do this in the command terminal by typing:</p>
 
 
-<pre><code>sudo dpkg -i opf-jpylyzer_2.0.0_all.deb</code></pre>
+<pre><code>sudo dpkg -i opf-jpylyzer_2.2.0_all.deb</code></pre>
 
 
 <p>In both cases you need to have administrative privileges.</p>
 
 
 <p>For <em>Ubuntu</em> and <em>Debian</em> alternative packages are available in the official release channels. To install simply run the following commands:</p>
 
@@ -400,18 +399,17 @@
 
 <h3 id="synopsis">Synopsis</h3>
 
 
 <p><em>Jpylyzer</em> can be invoked using the following command-line arguments:</p>
 
 
-<pre><code>usage: jpylyzer [-h] [--format FMT] [--legacyout] [--mix {1,2}] [--nopretty]
+<pre><code>usage: jpylyzer [-h] [--format FMT] [--mix {1,2}] [--nopretty]
           [--nullxml] [--recurse] [--packetmarkers] [--verbose]
-          [--version] [--wrapper]
-          jp2In [jp2In ...]</code></pre>
+          [--version] jp2In [jp2In ...]</code></pre>
 
 
 <h4 id="positional-arguments">Positional arguments</h4>
 
 
 <table>
 <thead>
@@ -419,15 +417,15 @@
 <th style="text-align: left;">Argument</th>
 <th style="text-align: left;">Description</th>
 </tr>
 </thead>
 <tbody>
 <tr class="odd">
 <td style="text-align: left;"><code>jp2In</code></td>
-<td style="text-align: left;">input JP2 image(s), may be one or more (whitespace-separated) path expressions; prefix wildcard (*) with backslash (\) in Linux</td>
+<td style="text-align: left;">input image(s), may be one or more (whitespace-separated) path expressions; prefix wildcard (*) with backslash (\) in Linux</td>
 </tr>
 </tbody>
 </table>
 
 
 <h4 id="optional-arguments">Optional arguments</h4>
 
@@ -442,52 +440,44 @@
 <tbody>
 <tr class="odd">
 <td style="text-align: left;"><code>[-h, --help]</code></td>
 <td style="text-align: left;">show help message and exit</td>
 </tr>
 <tr class="even">
 <td style="text-align: left;"><code>[--format FMT]</code></td>
-<td style="text-align: left;">validation format; allowed values are <code>jp2</code> (used by default) and <code>j2c</code> (which activates raw codestream validation)</td>
+<td style="text-align: left;">validation format; allowed values are <code>jp2</code> (JPEG 2000 Part 1, used by default), <code>j2c</code> (Part 1 codestream), <code>jph</code> (JPEG 2000 Part 15 / High Throughput JPEG 2000) and <code>jhc</code> (Part 15 codestream)</td>
 </tr>
 <tr class="odd">
 <td style="text-align: left;"><code>[--mix {1,2}]</code></td>
 <td style="text-align: left;">report additional output in NISO MIX format (version 1.0 or 2.0)</td>
 </tr>
 <tr class="even">
-<td style="text-align: left;"><code>[--legacyout]</code></td>
-<td style="text-align: left;">report output in jpylyzer 1.x format (provided for backward compatibility only)</td>
-</tr>
-<tr class="odd">
 <td style="text-align: left;"><code>[--nopretty]</code></td>
 <td style="text-align: left;">suppress pretty-printing of XML output</td>
 </tr>
-<tr class="even">
+<tr class="odd">
 <td style="text-align: left;"><code>[--nullxml]</code></td>
 <td style="text-align: left;">extract null-terminated XML content from XML and UUID boxes(doesn’t affect validation)</td>
 </tr>
-<tr class="odd">
+<tr class="even">
 <td style="text-align: left;"><code>[--recurse, -r]</code></td>
-<td style="text-align: left;">when analysing a directory, recurse into subdirectories (implies <code>--wrapper</code> if <code>--legacyout</code> is used)</td>
+<td style="text-align: left;">when analysing a directory, recurse into subdirectories</td>
 </tr>
-<tr class="even">
+<tr class="odd">
 <td style="text-align: left;"><code>[--packetmarkers]</code></td>
 <td style="text-align: left;">Report packet-level codestream markers (plm, ppm, plt, ppt)</td>
 </tr>
-<tr class="odd">
+<tr class="even">
 <td style="text-align: left;"><code>[--verbose]</code></td>
 <td style="text-align: left;">report test results in verbose format</td>
 </tr>
-<tr class="even">
+<tr class="odd">
 <td style="text-align: left;"><code>[-v, --version]</code></td>
 <td style="text-align: left;">show program’s version number and exit</td>
 </tr>
-<tr class="odd">
-<td style="text-align: left;"><code>[--wrapper, -w]</code></td>
-<td style="text-align: left;">wrap output for individual image(s) in ‘results’ XML element (deprecated from jpylyzer 2.x onward, only takes effect if <code>--legacyout</code> is used)</td>
-</tr>
 </tbody>
 </table>
 
 
 <p>Note that the input can either be a single image, a space-separated sequence of images, a pathname expression that includes multiple images, or any combination of the above. For example, the following command will process one single image:</p>
 
 
@@ -529,30 +519,36 @@
 
 <p>By default, <em>jpylyzer</em> validates against the <em>JP2</em> format specification. Starting with version 2.0, <em>jpylyzer</em> can also validate raw JPEG 2000 codestreams that are not wrapped inside a <em>JP2</em> container. For codestream validation, use the <code>--format</code> option with value <code>j2c</code>, e.g.:</p>
 
 
 <pre><code>jpylyzer --format j2c rubbish.j2c &gt; rubbish.xml</code></pre>
 
 
-<h3 id="mix-option">‘mix’ option</h3>
+<p>Starting with version 2.2, <em>jpylyzer</em> also supports JPEG 2000 Part 15 (High Throughput JPEG 2000) and its <em>JPH</em> container format. To validate a <em>JPH</em> file, use the <code>--format</code> option with value <code>jph</code>:</p>
 
 
-<p>When this option is used, <em>jpylyzer</em> reports additional output in <a href="https://www.loc.gov/standards/mix/"><em>NISO MIX</em></a> format. This option takes one argument that defines whether <em>MIX</em> 1.0 or <em>MIX</em> 2.0 is used. For example, the following command will result in <em>MIX</em> 2.0 output:</p>
+<pre><code>jpylyzer --format jph rubbish.jph &gt; rubbish.xml</code></pre>
 
 
-<pre><code>jpylyzer --mix 2 rubbish.jp2 &gt; rubbish.xml</code></pre>
+<p>And use <code>--format</code> with value <code>jhc</code> to validate a raw High Throughput codestream:</p>
+
+
+<pre><code>jpylyzer --format jhc rubbish.jhc &gt; rubbish.xml</code></pre>
 
 
-<p>The <em>MIX</em> output is wrapped inside a <em>file/propertiesExtension</em> element. Note that <em>MIX</em> output is <em>only</em> written for files that are valid JP2 (files that are not valid result in an empty <em>propertiesExtension</em> element). Also, the <code>--mix</code> option is ignored if <code>--format</code> is set to <code>j2c</code>, or if <code>--legacyout</code> (see below) is used.</p>
+<h3 id="mix-option">‘mix’ option</h3>
+
 
+<p>When this option is used, <em>jpylyzer</em> reports additional output in <a href="https://www.loc.gov/standards/mix/"><em>NISO MIX</em></a> format. This option takes one argument that defines whether <em>MIX</em> 1.0 or <em>MIX</em> 2.0 is used. For example, the following command will result in <em>MIX</em> 2.0 output:</p>
 
-<h3 id="legacyout-option">‘legacyout’ option</h3>
+
+<pre><code>jpylyzer --mix 2 rubbish.jp2 &gt; rubbish.xml</code></pre>
 
 
-<p>The output format of <em>jpylyzer</em> has changed in version 2.0, which may break existing workflows that expect output in 1.x format. For backward compatibility the <code>--legacyout</code> option results in output that follows the old 1.x format. Note that codestream validation is disabled if you use this option.</p>
+<p>The <em>MIX</em> output is wrapped inside a <em>file/propertiesExtension</em> element. Note that <em>MIX</em> output is <em>only</em> written for files that are valid JP2 or JPH (files that are not valid result in an empty <em>propertiesExtension</em> element). Also, the <code>--mix</code> option is ignored if <code>--format</code> is set to <code>j2c</code>.</p>
 
 
 <h3 id="recurse-option">‘recurse’ option</h3>
 
 
 <p>If the <code>--recurse</code> option is used, <em>jpylyzer</em> will recursively traverse all subdirectories of a filepath expression. E.g:</p>
 
@@ -576,45 +572,24 @@
 <li>PPT (packed packet headers, tile-part header) marker</li>
 </ul>
 
 
 <p>By default these are excluded from the output, in order to prevent excessive output size.</p>
 
 
-<h3 id="wrapper-option-deprecated">‘wrapper’ option (deprecated)</h3>
-
-
-<p>This deprecated option is included for backward-compatibility, and only takes effect if <code>--legacyout</code> (see above) is used.By default, the <em>jpylyzer</em> 1.x releases would create a separate XML tree for each analysed image, without any overarching hierarchy. For multiple-image pathname expressions this resulted in output that was <strong>not</strong> well-formed XML. The <code>--legacyout</code> option still results in this is behaviour. For example:</p>
-
-
-<pre><code>jpylyzer --legacyout rubbish.jp2 garbage.jp2 &gt; rubbish.xml</code></pre>
-
-
-<p>In this case, the file ‘rubbish.xml’ contains a succession of two XML trees, which by itself is not well-formed XML. The <code>--wrapper</code> option is provided to create valid XML instead:</p>
-
-
-<pre><code>jpylyzer --legacyout --wrapper rubbish.jp2 garbage.jp2 &gt; rubbish.xml</code></pre>
-
-
-<p>In the above case the XML trees of the individual images are wrapped inside a ‘results’ element. When the <code>--recurse</code> option is used, jpylyzer will automatically wrap the output in a ‘results’ element, so there’s no need to specify <code>--wrapper</code> in that case.</p>
-
-
-<p>Starting with version 2.0, <em>jpylyzer</em> <em>always</em> generates well-formed XML (unless the <code>--legacyout</code> option is used), which makes the <code>--wrapper</code> option largely obsolete, apart from cases where the ‘old’ behaviour is needed for backward-compatibility reasons.</p>
-
-
 <h3 id="nullxml-option">‘nullxml’ option</h3>
 
 
 <p>The <em>nullxml</em> option was added to enable extraction of XML content that is terminated by a null-byte. By default <em>jpylyzer</em> doesn’t report the XML in that case, because it throws an exception in the XML parser. Apparently some old versions of the Kakadu demo applications would erroneously add a null-byte to embedded XML, so this option can be used to force extraction for images that are affected by this.</p>
 
 
 <h3 id="user-warnings">User warnings</h3>
 
 
-<p>Under the following conditions <em>jpylyzer</em> will print a user warning to the standard error device (typically the console screen):</p>
+<p>Under the following conditions <em>jpylyzer</em> will report a user warning:</p>
 
 
 <h4 id="no-images-to-check">No images to check</h4>
 
 
 <p>If there are no input images to check (typically because the value of jp2In refers to a non-existent file), the following warning message is shown:</p>
 
@@ -678,27 +653,30 @@
 
 <pre><code>User warning: ignoring unknown box</code></pre>
 
 
 <p>This happens if <em>jpylyzer</em> encounters a box that is not defined by JPEG 2000 Part 1. It should be noted that, to a large extent, JPEG 2000 Part 1 permits the presence of boxes that are defined outside the standard. Again, <em>jpylyzer</em> will simply ignore these and process all other boxes normally.</p>
 
 
+<p>All user warnings are printed to the standard error device (typically the console screen). File-level warnings are also written to the <em>warnings</em> output element.</p>
+
+
 <h2 id="using-as-python-module">Using <em>jpylyzer</em> as a Python module</h2>
 
 
 <p>Instead of using <em>jpylyzer</em> from the command-line, you can also import it as a module in your own Python programs. To do so, install jpylyzer with <em>pip</em>. Then import <em>jpylyzer</em> into your code by adding:</p>
 
 
 <pre><code>from jpylyzer import jpylyzer</code></pre>
 
 
 <p>Subsequently you can call any function that is defined in <em>jpylyzer.py</em>. In practice you will most likely only need the <em>checkOneFile</em> function. The following minimal script shows how this works:</p>
 
 
-<pre><code>#! /usr/bin/env python
+<pre><code>#! /usr/bin/env python3
 
 from jpylyzer import jpylyzer
 
 # Define JP2
 myFile = "/home/johan/jpylyzer-test-files/aware.jp2"
 
 # Analyse with jpylyzer, result to Element object
@@ -708,28 +686,40 @@
 imageHeight = myResult.findtext('./properties/jp2HeaderBox/imageHeaderBox/height')
 print(imageHeight)</code></pre>
 
 
 <p>Here, <em>myResult</em> is an <em>Element</em> object that can either be used directly, or converted to XML using the <em>ElementTree</em> module<a href="#fn2" class="footnote-ref" id="fnref2" role="doc-noteref"><sup>2</sup></a>. The structure of the element object follows the XML output that described <a href="#output-format">here</a>.</p>
 
 
-<p>For validation a raw JPEG 2000 codestreams, call the <em>checkOneFile</em> function with the additional <em>validationFormat</em> argument, and set it to <code>j2c</code>:</p>
+<p>You may use the following optional arguments (which correspond to the command-line options explained above):</p>
+
+
+<ul>
+<li>validationFormat - sets the validation format. Values: ‘jp2’ (default), ‘jph’, ‘j2c’ or ‘jhc’.</li>
+<li>verboseFlag - report test results in verbose format. Values: False (default) or True.</li>
+<li>packetmarkersFlag - report packet-level codestream markers. Values: False (default) or True.</li>
+<li>nullxmlFlag - extract null-terminated XML content from XML and UUID boxes. Values: False (default) or True.</li>
+<li>mixFlag - report additional output in NISO MIX format (version 1.0 or 2.0). Values: 0 (default), 1 or 2.</li>
+</ul>
+
+
+<p>As an example, for validating a raw JPEG 2000 codestream, call the <em>checkOneFile</em> function with the additional <em>validationFormat</em> argument, and set it to <code>j2c</code>:</p>
 
 
 <pre><code># Define Codestream
 myFile = "/home/johan/jpylyzer-test-files/rubbish.j2c"
 
 # Analyse with jpylyzer, result to Element object
 myResult = jpylyzer.checkOneFile(myFile, 'j2c')</code></pre>
 
 
 <h2 id="java-integration">Java integration</h2>
 
 
-<p>It is possible to integrate <em>jpylyzer</em> into Java applications. A test class that shows how this works is included in the source repo <a href="https://github.com/openpreserve/jpylyzer/tree/master/jpylyzer/java_demo/CallJpylyzer.java">here</a>. This requires <a href="https://www.jython.org/">Jython</a>. Note that you may run into performance issues with (very) large images in this case, as Jython does not support <a href="https://docs.python.org/3/library/mmap.html">memory mapping</a>, so make sure you’ve got plenty of RAM available.</p>
+<p>It is possible to integrate <em>jpylyzer</em> into Java applications<a href="#fn3" class="footnote-ref" id="fnref3" role="doc-noteref"><sup>3</sup></a>. A test class that shows how this works is included in the source repo <a href="https://github.com/openpreserve/jpylyzer/tree/master/jpylyzer/java_demo/CallJpylyzer.java">here</a>. This requires <a href="https://www.jython.org/">Jython</a>. Note that you may run into performance issues with (very) large images in this case, as Jython does not support <a href="https://docs.python.org/3/library/mmap.html">memory mapping</a>, so make sure you’ve got plenty of RAM available.</p>
 
 
 <h1 id="structure-jp2">Structure of a JP2 file</h1>
 
 
 <h2 id="structure-scope">Scope of this section</h2>
 
@@ -930,15 +920,15 @@
 
 <p>This section explains <em>jpylyzer</em>’s output format.</p>
 
 
 <h2 id="output-format-overview">Overview</h2>
 
 
-<p><em>Jpylyzer</em> generates its output in XML format, which is defined by <a href="https://jpylyzer.openpreservation.org/jpylyzer-v-2-1.xsd">the schema that can be found here</a>. The following Figure shows the output structure:</p>
+<p><em>Jpylyzer</em> generates its output in XML format, which is defined by <a href="https://jpylyzer.openpreservation.org/jpylyzer-v-2-2.xsd">the schema that can be found here</a>. The following Figure shows the output structure:</p>
 
 
 <figure>
 <img src="images/outputStructure.png" alt="Jpylyzer’s XML output structure. ‘box’ elements under ‘tests’ and ‘properties’ contain further sub-elements."/><figcaption aria-hidden="true">Jpylyzer’s XML output structure. ‘box’ elements under ‘tests’ and ‘properties’ contain further sub-elements.</figcaption>
 </figure>
 
 
@@ -975,14 +965,15 @@
 <ol type="1">
 <li><p><em>fileInfo</em>: general information about the analysed file</p></li>
 <li><p><em>statusInfo</em>: information about the status of <em>jpylyzer</em>’s validation attempt</p></li>
 <li><p><em>isValid</em>: outcome of the validation</p></li>
 <li><p><em>tests</em>: outcome of the individual tests that are part of the validation process (organised by box)</p></li>
 <li><p><em>properties</em>: image properties (organised by box)</p></li>
 <li><p><em>propertiesExtension</em>: wrapper element for NISO <em>MIX</em> output (only if the <code>--mix</code> option is used)</p></li>
+<li><p><em>warnings</em>: reported warnings</p></li>
 </ol>
 
 
 <h2 id="fileinfo-element">fileInfo element</h2>
 
 
 <p>This element holds general information about the analysed file. Currently it contains the following sub-elements:</p>
@@ -1039,29 +1030,44 @@
 
 <p>If a file passed <em>all</em> tests, this is an indication that it is most likely valid JP2. In that case, the <a href="#isvalid-element"><em>isValid</em> element</a> has a value of “True” (and “False” in all other cases). These tests are all explained <a href="#jp2-box-by-box">here</a> and <a href="#contiguous-codestream-box-chapter">here</a>.</p>
 
 
 <h3 id="default-and-verbose-reporting-of-test-results">Default and verbose reporting of test results</h3>
 
 
-<p>By default, <em>jpylyzer</em> only reports any tests that failed (i.e. returned “False”), including the corresponding part of the box structure. For a valid JP2 the tests element will be empty. If the –verbose flag is used, the results of <em>all</em> tests are included (including those that returned “True”)<a href="#fn3" class="footnote-ref" id="fnref3" role="doc-noteref"><sup>3</sup></a>.</p>
+<p>By default, <em>jpylyzer</em> only reports any tests that failed (i.e. returned “False”), including the corresponding part of the box structure. For a valid JP2 the tests element will be empty. If the –verbose flag is used, the results of <em>all</em> tests are included (including those that returned “True”)<a href="#fn4" class="footnote-ref" id="fnref4" role="doc-noteref"><sup>4</sup></a>.</p>
 
 
 <h2 id="properties-element">properties element</h2>
 
 
 <p>This element contains the extracted image properties, which are organised in a hierarchical tree that corresponds to JP2’s box structure. See <a href="#jp2-box-by-box">here</a> and <a href="#contiguous-codestream-box-chapter">here</a> for a description of the reported properties.</p>
 
 
 <h2 id="propertiesExtension-element">propertiesExtension element</h2>
 
 
 <p>This optional element is reserved for output in alternative formats. Currently it is used to wrap output in NISO <em>MIX</em> format if the <code>--mix</code> option is used. See the <a href="https://www.loc.gov/standards/mix/"><em>MIX</em> documentation</a> for a description of the reported elements.</p>
 
 
+<h2 id="warnings-element">warnings element</h2>
+
+
+<p>This element is reserved for reporting any warnings that are not directly related to the validation process. Examples are:</p>
+
+
+<ul>
+<li>Jpylyzer encountered an unknown box type while parsing a file.</li>
+<li>Reading of a file failed because of system limitations.</li>
+</ul>
+
+
+<p>Each warning is wrapped in a ‘warning’ element. The results are organised in a hierarchical tree that corresponds to JP2’s box structure.</p>
+
+
 <h1 id="jp2-box-by-box">JP2: box by box</h1>
 
 
 <p>The following two sections provide a detailed explanation of <em>jpylyzer</em>’s functionality and its output. In particular, the following two aspects are addressed:</p>
 
 
 <ol type="1">
@@ -1175,23 +1181,23 @@
 <tbody>
 <tr class="odd">
 <td style="text-align: left;">boxLengthIsValid</td>
 <td style="text-align: left;">(Size of box – 8) /4 is a whole number (integer)</td>
 </tr>
 <tr class="even">
 <td style="text-align: left;">brandIsValid</td>
-<td style="text-align: left;"><em>br</em> equals 0x6a703220 (“jp2”)</td>
+<td style="text-align: left;"><em>br</em> equals 0x6a703220 (“jp2”) for JP2, or 0x6a706820 (“jph”)for JPH</td>
 </tr>
 <tr class="odd">
 <td style="text-align: left;">minorVersionIsValid</td>
 <td style="text-align: left;"><em>minV</em> equals 0</td>
 </tr>
 <tr class="even">
 <td style="text-align: left;">compatibilityListIsValid</td>
-<td style="text-align: left;">Sequence of compatibility (<em>cL</em>) fields includes one entry that equals 0x6a703220 (“jp2”)</td>
+<td style="text-align: left;">Sequence of compatibility (<em>cL</em>) fields includes one entry that equals 0x6a703220 (“jp2”) for JP2, or 0x6a706820 (“jph”)for JPH</td>
 </tr>
 </tbody>
 </table>
 
 
 <h2 id="jp2-header-box">JP2 Header box (superbox)</h2>
 
@@ -1306,14 +1312,18 @@
 <td style="text-align: left;">colourSpecificationBoxesAreContiguous</td>
 <td style="text-align: left;">In case of multiple Colour Specification boxes, they appear contiguously in the JP2 Header box</td>
 </tr>
 <tr class="even">
 <td style="text-align: left;">paletteAndComponentMappingBoxesOnlyTogether</td>
 <td style="text-align: left;">Box contains a Palette box (only if Component Mapping box is present); box contains a Component Mapping box (only if Palette box is present)</td>
 </tr>
+<tr class="odd">
+<td style="text-align: left;">noZeroCTypesIfNoColourBox</td>
+<td style="text-align: left;">If file does not contain a Colour Specification Box, no cTyp values (from Channel definition box) shall be equal to 0 (JPH)</td>
+</tr>
 </tbody>
 </table>
 
 
 <h2 id="image-header-box">Image Header box (child of JP2 Header box)</h2>
 
 
@@ -1495,32 +1505,48 @@
 <th style="text-align: left;">Property</th>
 <th style="text-align: left;">Description</th>
 </tr>
 </thead>
 <tbody>
 <tr class="odd">
 <td style="text-align: left;">meth</td>
-<td style="text-align: left;">Specification method. Indicates whether colourspace of this image is defined as an enumerated colourspace or using a (restricted) ICC profile.</td>
+<td style="text-align: left;">Specification method. Indicates how the colourspace is defined (enumerated colourspace, or restricted ICC profile for JP2, with additional Any ICC and Parameterized Colourspace methods for JPH.</td>
 </tr>
 <tr class="even">
 <td style="text-align: left;">prec</td>
 <td style="text-align: left;">Precedence</td>
 </tr>
 <tr class="odd">
 <td style="text-align: left;">approx</td>
 <td style="text-align: left;">Colourspace approximation</td>
 </tr>
 <tr class="even">
 <td style="text-align: left;">enumCS (if meth equals “Enumerated”)</td>
 <td style="text-align: left;">Enumerated colourspace (as descriptive text string)</td>
 </tr>
 <tr class="odd">
-<td style="text-align: left;">icc (if meth equals “Restricted ICC” or “Any ICC”<a href="#fn4" class="footnote-ref" id="fnref4" role="doc-noteref"><sup>4</sup></a>)</td>
+<td style="text-align: left;">icc (if meth equals “Restricted ICC” or “Any ICC”)</td>
 <td style="text-align: left;">Properties of ICC profile as child element (see below)</td>
 </tr>
+<tr class="even">
+<td style="text-align: left;">colPrims (if meth equals “Parameterized Colourspace”)</td>
+<td style="text-align: left;">ColourPrimaries value (JPH)<a href="#fn5" class="footnote-ref" id="fnref5" role="doc-noteref"><sup>5</sup></a>.</td>
+</tr>
+<tr class="odd">
+<td style="text-align: left;">transfC (if meth equals “Parameterized Colourspace”)</td>
+<td style="text-align: left;">TransferCharacteristics value (JPH)<a href="#fn6" class="footnote-ref" id="fnref6" role="doc-noteref"><sup>6</sup></a></td>
+</tr>
+<tr class="even">
+<td style="text-align: left;">matCoeffs (if meth equals “Parameterized Colourspace”)</td>
+<td style="text-align: left;">MatrixCoefficients value (JPH)<a href="#fn7" class="footnote-ref" id="fnref7" role="doc-noteref"><sup>7</sup></a></td>
+</tr>
+<tr class="odd">
+<td style="text-align: left;">vidFRng (if meth equals “Parameterized Colourspace”)</td>
+<td style="text-align: left;">VideoFullRangeFlag (“yes”/”no”) (JPH)<a href="#fn8" class="footnote-ref" id="fnref8" role="doc-noteref"><sup>8</sup></a></td>
+</tr>
 </tbody>
 </table>
 
 
 <h3 id="reported-properties-of-icc-profiles">Reported properties of ICC profiles</h3>
 
 
@@ -1668,20 +1694,32 @@
 </tr>
 <tr class="odd">
 <td style="text-align: left;">iccSizeIsValid (if meth equals “Restricted ICC”)</td>
 <td style="text-align: left;">Actual size of embedded ICC profile equals value of profileSize field in ICC header</td>
 </tr>
 <tr class="even">
 <td style="text-align: left;">iccPermittedProfileClass (if meth equals “Restricted ICC”)</td>
-<td style="text-align: left;">ICC profile class is “input device” or “display device”<a href="#fn5" class="footnote-ref" id="fnref5" role="doc-noteref"><sup>5</sup></a></td>
+<td style="text-align: left;">ICC profile class is “input device” or “display device”<a href="#fn9" class="footnote-ref" id="fnref9" role="doc-noteref"><sup>9</sup></a></td>
 </tr>
 <tr class="odd">
 <td style="text-align: left;">iccNoLUTBasedProfile (if meth equals “Restricted ICC”)</td>
 <td style="text-align: left;">ICC profile type is not N-component LUT based (which is not allowed in JP2)</td>
 </tr>
+<tr class="even">
+<td style="text-align: left;">colPrimsIsValid</td>
+<td style="text-align: left;"><em>colPrims</em> value is defined by ITU-T H.273 / ISO/IEC 23001-8 (JPH)</td>
+</tr>
+<tr class="odd">
+<td style="text-align: left;">transfCIsValid</td>
+<td style="text-align: left;"><em>transfC</em> value is defined by ITU-T H.273 / ISO/IEC 23001-8 (JPH)</td>
+</tr>
+<tr class="even">
+<td style="text-align: left;">matCoeffsIsValid</td>
+<td style="text-align: left;"><em>matCoeffs</em> value is defined by ITU-T H.273 / ISO/IEC 23001-8 (JPH)</td>
+</tr>
 </tbody>
 </table>
 
 
 <h2 id="palette-box">Palette box (child of JP2 Header box)</h2>
 
 
@@ -1886,20 +1924,28 @@
 </tr>
 <tr class="odd">
 <td style="text-align: left;">cNIsValid<sup>*</sup></td>
 <td style="text-align: left;"><em>cN</em> is within range [0, 65535] (repeated for all channels)</td>
 </tr>
 <tr class="even">
 <td style="text-align: left;">cTypIsValid<sup>*</sup></td>
-<td style="text-align: left;"><em>cType</em> is within range [0, 65535] (repeated for all channels)</td>
+<td style="text-align: left;"><em>cType</em> is one of the values defined in Table I.16 (repeated for all channels)<a href="#fn10" class="footnote-ref" id="fnref10" role="doc-noteref"><sup>10</sup></a></td>
 </tr>
 <tr class="odd">
 <td style="text-align: left;">cAssocIsValid<sup>*</sup></td>
 <td style="text-align: left;"><em>cAssoc</em> is within range [0, 65535] (repeated for all channels)</td>
 </tr>
+<tr class="even">
+<td style="text-align: left;">noMoreThanOneAlphaChannel</td>
+<td style="text-align: left;">At most one <em>cTyp</em> field is equal to 1 or 2 (JPH)</td>
+</tr>
+<tr class="odd">
+<td style="text-align: left;">cAssocAlphaChannelIsZero</td>
+<td style="text-align: left;">If <em>cTyp</em> is 1 or 2, the corresponding <em>cAssoc</em> value equals 0 (JPH)</td>
+</tr>
 </tbody>
 </table>
 
 
 <h2 id="resolution-box">Resolution box (child of JP2 Header box, superbox)</h2>
 
 
@@ -2013,27 +2059,27 @@
 </tr>
 <tr class="even">
 <td style="text-align: left;">hRcE</td>
 <td style="text-align: left;">Horizontal grid resolution exponent</td>
 </tr>
 <tr class="odd">
 <td style="text-align: left;">vRescInPixelsPerMeter</td>
-<td style="text-align: left;">Vertical grid resolution, expressed in pixels per meter<a href="#fn6" class="footnote-ref" id="fnref6" role="doc-noteref"><sup>6</sup></a></td>
+<td style="text-align: left;">Vertical grid resolution, expressed in pixels per meter<a href="#fn11" class="footnote-ref" id="fnref11" role="doc-noteref"><sup>11</sup></a></td>
 </tr>
 <tr class="even">
 <td style="text-align: left;">hRescInPixelsPerMeter</td>
-<td style="text-align: left;">Horizontal grid resolution, expressed in pixels per meter<a href="#fn7" class="footnote-ref" id="fnref7" role="doc-noteref"><sup>7</sup></a></td>
+<td style="text-align: left;">Horizontal grid resolution, expressed in pixels per meter<a href="#fn12" class="footnote-ref" id="fnref12" role="doc-noteref"><sup>12</sup></a></td>
 </tr>
 <tr class="odd">
 <td style="text-align: left;">vRescInPixelsPerInch</td>
-<td style="text-align: left;">Vertical grid resolution, expressed in pixels per inch<a href="#fn8" class="footnote-ref" id="fnref8" role="doc-noteref"><sup>8</sup></a></td>
+<td style="text-align: left;">Vertical grid resolution, expressed in pixels per inch<a href="#fn13" class="footnote-ref" id="fnref13" role="doc-noteref"><sup>13</sup></a></td>
 </tr>
 <tr class="even">
 <td style="text-align: left;">hRescInPixelsPerInch</td>
-<td style="text-align: left;">Horizontal grid resolution, expressed in pixels per inch<a href="#fn9" class="footnote-ref" id="fnref9" role="doc-noteref"><sup>9</sup></a></td>
+<td style="text-align: left;">Horizontal grid resolution, expressed in pixels per inch<a href="#fn14" class="footnote-ref" id="fnref14" role="doc-noteref"><sup>14</sup></a></td>
 </tr>
 </tbody>
 </table>
 
 
 <h3 id="tests-10">Tests</h3>
 
@@ -2126,27 +2172,27 @@
 </tr>
 <tr class="even">
 <td style="text-align: left;">hRdE</td>
 <td style="text-align: left;">Horizontal grid resolution exponent</td>
 </tr>
 <tr class="odd">
 <td style="text-align: left;">vResdInPixelsPerMeter</td>
-<td style="text-align: left;">Vertical grid resolution, expressed in pixels per meter<a href="#fn10" class="footnote-ref" id="fnref10" role="doc-noteref"><sup>10</sup></a></td>
+<td style="text-align: left;">Vertical grid resolution, expressed in pixels per meter<a href="#fn15" class="footnote-ref" id="fnref15" role="doc-noteref"><sup>15</sup></a></td>
 </tr>
 <tr class="even">
 <td style="text-align: left;">hResdInPixelsPerMeter</td>
-<td style="text-align: left;">Horizontal grid resolution, expressed in pixels per meter<a href="#fn11" class="footnote-ref" id="fnref11" role="doc-noteref"><sup>11</sup></a></td>
+<td style="text-align: left;">Horizontal grid resolution, expressed in pixels per meter<a href="#fn16" class="footnote-ref" id="fnref16" role="doc-noteref"><sup>16</sup></a></td>
 </tr>
 <tr class="odd">
 <td style="text-align: left;">vResdInPixelsPerInch</td>
-<td style="text-align: left;">Vertical grid resolution, expressed in pixels per inch<a href="#fn12" class="footnote-ref" id="fnref12" role="doc-noteref"><sup>12</sup></a></td>
+<td style="text-align: left;">Vertical grid resolution, expressed in pixels per inch<a href="#fn17" class="footnote-ref" id="fnref17" role="doc-noteref"><sup>17</sup></a></td>
 </tr>
 <tr class="even">
 <td style="text-align: left;">hResdInPixelsPerInch</td>
-<td style="text-align: left;">Horizontal grid resolution, expressed in pixels per inch<a href="#fn13" class="footnote-ref" id="fnref13" role="doc-noteref"><sup>13</sup></a></td>
+<td style="text-align: left;">Horizontal grid resolution, expressed in pixels per inch<a href="#fn18" class="footnote-ref" id="fnref18" role="doc-noteref"><sup>18</sup></a></td>
 </tr>
 </tbody>
 </table>
 
 
 <h3 id="tests-11">Tests</h3>
 
@@ -2242,15 +2288,15 @@
 
 <p>Note that <em>jpylyzer</em> does not check whether the XML is <em>valid</em>, as this is not required by the standard. Besides, doing so would make <em>jpylyzer</em> significantly slower for XML that contains references to external schemas and DTDs.</p>
 
 
 <h2 id="uuid-box">UUID box</h2>
 
 
-<p>This (optional) box contains additional (binary) information, which may be vendor-specific. Some applications (e.g. Kakadu and ExifTool) also use this box for storing XMP metadata (see Section 1.1.4 in Part 3 of the XMP specification<a href="#fn14" class="footnote-ref" id="fnref14" role="doc-noteref"><sup>14</sup></a>).</p>
+<p>This (optional) box contains additional (binary) information, which may be vendor-specific. Some applications (e.g. Kakadu and ExifTool) also use this box for storing XMP metadata (see Section 1.1.4 in Part 3 of the XMP specification<a href="#fn19" class="footnote-ref" id="fnref19" role="doc-noteref"><sup>19</sup></a>).</p>
 
 
 <h3 id="element-name-13">Element name</h3>
 
 
 <p>uuidBox</p>
 
@@ -2830,15 +2876,15 @@
 
 <p>The optional markers that are marked with an asterisk above are only minimally supported at this stage: if <em>jpylyzer</em> encounters them, it will include the corresponding element in the <em>properties</em> element of the output. However, <em>jpylyzer</em> does not analyse the contents of these marker segments, which means that the respective elements in the output will be empty.</p>
 
 
 <h3 id="bit-streams">Bit streams</h3>
 
 
-<p>In addition to the above limitations, <em>jpylyzer</em> can <em>not</em> be used to establish whether the data in the bitstream are correct (this would require decoding the compressed image data, which is completely out of <em>jpylyzer</em>’s scope)<a href="#fn15" class="footnote-ref" id="fnref15" role="doc-noteref"><sup>15</sup></a>. As a result, if <em>jpylyzer</em> is used as part of a quality assurance workflow, it is recommended to also include an additional check on the image contents<a href="#fn16" class="footnote-ref" id="fnref16" role="doc-noteref"><sup>16</sup></a>. Also, <em>jpylyzer</em> does not perform any checks on marker segments within the bit-stream: start-of packet (SOP) and end-of-packet (EPH) markers.</p>
+<p>In addition to the above limitations, <em>jpylyzer</em> can <em>not</em> be used to establish whether the data in the bitstream are correct (this would require decoding the compressed image data, which is completely out of <em>jpylyzer</em>’s scope)<a href="#fn20" class="footnote-ref" id="fnref20" role="doc-noteref"><sup>20</sup></a>. As a result, if <em>jpylyzer</em> is used as part of a quality assurance workflow, it is recommended to also include an additional check on the image contents<a href="#fn21" class="footnote-ref" id="fnref21" role="doc-noteref"><sup>21</sup></a>. Also, <em>jpylyzer</em> does not perform any checks on marker segments within the bit-stream: start-of packet (SOP) and end-of-packet (EPH) markers.</p>
 
 
 <h3 id="detection-of-incomplete-or-truncated-codestreams">Detection of incomplete or truncated codestreams</h3>
 
 
 <p>A JP2’s tile part header contains information that makes it possible to detect incomplete and truncated codestreams in most cases. Depending on the encoder software used, this method may fail for images that only contain one single tile part (i.e. images that do not contain tiling).</p>
 
@@ -2977,38 +3023,50 @@
 <td style="text-align: left;">First 2 bytes in codestream constitute a start of codestream (SOC) marker segment</td>
 </tr>
 <tr class="even">
 <td style="text-align: left;">foundSIZMarker</td>
 <td style="text-align: left;">Second marker segment in codestream is image and tile size (SIZ) marker segment</td>
 </tr>
 <tr class="odd">
+<td style="text-align: left;">foundCAPMarker</td>
+<td style="text-align: left;">Codestream main header contains Extended Capabilities (CAP) marker segment if second most significant bit of <em>rsiz</em> equals 1</td>
+</tr>
+<tr class="even">
 <td style="text-align: left;">foundCODMarker</td>
 <td style="text-align: left;">Codestream main header contains coding style default (COD) marker segment</td>
 </tr>
-<tr class="even">
+<tr class="odd">
 <td style="text-align: left;">foundQCDMarker</td>
 <td style="text-align: left;">Codestream main header contains quantization default (QCD) marker segment</td>
 </tr>
+<tr class="even">
+<td style="text-align: left;">CPFnumConsistentWithPRFnum</td>
+<td style="text-align: left;">Value of <em>CPFnum</em> in CPF marker segment is consistent with <em>PRFnum</em> value in PRF marker segment</td>
+</tr>
 <tr class="odd">
+<td style="text-align: left;">CPFnumConsistentWithRsiz</td>
+<td style="text-align: left;">Value of <em>CPFnum</em> in CPF marker segment is consistent with *rsiz^ value in SIZ marker segment</td>
+</tr>
+<tr class="even">
 <td style="text-align: left;">foundExpectedNumberOfTiles</td>
 <td style="text-align: left;">Number of encountered tiles is consistent with expected number of tiles (as calculated from <a href="#siz-marker">SIZ marker</a>)</td>
 </tr>
-<tr class="even">
+<tr class="odd">
 <td style="text-align: left;">foundExpectedNumberOfTileParts</td>
 <td style="text-align: left;">For all tiles, number of encountered tile parts is consistent with expected number of tile parts (values of <em>tnsot</em> from <a href="#sot-marker">SOT marker</a>)</td>
 </tr>
-<tr class="odd">
-<td style="text-align: left;">maxOneCcocPerComponent</td>
-<td style="text-align: left;">No more than one <em>ccoc</em> value for each component (only reported if codestream contains any COC marker segments)</td>
-</tr>
 <tr class="even">
-<td style="text-align: left;">maxOneCqccPerComponent</td>
-<td style="text-align: left;">No more than one <em>cqcc</em> value for each component (only reported if codestream contains any QCC marker segments)</td>
+<td style="text-align: left;">maxOneCcocPerComponentMain</td>
+<td style="text-align: left;">No more than one <em>ccoc</em> value for each component in main header (only reported if codestream contains any COC marker segments)</td>
 </tr>
 <tr class="odd">
+<td style="text-align: left;">maxOneCqccPerComponentMain</td>
+<td style="text-align: left;">No more than one <em>cqcc</em> value for each component in main header (only reported if codestream contains any QCC marker segments)</td>
+</tr>
+<tr class="even">
 <td style="text-align: left;">foundEOCMarker</td>
 <td style="text-align: left;">Last 2 bytes in codestream constitute an end of codestream (EOC) marker segment</td>
 </tr>
 </tbody>
 </table>
 
 
@@ -3034,69 +3092,73 @@
 <tbody>
 <tr class="odd">
 <td style="text-align: left;">lsiz</td>
 <td style="text-align: left;">Length of SIZ marker segment in bytes</td>
 </tr>
 <tr class="even">
 <td style="text-align: left;">rsiz</td>
-<td style="text-align: left;">Decoder capabilities</td>
+<td style="text-align: left;">Numerical value of <em>rsiz</em> (capabilities) field</td>
 </tr>
 <tr class="odd">
+<td style="text-align: left;">capability</td>
+<td style="text-align: left;">Capabilities (profile) encoded by <em>rsiz</em> value</td>
+</tr>
+<tr class="even">
 <td style="text-align: left;">xsiz</td>
 <td style="text-align: left;">Width of reference grid</td>
 </tr>
-<tr class="even">
+<tr class="odd">
 <td style="text-align: left;">ysiz</td>
 <td style="text-align: left;">Height of reference grid</td>
 </tr>
-<tr class="odd">
+<tr class="even">
 <td style="text-align: left;">xOsiz</td>
 <td style="text-align: left;">Horizontal offset from origin of reference grid to left of image area</td>
 </tr>
-<tr class="even">
+<tr class="odd">
 <td style="text-align: left;">yOsiz</td>
 <td style="text-align: left;">Vertical offset from origin of reference grid to top of image area</td>
 </tr>
-<tr class="odd">
+<tr class="even">
 <td style="text-align: left;">xTsiz</td>
 <td style="text-align: left;">Width of one reference tile with respect to the reference grid</td>
 </tr>
-<tr class="even">
+<tr class="odd">
 <td style="text-align: left;">yTsiz</td>
 <td style="text-align: left;">Height of one reference tile with respect to the reference grid</td>
 </tr>
-<tr class="odd">
+<tr class="even">
 <td style="text-align: left;">xTOsiz</td>
 <td style="text-align: left;">Horizontal offset from origin of reference grid to left side of first tile</td>
 </tr>
-<tr class="even">
+<tr class="odd">
 <td style="text-align: left;">yTOsiz</td>
 <td style="text-align: left;">Vertical offset from origin of reference grid to top side of first tile</td>
 </tr>
-<tr class="odd">
+<tr class="even">
 <td style="text-align: left;">numberOfTiles</td>
-<td style="text-align: left;">Number of tiles<a href="#fn17" class="footnote-ref" id="fnref17" role="doc-noteref"><sup>17</sup></a></td>
+<td style="text-align: left;">Number of tiles<a href="#fn22" class="footnote-ref" id="fnref22" role="doc-noteref"><sup>22</sup></a></td>
 </tr>
-<tr class="even">
+<tr class="odd">
 <td style="text-align: left;">csiz</td>
 <td style="text-align: left;">Number of components</td>
 </tr>
-<tr class="odd">
+<tr class="even">
 <td style="text-align: left;">ssizSign<sup>*</sup></td>
 <td style="text-align: left;">Indicates whether image component is signed or unsigned (repeated for all components)</td>
 </tr>
-<tr class="even">
+<tr class="odd">
 <td style="text-align: left;">ssizDepth<sup>*</sup></td>
 <td style="text-align: left;">Number of bits for this component (repeated for all components)</td>
 </tr>
-<tr class="odd">
+<tr class="even">
 <td style="text-align: left;">xRsiz<sup>*</sup></td>
 <td style="text-align: left;">Horizontal separation of sample of this component with respect to reference grid (repeated for all components)</td>
 </tr>
-<tr class="even">
+<tr class="odd">
 <td style="text-align: left;">yRsiz<sup>*</sup></td>
 <td style="text-align: left;">Vertical separation of sample of this component with respect to reference grid (repeated for all components)</td>
 </tr>
 </tbody>
 </table>
 
 
@@ -3113,15 +3175,15 @@
 <tbody>
 <tr class="odd">
 <td style="text-align: left;">lsizIsValid</td>
 <td style="text-align: left;"><em>lsiz</em> is within range [41,49190]</td>
 </tr>
 <tr class="even">
 <td style="text-align: left;">rsizIsValid</td>
-<td style="text-align: left;"><em>rsiz</em> equals 0 (“ISO/IEC 15444-1”), 1 (“Profile 0”) or 2 (“Profile 1”)</td>
+<td style="text-align: left;">Four most significant bits of <em>rsiz</em> are 0 (JP2, J2C); second most significant bit of <em>rsiz</em> equals 1 (JPH, JHC)</td>
 </tr>
 <tr class="odd">
 <td style="text-align: left;">xsizIsValid</td>
 <td style="text-align: left;"><em>xsiz</em> is within range [1,2<sup>32</sup> - 1]</td>
 </tr>
 <tr class="even">
 <td style="text-align: left;">ysizIsValid</td>
@@ -3237,31 +3299,31 @@
 </tr>
 <tr class="odd">
 <td style="text-align: left;">codingBypass</td>
 <td style="text-align: left;">Indicates use of coding bypass (“yes”/“no”)</td>
 </tr>
 <tr class="even">
 <td style="text-align: left;">resetOnBoundaries</td>
-<td style="text-align: left;">Indicates reset of context probabilities on coding pass boundaries (“yes”/“no”)</td>
+<td style="text-align: left;">Indicates reset of context probabilities on coding pass boundaries (“yes”/“no”) (does not apply to High Throughput code blocks)</td>
 </tr>
 <tr class="odd">
 <td style="text-align: left;">termOnEachPass</td>
 <td style="text-align: left;">Indicates termination on each coding pass (“yes”/“no”)</td>
 </tr>
 <tr class="even">
 <td style="text-align: left;">vertCausalContext</td>
 <td style="text-align: left;">Indicates vertically causal context (“yes”/“no”)</td>
 </tr>
 <tr class="odd">
 <td style="text-align: left;">predTermination</td>
-<td style="text-align: left;">Indicates predictable termination (“yes”/“no”)</td>
+<td style="text-align: left;">Indicates predictable termination (“yes”/“no”) (does not apply to High Throughput code blocks)</td>
 </tr>
 <tr class="even">
 <td style="text-align: left;">segmentationSymbols</td>
-<td style="text-align: left;">Indicates use of segmentation symbols (“yes”/“no”)</td>
+<td style="text-align: left;">Indicates use of segmentation symbols (“yes”/“no”) (does not apply to High Throughput code blocks)</td>
 </tr>
 <tr class="odd">
 <td style="text-align: left;">transformation</td>
 <td style="text-align: left;">Wavelet transformation: “9-7 irreversible” or “5-3 reversible”</td>
 </tr>
 <tr class="even">
 <td style="text-align: left;">precinctSizeX<sup>*</sup></td>
@@ -3530,15 +3592,15 @@
 </tr>
 <tr class="odd">
 <td style="text-align: left;">roiStyleIsValid</td>
 <td style="text-align: left;"><em>roiStyle</em> equals 0 (“Implicit ROI (maximum shift)”)</td>
 </tr>
 <tr class="even">
 <td style="text-align: left;">roiShiftIsValid</td>
-<td style="text-align: left;"><em>roiShift</em> is within range [0,255]</td>
+<td style="text-align: left;"><em>roiShift</em> is within range [0,255] (JP2, J2C) or [0,37] (JPH, JHC)</td>
 </tr>
 </tbody>
 </table>
 
 
 <h2 id="qcd-marker">Quantization default (QCD) marker segment</h2>
 
@@ -3895,27 +3957,223 @@
 <td style="text-align: left;">commentIsValid</td>
 <td style="text-align: left;">Comment is valid ISO/IEC8859-15 and does not contain control characters, other than tab, newline or carriage return</td>
 </tr>
 </tbody>
 </table>
 
 
+<h2 id="cap-marker">Extended capabilities (CAP) marker segment</h2>
+
+
+<p>This marker segment is defined in ISO/IEC 15444-2, and is used by ISO/IEC 15444-15 (as well as other parts of the standard).</p>
+
+
+<h3 id="element-name-29">Element name</h3>
+
+
+<p>cap</p>
+
+
+<h3 id="reported-properties-29">Reported properties</h3>
+
+
+<table>
+<thead>
+<tr class="header">
+<th style="text-align: left;">Property</th>
+<th style="text-align: left;">Description</th>
+</tr>
+</thead>
+<tbody>
+<tr class="odd">
+<td style="text-align: left;">lcap</td>
+<td style="text-align: left;">Length of CAP marker segment in bytes</td>
+</tr>
+<tr class="even">
+<td style="text-align: left;">pcapPart</td>
+<td style="text-align: left;">Indicates the use of capabilities from Part <em>pcapPart</em> of the ISO/IEC 15444 standard (repeated for all referenced parts)</td>
+</tr>
+<tr class="odd">
+<td style="text-align: left;">htCodeBlocks</td>
+<td style="text-align: left;">See section 8.2 of ISO/IEC 15444-15 (JPH, JHC)</td>
+</tr>
+<tr class="even">
+<td style="text-align: left;">htSets</td>
+<td style="text-align: left;">See section 8.3 of ISO/IEC 15444-15 (JPH, JHC)</td>
+</tr>
+<tr class="odd">
+<td style="text-align: left;">htRegion</td>
+<td style="text-align: left;">See section 8.4 of ISO/IEC 15444-15 (JPH, JHC)</td>
+</tr>
+<tr class="even">
+<td style="text-align: left;">htHomogeneous</td>
+<td style="text-align: left;">See section 8.5 of ISO/IEC 15444-15 (JPH, JHC)</td>
+</tr>
+<tr class="odd">
+<td style="text-align: left;">htReversible</td>
+<td style="text-align: left;">See section 8.7.2 of ISO/IEC 15444-15 (JPH, JHC)</td>
+</tr>
+<tr class="even">
+<td style="text-align: left;">htB</td>
+<td style="text-align: left;">Parameter <em>B</em> as used in <em>MAGBP</em> sets, see sections A.3.7 and 8.7.3 of ISO/IEC 15444-15 (JPH, JHC)</td>
+</tr>
+</tbody>
+</table>
+
+
+<h3 id="tests-28">Tests</h3>
+
+
+<table>
+<thead>
+<tr class="header">
+<th style="text-align: left;">Test name</th>
+<th style="text-align: left;">True if</th>
+</tr>
+</thead>
+<tbody>
+<tr class="odd">
+<td style="text-align: left;">lcapIsValid</td>
+<td style="text-align: left;">Number of <em>pcapPart</em> entries equals (<em>lcap</em> - 6)/2</td>
+</tr>
+<tr class="even">
+<td style="text-align: left;">pcap15IsValid</td>
+<td style="text-align: left;">15th most significant bit of <em>pcap</em> equals 1 (JPH, JHC)</td>
+</tr>
+</tbody>
+</table>
+
+
+<h2 id="prf-marker">Profile (PRF) marker segment</h2>
+
+
+<h3 id="element-name-30">Element name</h3>
+
+
+<p>prf</p>
+
+
+<h3 id="reported-properties-30">Reported properties</h3>
+
+
+<table>
+<thead>
+<tr class="header">
+<th style="text-align: left;">Property</th>
+<th style="text-align: left;">Description</th>
+</tr>
+</thead>
+<tbody>
+<tr class="odd">
+<td style="text-align: left;">lprf</td>
+<td style="text-align: left;">Length of PRF marker segment in bytes</td>
+</tr>
+<tr class="even">
+<td style="text-align: left;">PRFnum</td>
+<td style="text-align: left;">Profile number</td>
+</tr>
+</tbody>
+</table>
+
+
+<h3 id="tests-29">Tests</h3>
+
+
+<table>
+<thead>
+<tr class="header">
+<th style="text-align: left;">Test name</th>
+<th style="text-align: left;">True if</th>
+</tr>
+</thead>
+<tbody>
+<tr class="odd">
+<td style="text-align: left;">lprfIsValid</td>
+<td style="text-align: left;"><em>lprf</em> is within range [4,65534]</td>
+</tr>
+<tr class="even">
+<td style="text-align: left;">pprfIsValid</td>
+<td style="text-align: left;">last <em>pprf</em> value is not zero</td>
+</tr>
+<tr class="odd">
+<td style="text-align: left;">PRFnumIsValid</td>
+<td style="text-align: left;"><em>PRFnum</em> &gt; 4095</td>
+</tr>
+</tbody>
+</table>
+
+
+<h2 id="cpf-marker">Corresponding profile (CPF) marker segment</h2>
+
+
+<h3 id="element-name-31">Element name</h3>
+
+
+<p>cpf</p>
+
+
+<h3 id="reported-properties-31">Reported properties</h3>
+
+
+<table>
+<thead>
+<tr class="header">
+<th style="text-align: left;">Property</th>
+<th style="text-align: left;">Description</th>
+</tr>
+</thead>
+<tbody>
+<tr class="odd">
+<td style="text-align: left;">lcpf</td>
+<td style="text-align: left;">Length of CPF marker segment in bytes</td>
+</tr>
+<tr class="even">
+<td style="text-align: left;">CPFnum</td>
+<td style="text-align: left;">Profile number</td>
+</tr>
+</tbody>
+</table>
+
+
+<h3 id="tests-30">Tests</h3>
+
+
+<table>
+<thead>
+<tr class="header">
+<th style="text-align: left;">Test name</th>
+<th style="text-align: left;">True if</th>
+</tr>
+</thead>
+<tbody>
+<tr class="odd">
+<td style="text-align: left;">lcpfIsValid</td>
+<td style="text-align: left;"><em>lcpf</em> is within range [4,65534] (JPH, JHC)</td>
+</tr>
+<tr class="even">
+<td style="text-align: left;">pcpfIsValid</td>
+<td style="text-align: left;">last <em>pcpf</em> value is not zero (JPH, JHC)</td>
+</tr>
+</tbody>
+</table>
+
+
 <h2 id="tile-part">Tile part (child of Contiguous Codestream box)</h2>
 
 
 <p>Tile-part level properties and tests. This is not a box or a marker segment!</p>
 
 
-<h3 id="element-name-29">Element name</h3>
+<h3 id="element-name-32">Element name</h3>
 
 
 <p>tilePart (child of tileParts)</p>
 
 
-<h3 id="reported-properties-29">Reported properties</h3>
+<h3 id="reported-properties-32">Reported properties</h3>
 
 
 <p>Each tile part element can contain a number of child elements:</p>
 
 
 <table>
 <thead>
@@ -3988,47 +4246,75 @@
 <td style="text-align: left;">pptCount</td>
 <td style="text-align: left;">Number of PPT markers in tile part header</td>
 </tr>
 </tbody>
 </table>
 
 
-<h3 id="tests-28">Tests</h3>
+<h3 id="tests-31">Tests</h3>
 
 
 <table>
 <thead>
 <tr class="header">
 <th style="text-align: left;">Test name</th>
 <th style="text-align: left;">True if</th>
 </tr>
 </thead>
 <tbody>
 <tr class="odd">
+<td style="text-align: left;">CODAllowed</td>
+<td style="text-align: left;">COD marker is allowed in this tile part (only allowed in first tile-part of a tile)</td>
+</tr>
+<tr class="even">
+<td style="text-align: left;">COCAllowed</td>
+<td style="text-align: left;">COC marker is allowed in this tile part (only allowed in first tile-part of a tile)</td>
+</tr>
+<tr class="odd">
+<td style="text-align: left;">QCDAllowed</td>
+<td style="text-align: left;">QCD marker is allowed in this tile part (only allowed in first tile-part of a tile)</td>
+</tr>
+<tr class="even">
+<td style="text-align: left;">QCCAllowed</td>
+<td style="text-align: left;">QCC marker is allowed in this tile part (only allowed in first tile-part of a tile)</td>
+</tr>
+<tr class="odd">
+<td style="text-align: left;">RGNAllowed</td>
+<td style="text-align: left;">RGN marker is allowed in this tile part (only allowed in first tile-part of a tile)</td>
+</tr>
+<tr class="even">
+<td style="text-align: left;">maxOneCcocPerComponentTP</td>
+<td style="text-align: left;">No more than one <em>ccoc</em> value for each component in tile-part header (only reported if codestream contains any COC marker segments)</td>
+</tr>
+<tr class="odd">
+<td style="text-align: left;">maxOneCqccPerComponentTP</td>
+<td style="text-align: left;">No more than one <em>cqcc</em> value for each component in tile-part header (only reported if codestream contains any QCC marker segments)</td>
+</tr>
+<tr class="even">
 <td style="text-align: left;">foundNextTilePartOrEOC</td>
 <td style="text-align: left;">Tile part start offset + <em>tilePartLength</em> points to either start of new tile or EOC marker (useful for detecting within-codestream byte corruption)</td>
 </tr>
-<tr class="even">
+<tr class="odd">
 <td style="text-align: left;">foundSODMarker</td>
 <td style="text-align: left;">Last marker segment of tile part is a start-of-data (SOD) marker</td>
 </tr>
 </tbody>
 </table>
 
 
 <h2 id="sot-marker">Start of tile part (SOT) marker segment (child of tile part)</h2>
 
 
-<h3 id="element-name-30">Element name</h3>
+<h3 id="element-name-33">Element name</h3>
 
 
 <p>sot</p>
 
 
-<h3 id="reported-properties-30">Reported properties</h3>
+<h3 id="reported-properties-33">Reported properties</h3>
 
 
 <table>
 <thead>
 <tr class="header">
 <th style="text-align: left;">Property</th>
 <th style="text-align: left;">Description</th>
@@ -4055,15 +4341,15 @@
 <td style="text-align: left;">tnsot</td>
 <td style="text-align: left;">Number of tile-parts of a tile in the codestream (value of 0 indicates that number of tile-parts of tile in the codestream is not defined in current header)</td>
 </tr>
 </tbody>
 </table>
 
 
-<h3 id="tests-29">Tests</h3>
+<h3 id="tests-32">Tests</h3>
 
 
 <table>
 <thead>
 <tr class="header">
 <th style="text-align: left;">Test name</th>
 <th style="text-align: left;">True if</th>
@@ -4095,21 +4381,21 @@
 
 <p>The following marker segments are only minimally supported: <em>jpylyzer</em> will report their presence in the <em>properties</em> element, but it does not perform any further tests or analyses. This may change in upcoming versions of the software.</p>
 
 
 <h2 id="tlm-marker">Tile-part lengths (TLM) marker segment</h2>
 
 
-<h3 id="element-name-31">Element name</h3>
+<h3 id="element-name-34">Element name</h3>
 
 
 <p>tlm</p>
 
 
-<h3 id="reported-properties-31">Reported properties</h3>
+<h3 id="reported-properties-34">Reported properties</h3>
 
 
 <table>
 <thead>
 <tr class="header">
 <th style="text-align: left;">Property</th>
 <th style="text-align: left;">Description</th>
@@ -4124,15 +4410,15 @@
 <td style="text-align: left;"/>
 <td style="text-align: left;"/>
 </tr>
 </tbody>
 </table>
 
 
-<h3 id="tests-30">Tests</h3>
+<h3 id="tests-33">Tests</h3>
 
 
 <table>
 <thead>
 <tr class="header">
 <th style="text-align: left;">Test name</th>
 <th style="text-align: left;">True if</th>
@@ -4150,21 +4436,21 @@
 </tbody>
 </table>
 
 
 <h2 id="plm-marker">Packet length, main header (PLM) marker segment</h2>
 
 
-<h3 id="element-name-32">Element name</h3>
+<h3 id="element-name-35">Element name</h3>
 
 
 <p>plm</p>
 
 
-<h3 id="reported-properties20">Reported properties<a href="#fn18" class="footnote-ref" id="fnref18" role="doc-noteref"><sup>18</sup></a></h3>
+<h3 id="reported-properties20">Reported properties<a href="#fn23" class="footnote-ref" id="fnref23" role="doc-noteref"><sup>23</sup></a></h3>
 
 
 <table>
 <thead>
 <tr class="header">
 <th style="text-align: left;">Property</th>
 <th style="text-align: left;">Description</th>
@@ -4187,15 +4473,15 @@
 <td style="text-align: left;">iplm</td>
 <td style="text-align: left;">Comma separated list of packet length values (as hexadecimal strings)</td>
 </tr>
 </tbody>
 </table>
 
 
-<h3 id="tests-31">Tests</h3>
+<h3 id="tests-34">Tests</h3>
 
 
 <table>
 <thead>
 <tr class="header">
 <th style="text-align: left;">Test name</th>
 <th style="text-align: left;">True if</th>
@@ -4213,21 +4499,21 @@
 </tbody>
 </table>
 
 
 <h2 id="ppm-marker">Packed packet headers, main header (PPM) marker segment</h2>
 
 
-<h3 id="element-name-33">Element name</h3>
+<h3 id="element-name-36">Element name</h3>
 
 
 <p>ppm</p>
 
 
-<h3 id="reported-properties20-1">Reported properties<a href="#fn19" class="footnote-ref" id="fnref19" role="doc-noteref"><sup>19</sup></a></h3>
+<h3 id="reported-properties20-1">Reported properties<a href="#fn24" class="footnote-ref" id="fnref24" role="doc-noteref"><sup>24</sup></a></h3>
 
 
 <table>
 <thead>
 <tr class="header">
 <th style="text-align: left;">Property</th>
 <th style="text-align: left;">Description</th>
@@ -4242,15 +4528,15 @@
 <td style="text-align: left;"/>
 <td style="text-align: left;"/>
 </tr>
 </tbody>
 </table>
 
 
-<h3 id="tests-32">Tests</h3>
+<h3 id="tests-35">Tests</h3>
 
 
 <table>
 <thead>
 <tr class="header">
 <th style="text-align: left;">Test name</th>
 <th style="text-align: left;">True if</th>
@@ -4268,21 +4554,21 @@
 </tbody>
 </table>
 
 
 <h2 id="plt-marker">Packet length, tile-part header (PLT) marker segment</h2>
 
 
-<h3 id="element-name-34">Element name</h3>
+<h3 id="element-name-37">Element name</h3>
 
 
 <p>plt</p>
 
 
-<h3 id="reported-properties20-2">Reported properties<a href="#fn20" class="footnote-ref" id="fnref20" role="doc-noteref"><sup>20</sup></a></h3>
+<h3 id="reported-properties20-2">Reported properties<a href="#fn25" class="footnote-ref" id="fnref25" role="doc-noteref"><sup>25</sup></a></h3>
 
 
 <table>
 <thead>
 <tr class="header">
 <th style="text-align: left;">Property</th>
 <th style="text-align: left;">Description</th>
@@ -4305,15 +4591,15 @@
 <td style="text-align: left;">iplt</td>
 <td style="text-align: left;">Comma separated list of packet length values (as hexadecimal strings)</td>
 </tr>
 </tbody>
 </table>
 
 
-<h3 id="tests-33">Tests</h3>
+<h3 id="tests-36">Tests</h3>
 
 
 <table>
 <thead>
 <tr class="header">
 <th style="text-align: left;">Test name</th>
 <th style="text-align: left;">True if</th>
@@ -4331,21 +4617,21 @@
 </tbody>
 </table>
 
 
 <h2 id="ppt-marker">Packed packet headers, tile-part header (PPT) marker segment</h2>
 
 
-<h3 id="element-name-35">Element name</h3>
+<h3 id="element-name-38">Element name</h3>
 
 
 <p>ppt</p>
 
 
-<h3 id="reported-properties20-3">Reported properties<a href="#fn21" class="footnote-ref" id="fnref21" role="doc-noteref"><sup>21</sup></a></h3>
+<h3 id="reported-properties20-3">Reported properties<a href="#fn26" class="footnote-ref" id="fnref26" role="doc-noteref"><sup>26</sup></a></h3>
 
 
 <table>
 <thead>
 <tr class="header">
 <th style="text-align: left;">Property</th>
 <th style="text-align: left;">Description</th>
@@ -4360,15 +4646,15 @@
 <td style="text-align: left;"/>
 <td style="text-align: left;"/>
 </tr>
 </tbody>
 </table>
 
 
-<h3 id="tests-34">Tests</h3>
+<h3 id="tests-37">Tests</h3>
 
 
 <table>
 <thead>
 <tr class="header">
 <th style="text-align: left;">Test name</th>
 <th style="text-align: left;">True if</th>
@@ -4403,30 +4689,35 @@
 
 
 <section class="footnotes" role="doc-endnotes">
 <hr/>
 <ol>
 <li id="fn1" role="doc-endnote"><p>The <em>jpylyzer</em> binaries were created using the <em>PyInstaller</em> package: <a href="https://www.pyinstaller.org/">https://www.pyinstaller.org/</a><a href="#fnref1" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
 <li id="fn2" role="doc-endnote"><p>Note that <em>jpylyzer</em> versions 1.8 and earlier returned a formatted XML string instead of an element object!<a href="#fnref2" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
-<li id="fn3" role="doc-endnote"><p>Note that <em>jpylyzer</em> versions 1.4 and earlier used the verbose output format by default. This behaviour has changed in version 1.5 onwards, as the lengthy output turned out to be slightly confusing to some users.<a href="#fnref3" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
-<li id="fn4" role="doc-endnote"><p>The “Any ICC” method is defined in ISO/IEC 15444-2 (the JPX format), and is not allowed in JP2. However, <em>jpylyzer</em> offers limited support for JPX here by also reporting the properties of ICC profiles that were embedded using this method. Note that any file that uses this method will fail the “methIsValid” test (and thereby the validation).<a href="#fnref4" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
-<li id="fn5" role="doc-endnote"><p>Originally ISO/IEC 15444-1 only allowed “input device” profiles. Support of “display device” profiles was added through an <a href="http://www.itu.int/rec/T-REC-T.800-201303-P!Amd6/en">amendment</a> to the standard in 2013. The behaviour of <em>jpylyzer</em> is consistent with this amendment.<a href="#fnref5" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
-<li id="fn6" role="doc-endnote"><p>Calculated as: <math xmlns="http://www.w3.org/1998/Math/MathML"> <mrow> <mfrac> <mrow> <mi>vRcN</mi> </mrow> <mrow> <mi>vRcD</mi> </mrow> </mfrac> <mo>•</mo> <msup> <mn>10</mn> <mi>vRcE</mi> </msup> </mrow> </math><a href="#fnref6" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
-<li id="fn7" role="doc-endnote"><p>Calculated as: <math xmlns="http://www.w3.org/1998/Math/MathML"> <mrow> <mfrac> <mrow> <mi>hRcN</mi> </mrow> <mrow> <mi>hRcD</mi> </mrow> </mfrac> <mo>•</mo> <msup> <mn>10</mn> <mi>hRcE</mi> </msup> </mrow> </math><a href="#fnref7" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
-<li id="fn8" role="doc-endnote"><p>Calculated as: <math xmlns="http://www.w3.org/1998/Math/MathML"> <mrow> <mi>vRescInPixelsPerMeter</mi> <mo>•</mo> <mn>25.4</mn> <mo>•</mo> <msup> <mn>10</mn> <mi>-3</mi> </msup> </mrow> </math><a href="#fnref8" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
-<li id="fn9" role="doc-endnote"><p>Calculated as: <math xmlns="http://www.w3.org/1998/Math/MathML"> <mrow> <mi>hRescInPixelsPerMeter</mi> <mo>•</mo> <mn>25.4</mn> <mo>•</mo> <msup> <mn>10</mn> <mi>-3</mi> </msup> </mrow> </math><a href="#fnref9" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
-<li id="fn10" role="doc-endnote"><p>Calculated as: <math xmlns="http://www.w3.org/1998/Math/MathML"> <mrow> <mfrac> <mrow> <mi>vRdN</mi> </mrow> <mrow> <mi>vRdD</mi> </mrow> </mfrac> <mo>•</mo> <msup> <mn>10</mn> <mi>vRdE</mi> </msup> </mrow> </math><a href="#fnref10" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
-<li id="fn11" role="doc-endnote"><p>Calculated as: <math xmlns="http://www.w3.org/1998/Math/MathML"> <mrow> <mfrac> <mrow> <mi>hRdN</mi> </mrow> <mrow> <mi>hRdD</mi> </mrow> </mfrac> <mo>•</mo> <msup> <mn>10</mn> <mi>hRdE</mi> </msup> </mrow> </math><a href="#fnref11" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
-<li id="fn12" role="doc-endnote"><p>Calculated as: <math xmlns="http://www.w3.org/1998/Math/MathML"> <mrow> <mi>vResdInPixelsPerMeter</mi> <mo>•</mo> <mn>25.4</mn> <mo>•</mo> <msup> <mn>10</mn> <mi>-3</mi> </msup> </mrow> </math><a href="#fnref12" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
-<li id="fn13" role="doc-endnote"><p>Calculated as: <math xmlns="http://www.w3.org/1998/Math/MathML"> <mrow> <mi>hResdInPixelsPerMeter</mi> <mo>•</mo> <mn>25.4</mn> <mo>•</mo> <msup> <mn>10</mn> <mi>-3</mi> </msup> </mrow> </math><a href="#fnref13" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
-<li id="fn14" role="doc-endnote"><p>Link: <a href="https://wwwimages.adobe.com/www.adobe.com/content/dam/Adobe/en/devnet/xmp/pdfs/cs6/XMPSpecificationPart3.pdf">https://wwwimages.adobe.com/www.adobe.com/content/dam/Adobe/en/devnet/xmp/pdfs/cs6/XMPSpecificationPart3.pdf</a><a href="#fnref14" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
-<li id="fn15" role="doc-endnote"><p>However, support for start of packet (SOP) and end of packet (EPH) markers may be included in future versions.<a href="#fnref15" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
-<li id="fn16" role="doc-endnote"><p>For example, in a TIFF to JP2 conversion workflow one could include a pixel-by-pixel comparison of the values in the TIFF and the JP2.<a href="#fnref16" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
-<li id="fn17" role="doc-endnote"><p>Calculated as: <math xmlns="http://www.w3.org/1998/Math/MathML"> <mrow> <mi>numberOfTiles</mi> <mo>=</mo> <mo>[</mo> <mfrac> <mrow> <mi>xsiz</mi> <mo>-</mo> <mi>xOsiz</mi> </mrow> <mrow> <mi>xTsiz</mi> </mrow> </mfrac> <mo>]</mo> <mo>•</mo> <mo>[</mo> <mfrac> <mrow> <mi>ysiz</mi> <mo>-</mo> <mi>yOsiz</mi> </mrow> <mrow> <mi>yTsiz</mi> </mrow> </mfrac> <mo>]</mo> </mrow> </math><a href="#fnref17" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
-<li id="fn18" role="doc-endnote"><p>Only reported if the <code>--packetmarkers</code> option is used.<a href="#fnref18" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
-<li id="fn19" role="doc-endnote"><p>Only reported if the <code>--packetmarkers</code> option is used.<a href="#fnref19" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
-<li id="fn20" role="doc-endnote"><p>Only reported if the <code>--packetmarkers</code> option is used.<a href="#fnref20" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
-<li id="fn21" role="doc-endnote"><p>Only reported if the <code>--packetmarkers</code> option is used.<a href="#fnref21" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
+<li id="fn3" role="doc-endnote"><p>Jpylyzer 2.2 and more recent only work with Python &gt; 3.2. Since Jython still hasn’t been upgraded to support Python 3, Java integration with Jython currently doesn’t work.<a href="#fnref3" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
+<li id="fn4" role="doc-endnote"><p>Note that <em>jpylyzer</em> versions 1.4 and earlier used the verbose output format by default. This behaviour has changed in version 1.5 onwards, as the lengthy output turned out to be slightly confusing to some users.<a href="#fnref4" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
+<li id="fn5" role="doc-endnote"><p>Meaning of values defined in Table 2 of Rec. ITU-T H.273 / ISO/IEC 23001-8 <a href="https://www.itu.int/rec/dologin_pub.asp?lang=e&amp;id=T-REC-H.273-202107-I!!PDF-E&amp;type=items">“Coding-independent code points for video signal type identification”</a><a href="#fnref5" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
+<li id="fn6" role="doc-endnote"><p>Meaning of values defined in Table 3 of Rec. ITU-T H.273 / ISO/IEC 23001-8 <a href="https://www.itu.int/rec/dologin_pub.asp?lang=e&amp;id=T-REC-H.273-202107-I!!PDF-E&amp;type=items">“Coding-independent code points for video signal type identification”</a><a href="#fnref6" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
+<li id="fn7" role="doc-endnote"><p>Meaning of values defined in Table 4 of Rec. ITU-T H.273 / ISO/IEC 23001-8 <a href="https://www.itu.int/rec/dologin_pub.asp?lang=e&amp;id=T-REC-H.273-202107-I!!PDF-E&amp;type=items">“Coding-independent code points for video signal type identification”</a><a href="#fnref7" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
+<li id="fn8" role="doc-endnote"><p>Meaning defined in Rec. ITU-T H.273 / ISO/IEC 23001-8 <a href="https://www.itu.int/rec/dologin_pub.asp?lang=e&amp;id=T-REC-H.273-202107-I!!PDF-E&amp;type=items">“Coding-independent code points for video signal type identification”</a><a href="#fnref8" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
+<li id="fn9" role="doc-endnote"><p>Originally ISO/IEC 15444-1 only allowed “input device” profiles. Support of “display device” profiles was added through an <a href="http://www.itu.int/rec/T-REC-T.800-201303-P!Amd6/en">amendment</a> to the standard in 2013. The behaviour of <em>jpylyzer</em> is consistent with this amendment.<a href="#fnref9" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
+<li id="fn10" role="doc-endnote"><p>For JPH, an addition “application-defined” value is allowed (ISO/IEC 15444-15, Table D.4)<a href="#fnref10" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
+<li id="fn11" role="doc-endnote"><p>Calculated as: <math xmlns="http://www.w3.org/1998/Math/MathML"> <mrow> <mfrac> <mrow> <mi>vRcN</mi> </mrow> <mrow> <mi>vRcD</mi> </mrow> </mfrac> <mo>•</mo> <msup> <mn>10</mn> <mi>vRcE</mi> </msup> </mrow> </math><a href="#fnref11" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
+<li id="fn12" role="doc-endnote"><p>Calculated as: <math xmlns="http://www.w3.org/1998/Math/MathML"> <mrow> <mfrac> <mrow> <mi>hRcN</mi> </mrow> <mrow> <mi>hRcD</mi> </mrow> </mfrac> <mo>•</mo> <msup> <mn>10</mn> <mi>hRcE</mi> </msup> </mrow> </math><a href="#fnref12" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
+<li id="fn13" role="doc-endnote"><p>Calculated as: <math xmlns="http://www.w3.org/1998/Math/MathML"> <mrow> <mi>vRescInPixelsPerMeter</mi> <mo>•</mo> <mn>25.4</mn> <mo>•</mo> <msup> <mn>10</mn> <mi>-3</mi> </msup> </mrow> </math><a href="#fnref13" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
+<li id="fn14" role="doc-endnote"><p>Calculated as: <math xmlns="http://www.w3.org/1998/Math/MathML"> <mrow> <mi>hRescInPixelsPerMeter</mi> <mo>•</mo> <mn>25.4</mn> <mo>•</mo> <msup> <mn>10</mn> <mi>-3</mi> </msup> </mrow> </math><a href="#fnref14" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
+<li id="fn15" role="doc-endnote"><p>Calculated as: <math xmlns="http://www.w3.org/1998/Math/MathML"> <mrow> <mfrac> <mrow> <mi>vRdN</mi> </mrow> <mrow> <mi>vRdD</mi> </mrow> </mfrac> <mo>•</mo> <msup> <mn>10</mn> <mi>vRdE</mi> </msup> </mrow> </math><a href="#fnref15" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
+<li id="fn16" role="doc-endnote"><p>Calculated as: <math xmlns="http://www.w3.org/1998/Math/MathML"> <mrow> <mfrac> <mrow> <mi>hRdN</mi> </mrow> <mrow> <mi>hRdD</mi> </mrow> </mfrac> <mo>•</mo> <msup> <mn>10</mn> <mi>hRdE</mi> </msup> </mrow> </math><a href="#fnref16" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
+<li id="fn17" role="doc-endnote"><p>Calculated as: <math xmlns="http://www.w3.org/1998/Math/MathML"> <mrow> <mi>vResdInPixelsPerMeter</mi> <mo>•</mo> <mn>25.4</mn> <mo>•</mo> <msup> <mn>10</mn> <mi>-3</mi> </msup> </mrow> </math><a href="#fnref17" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
+<li id="fn18" role="doc-endnote"><p>Calculated as: <math xmlns="http://www.w3.org/1998/Math/MathML"> <mrow> <mi>hResdInPixelsPerMeter</mi> <mo>•</mo> <mn>25.4</mn> <mo>•</mo> <msup> <mn>10</mn> <mi>-3</mi> </msup> </mrow> </math><a href="#fnref18" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
+<li id="fn19" role="doc-endnote"><p>Link: <a href="https://wwwimages.adobe.com/www.adobe.com/content/dam/Adobe/en/devnet/xmp/pdfs/cs6/XMPSpecificationPart3.pdf">https://wwwimages.adobe.com/www.adobe.com/content/dam/Adobe/en/devnet/xmp/pdfs/cs6/XMPSpecificationPart3.pdf</a><a href="#fnref19" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
+<li id="fn20" role="doc-endnote"><p>However, support for start of packet (SOP) and end of packet (EPH) markers may be included in future versions.<a href="#fnref20" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
+<li id="fn21" role="doc-endnote"><p>For example, in a TIFF to JP2 conversion workflow one could include a pixel-by-pixel comparison of the values in the TIFF and the JP2.<a href="#fnref21" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
+<li id="fn22" role="doc-endnote"><p>Calculated as: <math xmlns="http://www.w3.org/1998/Math/MathML"> <mrow> <mi>numberOfTiles</mi> <mo>=</mo> <mo>[</mo> <mfrac> <mrow> <mi>xsiz</mi> <mo>-</mo> <mi>xOsiz</mi> </mrow> <mrow> <mi>xTsiz</mi> </mrow> </mfrac> <mo>]</mo> <mo>•</mo> <mo>[</mo> <mfrac> <mrow> <mi>ysiz</mi> <mo>-</mo> <mi>yOsiz</mi> </mrow> <mrow> <mi>yTsiz</mi> </mrow> </mfrac> <mo>]</mo> </mrow> </math><a href="#fnref22" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
+<li id="fn23" role="doc-endnote"><p>Only reported if the <code>--packetmarkers</code> option is used.<a href="#fnref23" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
+<li id="fn24" role="doc-endnote"><p>Only reported if the <code>--packetmarkers</code> option is used.<a href="#fnref24" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
+<li id="fn25" role="doc-endnote"><p>Only reported if the <code>--packetmarkers</code> option is used.<a href="#fnref25" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
+<li id="fn26" role="doc-endnote"><p>Only reported if the <code>--packetmarkers</code> option is used.<a href="#fnref26" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
 </ol>
 </section>
```

#### html2text {}

```diff
@@ -27,14 +27,15 @@
           o _f_i_l_e_ _e_l_e_m_e_n_t
           o _f_i_l_e_I_n_f_o_ _e_l_e_m_e_n_t
           o _s_t_a_t_u_s_I_n_f_o_ _e_l_e_m_e_n_t
           o _i_s_V_a_l_i_d_ _e_l_e_m_e_n_t
           o _t_e_s_t_s_ _e_l_e_m_e_n_t
           o _p_r_o_p_e_r_t_i_e_s_ _e_l_e_m_e_n_t
           o _p_r_o_p_e_r_t_i_e_s_E_x_t_e_n_s_i_o_n_ _e_l_e_m_e_n_t
+          o _w_a_r_n_i_n_g_s_ _e_l_e_m_e_n_t
     * _J_P_2_:_ _b_o_x_ _b_y_ _b_o_x
           o _A_b_o_u_t_ _t_h_e_ _p_r_o_p_e_r_t_i_e_s_ _a_n_d_ _t_e_s_t_s_ _t_r_e_e_s
           o _J_P_E_G_ _2_0_0_0_ _S_i_g_n_a_t_u_r_e_ _b_o_x
           o _F_i_l_e_ _T_y_p_e_ _b_o_x
           o _J_P_2_ _H_e_a_d_e_r_ _b_o_x_ _(_s_u_p_e_r_b_o_x_)
           o _I_m_a_g_e_ _H_e_a_d_e_r_ _b_o_x_ _(_c_h_i_l_d_ _o_f_ _J_P_2_ _H_e_a_d_e_r_ _b_o_x_)
           o _B_i_t_s_ _P_e_r_ _C_o_m_p_o_n_e_n_t_ _b_o_x_ _(_c_h_i_l_d_ _o_f_ _J_P_2_ _H_e_a_d_e_r_ _b_o_x_)
@@ -65,14 +66,17 @@
           o _C_o_d_i_n_g_ _s_t_y_l_e_ _c_o_m_p_o_n_e_n_t_ _(_C_O_C_)_ _m_a_r_k_e_r_ _s_e_g_m_e_n_t
           o _R_e_g_i_o_n_-_o_f_-_i_n_t_e_r_e_s_t_ _(_R_G_N_)_ _m_a_r_k_e_r_ _s_e_g_m_e_n_t
           o _Q_u_a_n_t_i_z_a_t_i_o_n_ _d_e_f_a_u_l_t_ _(_Q_C_D_)_ _m_a_r_k_e_r_ _s_e_g_m_e_n_t
           o _Q_u_a_n_t_i_z_a_t_i_o_n_ _c_o_m_p_o_n_e_n_t_ _(_Q_C_C_)_ _m_a_r_k_e_r_ _s_e_g_m_e_n_t
           o _P_r_o_g_r_e_s_s_i_o_n_ _o_r_d_e_r_ _c_h_a_n_g_e_ _(_P_O_C_)_ _m_a_r_k_e_r_ _s_e_g_m_e_n_t
           o _C_o_m_p_o_n_e_n_t_ _r_e_g_i_s_t_r_a_t_i_o_n_ _(_C_R_G_)_ _m_a_r_k_e_r_ _s_e_g_m_e_n_t
           o _C_o_m_m_e_n_t_ _(_C_O_M_)_ _m_a_r_k_e_r_ _s_e_g_m_e_n_t
+          o _E_x_t_e_n_d_e_d_ _c_a_p_a_b_i_l_i_t_i_e_s_ _(_C_A_P_)_ _m_a_r_k_e_r_ _s_e_g_m_e_n_t
+          o _P_r_o_f_i_l_e_ _(_P_R_F_)_ _m_a_r_k_e_r_ _s_e_g_m_e_n_t
+          o _C_o_r_r_e_s_p_o_n_d_i_n_g_ _p_r_o_f_i_l_e_ _(_C_P_F_)_ _m_a_r_k_e_r_ _s_e_g_m_e_n_t
           o _T_i_l_e_ _p_a_r_t_ _(_c_h_i_l_d_ _o_f_ _C_o_n_t_i_g_u_o_u_s_ _C_o_d_e_s_t_r_e_a_m_ _b_o_x_)
           o _S_t_a_r_t_ _o_f_ _t_i_l_e_ _p_a_r_t_ _(_S_O_T_)_ _m_a_r_k_e_r_ _s_e_g_m_e_n_t_ _(_c_h_i_l_d_ _o_f_ _t_i_l_e_ _p_a_r_t_)
           o _T_i_l_e_-_p_a_r_t_ _l_e_n_g_t_h_s_ _(_T_L_M_)_ _m_a_r_k_e_r_ _s_e_g_m_e_n_t
           o _P_a_c_k_e_t_ _l_e_n_g_t_h_,_ _m_a_i_n_ _h_e_a_d_e_r_ _(_P_L_M_)_ _m_a_r_k_e_r_ _s_e_g_m_e_n_t
           o _P_a_c_k_e_d_ _p_a_c_k_e_t_ _h_e_a_d_e_r_s_,_ _m_a_i_n_ _h_e_a_d_e_r_ _(_P_P_M_)_ _m_a_r_k_e_r_ _s_e_g_m_e_n_t
           o _P_a_c_k_e_t_ _l_e_n_g_t_h_,_ _t_i_l_e_-_p_a_r_t_ _h_e_a_d_e_r_ _(_P_L_T_)_ _m_a_r_k_e_r_ _s_e_g_m_e_n_t
           o _P_a_c_k_e_d_ _p_a_c_k_e_t_ _h_e_a_d_e_r_s_,_ _t_i_l_e_-_p_a_r_t_ _h_e_a_d_e_r_ _(_P_P_T_)_ _m_a_r_k_e_r_ _s_e_g_m_e_n_t
@@ -83,14 +87,16 @@
 images. JP2 is the still image format that is defined by JPEG 2000 Part 1 (ISO/
 IEC 15444-1). JJppyyllyyzzeerr was specifically created to answer the following
 questions that you might have about any JP2 file:
    1. Is this really a JP2 and does it really conform to the formatâs
       specifications (validation)?
    2. What are the technical characteristics of this image (feature
       extraction)?
+Starting with version 2.2, jjppyyllyyzzeerr also supports Part 15 of the standard (ISO/
+IEC 15444-15, High Throughput JPEG 2000), and its JPH image format.
 ********** VVaalliiddaattiioonn:: ssccooppee aanndd rreessttrriiccttiioonnss **********
 Since the word âvalidationâ means different things to different people, a
 few words about the overall scope of jjppyyllyyzzeerr. First of all, it is important to
 stress that jjppyyllyyzzeerr is not a âone stop solutionâ that will tell you that
 an image is 100% perfect. What jjppyyllyyzzeerr does is this: based on the JP2 format
 specification (ISO/IEC 15444-1), it parses a file. It then subjects the
 fileâs contents to a large number of tests, each of which is based on the
@@ -126,18 +132,14 @@
     * Format migration workflows (e.g.Â TIFF to JP2) should ideally also
       include some comparison between source and destination images (e.g.Â a
       pixel-wise comparison)
 Conversely, an image that successfully passes a rendering test or pixel-wise
 comparison may still contain problematic features (e.g. incorrect colour space
 information), so validation, rendering tests and pixel-wise comparisons are
 really complementary to each other.
-******** NNoottee oonn IICCCC pprrooffiillee ssuuppppoorrtt ********
-The support of ICC profiles in JP2 was recently extended through an _a_m_e_n_d_m_e_n_t
-to the standard. These changes are taken into account by jjppyyllyyzzeerr, which is in
-line with the most recent version of the (updated) standard.
 ********** OOuuttlliinnee ooff tthhiiss UUsseerr MMaannuuaall **********
 We start by describing the _i_n_s_t_a_l_l_a_t_i_o_n_ _p_r_o_c_e_s_s of jjppyyllyyzzeerr for Windows and
 Unix-based systems. We then explain its _b_a_s_i_c_ _u_s_a_g_e, either as a command-line
 tool, or as an importable Python module. This is followed by a brief overview
 of _t_h_e_ _s_t_r_u_c_t_u_r_e_ _o_f_ _t_h_e_ _J_P_2_ _f_o_r_m_a_t and its âboxâ structure, and an
 explanation of JJppyyllyyzzeerrâs _o_u_t_p_u_t_ _f_o_r_m_a_t. The final sections give a detailed
 description of the tests that jjppyyllyyzzeerr performs for validation, and the
@@ -167,16 +169,15 @@
 To obtain the latest version of the software please use the download links at
 the jjppyyllyyzzeerr homepage:
 _h_t_t_p_s_:_/_/_j_p_y_l_y_z_e_r_._o_p_e_n_p_r_e_s_e_r_v_a_t_i_o_n_._o_r_g_/
 You have three options:
    1. Install the software with the PPiipp package manager. This works on all
       platforms (Windows, Linux, Mac, etc.), but you need to have the Python
       interpreter available on your system. Jpylyzer is compatible with Python
-      2.7, and Python 3.2 and more recent (Python 3.0 and 3.1 are not
-      supported).
+      3.2 and more recent.
    2. Alternatively, for Windows users there is also a set of stand-alone
       binaries_1. These allow you to run jjppyyllyyzzeerr as an executable Windows
       application, without any need for installing Python. This option is
       particularly useful for Windows users who cannot (or donât want to)
       install software on their system.
    3. For Linux users Debian packages are available.
 These options are described in the following sub-sections.
@@ -204,18 +205,17 @@
 if [ -d "$HOME/.local/bin" ] ; then
     PATH="$HOME/.local/bin:$PATH"
 fi
 Save the file, log out of your session and then log in again. Open a command
 terminal and type:
 jpylyzer
 If all went well you now see this:
-usage: jpylyzer [-h] [--format FMT] [--legacyout] [--mix {1,2}] [--nopretty]
+usage: jpylyzer [-h] [--format FMT] [--mix {1,2}] [--nopretty]
           [--nullxml] [--recurse] [--packetmarkers] [--verbose]
-          [--version] [--wrapper]
-          jp2In [jp2In ...]
+          [--version] jp2In [jp2In ...]
 jpylyzer: error: the following arguments are required: jp2In
 Which means that the installation was successful!
 ******** GGlloobbaall iinnssttaallllaattiioonn ((LLiinnuuxx)) ********
 Simply enter:
 sudo -H pip install jpylyzer
 No further configuration is needed in this case.
 ******** NNoottee oonn pprree--rreelleeaasseess ********
@@ -231,18 +231,17 @@
 %jpylyzerPath%\jpylyzer
 In the above command, replace %%jjppyyllyyzzeerrPPaatthh%% with the full path to the jjppyyllyyzzeerr
 installation directory (i.e.Â the directory that contains âjpylyzer.exeâ
 and its associated files). For example, if you extracted the files to directory
 c:\tools\jpylyzer, the command would become:
 c:\tools\jpylyzer\jpylyzer
 Executing this command should result in the following screen output:
-usage: jpylyzer [-h] [--format FMT] [--legacyout] [--mix {1,2}] [--nopretty]
+usage: jpylyzer [-h] [--format FMT] [--mix {1,2}] [--nopretty]
           [--nullxml] [--recurse] [--packetmarkers] [--verbose]
-          [--version] [--wrapper]
-          jp2In [jp2In ...]
+          [--version] jp2In [jp2In ...]
 jpylyzer: error: the following arguments are required: jp2In
 ******** RRuunnnniinngg jjppyyllyyzzeerr wwiitthhoouutt ttyyppiinngg tthhee ffuullll ppaatthh ********
 Optionally, you may also want to add the full path of the jjppyyllyyzzeerr installation
 directory to the Windows âPathâ environment variable. Doing so allows you
 to run jjppyyllyyzzeerr from any directory on your PC without having to type the full
 path. In Windows 7 you can do this by selecting âsettingsâ from the
 âStartâ menu; then go to âcontrol panelâ/âsystemâ and go to the
@@ -250,15 +249,15 @@
 locate the âPathâ variable in the âsystem variablesâ window, click on
 âEditâ and add the full jjppyyllyyzzeerr path (this requires local Administrator
 privileges). The settings take effect on any newly opened command prompt.
 ********** IInnssttaallllaattiioonn ooff DDeebbiiaann ppaacckkaaggeess ((UUbbuunnttuu//LLiinnuuxx)) **********
 For Linux, Debian packages of jjppyyllyyzzeerr exist. To install, simply download the
 ..ddeebb file, double-click on it and select IInnssttaallll PPaacckkaaggee. Alternatively you can
 also do this in the command terminal by typing:
-sudo dpkg -i opf-jpylyzer_2.0.0_all.deb
+sudo dpkg -i opf-jpylyzer_2.2.0_all.deb
 In both cases you need to have administrative privileges.
 For UUbbuunnttuu and DDeebbiiaann alternative packages are available in the official
 release channels. To install simply run the following commands:
 sudo apt-get update
 sudo apt-get install python-jpylyzer
 ************ UUssiinngg jjppyyllyyzzeerr ************
 ********** OOvveerrvviieeww **********
@@ -274,42 +273,37 @@
 TThhiiss UUsseerr MMaannuuaall                      jjppyyllyyzzeerr
 Substitution example Linux            /home/jpylyzer/jpylyzer
 Substitution example Windows binaries c:\tools\jpylyzer\jpylyzer
 Furthermore, command line arguments that are given between square brackets
 (example: [-h]) are optional.
 ******** SSyynnooppssiiss ********
 JJppyyllyyzzeerr can be invoked using the following command-line arguments:
-usage: jpylyzer [-h] [--format FMT] [--legacyout] [--mix {1,2}] [--nopretty]
+usage: jpylyzer [-h] [--format FMT] [--mix {1,2}] [--nopretty]
           [--nullxml] [--recurse] [--packetmarkers] [--verbose]
-          [--version] [--wrapper]
-          jp2In [jp2In ...]
+          [--version] jp2In [jp2In ...]
 ****** PPoossiittiioonnaall aarrgguummeennttss ******
 AArrgguummeenntt DDeessccrriippttiioonn
-jp2In    input JP2 image(s), may be one or more (whitespace-separated) path
+jp2In    input image(s), may be one or more (whitespace-separated) path
          expressions; prefix wildcard (*) with backslash (\) in Linux
 ****** OOppttiioonnaall aarrgguummeennttss ******
 AArrgguummeenntt          DDeessccrriippttiioonn
 [-h, --help]      show help message and exit
-[--format FMT]    validation format; allowed values are jp2 (used by default)
-                  and j2c (which activates raw codestream validation)
+                  validation format; allowed values are jp2 (JPEG 2000 Part 1,
+[--format FMT]    used by default), j2c (Part 1 codestream), jph (JPEG 2000
+                  Part 15 / High Throughput JPEG 2000) and jhc (Part 15
+                  codestream)
 [--mix {1,2}]     report additional output in NISO MIX format (version 1.0 or
                   2.0)
-[--legacyout]     report output in jpylyzer 1.x format (provided for backward
-                  compatibility only)
 [--nopretty]      suppress pretty-printing of XML output
 [--nullxml]       extract null-terminated XML content from XML and UUID boxes
                   (doesnât affect validation)
 [--recurse, -r]   when analysing a directory, recurse into subdirectories
-                  (implies --wrapper if --legacyout is used)
 [--packetmarkers] Report packet-level codestream markers (plm, ppm, plt, ppt)
 [--verbose]       report test results in verbose format
 [-v, --version]   show programâs version number and exit
-                  wrap output for individual image(s) in âresultsâ XML
-[--wrapper, -w]   element (deprecated from jpylyzer 2.x onward, only takes
-                  effect if --legacyout is used)
 Note that the input can either be a single image, a space-separated sequence of
 images, a pathname expression that includes multiple images, or any combination
 of the above. For example, the following command will process one single image:
 jpylyzer rubbish.jp2
 The next example shows how to process all files with a âjp2â extension in
 the current directory:
 jpylyzer *.jp2
@@ -330,28 +324,29 @@
 The format of the XML output is described _h_e_r_e.
 ******** ?â??ffoorrmmaatt?â?? ooppttiioonn ********
 By default, jjppyyllyyzzeerr validates against the JJPP22 format specification. Starting
 with version 2.0, jjppyyllyyzzeerr can also validate raw JPEG 2000 codestreams that are
 not wrapped inside a JJPP22 container. For codestream validation, use the --format
 option with value j2c, e.g.:
 jpylyzer --format j2c rubbish.j2c > rubbish.xml
+Starting with version 2.2, jjppyyllyyzzeerr also supports JPEG 2000 Part 15 (High
+Throughput JPEG 2000) and its JJPPHH container format. To validate a JJPPHH file, use
+the --format option with value jph:
+jpylyzer --format jph rubbish.jph > rubbish.xml
+And use --format with value jhc to validate a raw High Throughput codestream:
+jpylyzer --format jhc rubbish.jhc > rubbish.xml
 ******** ?â??mmiixx?â?? ooppttiioonn ********
 When this option is used, jjppyyllyyzzeerr reports additional output in _NN_II_SS_OO_ _MM_II_XX
 format. This option takes one argument that defines whether MMIIXX 1.0 or MMIIXX 2.0
 is used. For example, the following command will result in MMIIXX 2.0 output:
 jpylyzer --mix 2 rubbish.jp2 > rubbish.xml
 The MMIIXX output is wrapped inside a ffiillee//pprrooppeerrttiieessEExxtteennssiioonn element. Note that
-MMIIXX output is oonnllyy written for files that are valid JP2 (files that are not
-valid result in an empty pprrooppeerrttiieessEExxtteennssiioonn element). Also, the --mix option
-is ignored if --format is set to j2c, or if --legacyout (see below) is used.
-******** ?â??lleeggaaccyyoouutt?â?? ooppttiioonn ********
-The output format of jjppyyllyyzzeerr has changed in version 2.0, which may break
-existing workflows that expect output in 1.x format. For backward compatibility
-the --legacyout option results in output that follows the old 1.x format. Note
-that codestream validation is disabled if you use this option.
+MMIIXX output is oonnllyy written for files that are valid JP2 or JPH (files that are
+not valid result in an empty pprrooppeerrttiieessEExxtteennssiioonn element). Also, the --mix
+option is ignored if --format is set to j2c.
 ******** ?â??rreeccuurrssee?â?? ooppttiioonn ********
 If the --recurse option is used, jjppyyllyyzzeerr will recursively traverse all
 subdirectories of a filepath expression. E.g:
 jpylyzer /home/myJP2s/*.jp2 > rubbish.xml
 In this case jjppyyllyyzzeerr analyses all files that have a ..jjpp22 extension in
 directory //hhoommee//mmyyJJPP22ss and all its subdirectories.
 ******** ?â??ppaacckkeettmmaarrkkeerrss?â?? ooppttiioonn ********
@@ -359,44 +354,23 @@
 following packet-level codestream markers:
     * PLM (packet length, main header) marker
     * PPM (packed packet headers, main header) marker
     * PLT (packet length, tile-part header) marker
     * PPT (packed packet headers, tile-part header) marker
 By default these are excluded from the output, in order to prevent excessive
 output size.
-******** ?â??wwrraappppeerr?â?? ooppttiioonn ((ddeepprreeccaatteedd)) ********
-This deprecated option is included for backward-compatibility, and only takes
-effect if --legacyout (see above) is used.By default, the jjppyyllyyzzeerr 1.x releases
-would create a separate XML tree for each analysed image, without any
-overarching hierarchy. For multiple-image pathname expressions this resulted in
-output that was nnoott well-formed XML. The --legacyout option still results in
-this is behaviour. For example:
-jpylyzer --legacyout rubbish.jp2 garbage.jp2 > rubbish.xml
-In this case, the file ârubbish.xmlâ contains a succession of two XML
-trees, which by itself is not well-formed XML. The --wrapper option is provided
-to create valid XML instead:
-jpylyzer --legacyout --wrapper rubbish.jp2 garbage.jp2 > rubbish.xml
-In the above case the XML trees of the individual images are wrapped inside a
-âresultsâ element. When the --recurse option is used, jpylyzer will
-automatically wrap the output in a âresultsâ element, so thereâs no need
-to specify --wrapper in that case.
-Starting with version 2.0, jjppyyllyyzzeerr aallwwaayyss generates well-formed XML (unless
-the --legacyout option is used), which makes the --wrapper option largely
-obsolete, apart from cases where the âoldâ behaviour is needed for
-backward-compatibility reasons.
 ******** ?â??nnuullllxxmmll?â?? ooppttiioonn ********
 The nnuullllxxmmll option was added to enable extraction of XML content that is
 terminated by a null-byte. By default jjppyyllyyzzeerr doesnât report the XML in that
 case, because it throws an exception in the XML parser. Apparently some old
 versions of the Kakadu demo applications would erroneously add a null-byte to
 embedded XML, so this option can be used to force extraction for images that
 are affected by this.
 ******** UUsseerr wwaarrnniinnggss ********
-Under the following conditions jjppyyllyyzzeerr will print a user warning to the
-standard error device (typically the console screen):
+Under the following conditions jjppyyllyyzzeerr will report a user warning:
 ****** NNoo iimmaaggeess ttoo cchheecckk ******
 If there are no input images to check (typically because the value of jp2In
 refers to a non-existent file), the following warning message is shown:
 User warning: no images to check!
 ****** UUnnssuuppppoorrtteedd bbooxx ******
 In some cases you will see the following warning message:
 User warning: ignoring 'boxName' (validator function not yet implemented)
@@ -426,23 +400,26 @@
 ****** UUnnkknnoowwnn bbooxx ******
 Occasionally, you may see this warning message:
 User warning: ignoring unknown box
 This happens if jjppyyllyyzzeerr encounters a box that is not defined by JPEG 2000 Part
 1. It should be noted that, to a large extent, JPEG 2000 Part 1 permits the
 presence of boxes that are defined outside the standard. Again, jjppyyllyyzzeerr will
 simply ignore these and process all other boxes normally.
+All user warnings are printed to the standard error device (typically the
+console screen). File-level warnings are also written to the wwaarrnniinnggss output
+element.
 ********** UUssiinngg jjppyyllyyzzeerr aass aa PPyytthhoonn mmoodduullee **********
 Instead of using jjppyyllyyzzeerr from the command-line, you can also import it as a
 module in your own Python programs. To do so, install jpylyzer with ppiipp. Then
 import jjppyyllyyzzeerr into your code by adding:
 from jpylyzer import jpylyzer
 Subsequently you can call any function that is defined in jjppyyllyyzzeerr..ppyy. In
 practice you will most likely only need the cchheecckkOOnneeFFiillee function. The
 following minimal script shows how this works:
-#! /usr/bin/env python
+#! /usr/bin/env python3
 
 from jpylyzer import jpylyzer
 
 # Define JP2
 myFile = "/home/johan/jpylyzer-test-files/aware.jp2"
 
 # Analyse with jpylyzer, result to Element object
@@ -451,23 +428,35 @@
 # Return image height value
 imageHeight = myResult.findtext('./properties/jp2HeaderBox/imageHeaderBox/
 height')
 print(imageHeight)
 Here, mmyyRReessuulltt is an EElleemmeenntt object that can either be used directly, or
 converted to XML using the EElleemmeennttTTrreeee module_2. The structure of the element
 object follows the XML output that described _h_e_r_e.
-For validation a raw JPEG 2000 codestreams, call the cchheecckkOOnneeFFiillee function with
-the additional vvaalliiddaattiioonnFFoorrmmaatt argument, and set it to j2c:
+You may use the following optional arguments (which correspond to the command-
+line options explained above):
+    * validationFormat - sets the validation format. Values: âjp2â
+      (default), âjphâ, âj2câ or âjhcâ.
+    * verboseFlag - report test results in verbose format. Values: False
+      (default) or True.
+    * packetmarkersFlag - report packet-level codestream markers. Values: False
+      (default) or True.
+    * nullxmlFlag - extract null-terminated XML content from XML and UUID
+      boxes. Values: False (default) or True.
+    * mixFlag - report additional output in NISO MIX format (version 1.0 or
+      2.0). Values: 0 (default), 1 or 2.
+As an example, for validating a raw JPEG 2000 codestream, call the cchheecckkOOnneeFFiillee
+function with the additional vvaalliiddaattiioonnFFoorrmmaatt argument, and set it to j2c:
 # Define Codestream
 myFile = "/home/johan/jpylyzer-test-files/rubbish.j2c"
 
 # Analyse with jpylyzer, result to Element object
 myResult = jpylyzer.checkOneFile(myFile, 'j2c')
 ********** JJaavvaa iinntteeggrraattiioonn **********
-It is possible to integrate jjppyyllyyzzeerr into Java applications. A test class that
+It is possible to integrate jjppyyllyyzzeerr into Java applications_3. A test class that
 shows how this works is included in the source repo _h_e_r_e. This requires _J_y_t_h_o_n.
 Note that you may run into performance issues with (very) large images in this
 case, as Jython does not support _m_e_m_o_r_y_ _m_a_p_p_i_n_g, so make sure youâve got
 plenty of RAM available.
 ************ SSttrruuccttuurree ooff aa JJPP22 ffiillee ************
 ********** SSccooppee ooff tthhiiss sseeccttiioonn **********
 This section gives a brief overview of the JP2 file format. A basic
@@ -608,14 +597,15 @@
       attempt
    3. iissVVaalliidd: outcome of the validation
    4. tteessttss: outcome of the individual tests that are part of the validation
       process (organised by box)
    5. pprrooppeerrttiieess: image properties (organised by box)
    6. pprrooppeerrttiieessEExxtteennssiioonn: wrapper element for NISO MMIIXX output (only if the --
       mix option is used)
+   7. wwaarrnniinnggss: reported warnings
 ********** ffiilleeIInnffoo eelleemmeenntt **********
 This element holds general information about the analysed file. Currently it
 contains the following sub-elements:
     * ffiilleennaammee: name of the analysed file without its path (e.g.
       ârubbish.jp2â)
     * ffiilleePPaatthh: name of the analysed file, including its full absolute path
       (e.g.Â âd:\data\images\rubbish.jp2â)
@@ -655,23 +645,30 @@
 If a file passed aallll tests, this is an indication that it is most likely valid
 JP2. In that case, the _ii_ss_VV_aa_ll_ii_dd_ _e_l_e_m_e_n_t has a value of âTrueâ (and
 âFalseâ in all other cases). These tests are all explained _h_e_r_e and _h_e_r_e.
 ******** DDeeffaauulltt aanndd vveerrbboossee rreeppoorrttiinngg ooff tteesstt rreessuullttss ********
 By default, jjppyyllyyzzeerr only reports any tests that failed (i.e.Â returned
 âFalseâ), including the corresponding part of the box structure. For a
 valid JP2 the tests element will be empty. If the âverbose flag is used, the
-results of aallll tests are included (including those that returned âTrueâ)_3.
+results of aallll tests are included (including those that returned âTrueâ)_4.
 ********** pprrooppeerrttiieess eelleemmeenntt **********
 This element contains the extracted image properties, which are organised in a
 hierarchical tree that corresponds to JP2âs box structure. See _h_e_r_e and _h_e_r_e
 for a description of the reported properties.
 ********** pprrooppeerrttiieessEExxtteennssiioonn eelleemmeenntt **********
 This optional element is reserved for output in alternative formats. Currently
 it is used to wrap output in NISO MMIIXX format if the --mix option is used. See
 the _MM_II_XX_ _d_o_c_u_m_e_n_t_a_t_i_o_n for a description of the reported elements.
+********** wwaarrnniinnggss eelleemmeenntt **********
+This element is reserved for reporting any warnings that are not directly
+related to the validation process. Examples are:
+    * Jpylyzer encountered an unknown box type while parsing a file.
+    * Reading of a file failed because of system limitations.
+Each warning is wrapped in a âwarningâ element. The results are organised
+in a hierarchical tree that corresponds to JP2âs box structure.
 ************ JJPP22:: bbooxx bbyy bbooxx ************
 The following two sections provide a detailed explanation of jjppyyllyyzzeerrâs
 functionality and its output. In particular, the following two aspects are
 addressed:
    1. The reported properties
    2. The tests that jjppyyllyyzzeerr performs to establish the validity of a file.
 ********** AAbboouutt tthhee pprrooppeerrttiieess aanndd tteessttss ttrreeeess **********
@@ -722,18 +719,20 @@
 PPrrooppeerrttyy DDeessccrriippttiioonn
 br       Brand
 minV     Minor version
 cL*      Compatibility field (repeatable)
 ******** TTeessttss ********
 TTeesstt nnaammee                TTrruuee iiff
 boxLengthIsValid         (Size of box â 8) /4 is a whole number (integer)
-brandIsValid             bbrr equals 0x6a703220 (âjp2â)
+brandIsValid             bbrr equals 0x6a703220 (âjp2â) for JP2, or
+                         0x6a706820 (âjphâ)for JPH
 minorVersionIsValid      mmiinnVV equals 0
-compatibilityListIsValid Sequence of compatibility (ccLL) fields includes one
-                         entry that equals 0x6a703220 (âjp2â)
+                         Sequence of compatibility (ccLL) fields includes one
+compatibilityListIsValid entry that equals 0x6a703220 (âjp2â) for JP2, or
+                         0x6a706820 (âjphâ)for JPH
 ********** JJPP22 HHeeaaddeerr bbooxx ((ssuuppeerrbbooxx)) **********
 This box is a superbox that holds a series of boxes that contain header-type
 information about the file.
 ******** EElleemmeenntt nnaammee ********
 jp2HeaderBox
 ******** RReeppoorrtteedd pprrooppeerrttiieess ********
 Since this is a superbox, it contains a number of child boxes. These are
@@ -774,14 +773,18 @@
 colourSpecificationBoxesAreContiguous       Specification boxes, they appear
                                             contiguously in the JP2 Header box
                                             Box contains a Palette box (only if
                                             Component Mapping box is present);
 paletteAndComponentMappingBoxesOnlyTogether box contains a Component Mapping
                                             box (only if Palette box is
                                             present)
+                                            If file does not contain a Colour
+noZeroCTypesIfNoColourBox                   Specification Box, no cTyp values
+                                            (from Channel definition box) shall
+                                            be equal to 0 (JPH)
 ********** IImmaaggee HHeeaaddeerr bbooxx ((cchhiilldd ooff JJPP22 HHeeaaddeerr bbooxx)) **********
 This box specifies the size of the image and other related fields.
 ******** EElleemmeenntt nnaammee ********
 imageHeaderBox
 ******** RReeppoorrtteedd pprrooppeerrttiieess ********
 PPrrooppeerrttyy DDeessccrriippttiioonn
 height   Image height in pixels
@@ -820,24 +823,34 @@
 bPCIsValid* bbPPCCDDeepptthh is within range [1,38] (repeated for all components)
 ********** CCoolloouurr SSppeecciiffiiccaattiioonn bbooxx ((cchhiilldd ooff JJPP22 HHeeaaddeerr bbooxx)) **********
 This box specifies the colourspace of the image.
 ******** EElleemmeenntt nnaammee ********
 colourSpecificationBox
 ******** RReeppoorrtteedd pprrooppeerrttiieess ********
 PPrrooppeerrttyy                          DDeessccrriippttiioonn
-                                  Specification method. Indicates whether
-meth                              colourspace of this image is defined as
-                                  an enumerated colourspace or using a
-                                  (restricted) ICC profile.
+                                  Specification method. Indicates how the
+                                  colourspace is defined (enumerated
+meth                              colourspace, or restricted ICC profile
+                                  for JP2, with additional Any ICC and
+                                  Parameterized Colourspace methods for
+                                  JPH.
 prec                              Precedence
 approx                            Colourspace approximation
 enumCS (if meth equals            Enumerated colourspace (as descriptive
 âEnumeratedâ)                 text string)
 icc (if meth equals âRestricted Properties of ICC profile as child
-ICCâ or âAny ICCâ_4)         element (see below)
+ICCâ or âAny ICCâ)          element (see below)
+colPrims (if meth equals          ColourPrimaries value (JPH)_5.
+âParameterized Colourspaceâ)
+transfC (if meth equals           TransferCharacteristics value (JPH)_6
+âParameterized Colourspaceâ)
+matCoeffs (if meth equals         MatrixCoefficients value (JPH)_7
+âParameterized Colourspaceâ)
+vidFRng (if meth equals           VideoFullRangeFlag (âyesâ/ânoâ)
+âParameterized Colourspaceâ)  (JPH)_8
 ******** RReeppoorrtteedd pprrooppeerrttiieess ooff IICCCC pprrooffiilleess ********
 If the colour specification box contains an embedded ICC profile, jjppyyllyyzzeerr will
 also report the following properties (which are all grouped in an âiccâ
 sub-element in the properties tree). An exhaustive explanation of these
 properties is given in the ICC specification (ISO 15076-1 / ICC.1:2004-10).
 Note that jjppyyllyyzzeerr does nnoott validate embedded ICC profiles (even though it does
 check if a specific ICC profile is allowed in JP2)!
@@ -886,17 +899,23 @@
 approxIsValid                        aapppprrooxx equals 0
 enumCSIsValid (if meth equals        eennuummCCSS equals 16 (âsRGBâ), 17
 âEnumeratedâ)                    (âgreyscaleâ) or 18 (âsYCCâ)
 iccSizeIsValid (if meth equals       Actual size of embedded ICC profile
 âRestricted ICCâ)                equals value of profileSize field in ICC
                                      header
 iccPermittedProfileClass (if meth    ICC profile class is âinput deviceâ
-equals âRestricted ICCâ)         or âdisplay deviceâ_5
+equals âRestricted ICCâ)         or âdisplay deviceâ_9
 iccNoLUTBasedProfile (if meth equals ICC profile type is not N-component LUT
 âRestricted ICCâ)                based (which is not allowed in JP2)
+colPrimsIsValid                      ccoollPPrriimmss value is defined by ITU-T H.273
+                                     / ISO/IEC 23001-8 (JPH)
+transfCIsValid                       ttrraannssffCC value is defined by ITU-T H.273
+                                     / ISO/IEC 23001-8 (JPH)
+matCoeffsIsValid                     mmaattCCooeeffffss value is defined by ITU-
+                                     T H.273 / ISO/IEC 23001-8 (JPH)
 ********** PPaalleettttee bbooxx ((cchhiilldd ooff JJPP22 HHeeaaddeerr bbooxx)) **********
 This (optional) box specifies the palette which maps a single component in
 index space to a multiple-component image.
 ******** EElleemmeenntt nnaammee ********
 paletteBox
 ******** RReeppoorrtteedd pprrooppeerrttiieess ********
 PPrrooppeerrttyy DDeessccrriippttiioonn
@@ -937,20 +956,26 @@
 ******** RReeppoorrtteedd pprrooppeerrttiieess ********
 PPrrooppeerrttyy DDeessccrriippttiioonn
 n        Number of channel descriptions
 cN*      Channel index (repeated for all channels)
 cTyp*    Channel type (repeated for all channels)
 cAssoc*  Channel association (repeated for all channels)
 ******** TTeessttss ********
-TTeesstt nnaammee        TTrruuee iiff
-nIsValid         nn is within range [1, 65535]
-boxLengthIsValid (Size of box â 2) / equals 6*nn
-cNIsValid*       ccNN is within range [0, 65535] (repeated for all channels)
-cTypIsValid*     ccTTyyppee is within range [0, 65535] (repeated for all channels)
-cAssocIsValid*   ccAAssssoocc is within range [0, 65535] (repeated for all channels)
+TTeesstt nnaammee                 TTrruuee iiff
+nIsValid                  nn is within range [1, 65535]
+boxLengthIsValid          (Size of box â 2) / equals 6*nn
+cNIsValid*                ccNN is within range [0, 65535] (repeated for all
+                          channels)
+cTypIsValid*              ccTTyyppee is one of the values defined in Table I.16
+                          (repeated for all channels)_1_0
+cAssocIsValid*            ccAAssssoocc is within range [0, 65535] (repeated for all
+                          channels)
+noMoreThanOneAlphaChannel At most one ccTTyypp field is equal to 1 or 2 (JPH)
+cAssocAlphaChannelIsZero  If ccTTyypp is 1 or 2, the corresponding ccAAssssoocc value
+                          equals 0 (JPH)
 ********** RReessoolluuttiioonn bbooxx ((cchhiilldd ooff JJPP22 HHeeaaddeerr bbooxx,, ssuuppeerrbbooxx)) **********
 This (optional) box contains the grid resolution.
 ******** EElleemmeenntt nnaammee ********
 resolutionBox
 ******** RReeppoorrtteedd pprrooppeerrttiieess ********
 Since this is a superbox, it contains one or two child boxes. These are
 represented as child elements in the properties tree:
@@ -979,19 +1004,20 @@
 PPrrooppeerrttyy              DDeessccrriippttiioonn
 vRcN                  Vertical grid resolution numerator
 vRcD                  Vertical grid resolution denominator
 hRcN                  Horizontal grid resolution numerator
 hRcD                  Horizontal grid resolution denominator
 vRcE                  Vertical grid resolution exponent
 hRcE                  Horizontal grid resolution exponent
-vRescInPixelsPerMeter Vertical grid resolution, expressed in pixels per meter_6
+vRescInPixelsPerMeter Vertical grid resolution, expressed in pixels per meter_1_1
 hRescInPixelsPerMeter Horizontal grid resolution, expressed in pixels per
-                      meter_7
-vRescInPixelsPerInch  Vertical grid resolution, expressed in pixels per inch_8
-hRescInPixelsPerInch  Horizontal grid resolution, expressed in pixels per inch_9
+                      meter_1_2
+vRescInPixelsPerInch  Vertical grid resolution, expressed in pixels per inch_1_3
+hRescInPixelsPerInch  Horizontal grid resolution, expressed in pixels per
+                      inch_1_4
 ******** TTeessttss ********
 TTeesstt nnaammee        TTrruuee iiff
 boxLengthIsValid Size of box contents equals 10 bytes
 vRcNIsValid      vvRRccNN is within range [1,65535]
 vRcDIsValid      vvRRccDD is within range [1,65535]
 hRcNIsValid      hhRRccNN is within range [1,65535]
 hRcDIsValid      hhRRccDD is within range [1,65535]
@@ -1010,20 +1036,20 @@
 PPrrooppeerrttyy              DDeessccrriippttiioonn
 vRdN                  Vertical grid resolution numerator
 vRdD                  Vertical grid resolution denominator
 hRdN                  Horizontal grid resolution numerator
 hRdD                  Horizontal grid resolution denominator
 vRdE                  Vertical grid resolution exponent
 hRdE                  Horizontal grid resolution exponent
-vResdInPixelsPerMeter Vertical grid resolution, expressed in pixels per meter_1_0
+vResdInPixelsPerMeter Vertical grid resolution, expressed in pixels per meter_1_5
 hResdInPixelsPerMeter Horizontal grid resolution, expressed in pixels per
-                      meter_1_1
-vResdInPixelsPerInch  Vertical grid resolution, expressed in pixels per inch_1_2
+                      meter_1_6
+vResdInPixelsPerInch  Vertical grid resolution, expressed in pixels per inch_1_7
 hResdInPixelsPerInch  Horizontal grid resolution, expressed in pixels per
-                      inch_1_3
+                      inch_1_8
 ******** TTeessttss ********
 TTeesstt nnaammee        TTrruuee iiff
 boxLengthIsValid Size of box contents equals 10 bytes
 vRdNIsValid      vvRRddNN is within range [1,65535]
 vRdDIsValid      vvRRddDD is within range [1,65535]
 hRdNIsValid      hhRRddNN is within range [1,65535]
 hRdDIsValid      hhRRddDD is within range [1,65535]
@@ -1056,15 +1082,15 @@
 Note that jjppyyllyyzzeerr does not check whether the XML is vvaalliidd, as this is not
 required by the standard. Besides, doing so would make jjppyyllyyzzeerr significantly
 slower for XML that contains references to external schemas and DTDs.
 ********** UUUUIIDD bbooxx **********
 This (optional) box contains additional (binary) information, which may be
 vendor-specific. Some applications (e.g.Â Kakadu and ExifTool) also use this
 box for storing XMP metadata (see Section 1.1.4 in Part 3 of the XMP
-specification_1_4).
+specification_1_9).
 ******** EElleemmeenntt nnaammee ********
 uuidBox
 ******** RReeppoorrtteedd pprrooppeerrttiieess ********
 If the value of uuuuiidd indicates the presence of XMP metadata and the contents of
 this box are well-formed XML, (see âtestsâ below), the âuuidBoxâ
 element in the properties tree will contain the XMP data. Note that, depending
 on the character encoding of the original XML, it may contain characters that
@@ -1302,17 +1328,17 @@
 supported at this stage: if jjppyyllyyzzeerr encounters them, it will include the
 corresponding element in the pprrooppeerrttiieess element of the output. However,
 jjppyyllyyzzeerr does not analyse the contents of these marker segments, which means
 that the respective elements in the output will be empty.
 ******** BBiitt ssttrreeaammss ********
 In addition to the above limitations, jjppyyllyyzzeerr can nnoott be used to establish
 whether the data in the bitstream are correct (this would require decoding the
-compressed image data, which is completely out of jjppyyllyyzzeerrâs scope)_1_5. As a
+compressed image data, which is completely out of jjppyyllyyzzeerrâs scope)_2_0. As a
 result, if jjppyyllyyzzeerr is used as part of a quality assurance workflow, it is
-recommended to also include an additional check on the image contents_1_6. Also,
+recommended to also include an additional check on the image contents_2_1. Also,
 jjppyyllyyzzeerr does not perform any checks on marker segments within the bit-stream:
 start-of packet (SOP) and end-of-packet (EPH) markers.
 ******** DDeetteeccttiioonn ooff iinnccoommpplleettee oorr ttrruunnccaatteedd ccooddeessttrreeaammss ********
 A JP2âs tile part header contains information that makes it possible to
 detect incomplete and truncated codestreams in most cases. Depending on the
 encoder software used, this method may fail for images that only contain one
 single tile part (i.e.Â images that do not contain tiling).
@@ -1368,66 +1394,76 @@
 ppmCount Number of PPM markers in main header
 ******** TTeessttss ********
 TTeesstt nnaammee                      TTrruuee iiff
 codestreamStartsWithSOCMarker  First 2 bytes in codestream constitute a start
                                of codestream (SOC) marker segment
 foundSIZMarker                 Second marker segment in codestream is image and
                                tile size (SIZ) marker segment
+                               Codestream main header contains Extended
+foundCAPMarker                 Capabilities (CAP) marker segment if second most
+                               significant bit of rrssiizz equals 1
 foundCODMarker                 Codestream main header contains coding style
                                default (COD) marker segment
 foundQCDMarker                 Codestream main header contains quantization
                                default (QCD) marker segment
+                               Value of CCPPFFnnuumm in CPF marker segment is
+CPFnumConsistentWithPRFnum     consistent with PPRRFFnnuumm value in PRF marker
+                               segment
+                               Value of CCPPFFnnuumm in CPF marker segment is
+CPFnumConsistentWithRsiz       consistent with *rsiz^ value in SIZ marker
+                               segment
                                Number of encountered tiles is consistent with
 foundExpectedNumberOfTiles     expected number of tiles (as calculated from _S_I_Z
                                _m_a_r_k_e_r)
                                For all tiles, number of encountered tile parts
 foundExpectedNumberOfTileParts is consistent with expected number of tile parts
                                (values of ttnnssoott from _S_O_T_ _m_a_r_k_e_r)
                                No more than one ccccoocc value for each component
-maxOneCcocPerComponent         (only reported if codestream contains any COC
-                               marker segments)
+maxOneCcocPerComponentMain     in main header (only reported if codestream
+                               contains any COC marker segments)
                                No more than one ccqqcccc value for each component
-maxOneCqccPerComponent         (only reported if codestream contains any QCC
-                               marker segments)
+maxOneCqccPerComponentMain     in main header (only reported if codestream
+                               contains any QCC marker segments)
 foundEOCMarker                 Last 2 bytes in codestream constitute an end of
                                codestream (EOC) marker segment
 ********** IImmaaggee aanndd ttiillee ssiizzee ((SSIIZZ)) mmaarrkkeerr sseeggmmeenntt ((cchhiilldd ooff CCoonnttiigguuoouuss CCooddeessttrreeaamm
 bbooxx)) **********
 ******** EElleemmeenntt nnaammee ********
 siz
 ******** RReeppoorrtteedd pprrooppeerrttiieess ********
 PPrrooppeerrttyy      DDeessccrriippttiioonn
 lsiz          Length of SIZ marker segment in bytes
-rsiz          Decoder capabilities
+rsiz          Numerical value of rrssiizz (capabilities) field
+capability    Capabilities (profile) encoded by rrssiizz value
 xsiz          Width of reference grid
 ysiz          Height of reference grid
 xOsiz         Horizontal offset from origin of reference grid to left of image
               area
 yOsiz         Vertical offset from origin of reference grid to top of image
               area
 xTsiz         Width of one reference tile with respect to the reference grid
 yTsiz         Height of one reference tile with respect to the reference grid
 xTOsiz        Horizontal offset from origin of reference grid to left side of
               first tile
 yTOsiz        Vertical offset from origin of reference grid to top side of
               first tile
-numberOfTiles Number of tiles_1_7
+numberOfTiles Number of tiles_2_2
 csiz          Number of components
 ssizSign*     Indicates whether image component is signed or unsigned (repeated
               for all components)
 ssizDepth*    Number of bits for this component (repeated for all components)
 xRsiz*        Horizontal separation of sample of this component with respect to
               reference grid (repeated for all components)
 yRsiz*        Vertical separation of sample of this component with respect to
               reference grid (repeated for all components)
 ******** TTeessttss ********
 TTeesstt nnaammee              TTrruuee iiff
 lsizIsValid            llssiizz is within range [41,49190]
-rsizIsValid            rrssiizz equals 0 (âISO/IEC 15444-1â), 1 (âProfile
-                       0â) or 2 (âProfile 1â)
+rsizIsValid            Four most significant bits of rrssiizz are 0 (JP2, J2C);
+                       second most significant bit of rrssiizz equals 1 (JPH, JHC)
 xsizIsValid            xxssiizz is within range [1,232 - 1]
 ysizIsValid            yyssiizz is within range [1,232 - 1]
 xOsizIsValid           xxOOssiizz is within range [0,232 - 2]
 yOsizIsValid           yyOOssiizz is within range [0,232 - 2]
 xTsizIsValid           xxTTssiizz is within range [1,232 - 1]
 yTsizIsValid           yyTTssiizz is within range [1,232 - 1]
 xTOsizIsValid          xxTTOOssiizz is within range [0,232 - 2]
@@ -1457,24 +1493,27 @@
 multipleComponentTransformation Indicates use of multiple component
                                 transformation (âyesâ/ânoâ)
 levels                          Number of decomposition levels
 codeBlockWidth                  Code block width
 codeBlockHeight                 Code block height
 codingBypass                    Indicates use of coding bypass (âyesâ/
                                 ânoâ)
-resetOnBoundaries               Indicates reset of context probabilities on
-                                coding pass boundaries (âyesâ/ânoâ)
+                                Indicates reset of context probabilities on
+resetOnBoundaries               coding pass boundaries (âyesâ/ânoâ)
+                                (does not apply to High Throughput code blocks)
 termOnEachPass                  Indicates termination on each coding pass
                                 (âyesâ/ânoâ)
 vertCausalContext               Indicates vertically causal context (âyesâ/
                                 ânoâ)
-predTermination                 Indicates predictable termination (âyesâ/
-                                ânoâ)
-segmentationSymbols             Indicates use of segmentation symbols
-                                (âyesâ/ânoâ)
+                                Indicates predictable termination (âyesâ/
+predTermination                 ânoâ) (does not apply to High Throughput
+                                code blocks)
+                                Indicates use of segmentation symbols
+segmentationSymbols             (âyesâ/ânoâ) (does not apply to High
+                                Throughput code blocks)
 transformation                  Wavelet transformation: â9-7 irreversibleâ
                                 or â5-3 reversibleâ
                                 Precinct width (repeated for all resolution
 precinctSizeX*                  levels; order: low to high). Equals 32768 if
                                 pprreecciinnccttss is âdefaultâ
                                 Precinct height (repeated for all resolution
 precinctSizeY*                  levels; order: low to high). Equals 32768 if
@@ -1558,15 +1597,16 @@
 roiShift Implicit ROI shift
 ******** TTeessttss ********
 TTeesstt nnaammee       TTrruuee iiff
 lrgnIsValid     llrrggnn is within range [5,6]
 crgnIsValid     ccrrggnn is within range [0,255] (ccssiizz < 257) or [0,16383] (ccssiizz >=
                 257)
 roiStyleIsValid rrooiiSSttyyllee equals 0 (âImplicit ROI (maximum shift)â)
-roiShiftIsValid rrooiiSShhiifftt is within range [0,255]
+roiShiftIsValid rrooiiSShhiifftt is within range [0,255] (JP2, J2C) or [0,37] (JPH,
+                JHC)
 ********** QQuuaannttiizzaattiioonn ddeeffaauulltt ((QQCCDD)) mmaarrkkeerr sseeggmmeenntt **********
 ******** EElleemmeenntt nnaammee ********
 qcd
 ******** RReeppoorrtteedd pprrooppeerrttiieess ********
 PPrrooppeerrttyy  DDeessccrriippttiioonn
 lqcd      Length of QCD marker segment in bytes
 qStyle    Quantization style for all components
@@ -1677,14 +1717,58 @@
 ******** TTeessttss ********
 TTeesstt nnaammee      TTrruuee iiff
 lcomIsValid    llqqccdd is within range [5,65535]
 rcomIsValid    rrccoomm equals 0 (âbinaryâ) or 1 (âISO/IEC 8859-15
                (Latinâ))
 commentIsValid Comment is valid ISO/IEC8859-15 and does not contain control
                characters, other than tab, newline or carriage return
+********** EExxtteennddeedd ccaappaabbiilliittiieess ((CCAAPP)) mmaarrkkeerr sseeggmmeenntt **********
+This marker segment is defined in ISO/IEC 15444-2, and is used by ISO/IEC
+15444-15 (as well as other parts of the standard).
+******** EElleemmeenntt nnaammee ********
+cap
+******** RReeppoorrtteedd pprrooppeerrttiieess ********
+PPrrooppeerrttyy      DDeessccrriippttiioonn
+lcap          Length of CAP marker segment in bytes
+pcapPart      Indicates the use of capabilities from Part ppccaappPPaarrtt of the ISO/
+              IEC 15444 standard (repeated for all referenced parts)
+htCodeBlocks  See section 8.2 of ISO/IEC 15444-15 (JPH, JHC)
+htSets        See section 8.3 of ISO/IEC 15444-15 (JPH, JHC)
+htRegion      See section 8.4 of ISO/IEC 15444-15 (JPH, JHC)
+htHomogeneous See section 8.5 of ISO/IEC 15444-15 (JPH, JHC)
+htReversible  See section 8.7.2 of ISO/IEC 15444-15 (JPH, JHC)
+htB           Parameter BB as used in MMAAGGBBPP sets, see sections A.3.7 and 8.7.3
+              of ISO/IEC 15444-15 (JPH, JHC)
+******** TTeessttss ********
+TTeesstt nnaammee     TTrruuee iiff
+lcapIsValid   Number of ppccaappPPaarrtt entries equals (llccaapp - 6)/2
+pcap15IsValid 15th most significant bit of ppccaapp equals 1 (JPH, JHC)
+********** PPrrooffiillee ((PPRRFF)) mmaarrkkeerr sseeggmmeenntt **********
+******** EElleemmeenntt nnaammee ********
+prf
+******** RReeppoorrtteedd pprrooppeerrttiieess ********
+PPrrooppeerrttyy DDeessccrriippttiioonn
+lprf     Length of PRF marker segment in bytes
+PRFnum   Profile number
+******** TTeessttss ********
+TTeesstt nnaammee     TTrruuee iiff
+lprfIsValid   llpprrff is within range [4,65534]
+pprfIsValid   last pppprrff value is not zero
+PRFnumIsValid PPRRFFnnuumm > 4095
+********** CCoorrrreessppoonnddiinngg pprrooffiillee ((CCPPFF)) mmaarrkkeerr sseeggmmeenntt **********
+******** EElleemmeenntt nnaammee ********
+cpf
+******** RReeppoorrtteedd pprrooppeerrttiieess ********
+PPrrooppeerrttyy DDeessccrriippttiioonn
+lcpf     Length of CPF marker segment in bytes
+CPFnum   Profile number
+******** TTeessttss ********
+TTeesstt nnaammee   TTrruuee iiff
+lcpfIsValid llccppff is within range [4,65534] (JPH, JHC)
+pcpfIsValid last ppccppff value is not zero (JPH, JHC)
 ********** TTiillee ppaarrtt ((cchhiilldd ooff CCoonnttiigguuoouuss CCooddeessttrreeaamm bbooxx)) **********
 Tile-part level properties and tests. This is not a box or a marker segment!
 ******** EElleemmeenntt nnaammee ********
 tilePart (child of tileParts)
 ******** RReeppoorrtteedd pprrooppeerrttiieess ********
 Each tile part element can contain a number of child elements:
 CChhiilldd eelleemmeenntt DDeessccrriippttiioonn
@@ -1711,20 +1795,36 @@
 option is used. The number of PLT and PPT markers is given by the following 2
 derived properties (these are always reported, irrespective of --
 packetmarkers):
 PPrrooppeerrttyy DDeessccrriippttiioonn
 pltCount Number of PLT markers in tile part header
 pptCount Number of PPT markers in tile part header
 ******** TTeessttss ********
-TTeesstt nnaammee              TTrruuee iiff
-                       Tile part start offset + ttiilleePPaarrttLLeennggtthh points to either
-foundNextTilePartOrEOC start of new tile or EOC marker (useful for detecting
-                       within-codestream byte corruption)
-foundSODMarker         Last marker segment of tile part is a start-of-data
-                       (SOD) marker
+TTeesstt nnaammee                TTrruuee iiff
+CODAllowed               COD marker is allowed in this tile part (only allowed
+                         in first tile-part of a tile)
+COCAllowed               COC marker is allowed in this tile part (only allowed
+                         in first tile-part of a tile)
+QCDAllowed               QCD marker is allowed in this tile part (only allowed
+                         in first tile-part of a tile)
+QCCAllowed               QCC marker is allowed in this tile part (only allowed
+                         in first tile-part of a tile)
+RGNAllowed               RGN marker is allowed in this tile part (only allowed
+                         in first tile-part of a tile)
+                         No more than one ccccoocc value for each component in
+maxOneCcocPerComponentTP tile-part header (only reported if codestream contains
+                         any COC marker segments)
+                         No more than one ccqqcccc value for each component in
+maxOneCqccPerComponentTP tile-part header (only reported if codestream contains
+                         any QCC marker segments)
+                         Tile part start offset + ttiilleePPaarrttLLeennggtthh points to
+foundNextTilePartOrEOC   either start of new tile or EOC marker (useful for
+                         detecting within-codestream byte corruption)
+foundSODMarker           Last marker segment of tile part is a start-of-data
+                         (SOD) marker
 ********** SSttaarrtt ooff ttiillee ppaarrtt ((SSOOTT)) mmaarrkkeerr sseeggmmeenntt ((cchhiilldd ooff ttiillee ppaarrtt)) **********
 ******** EElleemmeenntt nnaammee ********
 sot
 ******** RReeppoorrtteedd pprrooppeerrttiieess ********
 PPrrooppeerrttyy DDeessccrriippttiioonn
 lsot     Length of SOT marker segment in bytes
 isot     Tile index
@@ -1750,44 +1850,44 @@
 ******** RReeppoorrtteedd pprrooppeerrttiieess ********
 PPrrooppeerrttyy DDeessccrriippttiioonn
 ******** TTeessttss ********
 TTeesstt nnaammee TTrruuee iiff
 ********** PPaacckkeett lleennggtthh,, mmaaiinn hheeaaddeerr ((PPLLMM)) mmaarrkkeerr sseeggmmeenntt **********
 ******** EElleemmeenntt nnaammee ********
 plm
-******** RReeppoorrtteedd pprrooppeerrttiieess_11_88 ********
+******** RReeppoorrtteedd pprrooppeerrttiieess_22_33 ********
 PPrrooppeerrttyy DDeessccrriippttiioonn
 lplm     Length of PLM marker segment in bytes
 zplm     PLM marker segment index
 nplm     Number of bytes of Iplm information for the ith tile-part
 iplm     Comma separated list of packet length values (as hexadecimal strings)
 ******** TTeessttss ********
 TTeesstt nnaammee TTrruuee iiff
 ********** PPaacckkeedd ppaacckkeett hheeaaddeerrss,, mmaaiinn hheeaaddeerr ((PPPPMM)) mmaarrkkeerr sseeggmmeenntt **********
 ******** EElleemmeenntt nnaammee ********
 ppm
-******** RReeppoorrtteedd pprrooppeerrttiieess_11_99 ********
+******** RReeppoorrtteedd pprrooppeerrttiieess_22_44 ********
 PPrrooppeerrttyy DDeessccrriippttiioonn
 ******** TTeessttss ********
 TTeesstt nnaammee TTrruuee iiff
 ********** PPaacckkeett lleennggtthh,, ttiillee--ppaarrtt hheeaaddeerr ((PPLLTT)) mmaarrkkeerr sseeggmmeenntt **********
 ******** EElleemmeenntt nnaammee ********
 plt
-******** RReeppoorrtteedd pprrooppeerrttiieess_22_00 ********
+******** RReeppoorrtteedd pprrooppeerrttiieess_22_55 ********
 PPrrooppeerrttyy DDeessccrriippttiioonn
 lplt     Length of PLT marker segment in bytes
 zplt     PLT marker segment index
 nplm     Number of bytes of Iplm information for the ith tile-part
 iplt     Comma separated list of packet length values (as hexadecimal strings)
 ******** TTeessttss ********
 TTeesstt nnaammee TTrruuee iiff
 ********** PPaacckkeedd ppaacckkeett hheeaaddeerrss,, ttiillee--ppaarrtt hheeaaddeerr ((PPPPTT)) mmaarrkkeerr sseeggmmeenntt **********
 ******** EElleemmeenntt nnaammee ********
 ppt
-******** RReeppoorrtteedd pprrooppeerrttiieess_22_11 ********
+******** RReeppoorrtteedd pprrooppeerrttiieess_22_66 ********
 PPrrooppeerrttyy DDeessccrriippttiioonn
 ******** TTeessttss ********
 TTeesstt nnaammee TTrruuee iiff
 ************ RReeffeerreenncceess ************
 ICC. Specification ICC.1:1998-09 â File Format for Color Profiles.
 International Color Consortium, 1998. _h_t_t_p_s_:_/_/_w_w_w_._c_o_l_o_r_._o_r_g_/_I_C_C_-_1___1_9_9_8_-_0_9_._p_d_f.
 ISO/IEC. Information technology â JPEG 2000 image coding system: Core coding
@@ -1800,40 +1900,51 @@
 Leach, P., Mealling, M. & Salz, R. A Universally Unique IDentifier (UUID) URN
 namespace. Memo, IETF. _h_t_t_p_s_:_/_/_t_o_o_l_s_._i_e_t_f_._o_r_g_/_h_t_m_l_/_r_f_c_4_1_2_2_._h_t_m_l.
 ===============================================================================
    1. The jjppyyllyyzzeerr binaries were created using the PPyyIInnssttaalllleerr package: _h_t_t_p_s_:_/
       _/_w_w_w_._p_y_i_n_s_t_a_l_l_e_r_._o_r_g_/_â__©_ï_¸_
    2. Note that jjppyyllyyzzeerr versions 1.8 and earlier returned a formatted XML
       string instead of an element object!_â__©_ï_¸_
-   3. Note that jjppyyllyyzzeerr versions 1.4 and earlier used the verbose output
+   3. Jpylyzer 2.2 and more recent only work with Python > 3.2. Since Jython
+      still hasnât been upgraded to support Python 3, Java integration with
+      Jython currently doesnât work._â__©_ï_¸_
+   4. Note that jjppyyllyyzzeerr versions 1.4 and earlier used the verbose output
       format by default. This behaviour has changed in version 1.5 onwards, as
       the lengthy output turned out to be slightly confusing to some
       users._â__©_ï_¸_
-   4. The âAny ICCâ method is defined in ISO/IEC 15444-2 (the JPX format),
-      and is not allowed in JP2. However, jjppyyllyyzzeerr offers limited support for
-      JPX here by also reporting the properties of ICC profiles that were
-      embedded using this method. Note that any file that uses this method will
-      fail the âmethIsValidâ test (and thereby the validation)._â__©_ï_¸_
-   5. Originally ISO/IEC 15444-1 only allowed âinput deviceâ profiles.
+   5. Meaning of values defined in Table 2 of Rec. ITU-T H.273 / ISO/IEC 23001-
+      8 _â___C_o_d_i_n_g_-_i_n_d_e_p_e_n_d_e_n_t_ _c_o_d_e_ _p_o_i_n_t_s_ _f_o_r_ _v_i_d_e_o_ _s_i_g_n_a_l_ _t_y_p_e
+      _i_d_e_n_t_i_f_i_c_a_t_i_o_n_â___â__©_ï_¸_
+   6. Meaning of values defined in Table 3 of Rec. ITU-T H.273 / ISO/IEC 23001-
+      8 _â___C_o_d_i_n_g_-_i_n_d_e_p_e_n_d_e_n_t_ _c_o_d_e_ _p_o_i_n_t_s_ _f_o_r_ _v_i_d_e_o_ _s_i_g_n_a_l_ _t_y_p_e
+      _i_d_e_n_t_i_f_i_c_a_t_i_o_n_â___â__©_ï_¸_
+   7. Meaning of values defined in Table 4 of Rec. ITU-T H.273 / ISO/IEC 23001-
+      8 _â___C_o_d_i_n_g_-_i_n_d_e_p_e_n_d_e_n_t_ _c_o_d_e_ _p_o_i_n_t_s_ _f_o_r_ _v_i_d_e_o_ _s_i_g_n_a_l_ _t_y_p_e
+      _i_d_e_n_t_i_f_i_c_a_t_i_o_n_â___â__©_ï_¸_
+   8. Meaning defined in Rec. ITU-T H.273 / ISO/IEC 23001-8 _â___C_o_d_i_n_g_-
+      _i_n_d_e_p_e_n_d_e_n_t_ _c_o_d_e_ _p_o_i_n_t_s_ _f_o_r_ _v_i_d_e_o_ _s_i_g_n_a_l_ _t_y_p_e_ _i_d_e_n_t_i_f_i_c_a_t_i_o_n_â___â__©_ï_¸_
+   9. Originally ISO/IEC 15444-1 only allowed âinput deviceâ profiles.
       Support of âdisplay deviceâ profiles was added through an _a_m_e_n_d_m_e_n_t
       to the standard in 2013. The behaviour of jjppyyllyyzzeerr is consistent with
       this amendment._â__©_ï_¸_
-   6. Calculated as: vRcN vRcD â¢ 10 vRcE _â__©_ï_¸_
-   7. Calculated as: hRcN hRcD â¢ 10 hRcE _â__©_ï_¸_
-   8. Calculated as: vRescInPixelsPerMeter â¢ 25.4 â¢ 10 -3 _â__©_ï_¸_
-   9. Calculated as: hRescInPixelsPerMeter â¢ 25.4 â¢ 10 -3 _â__©_ï_¸_
-  10. Calculated as: vRdN vRdD â¢ 10 vRdE _â__©_ï_¸_
-  11. Calculated as: hRdN hRdD â¢ 10 hRdE _â__©_ï_¸_
-  12. Calculated as: vResdInPixelsPerMeter â¢ 25.4 â¢ 10 -3 _â__©_ï_¸_
-  13. Calculated as: hResdInPixelsPerMeter â¢ 25.4 â¢ 10 -3 _â__©_ï_¸_
-  14. Link: _h_t_t_p_s_:_/_/_w_w_w_i_m_a_g_e_s_._a_d_o_b_e_._c_o_m_/_w_w_w_._a_d_o_b_e_._c_o_m_/_c_o_n_t_e_n_t_/_d_a_m_/_A_d_o_b_e_/_e_n_/
+  10. For JPH, an addition âapplication-definedâ value is allowed (ISO/IEC
+      15444-15, Table D.4)_â__©_ï_¸_
+  11. Calculated as: vRcN vRcD â¢ 10 vRcE _â__©_ï_¸_
+  12. Calculated as: hRcN hRcD â¢ 10 hRcE _â__©_ï_¸_
+  13. Calculated as: vRescInPixelsPerMeter â¢ 25.4 â¢ 10 -3 _â__©_ï_¸_
+  14. Calculated as: hRescInPixelsPerMeter â¢ 25.4 â¢ 10 -3 _â__©_ï_¸_
+  15. Calculated as: vRdN vRdD â¢ 10 vRdE _â__©_ï_¸_
+  16. Calculated as: hRdN hRdD â¢ 10 hRdE _â__©_ï_¸_
+  17. Calculated as: vResdInPixelsPerMeter â¢ 25.4 â¢ 10 -3 _â__©_ï_¸_
+  18. Calculated as: hResdInPixelsPerMeter â¢ 25.4 â¢ 10 -3 _â__©_ï_¸_
+  19. Link: _h_t_t_p_s_:_/_/_w_w_w_i_m_a_g_e_s_._a_d_o_b_e_._c_o_m_/_w_w_w_._a_d_o_b_e_._c_o_m_/_c_o_n_t_e_n_t_/_d_a_m_/_A_d_o_b_e_/_e_n_/
       _d_e_v_n_e_t_/_x_m_p_/_p_d_f_s_/_c_s_6_/_X_M_P_S_p_e_c_i_f_i_c_a_t_i_o_n_P_a_r_t_3_._p_d_f_â__©_ï_¸_
-  15. However, support for start of packet (SOP) and end of packet (EPH)
+  20. However, support for start of packet (SOP) and end of packet (EPH)
       markers may be included in future versions._â__©_ï_¸_
-  16. For example, in a TIFF to JP2 conversion workflow one could include a
+  21. For example, in a TIFF to JP2 conversion workflow one could include a
       pixel-by-pixel comparison of the values in the TIFF and the JP2._â__©_ï_¸_
-  17. Calculated as: numberOfTiles = [ xsiz - xOsiz xTsiz ] â¢ [ ysiz - yOsiz
+  22. Calculated as: numberOfTiles = [ xsiz - xOsiz xTsiz ] â¢ [ ysiz - yOsiz
       yTsiz ] _â__©_ï_¸_
-  18. Only reported if the --packetmarkers option is used._â__©_ï_¸_
-  19. Only reported if the --packetmarkers option is used._â__©_ï_¸_
-  20. Only reported if the --packetmarkers option is used._â__©_ï_¸_
-  21. Only reported if the --packetmarkers option is used._â__©_ï_¸_
+  23. Only reported if the --packetmarkers option is used._â__©_ï_¸_
+  24. Only reported if the --packetmarkers option is used._â__©_ï_¸_
+  25. Only reported if the --packetmarkers option is used._â__©_ï_¸_
+  26. Only reported if the --packetmarkers option is used._â__©_ï_¸_
```

### Comparing `jpylyzer-2.2.0b1/tests/unit/test_testfiles.py` & `jpylyzer-2.2.0rc1/tests/unit/test_testfiles.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,26 +114,30 @@
 "bitwiser-resolutionbox-corrupted-boxlength-8127.jp2": "False",
 "bitwiser-resolutionbox-corrupted-boxlength-8154.jp2": "False",
 "bitwiser-resolutionbox-corrupted-boxlength-8730.jp2": "False",
 "oj-tileindex-error-1.jp2": "False",
 "oj-tileindex-error-2.jp2": "False",
 "oj-tileindex-error-3.jp2": "False",
 "oj-tileindex-error-4.jp2": "False",
-"oj-tileindex-error-5.jp2": "False"
+"erdas-nullinput-uint8-rgb-null-2tileparts.jp2": "True",
+"erdas-sandiego1m_null.jp2": "True",
+"erdas-sandiego3i_5.2.jp2": "True",
+"erdas-sandiego3i_5.5.jp2": "True"
 }
 
 # Dictionary with names of all test files and validity against codestream
 validityLookupJ2C = {
 "is_codestream.jp2": "True"
 }
 
 # Dictionary with names of all test files and validity against JPH
 validityLookupJPH = {
-"oht-ht.jph": "False",
-"oj-ht-byte.jph": "True"
+"oht-ht.jph": "True",
+"oj-ht-byte.jph": "True",
+"wrongbpc-ht.jph": "False"
 }
 
 # Dictionary with names of all test files and validity against JHC
 validityLookupJHC = {
 "grok-ht.jhc": "True",
 "htj2k_cpf_broadcast.jhc": "False",
 "oht-ht.jhc": "True",
@@ -156,14 +160,23 @@
         thisFile = os.path.join(testFilesDir, key)
         assert os.path.isfile(thisFile)
 
     for key in validityLookupJ2C:
         thisFile = os.path.join(testFilesDir, key)
         assert os.path.isfile(thisFile)
 
+    for key in validityLookupJPH:
+        thisFile = os.path.join(testFilesDir, key)
+        assert os.path.isfile(thisFile)
+
+    for key in validityLookupJHC:
+        thisFile = os.path.join(testFilesDir, key)
+        assert os.path.isfile(thisFile)
+
+
 @pytest.mark.parametrize('inJP2', testFiles)
 
 def test_status_jp2(inJP2):
     """
     Tests for any internal errors based on statusInfo value
     using JP2 validation
     """
@@ -336,15 +349,14 @@
     # Parse XSD schema
     xmlschema_doc = etree.parse(xsdFile)
     xmlschema = etree.XMLSchema(xmlschema_doc)
     # Parse XML
     xml_doc = etree.fromstring(xmlOut.encode())
     assert xmlschema.validate(xml_doc)
 
-
 def test_xml_is_valid_jhc(capsys):
     """
     Run checkfiles function on all files in test corpus and
     verify resulting XML output validates against XSD schema
     """
     config.VALIDATION_FORMAT = "jhc"
     config.MIX_FLAG = 0
```

### Comparing `jpylyzer-2.2.0b1/tests/unit/test_jpylyzer.py` & `jpylyzer-2.2.0rc1/tests/unit/test_jpylyzer.py`

 * *Files identical despite different names*

### Comparing `jpylyzer-2.2.0b1/tests/unit/notest_openjpeg.py` & `jpylyzer-2.2.0rc1/tests/unit/notest_openjpeg.py`

 * *Files identical despite different names*

### Comparing `jpylyzer-2.2.0b1/PKG-INFO` & `jpylyzer-2.2.0rc1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: jpylyzer
-Version: 2.2.0b1
+Version: 2.2.0rc1
 Summary: JP2 (JPEG 2000 Part 1) image validator and properties extractor
 Home-page: http://jpylyzer.openpreservation.org/
 Author: Johan van der Knijff
 Author-email: johan.vanderknijff@kb.nl
 Maintainer: Johan van der Knijff
 Maintainer-email: johan.vanderknijff@kb.nl
 License: LGPL
-Download-URL: https://github.com/openpreserve/jpylyzer/archive/2.2.0b1.tar.gz
+Download-URL: https://github.com/openpreserve/jpylyzer/archive/2.2.0rc1.tar.gz
 Platform: POSIX
 Platform: Windows
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.2, <4
 Description-Content-Type: text/markdown
 Provides-Extra: testing
@@ -37,47 +37,71 @@
 - [![Build Status](https://jenkins.openpreservation.org/buildStatus/icon?job=jpylyzer%2Fjpylyzer)](https://jenkins.openpreservation.org/job/jpylyzer/job/jpylyzer/) OPF Jenkins
 <!-- Start of text to be copied to usage.md of jpylyzer website -->
 
 ## Using jpylyzer from the command line
 
 Calling *jpylyzer* in a command window without any arguments results in the following helper message:
 
-    usage: jpylyzer [-h] [--format FMT] [--mix {1,2}] [--nopretty]
-              [--nullxml] [--recurse] [--packetmarkers] [--verbose]
-              [--version] jp2In [jp2In ...]
+```
+usage: jpylyzer [-h] [--format FMT] [--mix {1,2}] [--nopretty]
+            [--nullxml] [--recurse] [--packetmarkers] [--verbose]
+            [--version] jp2In [jp2In ...]
+```
 
 ### Positional arguments
 
 |Argument|Description|
 |:--|:--|
-|`jp2In`|input JP2 image(s), may be one or more (whitespace-separated) path expressions; prefix wildcard (\*) with backslash (\\) in Linux|
+|`jp2In`|input image(s), may be one or more (whitespace-separated) path expressions; prefix wildcard (\*) with backslash (\\) in Linux|
 
 ### Optional arguments
 
 |Argument|Description|
 |:--|:--|
 |`[-h, --help]`|show help message and exit|
-|`[--format FMT]`|validation format; allowed values are `jp2` (used by default) and `j2c` (which activates raw codestream validation)|
+|`[--format FMT]`|validation format; allowed values are `jp2` (JPEG 2000 Part 1, used by default), `j2c` (Part 1 codestream), `jph` (JPEG 2000 Part 15 / High Throughput JPEG 2000) and `jhc` (Part 15 codestream)|
 |`[--mix {1,2}]`|report additional output in NISO MIX format (version 1.0 or 2.0)|
 |`[--nopretty]`|suppress pretty-printing of XML output|
 |`[--nullxml]`|extract null-terminated XML content from XML and UUID boxes(doesn't affect validation)|
 |`[--recurse, -r]`|when analysing a directory, recurse into subdirectories|
 |`[--packetmarkers]`|Report packet-level codestream markers (plm, ppm, plt, ppt)|
 |`[--verbose]`|report test results in verbose format|
 |`[-v, --version]`|show program's version number and exit|
 
 ## Output
 
 Output is directed to the standard output device (*stdout*).
 
-### Example
+## Examples
+
+Validate JP2 image:
+
+```
+jpylyzer rubbish.jp2 > rubbish-jp2.xml`
+```
+
+Validate JPEG 2000 Part 1 codestream:
+
+```
+jpylyzer --format j2c rubbish.j2c > rubbish-j2c.xml`
+```
+
+Validate JPH (High Throughput) image:
 
-`jpylyzer rubbish.jp2 > rubbish.xml`
+```
+jpylyzer --format jph rubbish.jph > rubbish-jph.xml`
+```
 
-In the above example, output is redirected to the file &#8216;rubbish.xml&#8217;. By default *jpylyzer*&#8217;s XML is pretty-printed, so you should be able to view the file using your favourite text editor. Alternatively use a dedicated XML editor, or open the file in your web browser.
+Validate JPEG 2000 Part 15 (High Throughput) codestream:
+
+```
+jpylyzer --format jhc rubbish.jhc > rubbish-jhc.xml`
+```
+
+In the above examples, output is redirected to the output files &#8216;rubbish-???.xml&#8217;. By default *jpylyzer*&#8217;s XML is pretty-printed, so you should be able to view the file using your favourite text editor. Alternatively use a dedicated XML editor, or open the file in your web browser.
 
 ## Output format
 
 The output file contains the following top-level elements:
 
 1. One *toolInfo* element, which contains information about *jpylyzer* (its name and version number)
 
@@ -96,14 +120,16 @@
 4. *tests*: outcome of the individual tests that are part of the
 validation process (organised by box)
 
 5. *properties*: image properties (organised by box)
 
 6. *propertiesExtension*: wrapper element for NISO *MIX* output (only if the `--mix` option is used)
 
+7. *warnings*: reported warnings
+
 ## Using jpylyzer as a Python module
 
 Instead of using *jpylyzer* from the command-line, you can also import
 it as a module in your own Python programs. To do so, install jpylyzer
 with *pip*. Then import *jpylyzer* into your code by adding:
 
 ```python
@@ -126,16 +152,15 @@
 
 # Return image height value
 imageHeight = myResult.findtext('./properties/jp2HeaderBox/imageHeaderBox/height')
 print(imageHeight)
 ```
 
 Here, *myResult* is an *Element* object that can either be used directly,
-or converted to XML using the *ElementTree* module[^3]. The structure of the
-element object follows the XML output that described in [Chapter 5](#output-format).
+or converted to XML using the *ElementTree* module[^3].
 
 For validation a raw JPEG 2000 codestreams, call the *checkOneFile* function with the additional
 *validationFormat* argument, and set it to `j2c`:
 
 ```python
 # Define Codestream
 myFile = "/home/johan/jpylyzer-test-files/rubbish.j2c"
```

### Comparing `jpylyzer-2.2.0b1/LICENSE` & `jpylyzer-2.2.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `jpylyzer-2.2.0b1/jpylyzer.egg-info/SOURCES.txt` & `jpylyzer-2.2.0rc1/jpylyzer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jpylyzer-2.2.0b1/jpylyzer.egg-info/PKG-INFO` & `jpylyzer-2.2.0rc1/jpylyzer.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: jpylyzer
-Version: 2.2.0b1
+Version: 2.2.0rc1
 Summary: JP2 (JPEG 2000 Part 1) image validator and properties extractor
 Home-page: http://jpylyzer.openpreservation.org/
 Author: Johan van der Knijff
 Author-email: johan.vanderknijff@kb.nl
 Maintainer: Johan van der Knijff
 Maintainer-email: johan.vanderknijff@kb.nl
 License: LGPL
-Download-URL: https://github.com/openpreserve/jpylyzer/archive/2.2.0b1.tar.gz
+Download-URL: https://github.com/openpreserve/jpylyzer/archive/2.2.0rc1.tar.gz
 Platform: POSIX
 Platform: Windows
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.2, <4
 Description-Content-Type: text/markdown
 Provides-Extra: testing
@@ -37,47 +37,71 @@
 - [![Build Status](https://jenkins.openpreservation.org/buildStatus/icon?job=jpylyzer%2Fjpylyzer)](https://jenkins.openpreservation.org/job/jpylyzer/job/jpylyzer/) OPF Jenkins
 <!-- Start of text to be copied to usage.md of jpylyzer website -->
 
 ## Using jpylyzer from the command line
 
 Calling *jpylyzer* in a command window without any arguments results in the following helper message:
 
-    usage: jpylyzer [-h] [--format FMT] [--mix {1,2}] [--nopretty]
-              [--nullxml] [--recurse] [--packetmarkers] [--verbose]
-              [--version] jp2In [jp2In ...]
+```
+usage: jpylyzer [-h] [--format FMT] [--mix {1,2}] [--nopretty]
+            [--nullxml] [--recurse] [--packetmarkers] [--verbose]
+            [--version] jp2In [jp2In ...]
+```
 
 ### Positional arguments
 
 |Argument|Description|
 |:--|:--|
-|`jp2In`|input JP2 image(s), may be one or more (whitespace-separated) path expressions; prefix wildcard (\*) with backslash (\\) in Linux|
+|`jp2In`|input image(s), may be one or more (whitespace-separated) path expressions; prefix wildcard (\*) with backslash (\\) in Linux|
 
 ### Optional arguments
 
 |Argument|Description|
 |:--|:--|
 |`[-h, --help]`|show help message and exit|
-|`[--format FMT]`|validation format; allowed values are `jp2` (used by default) and `j2c` (which activates raw codestream validation)|
+|`[--format FMT]`|validation format; allowed values are `jp2` (JPEG 2000 Part 1, used by default), `j2c` (Part 1 codestream), `jph` (JPEG 2000 Part 15 / High Throughput JPEG 2000) and `jhc` (Part 15 codestream)|
 |`[--mix {1,2}]`|report additional output in NISO MIX format (version 1.0 or 2.0)|
 |`[--nopretty]`|suppress pretty-printing of XML output|
 |`[--nullxml]`|extract null-terminated XML content from XML and UUID boxes(doesn't affect validation)|
 |`[--recurse, -r]`|when analysing a directory, recurse into subdirectories|
 |`[--packetmarkers]`|Report packet-level codestream markers (plm, ppm, plt, ppt)|
 |`[--verbose]`|report test results in verbose format|
 |`[-v, --version]`|show program's version number and exit|
 
 ## Output
 
 Output is directed to the standard output device (*stdout*).
 
-### Example
+## Examples
+
+Validate JP2 image:
+
+```
+jpylyzer rubbish.jp2 > rubbish-jp2.xml`
+```
+
+Validate JPEG 2000 Part 1 codestream:
+
+```
+jpylyzer --format j2c rubbish.j2c > rubbish-j2c.xml`
+```
+
+Validate JPH (High Throughput) image:
 
-`jpylyzer rubbish.jp2 > rubbish.xml`
+```
+jpylyzer --format jph rubbish.jph > rubbish-jph.xml`
+```
 
-In the above example, output is redirected to the file &#8216;rubbish.xml&#8217;. By default *jpylyzer*&#8217;s XML is pretty-printed, so you should be able to view the file using your favourite text editor. Alternatively use a dedicated XML editor, or open the file in your web browser.
+Validate JPEG 2000 Part 15 (High Throughput) codestream:
+
+```
+jpylyzer --format jhc rubbish.jhc > rubbish-jhc.xml`
+```
+
+In the above examples, output is redirected to the output files &#8216;rubbish-???.xml&#8217;. By default *jpylyzer*&#8217;s XML is pretty-printed, so you should be able to view the file using your favourite text editor. Alternatively use a dedicated XML editor, or open the file in your web browser.
 
 ## Output format
 
 The output file contains the following top-level elements:
 
 1. One *toolInfo* element, which contains information about *jpylyzer* (its name and version number)
 
@@ -96,14 +120,16 @@
 4. *tests*: outcome of the individual tests that are part of the
 validation process (organised by box)
 
 5. *properties*: image properties (organised by box)
 
 6. *propertiesExtension*: wrapper element for NISO *MIX* output (only if the `--mix` option is used)
 
+7. *warnings*: reported warnings
+
 ## Using jpylyzer as a Python module
 
 Instead of using *jpylyzer* from the command-line, you can also import
 it as a module in your own Python programs. To do so, install jpylyzer
 with *pip*. Then import *jpylyzer* into your code by adding:
 
 ```python
@@ -126,16 +152,15 @@
 
 # Return image height value
 imageHeight = myResult.findtext('./properties/jp2HeaderBox/imageHeaderBox/height')
 print(imageHeight)
 ```
 
 Here, *myResult* is an *Element* object that can either be used directly,
-or converted to XML using the *ElementTree* module[^3]. The structure of the
-element object follows the XML output that described in [Chapter 5](#output-format).
+or converted to XML using the *ElementTree* module[^3].
 
 For validation a raw JPEG 2000 codestreams, call the *checkOneFile* function with the additional
 *validationFormat* argument, and set it to `j2c`:
 
 ```python
 # Define Codestream
 myFile = "/home/johan/jpylyzer-test-files/rubbish.j2c"
```

