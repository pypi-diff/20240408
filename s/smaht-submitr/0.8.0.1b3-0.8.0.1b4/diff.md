# Comparing `tmp/smaht_submitr-0.8.0.1b3.tar.gz` & `tmp/smaht_submitr-0.8.0.1b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smaht_submitr-0.8.0.1b3.tar", max compression
+gzip compressed data, was "smaht_submitr-0.8.0.1b4.tar", max compression
```

## Comparing `smaht_submitr-0.8.0.1b3.tar` & `smaht_submitr-0.8.0.1b4.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     1098 2024-04-07 23:17:40.662078 smaht_submitr-0.8.0.1b3/LICENSE.txt
--rw-r--r--   0        0        0     2602 2024-04-07 23:17:40.662078 smaht_submitr-0.8.0.1b3/README.rst
--rw-r--r--   0        0        0     3425 2024-04-07 23:17:40.702078 smaht_submitr-0.8.0.1b3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-07 23:17:40.702078 smaht_submitr-0.8.0.1b3/submitr/__init__.py
--rw-r--r--   0        0        0      731 2024-04-07 23:17:40.702078 smaht_submitr-0.8.0.1b3/submitr/base.py
--rw-r--r--   0        0        0      294 2024-04-07 23:17:40.702078 smaht_submitr-0.8.0.1b3/submitr/exceptions.py
--rw-r--r--   0        0        0     2628 2024-04-07 23:17:40.702078 smaht_submitr-0.8.0.1b3/submitr/output.py
--rw-r--r--   0        0        0    13421 2024-04-07 23:17:40.702078 smaht_submitr-0.8.0.1b3/submitr/progress_bar.py
--rw-r--r--   0        0        0    10819 2024-04-07 23:17:40.702078 smaht_submitr-0.8.0.1b3/submitr/s3_utils.py
--rw-r--r--   0        0        0        0 2024-04-07 23:17:40.702078 smaht_submitr-0.8.0.1b3/submitr/scripts/__init__.py
--rw-r--r--   0        0        0     4785 2024-04-07 23:17:40.702078 smaht_submitr-0.8.0.1b3/submitr/scripts/check_submission.py
--rw-r--r--   0        0        0     8920 2024-04-07 23:17:40.702078 smaht_submitr-0.8.0.1b3/submitr/scripts/cli_utils.py
--rw-r--r--   0        0        0     1828 2024-04-07 23:17:40.702078 smaht_submitr-0.8.0.1b3/submitr/scripts/list_submissions.py
--rw-r--r--   0        0        0      940 2024-04-07 23:17:40.702078 smaht_submitr-0.8.0.1b3/submitr/scripts/make_sample_fastq_file.py
--rw-r--r--   0        0        0     5709 2024-04-07 23:17:40.702078 smaht_submitr-0.8.0.1b3/submitr/scripts/resume_uploads.py
--rw-r--r--   0        0        0     1368 2024-04-07 23:17:40.702078 smaht_submitr-0.8.0.1b3/submitr/scripts/show_upload_info.py
--rw-r--r--   0        0        0     1572 2024-04-07 23:17:40.702078 smaht_submitr-0.8.0.1b3/submitr/scripts/submit_genelist.py
--rw-r--r--   0        0        0    19891 2024-04-07 23:17:40.702078 smaht_submitr-0.8.0.1b3/submitr/scripts/submit_metadata_bundle.py
--rw-r--r--   0        0        0     3437 2024-04-07 23:17:40.702078 smaht_submitr-0.8.0.1b3/submitr/scripts/submit_ontology.py
--rw-r--r--   0        0        0     1616 2024-04-07 23:17:40.702078 smaht_submitr-0.8.0.1b3/submitr/scripts/upload_item_data.py
--rw-r--r--   0        0        0    28731 2024-04-07 23:17:40.702078 smaht_submitr-0.8.0.1b3/submitr/scripts/view_portal_object.py
--rw-r--r--   0        0        0   152631 2024-04-07 23:17:40.706078 smaht_submitr-0.8.0.1b3/submitr/submission.py
--rw-r--r--   0        0        0        0 2024-04-07 23:17:40.706078 smaht_submitr-0.8.0.1b3/submitr/tests/__init__.py
--rw-r--r--   0        0        0      355 2024-04-07 23:17:40.706078 smaht_submitr-0.8.0.1b3/submitr/tests/conftest_settings.py
--rw-r--r--   0        0        0      163 2024-04-07 23:17:40.706078 smaht_submitr-0.8.0.1b3/submitr/tests/data/f1_R1.fastq.gz
--rw-r--r--   0        0        0      165 2024-04-07 23:17:40.706078 smaht_submitr-0.8.0.1b3/submitr/tests/data/f1_R2.fastq.gz
--rw-r--r--   0        0        0      167 2024-04-07 23:17:40.706078 smaht_submitr-0.8.0.1b3/submitr/tests/data/f2_R1.fastq.gz
--rw-r--r--   0        0        0      164 2024-04-07 23:17:40.706078 smaht_submitr-0.8.0.1b3/submitr/tests/data/f2_R2.fastq.gz
--rw-r--r--   0        0        0      272 2024-04-07 23:17:40.706078 smaht_submitr-0.8.0.1b3/submitr/tests/data/simulated_bundle.json
--rw-r--r--   0        0        0    10870 2024-04-07 23:17:40.706078 smaht_submitr-0.8.0.1b3/submitr/tests/data/submission_simple.xlsx
--rw-r--r--   0        0        0    10875 2024-04-07 23:17:40.706078 smaht_submitr-0.8.0.1b3/submitr/tests/data/submission_simple2.xlsx
--rw-r--r--   0        0        0    13306 2024-04-07 23:17:40.706078 smaht_submitr-0.8.0.1b3/submitr/tests/data/submission_test.xlsx
--rw-r--r--   0        0        0    13192 2024-04-07 23:17:40.706078 smaht_submitr-0.8.0.1b3/submitr/tests/data/submission_test_with_errors.xlsx
--rw-r--r--   0        0        0      169 2024-04-07 23:17:40.706078 smaht_submitr-0.8.0.1b3/submitr/tests/data/test1_R1.fastq.gz
--rw-r--r--   0        0        0      168 2024-04-07 23:17:40.706078 smaht_submitr-0.8.0.1b3/submitr/tests/data/test1_R2.fastq.gz
--rw-r--r--   0        0        0     1333 2024-04-07 23:17:40.706078 smaht_submitr-0.8.0.1b3/submitr/tests/test_base.py
--rw-r--r--   0        0        0     2629 2024-04-07 23:17:40.706078 smaht_submitr-0.8.0.1b3/submitr/tests/test_check_submission.py
--rw-r--r--   0        0        0      551 2024-04-07 23:17:40.706078 smaht_submitr-0.8.0.1b3/submitr/tests/test_exceptions.py
--rw-r--r--   0        0        0     1620 2024-04-07 23:17:40.706078 smaht_submitr-0.8.0.1b3/submitr/tests/test_make_sample_fastq_file.py
--rw-r--r--   0        0        0     1421 2024-04-07 23:17:40.706078 smaht_submitr-0.8.0.1b3/submitr/tests/test_misc.py
--rw-r--r--   0        0        0    11606 2024-04-07 23:17:40.706078 smaht_submitr-0.8.0.1b3/submitr/tests/test_resume_uploads.py
--rw-r--r--   0        0        0     2478 2024-04-07 23:17:40.706078 smaht_submitr-0.8.0.1b3/submitr/tests/test_show_upload_info.py
--rw-r--r--   0        0        0   157490 2024-04-07 23:17:40.706078 smaht_submitr-0.8.0.1b3/submitr/tests/test_submission.py
--rw-r--r--   0        0        0     2836 2024-04-07 23:17:40.706078 smaht_submitr-0.8.0.1b3/submitr/tests/test_submit_genelist.py
--rw-r--r--   0        0        0     6874 2024-04-07 23:17:40.706078 smaht_submitr-0.8.0.1b3/submitr/tests/test_submit_metadata_bundle.py
--rw-r--r--   0        0        0     3013 2024-04-07 23:17:40.706078 smaht_submitr-0.8.0.1b3/submitr/tests/test_submit_ontology.py
--rw-r--r--   0        0        0     1300 2024-04-07 23:17:40.706078 smaht_submitr-0.8.0.1b3/submitr/tests/test_testing_helpers.py
--rw-r--r--   0        0        0     3661 2024-04-07 23:17:40.706078 smaht_submitr-0.8.0.1b3/submitr/tests/test_upload_item_data.py
--rw-r--r--   0        0        0     4353 2024-04-07 23:17:40.706078 smaht_submitr-0.8.0.1b3/submitr/tests/test_utils.py
--rw-r--r--   0        0        0     1351 2024-04-07 23:17:40.706078 smaht_submitr-0.8.0.1b3/submitr/tests/testing_helpers.py
--rw-r--r--   0        0        0    12167 2024-04-07 23:17:40.706078 smaht_submitr-0.8.0.1b3/submitr/utils.py
--rw-r--r--   0        0        0     3994 1970-01-01 00:00:00.000000 smaht_submitr-0.8.0.1b3/PKG-INFO
+-rw-r--r--   0        0        0     1098 2024-04-08 02:00:21.319269 smaht_submitr-0.8.0.1b4/LICENSE.txt
+-rw-r--r--   0        0        0     2602 2024-04-08 02:00:21.319269 smaht_submitr-0.8.0.1b4/README.rst
+-rw-r--r--   0        0        0     3425 2024-04-08 02:00:21.359269 smaht_submitr-0.8.0.1b4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-08 02:00:21.359269 smaht_submitr-0.8.0.1b4/submitr/__init__.py
+-rw-r--r--   0        0        0      731 2024-04-08 02:00:21.359269 smaht_submitr-0.8.0.1b4/submitr/base.py
+-rw-r--r--   0        0        0      294 2024-04-08 02:00:21.359269 smaht_submitr-0.8.0.1b4/submitr/exceptions.py
+-rw-r--r--   0        0        0     2628 2024-04-08 02:00:21.359269 smaht_submitr-0.8.0.1b4/submitr/output.py
+-rw-r--r--   0        0        0    13423 2024-04-08 02:00:21.359269 smaht_submitr-0.8.0.1b4/submitr/progress_bar.py
+-rw-r--r--   0        0        0    10819 2024-04-08 02:00:21.359269 smaht_submitr-0.8.0.1b4/submitr/s3_utils.py
+-rw-r--r--   0        0        0        0 2024-04-08 02:00:21.359269 smaht_submitr-0.8.0.1b4/submitr/scripts/__init__.py
+-rw-r--r--   0        0        0     4785 2024-04-08 02:00:21.359269 smaht_submitr-0.8.0.1b4/submitr/scripts/check_submission.py
+-rw-r--r--   0        0        0     9732 2024-04-08 02:00:21.359269 smaht_submitr-0.8.0.1b4/submitr/scripts/cli_utils.py
+-rw-r--r--   0        0        0     1828 2024-04-08 02:00:21.359269 smaht_submitr-0.8.0.1b4/submitr/scripts/list_submissions.py
+-rw-r--r--   0        0        0      940 2024-04-08 02:00:21.359269 smaht_submitr-0.8.0.1b4/submitr/scripts/make_sample_fastq_file.py
+-rw-r--r--   0        0        0     5709 2024-04-08 02:00:21.359269 smaht_submitr-0.8.0.1b4/submitr/scripts/resume_uploads.py
+-rw-r--r--   0        0        0     1368 2024-04-08 02:00:21.359269 smaht_submitr-0.8.0.1b4/submitr/scripts/show_upload_info.py
+-rw-r--r--   0        0        0     1572 2024-04-08 02:00:21.359269 smaht_submitr-0.8.0.1b4/submitr/scripts/submit_genelist.py
+-rw-r--r--   0        0        0    19891 2024-04-08 02:00:21.359269 smaht_submitr-0.8.0.1b4/submitr/scripts/submit_metadata_bundle.py
+-rw-r--r--   0        0        0     3437 2024-04-08 02:00:21.359269 smaht_submitr-0.8.0.1b4/submitr/scripts/submit_ontology.py
+-rw-r--r--   0        0        0     1616 2024-04-08 02:00:21.359269 smaht_submitr-0.8.0.1b4/submitr/scripts/upload_item_data.py
+-rw-r--r--   0        0        0    28731 2024-04-08 02:00:21.359269 smaht_submitr-0.8.0.1b4/submitr/scripts/view_portal_object.py
+-rw-r--r--   0        0        0   152631 2024-04-08 02:00:21.359269 smaht_submitr-0.8.0.1b4/submitr/submission.py
+-rw-r--r--   0        0        0        0 2024-04-08 02:00:21.359269 smaht_submitr-0.8.0.1b4/submitr/tests/__init__.py
+-rw-r--r--   0        0        0      355 2024-04-08 02:00:21.359269 smaht_submitr-0.8.0.1b4/submitr/tests/conftest_settings.py
+-rw-r--r--   0        0        0      163 2024-04-08 02:00:21.359269 smaht_submitr-0.8.0.1b4/submitr/tests/data/f1_R1.fastq.gz
+-rw-r--r--   0        0        0      165 2024-04-08 02:00:21.359269 smaht_submitr-0.8.0.1b4/submitr/tests/data/f1_R2.fastq.gz
+-rw-r--r--   0        0        0      167 2024-04-08 02:00:21.359269 smaht_submitr-0.8.0.1b4/submitr/tests/data/f2_R1.fastq.gz
+-rw-r--r--   0        0        0      164 2024-04-08 02:00:21.359269 smaht_submitr-0.8.0.1b4/submitr/tests/data/f2_R2.fastq.gz
+-rw-r--r--   0        0        0      272 2024-04-08 02:00:21.359269 smaht_submitr-0.8.0.1b4/submitr/tests/data/simulated_bundle.json
+-rw-r--r--   0        0        0    10870 2024-04-08 02:00:21.359269 smaht_submitr-0.8.0.1b4/submitr/tests/data/submission_simple.xlsx
+-rw-r--r--   0        0        0    10875 2024-04-08 02:00:21.359269 smaht_submitr-0.8.0.1b4/submitr/tests/data/submission_simple2.xlsx
+-rw-r--r--   0        0        0    13306 2024-04-08 02:00:21.359269 smaht_submitr-0.8.0.1b4/submitr/tests/data/submission_test.xlsx
+-rw-r--r--   0        0        0    13192 2024-04-08 02:00:21.359269 smaht_submitr-0.8.0.1b4/submitr/tests/data/submission_test_with_errors.xlsx
+-rw-r--r--   0        0        0      169 2024-04-08 02:00:21.359269 smaht_submitr-0.8.0.1b4/submitr/tests/data/test1_R1.fastq.gz
+-rw-r--r--   0        0        0      168 2024-04-08 02:00:21.359269 smaht_submitr-0.8.0.1b4/submitr/tests/data/test1_R2.fastq.gz
+-rw-r--r--   0        0        0     1333 2024-04-08 02:00:21.359269 smaht_submitr-0.8.0.1b4/submitr/tests/test_base.py
+-rw-r--r--   0        0        0     2629 2024-04-08 02:00:21.359269 smaht_submitr-0.8.0.1b4/submitr/tests/test_check_submission.py
+-rw-r--r--   0        0        0      551 2024-04-08 02:00:21.359269 smaht_submitr-0.8.0.1b4/submitr/tests/test_exceptions.py
+-rw-r--r--   0        0        0     1620 2024-04-08 02:00:21.359269 smaht_submitr-0.8.0.1b4/submitr/tests/test_make_sample_fastq_file.py
+-rw-r--r--   0        0        0     1421 2024-04-08 02:00:21.359269 smaht_submitr-0.8.0.1b4/submitr/tests/test_misc.py
+-rw-r--r--   0        0        0    11606 2024-04-08 02:00:21.359269 smaht_submitr-0.8.0.1b4/submitr/tests/test_resume_uploads.py
+-rw-r--r--   0        0        0     2478 2024-04-08 02:00:21.359269 smaht_submitr-0.8.0.1b4/submitr/tests/test_show_upload_info.py
+-rw-r--r--   0        0        0   157490 2024-04-08 02:00:21.363268 smaht_submitr-0.8.0.1b4/submitr/tests/test_submission.py
+-rw-r--r--   0        0        0     2836 2024-04-08 02:00:21.363268 smaht_submitr-0.8.0.1b4/submitr/tests/test_submit_genelist.py
+-rw-r--r--   0        0        0     6874 2024-04-08 02:00:21.363268 smaht_submitr-0.8.0.1b4/submitr/tests/test_submit_metadata_bundle.py
+-rw-r--r--   0        0        0     3013 2024-04-08 02:00:21.363268 smaht_submitr-0.8.0.1b4/submitr/tests/test_submit_ontology.py
+-rw-r--r--   0        0        0     1300 2024-04-08 02:00:21.363268 smaht_submitr-0.8.0.1b4/submitr/tests/test_testing_helpers.py
+-rw-r--r--   0        0        0     3661 2024-04-08 02:00:21.363268 smaht_submitr-0.8.0.1b4/submitr/tests/test_upload_item_data.py
+-rw-r--r--   0        0        0     4353 2024-04-08 02:00:21.363268 smaht_submitr-0.8.0.1b4/submitr/tests/test_utils.py
+-rw-r--r--   0        0        0     1351 2024-04-08 02:00:21.363268 smaht_submitr-0.8.0.1b4/submitr/tests/testing_helpers.py
+-rw-r--r--   0        0        0    12167 2024-04-08 02:00:21.363268 smaht_submitr-0.8.0.1b4/submitr/utils.py
+-rw-r--r--   0        0        0     3994 1970-01-01 00:00:00.000000 smaht_submitr-0.8.0.1b4/PKG-INFO
```

### Comparing `smaht_submitr-0.8.0.1b3/LICENSE.txt` & `smaht_submitr-0.8.0.1b4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b3/README.rst` & `smaht_submitr-0.8.0.1b4/README.rst`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b3/pyproject.toml` & `smaht_submitr-0.8.0.1b4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "smaht-submitr"
-version = "0.8.0.1b3"  # TODO: To become 0.8.1
+version = "0.8.0.1b4"  # TODO: To become 0.8.1
 description = "Support for uploading file submissions to SMAHT."
 # TODO: Update this email address when a more specific one is available for SMaHT.
 authors = ["SMaHT DAC <smhelp@hms-dbmi.atlassian.net >"]
 license = "MIT"
 readme = "README.rst"
 keywords = ["submitr", "smaht"]
 homepage = "https://github.com/smaht-dac/submitr"
```

