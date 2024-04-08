# Comparing `tmp/ocptv-pci_lmt-1.2.1.tar.gz` & `tmp/ocptv-pci_lmt-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocptv-pci_lmt-1.2.1.tar", last modified: Wed Nov 15 19:03:20 2023, max compression
+gzip compressed data, was "ocptv-pci_lmt-1.3.0.tar", last modified: Mon Apr  8 19:41:45 2024, max compression
```

## Comparing `ocptv-pci_lmt-1.2.1.tar` & `ocptv-pci_lmt-1.3.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 19:03:20.382171 ocptv-pci_lmt-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2023-11-15 19:03:07.000000 ocptv-pci_lmt-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-11-15 19:03:07.000000 ocptv-pci_lmt-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5966 2023-11-15 19:03:20.382171 ocptv-pci_lmt-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3719 2023-11-15 19:03:07.000000 ocptv-pci_lmt-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 19:03:20.378171 ocptv-pci_lmt-1.2.1/configs/
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2023-11-15 19:03:07.000000 ocptv-pci_lmt-1.2.1/configs/test_config.json
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2023-11-15 19:03:07.000000 ocptv-pci_lmt-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-15 19:03:20.382171 ocptv-pci_lmt-1.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 19:03:20.378171 ocptv-pci_lmt-1.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 19:03:20.378171 ocptv-pci_lmt-1.2.1/src/ocptv_pci_lmt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5966 2023-11-15 19:03:20.000000 ocptv-pci_lmt-1.2.1/src/ocptv_pci_lmt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      585 2023-11-15 19:03:20.000000 ocptv-pci_lmt-1.2.1/src/ocptv_pci_lmt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-15 19:03:20.000000 ocptv-pci_lmt-1.2.1/src/ocptv_pci_lmt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2023-11-15 19:03:20.000000 ocptv-pci_lmt-1.2.1/src/ocptv_pci_lmt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2023-11-15 19:03:20.000000 ocptv-pci_lmt-1.2.1/src/ocptv_pci_lmt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-11-15 19:03:20.000000 ocptv-pci_lmt-1.2.1/src/ocptv_pci_lmt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 19:03:20.378171 ocptv-pci_lmt-1.2.1/src/pci_lmt/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2023-11-15 19:03:07.000000 ocptv-pci_lmt-1.2.1/src/pci_lmt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2023-11-15 19:03:07.000000 ocptv-pci_lmt-1.2.1/src/pci_lmt/args.py
--rw-r--r--   0 runner    (1001) docker     (127)    11467 2023-11-15 19:03:07.000000 ocptv-pci_lmt-1.2.1/src/pci_lmt/collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2023-11-15 19:03:07.000000 ocptv-pci_lmt-1.2.1/src/pci_lmt/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6658 2023-11-15 19:03:07.000000 ocptv-pci_lmt-1.2.1/src/pci_lmt/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    10538 2023-11-15 19:03:07.000000 ocptv-pci_lmt-1.2.1/src/pci_lmt/device.py
--rw-r--r--   0 runner    (1001) docker     (127)      518 2023-11-15 19:03:07.000000 ocptv-pci_lmt-1.2.1/src/pci_lmt/host.py
--rw-r--r--   0 runner    (1001) docker     (127)    40032 2023-11-15 19:03:07.000000 ocptv-pci_lmt-1.2.1/src/pci_lmt/pcie_lane_margining.py
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2023-11-15 19:03:07.000000 ocptv-pci_lmt-1.2.1/src/pci_lmt/results.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 19:03:20.378171 ocptv-pci_lmt-1.2.1/src/pci_lmt_bin/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2023-11-15 19:03:07.000000 ocptv-pci_lmt-1.2.1/src/pci_lmt_bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2023-11-15 19:03:07.000000 ocptv-pci_lmt-1.2.1/src/pci_lmt_bin/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:41:45.987695 ocptv-pci_lmt-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-08 19:41:36.000000 ocptv-pci_lmt-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-08 19:41:36.000000 ocptv-pci_lmt-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5966 2024-04-08 19:41:45.987695 ocptv-pci_lmt-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-04-08 19:41:36.000000 ocptv-pci_lmt-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:41:45.983695 ocptv-pci_lmt-1.3.0/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-08 19:41:36.000000 ocptv-pci_lmt-1.3.0/configs/test_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-04-08 19:41:36.000000 ocptv-pci_lmt-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 19:41:45.987695 ocptv-pci_lmt-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:41:45.983695 ocptv-pci_lmt-1.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:41:45.987695 ocptv-pci_lmt-1.3.0/src/ocptv_pci_lmt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5966 2024-04-08 19:41:45.000000 ocptv-pci_lmt-1.3.0/src/ocptv_pci_lmt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-08 19:41:45.000000 ocptv-pci_lmt-1.3.0/src/ocptv_pci_lmt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 19:41:45.000000 ocptv-pci_lmt-1.3.0/src/ocptv_pci_lmt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-08 19:41:45.000000 ocptv-pci_lmt-1.3.0/src/ocptv_pci_lmt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-08 19:41:45.000000 ocptv-pci_lmt-1.3.0/src/ocptv_pci_lmt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-08 19:41:45.000000 ocptv-pci_lmt-1.3.0/src/ocptv_pci_lmt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:41:45.983695 ocptv-pci_lmt-1.3.0/src/pci_lmt/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-08 19:41:36.000000 ocptv-pci_lmt-1.3.0/src/pci_lmt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-08 19:41:36.000000 ocptv-pci_lmt-1.3.0/src/pci_lmt/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11973 2024-04-08 19:41:36.000000 ocptv-pci_lmt-1.3.0/src/pci_lmt/collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-08 19:41:36.000000 ocptv-pci_lmt-1.3.0/src/pci_lmt/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6658 2024-04-08 19:41:36.000000 ocptv-pci_lmt-1.3.0/src/pci_lmt/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10538 2024-04-08 19:41:36.000000 ocptv-pci_lmt-1.3.0/src/pci_lmt/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-08 19:41:36.000000 ocptv-pci_lmt-1.3.0/src/pci_lmt/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39776 2024-04-08 19:41:36.000000 ocptv-pci_lmt-1.3.0/src/pci_lmt/pcie_lane_margining.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-08 19:41:36.000000 ocptv-pci_lmt-1.3.0/src/pci_lmt/results.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:41:45.983695 ocptv-pci_lmt-1.3.0/src/pci_lmt_bin/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-08 19:41:36.000000 ocptv-pci_lmt-1.3.0/src/pci_lmt_bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-04-08 19:41:36.000000 ocptv-pci_lmt-1.3.0/src/pci_lmt_bin/main.py
```

### Comparing `ocptv-pci_lmt-1.2.1/LICENSE` & `ocptv-pci_lmt-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ocptv-pci_lmt-1.2.1/PKG-INFO` & `ocptv-pci_lmt-1.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocptv-pci_lmt
-Version: 1.2.1
+Version: 1.3.0
 Summary: PCI Lane Margining Tool
 Author-email: OCP Test & Validation <ocp-test-validation@OCP-All.groups.io>
 License: MIT License
         
         Copyright (c) 2023 Open Compute Project
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -27,17 +27,17 @@
         
 Project-URL: Homepage, https://github.com/opencomputeproject/ocp-diag-pci_lmt
 Project-URL: Bug reports, https://github.com/opencomputeproject/ocp-diag-pci_lmt/issues
 Project-URL: Source, https://github.com/opencomputeproject/ocp-diag-pci_lmt
 Keywords: ocp,ocptv,pci,pcie,lmt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: System :: Hardware
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: bumpver; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
```

### Comparing `ocptv-pci_lmt-1.2.1/README.md` & `ocptv-pci_lmt-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ocptv-pci_lmt-1.2.1/configs/test_config.json` & `ocptv-pci_lmt-1.3.0/configs/test_config.json`

 * *Files identical despite different names*

### Comparing `ocptv-pci_lmt-1.2.1/pyproject.toml` & `ocptv-pci_lmt-1.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ocptv-pci_lmt"
-version = "1.2.1"
+version = "1.3.0"
 description = "PCI Lane Margining Tool"
 readme = "README.md"
 authors = [
     { name = "OCP Test & Validation", email = "ocp-test-validation@OCP-All.groups.io" },
 ]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
-    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.8",
     "Topic :: System :: Hardware",
 ]
 keywords = ["ocp", "ocptv", "pci", "pcie", "lmt"]
 dependencies = []
-requires-python = ">=3.9"
+requires-python = ">=3.8"
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pylint", "mypy", "build", "twine"]
 
 [project.urls]
 "Homepage" = "https://github.com/opencomputeproject/ocp-diag-pci_lmt"
 "Bug reports" = "https://github.com/opencomputeproject/ocp-diag-pci_lmt/issues"
@@ -32,15 +32,15 @@
 [project.scripts]
 pci_lmt = "pci_lmt_bin.main:main"
 
 # Increment MAJOR version when you make incompatible API changes
 # Increment MINOR version when you add functionality in a backward compatible manner
 # Increment PATCH version when you make backward compatible bug fixes
 [tool.bumpver]
-current_version = "1.2.1"
+current_version = "1.3.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `ocptv-pci_lmt-1.2.1/src/ocptv_pci_lmt.egg-info/PKG-INFO` & `ocptv-pci_lmt-1.3.0/src/ocptv_pci_lmt.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ocptv-pci-lmt
-Version: 1.2.1
+Name: ocptv-pci_lmt
+Version: 1.3.0
 Summary: PCI Lane Margining Tool
 Author-email: OCP Test & Validation <ocp-test-validation@OCP-All.groups.io>
 License: MIT License
         
         Copyright (c) 2023 Open Compute Project
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -27,17 +27,17 @@
         
 Project-URL: Homepage, https://github.com/opencomputeproject/ocp-diag-pci_lmt
 Project-URL: Bug reports, https://github.com/opencomputeproject/ocp-diag-pci_lmt/issues
 Project-URL: Source, https://github.com/opencomputeproject/ocp-diag-pci_lmt
 Keywords: ocp,ocptv,pci,pcie,lmt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: System :: Hardware
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: bumpver; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
```

### Comparing `ocptv-pci_lmt-1.2.1/src/ocptv_pci_lmt.egg-info/SOURCES.txt` & `ocptv-pci_lmt-1.3.0/src/ocptv_pci_lmt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ocptv-pci_lmt-1.2.1/src/pci_lmt/args.py` & `ocptv-pci_lmt-1.3.0/src/pci_lmt/args.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,7 +41,13 @@
     )
     parser.add_argument(
         "--version",
         action="version",
         help="Print tool version and exit.",
         version="%(prog)s " + PCI_LMT_VERSION,
     )