### Comparing `smaht_submitr-0.8.0.1b3/submitr/base.py` & `smaht_submitr-0.8.0.1b4/submitr/base.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b3/submitr/output.py` & `smaht_submitr-0.8.0.1b4/submitr/output.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b3/submitr/progress_bar.py` & `smaht_submitr-0.8.0.1b4/submitr/progress_bar.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
         self._interrupt_handler = None
         if self._catch_interrupt:
             self._interrupt_handler = self._define_interrupt_handler()
         if self._tidy_output_hack is True:
             self._tidy_output_hack = self._define_tidy_output_hack()
         self._total = total if isinstance(total, int) and total >= 0 else 0
         self._description = self._format_description(description)
-        self._initialize()
+        # self._initialize()
 
     def _initialize(self) -> bool:
         # Do not actually create the tqdm object unless/until we have a positive total.
         if (self._bar is None) and (self._total > 0):
             bar_format = "{l_bar}{bar}| {n_fmt}/{total_fmt} | {rate_fmt} | {elapsed}{postfix} | ETA: {remaining} "
             self._bar = TQDM(total=self._total, desc=self._description,
                              dynamic_ncols=True, bar_format=bar_format, unit="", file=sys.stdout)
```

### Comparing `smaht_submitr-0.8.0.1b3/submitr/s3_utils.py` & `smaht_submitr-0.8.0.1b4/submitr/s3_utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b3/submitr/scripts/check_submission.py` & `smaht_submitr-0.8.0.1b4/submitr/scripts/check_submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b3/submitr/scripts/cli_utils.py` & `smaht_submitr-0.8.0.1b4/submitr/scripts/cli_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import argparse
 from functools import lru_cache
 import io