+    parser.add_argument(
+        "--force",
+        dest="force_margin",
+        action="store_true",
+        help="Force margining on devices that doesn't support independent sampling. Default: False",
+    )
```

### Comparing `ocptv-pci_lmt-1.2.1/src/pci_lmt/collector.py` & `ocptv-pci_lmt-1.3.0/src/pci_lmt/collector.py`

 * *Files 11% similar despite different names*

```diff
@@ -47,38 +47,45 @@
                 dev.clear_error_log(lane=lane, receiver_number=self.receiver_number)
 
     def no_command_on_device_list(self):
         for dev in self._primed_devices:
             for lane in range(dev.device_info.width):
                 dev.no_command(lane=lane)
 
-    def info_lane_margin_on_device_list(self):
+    def info_lane_margin_on_device_list(self, args: argparse.Namespace):
         for dev in self.devices:
-            for lane in [0]:
-                ret = dev.goto_normal_settings(lane=lane, receiver_number=self.receiver_number)
-                ret = dev.fetch_margin_control_capabilities(lane=lane, receiver_number=self.receiver_number)
-                if ret["error"] is None:
+            # Collect lane margin capabilties only from lane-0 since it's going to be same
+            # for all lanes on that device.
+            ret = dev.goto_normal_settings(lane=0, receiver_number=self.receiver_number)
+            ret = dev.fetch_margin_control_capabilities(lane=0, receiver_number=self.receiver_number)
+
+            status_str = f"Device {dev.device_info.bdf} ReceiverNum {self.receiver_number} "
+            if ret["error"]:
+                dev.primed = False
+                status_str += f"NOT PRIMED {ret['error']}"
+            else:
+                # By default, allow devices only with independent error sampler to be primed.
+                # Allow devices with no independent error sampler to be primed only if it's forced by user.
+                if dev.device_info.ind_error_sampler:
                     dev.primed = True
-                    logger.info(
-                        "Device %s ReceiverNum %d PRIMED: %s",
-                        dev.device_info.bdf,
-                        self.receiver_number,
-                        dev.device_info,
-                    )
-                    continue
+                    status_str += "PRIMED"
+                elif args.force_margin:
+                    dev.primed = True
+                    status_str += "PRIMED (forcing margin on non-independent sampler)"
+                else:
+                    dev.primed = False
+                    status_str += "NOT PRIMED (doesn't support independent error sampler)"
 
-                logger.warning(
-                    "Device %s ReceiverNum %d NOT PRIMED: %s",
-                    dev.device_info.bdf,
-                    self.receiver_number,
-                    ret["error"],
-                )
+            if dev.primed:
+                logger.info(status_str)
+            else:
+                logger.warning(status_str)
                 # Mark all lanes faulty.
                 for lane in range(dev.device_info.width):
-                    dev.lane_errors[lane] = ret["error"]
+                    dev.lane_errors[lane] = status_str
 
     def setup_lane_margin_on_device_list(self):
         for dev in self._primed_devices:
             for lane in range(dev.device_info.width):
                 dev.set_error_count_limit(
                     lane=lane,
                     receiver_number=self.receiver_number,
@@ -185,60 +192,59 @@
 
 def get_curr_timestamp() -> int:
     """Returns the current unix timestamp."""
     return int(os.popen("date +%s").read().split("\n")[0])
 
 
 # pylint: disable=too-many-arguments,too-many-locals
+# FIXME: The args param should not be here, arg parsing and usage should be limited to main.py
 def collect_lmt_on_bdfs(
+    args: argparse.Namespace,
     hostname,
     host_id,
     model_name,
     bdf_list,
     receiver_number: int = 0x1,
-    error_count_limit: int = 50,
     left_right_none: int = 0,
     up_down=None,
     steps: int = 13,
     voltage_or_timing: str = "TIMING",
-    dwell_time: int = 5,
-    annotation: str = "",
 ) -> ty.List[LmtLaneResult]:
     # Gather test level info.
     test_info = LmtTestInfo()
     test_info.run_id = get_run_id()
     test_info.timestamp = get_curr_timestamp()
     test_info.host_id = host_id
     test_info.hostname = hostname
     test_info.model_name = model_name
-    test_info.dwell_time_secs = dwell_time
-    test_info.error_count_limit = error_count_limit
+    test_info.dwell_time_secs = args.dwell_time
+    test_info.error_count_limit = args.error_count_limit
     test_info.test_version = PCI_LMT_VERSION
-    test_info.annotation = annotation
+    test_info.annotation = args.annotation
 
     logger.info("%s", test_info)
     devices = PcieLmCollector(bdf_list)
 
     devices.sampler_setup(
         receiver_number=receiver_number,
-        error_count_limit=error_count_limit,
+        error_count_limit=args.error_count_limit,
         left_right_none=left_right_none,
         up_down=up_down,
         steps=steps,
         voltage_or_timing=voltage_or_timing,
     )
     devices.no_command_on_device_list()
-    devices.info_lane_margin_on_device_list()
+    devices.info_lane_margin_on_device_list(args)
     devices.no_command_on_device_list()
     devices.clear_error_log_on_device_list()
     devices.normal_settings_on_device_list()
     devices.setup_lane_margin_on_device_list()
 
     start_time = time.time()
-    time.sleep(dwell_time)
+    time.sleep(args.dwell_time)
     results = devices.collect_lane_margin_on_device_list(
         voltage_or_timing=devices.voltage_or_timing,
         steps=devices.steps,
         up_down=devices.up_down,
         left_right_none=devices.left_right_none,
     )
     stop_time = time.time()
@@ -256,15 +262,15 @@
 # pylint: disable=too-many-locals
 def run_lmt(args: argparse.Namespace, config: PlatformConfig, host: HostInfo, reporter: Reporter) -> None:
     """Runs LMT tests on all the interfaces listed in the platform_config."""
 
     logger.info("Loading config: %s", config)
 
     for group in config.lmt_groups:
-        annotation = args.annotation if args.annotation else group.name
+        args.annotation = args.annotation if args.annotation else group.name
         left_right_none, up_down = group.margin_directions_tuple
         # Loop through each step running LMT on all BDFs.
         for step in group.margin_steps:
             bdf_list = group.bdf_list
             margin_type = group.margin_type
             receiver_number = group.receiver_number
             logger.info(
@@ -272,23 +278,21 @@
                 margin_type,
                 len(bdf_list),
                 receiver_number,
                 step,
                 args.dwell_time,
             )
             results = collect_lmt_on_bdfs(
+                args=args,
                 hostname=host.hostname,
                 host_id=host.host_id,
                 model_name=host.model_name,
                 bdf_list=bdf_list,
                 receiver_number=receiver_number,
-                error_count_limit=args.error_count_limit,
                 left_right_none=left_right_none,
                 up_down=up_down,
                 steps=step,
                 voltage_or_timing=margin_type,
-                dwell_time=args.dwell_time,
-                annotation=annotation,
             )
             for result in results:
                 logger.info(result)
                 reporter.write(result)
```

### Comparing `ocptv-pci_lmt-1.2.1/src/pci_lmt/config.py` & `ocptv-pci_lmt-1.3.0/src/pci_lmt/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,23 +44,25 @@
                 f"Invalid values for margin_type {self.margin_type} and/or margin_direction {self.margin_direction}."
             )
 
         return (left_right_none, up_down)
 
     def __str__(self) -> str:
         bdf = textwrap.indent("\n".join(self.bdf_list), " " * 16).lstrip()