+import subprocess
 import sys
 import webbrowser
 from typing import List, Optional, Union
+from dcicutils.command_utils import yes_or_no
 from dcicutils.misc_utils import PRINT
 from submitr.utils import get_version, get_most_recent_version_info, print_boxed
 
 
 class CustomArgumentParser(argparse.ArgumentParser):
 
     PACKAGE = "smaht-submitr"
@@ -149,14 +151,23 @@
                     "===",
                     "For all versions please see: https://pypi.org/project/smaht-submitr",
                     "===",
                     self.COPYRIGHT,
                     "==="
                 ]
                 print_boxed(lines, right_justified_macro=("[VERSION]", self._get_version))
+                if not has_most_recent_version and most_recent_version_info.this_release_date:
+                    is_beta_version = ("a" in most_recent_version_info.this_version or
+                                       "b" in most_recent_version_info.this_version)
+                    if is_beta_version and most_recent_version_info.beta_version:
+                        version_to_update_to = most_recent_version_info.beta_version
+                    else:
+                        version_to_update_to = most_recent_version_info.version
+                    if yes_or_no(f"Do you want to install the newer version ({version_to_update_to})?"):
+                        subprocess.run(["pip", "install", f"{self._package}=={version_to_update_to}"])
                 return
             else:
                 PRINT(f"{self._package or 'COMMAND'}: {version}")
                 return
         PRINT(f"{self._package or 'COMMAND'}: No version available")
 
     @lru_cache(maxsize=1)