-        return textwrap.dedent(f"""
+        return textwrap.dedent(
+            f"""
             {self.name}
             receiver_number: {self.receiver_number}
             bdf:
                 {bdf}
             type: {self.margin_type}
             direction: {self.margin_direction}
             steps: {self.margin_steps}
-        """)
+        """
+        )
 
     @staticmethod
     def from_json(data: ty.Dict[str, ty.Any]) -> "ConfigLmtGroup":
         return ConfigLmtGroup(
             name=data["name"],
             receiver_number=data["receiver_number"],
             bdf_list=data["bdf_list"],
@@ -73,19 +75,21 @@
 @dc.dataclass
 class PlatformConfig:
     platform_name: str
     lmt_groups: ty.List[ConfigLmtGroup]
 
     def __str__(self) -> str:
         groups = textwrap.indent("".join(str(g) for g in self.lmt_groups), " " * 16).lstrip()
-        return textwrap.dedent(f"""
+        return textwrap.dedent(
+            f"""
             platform: {self.platform_name}
             groups:
                 {groups}
-        """)
+        """
+        )
 
     @staticmethod
     def from_json(data: ty.Dict[str, ty.Any]) -> "PlatformConfig":
         return PlatformConfig(
             platform_name=data["platform_name"],
             lmt_groups=[ConfigLmtGroup.from_json(group) for group in data["lmt_groups"]],
         )
```

### Comparing `ocptv-pci_lmt-1.2.1/src/pci_lmt/constants.py` & `ocptv-pci_lmt-1.3.0/src/pci_lmt/constants.py`

 * *Files identical despite different names*

### Comparing `ocptv-pci_lmt-1.2.1/src/pci_lmt/device.py` & `ocptv-pci_lmt-1.3.0/src/pci_lmt/device.py`

 * *Files identical despite different names*

### Comparing `ocptv-pci_lmt-1.2.1/src/pci_lmt/host.py` & `ocptv-pci_lmt-1.3.0/src/pci_lmt/host.py`

 * *Files identical despite different names*

### Comparing `ocptv-pci_lmt-1.2.1/src/pci_lmt/pcie_lane_margining.py` & `ocptv-pci_lmt-1.3.0/src/pci_lmt/pcie_lane_margining.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 # Use of this source code is governed by an MIT-style
 # license that can be found in the LICENSE file or at
 # https://opensource.org/licenses/MIT.
 
 import logging
 import time
 import typing as ty
+from typing import List
 from dataclasses import dataclass
 
-from pci_lmt.constants import MARGIN_RESPONSE, PARAMETERS
+from pci_lmt.constants import MARGIN_RESPONSE
 from pci_lmt.device import PciDevice
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 TIMEOUT = 0.5  # seconds
 
 
@@ -100,15 +101,15 @@
         if lmt_cap_info.err_msg:
             self.device_error = f"BDF: {self.device.bdf} Lane Margining unsupported {lmt_cap_info.err_msg}"
             return
         self.cap_lmt_offset = lmt_cap_info.offset
 
         # Place holder to store the errors encountered on each lane.
         # This is checked in each function call (via handle_lane_status decorator).
-        self.lane_errors = [None] * self.device_info.width
+        self.lane_errors: List[str] = [""] * self.device_info.width
 
     @handle_lane_status
     def write_margining_lane_control_register(
         self,
         lane: int = 0,
         receiver_number: int = 0x0,
         # FIXME: these magical constants should really be either named or better enums
@@ -714,22 +715,14 @@
         # 00b: Too many errors – Receiver autonomously went back to its default settings. MErrorCount reflects the
         #      number of errors detected as defined in Section 8.4.4. Note that MErrorCount might be greater than
         #      Error Count Limit.
         # Margin Payload[5:0] = MErrorCount
         if receiver_number not in [*range(0x1, 0x7)]:
             return {"error": f"ERROR: StepMarginVoltageOffsetUpDownOfDefault - BAD receiver_number {receiver_number}"}
 
-        if steps not in [
-            *range(
-                PARAMETERS["NumVoltageSteps"].min,
-                PARAMETERS["NumVoltageSteps"].max + 1,
-            )
-        ]:
-            return {"error": f"ERROR: StepMarginVoltageOffsetUpDownOfDefault - BAD Steps {steps}"}
-
         if up_down in (0, 1):
             margin_payload = up_down << 6 | steps
         else:
             return {"error": f"ERROR: StepMarginVoltageOffsetUpDownOfDefault - BAD UpDown {up_down}"}
 
         self.no_command(lane=lane)
         self.write_margining_lane_control_register(
```

### Comparing `ocptv-pci_lmt-1.2.1/src/pci_lmt/results.py` & `ocptv-pci_lmt-1.3.0/src/pci_lmt/results.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,16 +26,16 @@
     annotation: str = ""
 
 
 @dc.dataclass
 class LmtLaneResult:  # pylint: disable=too-many-instance-attributes,too-few-public-methods
     """Class to hold lane level info for the LMT test."""
 
-    test_info: LmtTestInfo = LmtTestInfo()
-    device_info: LmtDeviceInfo = LmtDeviceInfo()
+    test_info: LmtTestInfo = dc.field(default_factory=LmtTestInfo)
+    device_info: LmtDeviceInfo = dc.field(default_factory=LmtDeviceInfo)
     lane: int = -1
     receiver_number: int = -1
     margin_type: str = ""
     step: int = -1
     sample_count: int = -1
     sample_count_bits: int = -1
     error_count: int = -1
```

### Comparing `ocptv-pci_lmt-1.2.1/src/pci_lmt_bin/main.py` & `ocptv-pci_lmt-1.3.0/src/pci_lmt_bin/main.py`

 * *Files identical despite different names*