```

### Comparing `smaht_submitr-0.8.0.1b3/submitr/scripts/list_submissions.py` & `smaht_submitr-0.8.0.1b4/submitr/scripts/list_submissions.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b3/submitr/scripts/make_sample_fastq_file.py` & `smaht_submitr-0.8.0.1b4/submitr/scripts/make_sample_fastq_file.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b3/submitr/scripts/resume_uploads.py` & `smaht_submitr-0.8.0.1b4/submitr/scripts/resume_uploads.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b3/submitr/scripts/show_upload_info.py` & `smaht_submitr-0.8.0.1b4/submitr/scripts/show_upload_info.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b3/submitr/scripts/submit_genelist.py` & `smaht_submitr-0.8.0.1b4/submitr/scripts/submit_genelist.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b3/submitr/scripts/submit_metadata_bundle.py` & `smaht_submitr-0.8.0.1b4/submitr/scripts/submit_metadata_bundle.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b3/submitr/scripts/submit_ontology.py` & `smaht_submitr-0.8.0.1b4/submitr/scripts/submit_ontology.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b3/submitr/scripts/upload_item_data.py` & `smaht_submitr-0.8.0.1b4/submitr/scripts/upload_item_data.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b3/submitr/scripts/view_portal_object.py` & `smaht_submitr-0.8.0.1b4/submitr/scripts/view_portal_object.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b3/submitr/submission.py` & `smaht_submitr-0.8.0.1b4/submitr/submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b3/submitr/tests/data/submission_simple.xlsx` & `smaht_submitr-0.8.0.1b4/submitr/tests/data/submission_simple.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b3/submitr/tests/data/submission_simple2.xlsx` & `smaht_submitr-0.8.0.1b4/submitr/tests/data/submission_simple2.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b3/submitr/tests/data/submission_test.xlsx` & `smaht_submitr-0.8.0.1b4/submitr/tests/data/submission_test.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b3/submitr/tests/data/submission_test_with_errors.xlsx` & `smaht_submitr-0.8.0.1b4/submitr/tests/data/submission_test_with_errors.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b3/submitr/tests/test_base.py` & `smaht_submitr-0.8.0.1b4/submitr/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b3/submitr/tests/test_check_submission.py` & `smaht_submitr-0.8.0.1b4/submitr/tests/test_check_submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b3/submitr/tests/test_exceptions.py` & `smaht_submitr-0.8.0.1b4/submitr/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b3/submitr/tests/test_make_sample_fastq_file.py` & `smaht_submitr-0.8.0.1b4/submitr/tests/test_make_sample_fastq_file.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b3/submitr/tests/test_misc.py` & `smaht_submitr-0.8.0.1b4/submitr/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b3/submitr/tests/test_resume_uploads.py` & `smaht_submitr-0.8.0.1b4/submitr/tests/test_resume_uploads.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b3/submitr/tests/test_show_upload_info.py` & `smaht_submitr-0.8.0.1b4/submitr/tests/test_show_upload_info.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b3/submitr/tests/test_submission.py` & `smaht_submitr-0.8.0.1b4/submitr/tests/test_submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b3/submitr/tests/test_submit_genelist.py` & `smaht_submitr-0.8.0.1b4/submitr/tests/test_submit_genelist.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b3/submitr/tests/test_submit_metadata_bundle.py` & `smaht_submitr-0.8.0.1b4/submitr/tests/test_submit_metadata_bundle.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b3/submitr/tests/test_submit_ontology.py` & `smaht_submitr-0.8.0.1b4/submitr/tests/test_submit_ontology.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b3/submitr/tests/test_testing_helpers.py` & `smaht_submitr-0.8.0.1b4/submitr/tests/test_testing_helpers.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b3/submitr/tests/test_upload_item_data.py` & `smaht_submitr-0.8.0.1b4/submitr/tests/test_upload_item_data.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b3/submitr/tests/test_utils.py` & `smaht_submitr-0.8.0.1b4/submitr/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b3/submitr/tests/testing_helpers.py` & `smaht_submitr-0.8.0.1b4/submitr/tests/testing_helpers.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b3/submitr/utils.py` & `smaht_submitr-0.8.0.1b4/submitr/utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b3/PKG-INFO` & `smaht_submitr-0.8.0.1b4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smaht-submitr
-Version: 0.8.0.1b3
+Version: 0.8.0.1b4
 Summary: Support for uploading file submissions to SMAHT.
 Home-page: https://github.com/smaht-dac/submitr
 License: MIT
 Keywords: submitr,smaht
 Author: SMaHT DAC
 Author-email: smhelp@hms-dbmi.atlassian.net 
 Requires-Python: >=3.8.0,<3.12
```

