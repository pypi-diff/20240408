# Comparing `tmp/ms2rescore-3.0.2.tar.gz` & `tmp/ms2rescore-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms2rescore-3.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ms2rescore-3.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ms2rescore-3.0.2.tar` & `ms2rescore-3.0.3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0    11357 2024-03-15 12:49:37.205432 ms2rescore-3.0.2/LICENSE
--rw-r--r--   0        0        0     6454 2024-03-15 12:49:37.205432 ms2rescore-3.0.2/README.md
--rw-r--r--   0        0        0      453 2024-03-15 12:49:37.257431 ms2rescore-3.0.2/ms2rescore/__init__.py
--rw-r--r--   0        0        0     5252 2024-03-15 12:49:37.257431 ms2rescore-3.0.2/ms2rescore/__main__.py
--rw-r--r--   0        0        0     5957 2024-03-15 12:49:37.257431 ms2rescore-3.0.2/ms2rescore/config_parser.py
--rw-r--r--   0        0        0     7467 2024-03-15 12:49:37.257431 ms2rescore-3.0.2/ms2rescore/core.py
--rw-r--r--   0        0        0      529 2024-03-15 12:49:37.257431 ms2rescore-3.0.2/ms2rescore/exceptions.py
--rw-r--r--   0        0        0      689 2024-03-15 12:49:37.257431 ms2rescore-3.0.2/ms2rescore/feature_generators/__init__.py
--rw-r--r--   0        0        0      522 2024-03-15 12:49:37.257431 ms2rescore-3.0.2/ms2rescore/feature_generators/base.py
--rw-r--r--   0        0        0     3436 2024-03-15 12:49:37.257431 ms2rescore-3.0.2/ms2rescore/feature_generators/basic.py
--rw-r--r--   0        0        0    10699 2024-03-15 12:49:37.261431 ms2rescore-3.0.2/ms2rescore/feature_generators/deeplc.py
--rw-r--r--   0        0        0    10796 2024-03-15 12:49:37.261431 ms2rescore-3.0.2/ms2rescore/feature_generators/ionmob.py
--rw-r--r--   0        0        0     7069 2024-03-15 12:49:37.261431 ms2rescore-3.0.2/ms2rescore/feature_generators/maxquant.py
--rw-r--r--   0        0        0    17022 2024-03-15 12:49:37.261431 ms2rescore-3.0.2/ms2rescore/feature_generators/ms2pip.py
--rw-r--r--   0        0        0        0 2024-03-15 12:49:37.261431 ms2rescore-3.0.2/ms2rescore/gui/__init__.py
--rw-r--r--   0        0        0      419 2024-03-15 12:49:37.261431 ms2rescore-3.0.2/ms2rescore/gui/__main__.py
--rw-r--r--   0        0        0    25033 2024-03-15 12:49:37.261431 ms2rescore-3.0.2/ms2rescore/gui/app.py
--rw-r--r--   0        0        0    11797 2024-03-15 12:49:37.261431 ms2rescore-3.0.2/ms2rescore/gui/function2ctk.py
--rw-r--r--   0        0        0    14890 2024-03-15 12:49:37.261431 ms2rescore-3.0.2/ms2rescore/gui/widgets.py
--rw-r--r--   0        0        0        0 2024-03-15 12:49:37.261431 ms2rescore-3.0.2/ms2rescore/package_data/__init__.py
--rw-r--r--   0        0        0     1084 2024-03-15 12:49:37.261431 ms2rescore-3.0.2/ms2rescore/package_data/config_default.json
--rw-r--r--   0        0        0    11078 2024-03-15 12:49:37.261431 ms2rescore-3.0.2/ms2rescore/package_data/config_schema.json
--rw-r--r--   0        0        0        0 2024-03-15 12:49:37.261431 ms2rescore-3.0.2/ms2rescore/package_data/img/__init__.py
--rw-r--r--   0        0        0 44669194 2024-03-15 12:49:37.413431 ms2rescore-3.0.2/ms2rescore/package_data/img/config_icon.png
--rw-r--r--   0        0        0     4837 2024-03-15 12:49:37.413431 ms2rescore-3.0.2/ms2rescore/package_data/img/github-mark-white.png
--rw-r--r--   0        0        0     5557 2024-03-15 12:49:37.413431 ms2rescore-3.0.2/ms2rescore/package_data/img/github-mark.png
--rw-r--r--   0        0        0    52066 2024-03-15 12:49:37.413431 ms2rescore-3.0.2/ms2rescore/package_data/img/ms2rescore_logo.png
--rw-r--r--   0        0        0    43034 2024-03-15 12:49:37.413431 ms2rescore-3.0.2/ms2rescore/package_data/img/program_icon.ico
--rw-r--r--   0        0        0     5068 2024-03-15 12:49:37.413431 ms2rescore-3.0.2/ms2rescore/package_data/ms2rescore-gui-theme.json
--rw-r--r--   0        0        0     5984 2024-03-15 12:49:37.413431 ms2rescore-3.0.2/ms2rescore/parse_psms.py
--rw-r--r--   0        0        0     5109 2024-03-15 12:49:37.417431 ms2rescore-3.0.2/ms2rescore/parse_spectra.py
--rw-r--r--   0        0        0      138 2024-03-15 12:49:37.417431 ms2rescore-3.0.2/ms2rescore/report/__init__.py
--rw-r--r--   0        0        0      614 2024-03-15 12:49:37.417431 ms2rescore-3.0.2/ms2rescore/report/__main__.py
--rw-r--r--   0        0        0    18037 2024-03-15 12:49:37.417431 ms2rescore-3.0.2/ms2rescore/report/charts.py
--rw-r--r--   0        0        0    13942 2024-03-15 12:49:37.417431 ms2rescore-3.0.2/ms2rescore/report/generate.py
--rw-r--r--   0        0        0        0 2024-03-15 12:49:37.417431 ms2rescore-3.0.2/ms2rescore/report/templates/__init__.py
--rw-r--r--   0        0        0     1677 2024-03-15 12:49:37.417431 ms2rescore-3.0.2/ms2rescore/report/templates/about.html
--rw-r--r--   0        0        0     3182 2024-03-15 12:49:37.417431 ms2rescore-3.0.2/ms2rescore/report/templates/base.html
--rw-r--r--   0        0        0      107 2024-03-15 12:49:37.417431 ms2rescore-3.0.2/ms2rescore/report/templates/config.html
--rw-r--r--   0        0        0      138 2024-03-15 12:49:37.417431 ms2rescore-3.0.2/ms2rescore/report/templates/features.html
--rw-r--r--   0        0        0       22 2024-03-15 12:49:37.417431 ms2rescore-3.0.2/ms2rescore/report/templates/log.html
--rw-r--r--   0        0        0      559 2024-03-15 12:49:37.417431 ms2rescore-3.0.2/ms2rescore/report/templates/metadata.html
--rw-r--r--   0        0        0      341 2024-03-15 12:49:37.417431 ms2rescore-3.0.2/ms2rescore/report/templates/overview.html
--rw-r--r--   0        0        0      831 2024-03-15 12:49:37.417431 ms2rescore-3.0.2/ms2rescore/report/templates/stats-card.html
--rw-r--r--   0        0        0     1904 2024-03-15 12:49:37.417431 ms2rescore-3.0.2/ms2rescore/report/templates/style.html
--rw-r--r--   0        0        0      138 2024-03-15 12:49:37.417431 ms2rescore-3.0.2/ms2rescore/report/templates/target-decoy.html
--rw-r--r--   0        0        0     5001 2024-03-15 12:49:37.417431 ms2rescore-3.0.2/ms2rescore/report/templates/texts.toml
--rw-r--r--   0        0        0     2971 2024-03-15 12:49:37.417431 ms2rescore-3.0.2/ms2rescore/report/utils.py
--rw-r--r--   0        0        0      302 2024-03-15 12:49:37.417431 ms2rescore-3.0.2/ms2rescore/rescoring_engines/__init__.py
--rw-r--r--   0        0        0     8617 2024-03-15 12:49:37.417431 ms2rescore-3.0.2/ms2rescore/rescoring_engines/mokapot.py
--rw-r--r--   0        0        0     7869 2024-03-15 12:49:37.417431 ms2rescore-3.0.2/ms2rescore/rescoring_engines/percolator.py
--rw-r--r--   0        0        0     2911 2024-03-15 12:49:37.417431 ms2rescore-3.0.2/ms2rescore/utils.py
--rw-r--r--   0        0        0     2527 2024-03-15 12:49:37.417431 ms2rescore-3.0.2/pyproject.toml
--rw-r--r--   0        0        0     8934 1970-01-01 00:00:00.000000 ms2rescore-3.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-08 15:45:32.756445 ms2rescore-3.0.3/LICENSE
+-rw-r--r--   0        0        0     6477 2024-04-08 15:45:32.756445 ms2rescore-3.0.3/README.md
+-rw-r--r--   0        0        0      453 2024-04-08 15:45:32.808445 ms2rescore-3.0.3/ms2rescore/__init__.py
+-rw-r--r--   0        0        0     5252 2024-04-08 15:45:32.808445 ms2rescore-3.0.3/ms2rescore/__main__.py
+-rw-r--r--   0        0        0     5957 2024-04-08 15:45:32.808445 ms2rescore-3.0.3/ms2rescore/config_parser.py
+-rw-r--r--   0        0        0     7473 2024-04-08 15:45:32.808445 ms2rescore-3.0.3/ms2rescore/core.py
+-rw-r--r--   0        0        0      529 2024-04-08 15:45:32.808445 ms2rescore-3.0.3/ms2rescore/exceptions.py
+-rw-r--r--   0        0        0      689 2024-04-08 15:45:32.808445 ms2rescore-3.0.3/ms2rescore/feature_generators/__init__.py
+-rw-r--r--   0        0        0      522 2024-04-08 15:45:32.808445 ms2rescore-3.0.3/ms2rescore/feature_generators/base.py
+-rw-r--r--   0        0        0     3436 2024-04-08 15:45:32.808445 ms2rescore-3.0.3/ms2rescore/feature_generators/basic.py
+-rw-r--r--   0        0        0    10699 2024-04-08 15:45:32.808445 ms2rescore-3.0.3/ms2rescore/feature_generators/deeplc.py
+-rw-r--r--   0        0        0    10796 2024-04-08 15:45:32.808445 ms2rescore-3.0.3/ms2rescore/feature_generators/ionmob.py
+-rw-r--r--   0        0        0     7069 2024-04-08 15:45:32.808445 ms2rescore-3.0.3/ms2rescore/feature_generators/maxquant.py
+-rw-r--r--   0        0        0    17267 2024-04-08 15:45:32.808445 ms2rescore-3.0.3/ms2rescore/feature_generators/ms2pip.py
+-rw-r--r--   0        0        0        0 2024-04-08 15:45:32.808445 ms2rescore-3.0.3/ms2rescore/gui/__init__.py
+-rw-r--r--   0        0        0      419 2024-04-08 15:45:32.808445 ms2rescore-3.0.3/ms2rescore/gui/__main__.py
+-rw-r--r--   0        0        0    25033 2024-04-08 15:45:32.808445 ms2rescore-3.0.3/ms2rescore/gui/app.py
+-rw-r--r--   0        0        0    11797 2024-04-08 15:45:32.808445 ms2rescore-3.0.3/ms2rescore/gui/function2ctk.py
+-rw-r--r--   0        0        0    14890 2024-04-08 15:45:32.808445 ms2rescore-3.0.3/ms2rescore/gui/widgets.py
+-rw-r--r--   0        0        0        0 2024-04-08 15:45:32.808445 ms2rescore-3.0.3/ms2rescore/package_data/__init__.py
+-rw-r--r--   0        0        0     1084 2024-04-08 15:45:32.808445 ms2rescore-3.0.3/ms2rescore/package_data/config_default.json
+-rw-r--r--   0        0        0    11078 2024-04-08 15:45:32.808445 ms2rescore-3.0.3/ms2rescore/package_data/config_schema.json
+-rw-r--r--   0        0        0        0 2024-04-08 15:45:32.812445 ms2rescore-3.0.3/ms2rescore/package_data/img/__init__.py
+-rw-r--r--   0        0        0 44669194 2024-04-08 15:45:32.968447 ms2rescore-3.0.3/ms2rescore/package_data/img/config_icon.png
+-rw-r--r--   0        0        0     4837 2024-04-08 15:45:32.968447 ms2rescore-3.0.3/ms2rescore/package_data/img/github-mark-white.png
+-rw-r--r--   0        0        0     5557 2024-04-08 15:45:32.968447 ms2rescore-3.0.3/ms2rescore/package_data/img/github-mark.png
+-rw-r--r--   0        0        0    52066 2024-04-08 15:45:32.968447 ms2rescore-3.0.3/ms2rescore/package_data/img/ms2rescore_logo.png
+-rw-r--r--   0        0        0    43034 2024-04-08 15:45:32.968447 ms2rescore-3.0.3/ms2rescore/package_data/img/program_icon.ico
+-rw-r--r--   0        0        0     5068 2024-04-08 15:45:32.968447 ms2rescore-3.0.3/ms2rescore/package_data/ms2rescore-gui-theme.json
+-rw-r--r--   0        0        0     5950 2024-04-08 15:45:32.968447 ms2rescore-3.0.3/ms2rescore/parse_psms.py
+-rw-r--r--   0        0        0     1967 2024-04-08 15:45:32.968447 ms2rescore-3.0.3/ms2rescore/parse_spectra.py
+-rw-r--r--   0        0        0      138 2024-04-08 15:45:32.968447 ms2rescore-3.0.3/ms2rescore/report/__init__.py
+-rw-r--r--   0        0        0      614 2024-04-08 15:45:32.968447 ms2rescore-3.0.3/ms2rescore/report/__main__.py
+-rw-r--r--   0        0        0    18659 2024-04-08 15:45:32.968447 ms2rescore-3.0.3/ms2rescore/report/charts.py
+-rw-r--r--   0        0        0    14085 2024-04-08 15:45:32.968447 ms2rescore-3.0.3/ms2rescore/report/generate.py
+-rw-r--r--   0        0        0        0 2024-04-08 15:45:32.968447 ms2rescore-3.0.3/ms2rescore/report/templates/__init__.py
+-rw-r--r--   0        0        0     1677 2024-04-08 15:45:32.968447 ms2rescore-3.0.3/ms2rescore/report/templates/about.html
+-rw-r--r--   0        0        0     3182 2024-04-08 15:45:32.968447 ms2rescore-3.0.3/ms2rescore/report/templates/base.html
+-rw-r--r--   0        0        0      107 2024-04-08 15:45:32.968447 ms2rescore-3.0.3/ms2rescore/report/templates/config.html
+-rw-r--r--   0        0        0      138 2024-04-08 15:45:32.968447 ms2rescore-3.0.3/ms2rescore/report/templates/features.html
+-rw-r--r--   0        0        0       22 2024-04-08 15:45:32.968447 ms2rescore-3.0.3/ms2rescore/report/templates/log.html
+-rw-r--r--   0        0        0      559 2024-04-08 15:45:32.968447 ms2rescore-3.0.3/ms2rescore/report/templates/metadata.html
+-rw-r--r--   0        0        0      341 2024-04-08 15:45:32.968447 ms2rescore-3.0.3/ms2rescore/report/templates/overview.html
+-rw-r--r--   0        0        0      831 2024-04-08 15:45:32.968447 ms2rescore-3.0.3/ms2rescore/report/templates/stats-card.html
+-rw-r--r--   0        0        0     1904 2024-04-08 15:45:32.968447 ms2rescore-3.0.3/ms2rescore/report/templates/style.html
+-rw-r--r--   0        0        0      138 2024-04-08 15:45:32.968447 ms2rescore-3.0.3/ms2rescore/report/templates/target-decoy.html
+-rw-r--r--   0        0        0     5001 2024-04-08 15:45:32.968447 ms2rescore-3.0.3/ms2rescore/report/templates/texts.toml
+-rw-r--r--   0        0        0     2804 2024-04-08 15:45:32.968447 ms2rescore-3.0.3/ms2rescore/report/utils.py
+-rw-r--r--   0        0        0      302 2024-04-08 15:45:32.968447 ms2rescore-3.0.3/ms2rescore/rescoring_engines/__init__.py
+-rw-r--r--   0        0        0     8749 2024-04-08 15:45:32.968447 ms2rescore-3.0.3/ms2rescore/rescoring_engines/mokapot.py
+-rw-r--r--   0        0        0     7869 2024-04-08 15:45:32.968447 ms2rescore-3.0.3/ms2rescore/rescoring_engines/percolator.py
+-rw-r--r--   0        0        0     2911 2024-04-08 15:45:32.968447 ms2rescore-3.0.3/ms2rescore/utils.py
+-rw-r--r--   0        0        0     2553 2024-04-08 15:45:32.968447 ms2rescore-3.0.3/pyproject.toml
+-rw-r--r--   0        0        0     8986 1970-01-01 00:00:00.000000 ms2rescore-3.0.3/PKG-INFO
```

### Comparing `ms2rescore-3.0.2/LICENSE` & `ms2rescore-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.2/README.md` & `ms2rescore-3.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
 ## Citing
 
 **Latest MS²Rescore publication:**
 
 > **MS²Rescore 3.0 is a modular, flexible, and user-friendly platform to boost peptide identifications, as showcased with MS Amanda 3.0.**
 > Louise Marie Buur*, Arthur Declercq*, Marina Strobl, Robbin Bouwmeester, Sven Degroeve, Lennart Martens, Viktoria Dorfer*, and Ralf Gabriels*.
-> _ChemRxiv_ (2023) [doi:10.26434/chemrxiv-2023-rvr9n](https://doi.org/10.26434/chemrxiv-2023-rvr9n) <br/> \*contributed equally <span class="__dimensions_badge_embed__" data-doi="10.26434/chemrxiv-2023-rvr9n" data-hide-zero-citations="true" data-style="small_rectangle"></span>
+> _Journal of Proteome Research_ (2024) [doi:10.1021/acs.jproteome.3c00785](https://doi.org/10.1021/acs.jproteome.3c00785) <br/> \*contributed equally <span class="__dimensions_badge_embed__" data-doi="10.1021/acs.jproteome.3c00785" data-hide-zero-citations="true" data-style="small_rectangle"></span>
 
 **MS²Rescore for immunopeptidomics:**
 
 > **MS2Rescore: Data-driven rescoring dramatically boosts immunopeptide identification rates.**
 > Arthur Declercq, Robbin Bouwmeester, Aurélie Hirschler, Christine Carapito, Sven Degroeve, Lennart Martens, and Ralf Gabriels.
 > _Molecular & Cellular Proteomics_ (2021) [doi:10.1016/j.mcpro.2022.100266](https://doi.org/10.1016/j.mcpro.2022.100266) <span class="__dimensions_badge_embed__" data-doi="10.1016/j.mcpro.2022.100266" data-hide-zero-citations="true" data-style="small_rectangle"></span>
```

### Comparing `ms2rescore-3.0.2/ms2rescore/__main__.py` & `ms2rescore-3.0.3/ms2rescore/__main__.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.2/ms2rescore/config_parser.py` & `ms2rescore-3.0.3/ms2rescore/config_parser.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.2/ms2rescore/core.py` & `ms2rescore-3.0.3/ms2rescore/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     )
 
     # TODO: avoid hard coding feature generators in some way
     rt_required = "deeplc" in config["feature_generators"] and None in psm_list["retention_time"]
     im_required = "ionmob" in config["feature_generators"] and None in psm_list["ion_mobility"]
     if rt_required or im_required:
         logger.info("Parsing missing retention time and/or ion mobility values from spectra...")
-        get_missing_values(config, psm_list, missing_rt=rt_required, missing_im=im_required)
+        get_missing_values(psm_list, config, rt_required=rt_required, im_required=im_required)
 
     # Add rescoring features
     for fgen_name, fgen_config in config["feature_generators"].items():
         # TODO: Handle this somewhere else, more generally?
         if fgen_name == "maxquant" and not (psm_list["source"] == "msms").all():
             logger.warning(
                 "MaxQuant feature generator requires PSMs from a MaxQuant msms.txt file. Skipping "
@@ -153,15 +153,15 @@
     # Write report
     if config["write_report"]:
         try:
             generate.generate_report(
                 output_file_root, psm_list=psm_list, feature_names=feature_names, use_txt_log=True
             )
         except exceptions.ReportGenerationError as e:
-            logger.error(e)
+            logger.exception(e)
 
 
 def _write_feature_names(feature_names, output_file_root):
     """Write feature names to file."""
     with open(output_file_root + ".feature_names.tsv", "w") as f:
         f.write("feature_generator\tfeature_name\n")
         for fgen, fgen_features in feature_names.items():
```

### Comparing `ms2rescore-3.0.2/ms2rescore/exceptions.py` & `ms2rescore-3.0.3/ms2rescore/exceptions.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.2/ms2rescore/feature_generators/__init__.py` & `ms2rescore-3.0.3/ms2rescore/feature_generators/__init__.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.2/ms2rescore/feature_generators/base.py` & `ms2rescore-3.0.3/ms2rescore/feature_generators/base.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.2/ms2rescore/feature_generators/basic.py` & `ms2rescore-3.0.3/ms2rescore/feature_generators/basic.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.2/ms2rescore/feature_generators/deeplc.py` & `ms2rescore-3.0.3/ms2rescore/feature_generators/deeplc.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.2/ms2rescore/feature_generators/ionmob.py` & `ms2rescore-3.0.3/ms2rescore/feature_generators/ionmob.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.2/ms2rescore/feature_generators/maxquant.py` & `ms2rescore-3.0.3/ms2rescore/feature_generators/maxquant.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.2/ms2rescore/feature_generators/ms2pip.py` & `ms2rescore-3.0.3/ms2rescore/feature_generators/ms2pip.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,15 @@
     def __init__(
         self,
         *args,
         model: str = "HCD",
         ms2_tolerance: float = 0.02,
         spectrum_path: Optional[str] = None,
         spectrum_id_pattern: str = "(.*)",
+        model_dir: Optional[str] = None,
         processes: 1,
         **kwargs,
     ) -> None:
         """
         Generate MS²PIP-based features.
 
         Parameters
@@ -67,28 +68,31 @@
             MS2 mass tolerance in Da. Defaults to :py:const:`0.02`.
         spectrum_path
             Path to spectrum file or directory with spectrum files. If None, inferred from ``run``
             field in PSMs. Defaults to :py:const:`None`.
         spectrum_id_pattern : str, optional
             Regular expression pattern to extract spectrum ID from spectrum file. Defaults to
             :py:const:`.*`.
+        model_dir
+            Directory containing MS²PIP models. Defaults to :py:const:`None` (use MS²PIP default).
         processes : int, optional
             Number of processes to use. Defaults to 1.
 
         Attributes
         ----------
         feature_names: list[str]
             Names of the features that will be added to the PSMs.
 
         """
         super().__init__(*args, **kwargs)
         self.model = model
         self.ms2_tolerance = ms2_tolerance
         self.spectrum_path = spectrum_path
         self.spectrum_id_pattern = spectrum_id_pattern
+        self.model_dir = model_dir
         self.processes = processes
 
     @property
     def feature_names(self):
         return [
             "spec_pearson_norm",
             "ionb_pearson_norm",
@@ -190,14 +194,15 @@
                     ms2pip_results = correlate(
                         psms=psm_list_run,
                         spectrum_file=spectrum_filename,
                         spectrum_id_pattern=self.spectrum_id_pattern,
                         model=self.model,
                         ms2_tolerance=self.ms2_tolerance,
                         compute_correlations=False,
+                        model_dir=self.model_dir,
                         processes=self.processes,
                     )
                 except NoMatchingSpectraFound as e:
                     raise FeatureGeneratorException(
                         f"Could not find any matching spectra for PSMs from run `{run}`. "
                         "Please check that the `spectrum_id_pattern` and `psm_id_pattern` "
                         "options are configured correctly. See "
```

### Comparing `ms2rescore-3.0.2/ms2rescore/gui/app.py` & `ms2rescore-3.0.3/ms2rescore/gui/app.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.2/ms2rescore/gui/function2ctk.py` & `ms2rescore-3.0.3/ms2rescore/gui/function2ctk.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.2/ms2rescore/gui/widgets.py` & `ms2rescore-3.0.3/ms2rescore/gui/widgets.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.2/ms2rescore/package_data/config_default.json` & `ms2rescore-3.0.3/ms2rescore/package_data/config_default.json`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.2/ms2rescore/package_data/config_schema.json` & `ms2rescore-3.0.3/ms2rescore/package_data/config_schema.json`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.2/ms2rescore/package_data/img/config_icon.png` & `ms2rescore-3.0.3/ms2rescore/package_data/img/config_icon.png`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.2/ms2rescore/package_data/img/github-mark-white.png` & `ms2rescore-3.0.3/ms2rescore/package_data/img/github-mark-white.png`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.2/ms2rescore/package_data/img/github-mark.png` & `ms2rescore-3.0.3/ms2rescore/package_data/img/github-mark.png`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.2/ms2rescore/package_data/img/ms2rescore_logo.png` & `ms2rescore-3.0.3/ms2rescore/package_data/img/ms2rescore_logo.png`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.2/ms2rescore/package_data/img/program_icon.ico` & `ms2rescore-3.0.3/ms2rescore/package_data/img/program_icon.ico`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.2/ms2rescore/package_data/ms2rescore-gui-theme.json` & `ms2rescore-3.0.3/ms2rescore/package_data/ms2rescore-gui-theme.json`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.2/ms2rescore/parse_psms.py` & `ms2rescore-3.0.3/ms2rescore/parse_psms.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import logging
 import re
-from itertools import chain
 from typing import Dict, Union
 
 import psm_utils.io
 from psm_utils import PSMList
 
 from ms2rescore.exceptions import MS2RescoreConfigurationError
 
@@ -56,17 +55,17 @@
         )
     psm_list.rename_modifications(config["modification_mapping"])
     psm_list.add_fixed_modifications(config["fixed_modifications"])
     psm_list.apply_fixed_modifications()
 
     if config["psm_id_pattern"]:
         pattern = re.compile(config["psm_id_pattern"])
-        logger.debug("Applying `psm_id_pattern`...")
+        logger.debug("Applying 'psm_id_pattern'...")
         logger.debug(
-            f"Parsing `{psm_list['spectrum_id'][0]}` to `{_match_psm_ids(psm_list['spectrum_id'][0], pattern)}`"
+            f"Parsing '{psm_list[0].spectrum_id}' to '{_match_psm_ids(psm_list[0].spectrum_id, pattern)}'"
         )
         new_ids = [_match_psm_ids(old_id, pattern) for old_id in psm_list["spectrum_id"]]
         psm_list["spectrum_id"] = new_ids
 
     # TODO: Temporary fix until implemented in psm_utils
     # Ensure that spectrum IDs are strings (Pydantic 2.0 does not coerce int to str)
     psm_list["spectrum_id"] = [str(spec_id) for spec_id in psm_list["spectrum_id"]]
@@ -82,27 +81,27 @@
         current_file = 1
         total_files = len(config["psm_file"])
         valid_psms_list = []
         total_psms = 0
         valid_psms = 0
         for psm_file in config["psm_file"]:
             logger.info(
-                f"Reading PSMs from PSM file ({current_file}/{total_files}): `{psm_file}`..."
+                f"Reading PSMs from PSM file ({current_file}/{total_files}): '{psm_file}'..."
             )
             try:
                 id_file_psm_list = psm_utils.io.read_file(
                     psm_file,
                     filetype=config["psm_file_type"],
                     show_progressbar=True,
                     **config["psm_reader_kwargs"],
                 )
             except psm_utils.io.PSMUtilsIOException:
                 raise MS2RescoreConfigurationError(
-                    "Error occurred while reading PSMs. Please check the `psm_file` and "
-                    "`psm_file_type` settings. See "
+                    "Error occurred while reading PSMs. Please check the 'psm_file' and "
+                    "'psm_file_type' settings. See "
                     "https://ms2rescore.readthedocs.io/en/latest/userguide/input-files/"
                     " for more information."
                 )
 
             total_psms += len(id_file_psm_list.psm_list)
             for psm in id_file_psm_list.psm_list:
                 if not _has_invalid_aminoacids(psm):
@@ -125,15 +124,15 @@
     n_psms = len(psm_list)
     percent_decoys = sum(psm_list["is_decoy"]) / n_psms * 100
     logger.info(f"Found {n_psms} PSMs, of which {percent_decoys:.2f}% are decoys.")
 
     if not any(psm_list["is_decoy"]):
         raise MS2RescoreConfigurationError(
             "No decoy PSMs found. Please check if decoys are present in the PSM file and that "
-            "the `id_decoy_pattern` option is correct. See "
+            "the 'id_decoy_pattern' option is correct. See "
             "https://ms2rescore.readthedocs.io/en/latest/userguide/configuration/#selecting-decoy-psms"
             " for more information."
         )
 
 
 def _calculate_qvalues(config, psm_list):
     """Calculate q-values for PSMs if not present."""
@@ -146,15 +145,15 @@
 def _match_psm_ids(old_id, regex_pattern):
     """Match PSM IDs to regex pattern or raise Exception if no match present."""
     match = re.search(regex_pattern, str(old_id))
     try:
         return match[1]
     except (TypeError, IndexError):
         raise MS2RescoreConfigurationError(
-            f"`psm_id_pattern` could not be extracted from PSM spectrum IDs (i.e. {old_id})."
+            f"'psm_id_pattern' could not be extracted from PSM spectrum IDs (i.e. {old_id})."
             " Ensure that the regex contains a capturing group?"
         )
 
 
 def _has_invalid_aminoacids(psm):
     """Check if a PSM contains invalid amino acids."""
```

### Comparing `ms2rescore-3.0.2/ms2rescore/report/__main__.py` & `ms2rescore-3.0.3/ms2rescore/report/__main__.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.2/ms2rescore/report/charts.py` & `ms2rescore-3.0.3/ms2rescore/report/charts.py`

 * *Files 6% similar despite different names*

```diff
@@ -210,14 +210,22 @@
         Mokapot linear confidence results after rescoring.
     level
         Level of confidence estimates to plot. Must be one of "psms", "peptides", or "proteins".
     indexer
         Column with index for each PSM, peptide, or protein to use for merging data frames.
 
     """
+    if not before or not after:
+        figure = go.Figure()
+        figure.add_annotation(
+            text="No data available for comparison.",
+            showarrow=False,
+        )
+        return figure
+
     # Restructure data
     merge_columns = [indexer, "mokapot score", "mokapot q-value", "mokapot PEP"]
     ce_psms_targets = pd.merge(
         left=before.confidence_estimates[level],
         right=after.confidence_estimates[level][merge_columns],
         on=indexer,
         suffixes=(" before", " after"),
@@ -284,14 +292,22 @@
         Mokapot linear confidence results after rescoring.
     level
         Level of confidence estimates to plot. Must be one of "psms", "peptides", or "proteins".
     indexer
         Column with index for each PSM, peptide, or protein to use for merging dataframes.
 
     """
+    if not before or not after:
+        figure = go.Figure()
+        figure.add_annotation(
+            text="No data available for comparison.",
+            showarrow=False,
+        )
+        return figure
+
     # Prepare data
     ce_psms_targets_melted = (
         pd.merge(
             left=before.confidence_estimates[level],
             right=after.confidence_estimates[level][
                 [indexer, "mokapot score", "mokapot q-value", "mokapot PEP"]
             ],
@@ -332,26 +348,34 @@
     fig.update_layout(yaxis_title="Identified PSMs")
     return fig
 
 
 def identification_overlap(
     before: mokapot.LinearConfidence,
     after: mokapot.LinearConfidence,
-) -> go.Figure():
+) -> go.Figure:
     """
     Plot stacked bar charts of removed, retained, and gained PSMs, peptides, and proteins.
 
     Parameters
     ----------
     before
         Mokapot linear confidence results before rescoring.
     after
         Mokapot linear confidence results after rescoring.
 
     """
+    if not before or not after:
+        figure = go.Figure()
+        figure.add_annotation(
+            text="No data available for comparison.",
+            showarrow=False,
+        )
+        return figure
+
     levels = before.levels  # ["psms", "peptides", "proteins"] if all available
     indexers = ["index", "index", "mokapot protein group"]
 
     overlap_data = defaultdict(dict)
     for level, indexer in zip(levels, indexers):
         df_before = before.confidence_estimates[level]
         df_after = after.confidence_estimates[level]
```

### Comparing `ms2rescore-3.0.2/ms2rescore/report/generate.py` & `ms2rescore-3.0.3/ms2rescore/report/generate.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,14 +160,19 @@
 
 def _get_stats_context(confidence_before, confidence_after):
     """Return context for overview statistics pane."""
     stats = []
     levels = ["psms", "peptides", "proteins"]
     level_names = ["PSMs", "Peptides", "Protein groups"]
     card_colors = ["card-bg-blue", "card-bg-green", "card-bg-red"]
+
+    # Cannot report stats if confidence estimates are not present
+    if not confidence_before or not confidence_after:
+        return stats
+
     for level, level_name, card_color in zip(levels, level_names, card_colors):
         try:
             before = confidence_before.accepted[level.lower()]
             after = confidence_after.accepted[level.lower()]
         except KeyError:
             continue  # Level not present (e.g. no fasta provided)
         if not before or not after:
```

### Comparing `ms2rescore-3.0.2/ms2rescore/report/templates/about.html` & `ms2rescore-3.0.3/ms2rescore/report/templates/about.html`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.2/ms2rescore/report/templates/base.html` & `ms2rescore-3.0.3/ms2rescore/report/templates/base.html`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.2/ms2rescore/report/templates/metadata.html` & `ms2rescore-3.0.3/ms2rescore/report/templates/metadata.html`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.2/ms2rescore/report/templates/stats-card.html` & `ms2rescore-3.0.3/ms2rescore/report/templates/stats-card.html`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.2/ms2rescore/report/templates/style.html` & `ms2rescore-3.0.3/ms2rescore/report/templates/style.html`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.2/ms2rescore/report/templates/texts.toml` & `ms2rescore-3.0.3/ms2rescore/report/templates/texts.toml`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.2/ms2rescore/report/utils.py` & `ms2rescore-3.0.3/ms2rescore/report/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -76,14 +76,11 @@
             peptide_column="peptide",
         )
         if fasta_file:
             lin_psm_dataset.add_proteins(fasta)
 
         try:
             confidence[when] = lin_psm_dataset.assign_confidence()
-        except RuntimeError as e:
-            raise ReportGenerationError(
-                f"Error while assigning confidence estimates to PSMs ({when} rescoring). "
-                "Could not generate report."
-            ) from e
+        except RuntimeError:
+            confidence[when] = None
 
     return confidence["before"], confidence["after"]
```

### Comparing `ms2rescore-3.0.2/ms2rescore/rescoring_engines/mokapot.py` & `ms2rescore-3.0.3/ms2rescore/rescoring_engines/mokapot.py`

 * *Files 5% similar despite different names*

```diff
@@ -167,14 +167,18 @@
         "retention_time",
         "charge",
     ]
     feature_df = pd.DataFrame(list(psm_df["rescoring_features"])).astype(float).fillna(0.0)
     feature_df.columns = [f"feature:{f}" for f in feature_df.columns]
     combined_df = pd.concat([psm_df[required_columns], feature_df], axis=1)
 
+    # Ensure filename for FlashLFQ txt output
+    if not combined_df["run"].notnull().all():
+        combined_df["run"] = "ms_run"
+
     feature_names = [f"feature:{f}" for f in feature_names] if feature_names else None
 
     lin_psm_data = LinearPsmDataset(
         psms=combined_df,
         target_column="is_target",
         spectrum_columns="index",  # Use artificial index to allow multi-rank rescoring
         peptide_column="peptide",
```

### Comparing `ms2rescore-3.0.2/ms2rescore/rescoring_engines/percolator.py` & `ms2rescore-3.0.3/ms2rescore/rescoring_engines/percolator.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.2/ms2rescore/utils.py` & `ms2rescore-3.0.3/ms2rescore/utils.py`

 * *Files identical despite different names*

### Comparing `ms2rescore-3.0.2/pyproject.toml` & `ms2rescore-3.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -28,30 +28,31 @@
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Scientific/Engineering :: Bio-Informatics",
     "Development Status :: 5 - Production/Stable",
 ]
 dynamic = ["version"]
 requires-python = ">=3.8"
 dependencies = [
+    "ms2rescore_rs",
     "numpy>=1.16.0; python_version != '3.11'",
-    "numpy==1.24.3; python_version == '3.11'",  # Incompatibility with sklearn, pygam, and TF...
+    "numpy==1.24.3; python_version == '3.11'", # Incompatibility with sklearn, pygam, and TF...
     "pandas>=1.0",
     "rich>=12",
     "pyteomics>=4.1.0",
     "lxml>=4.5",
     "ms2pip>=4.0.0-dev4",
     "click>=7",
     "cascade-config>=0.4.0",
     "deeplc>=2.2",
     "deeplcretrainer>=0.2",
     "tomli>=2; python_version < '3.11'",
     "psm_utils>=0.4",
     "customtkinter>=5,<6",
     "mokapot>=0.9",
-    "pydantic>=1.8.2,<2",                # Fix compatibility with v2 in psm_utils
+    "pydantic>=1.8.2,<2",                      # Fix compatibility with v2 in psm_utils
     "jinja2>=3",
     "plotly>=5",
 ]
 
 [project.optional-dependencies]
 ionmob = ["ionmob>=0.2", "tensorflow"]
 dev = ["ruff", "black", "pytest", "pytest-cov", "pre-commit"]
```

### Comparing `ms2rescore-3.0.2/PKG-INFO` & `ms2rescore-3.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: ms2rescore
-Version: 3.0.2
+Version: 3.0.3
 Summary: MS²Rescore: Sensitive PSM rescoring with predicted MS² peak intensities and retention times.
 Keywords: MS2Rescore,MS2PIP,DeepLC,Percolator,proteomics,mass spectrometry,peptide identification,rescoring,machine learning
 Author: Ana Sílvia C. Silva, Robbin Bouwmeester, Louise Buur
 Author-email: Ralf Gabriels <ralf@gabriels.dev>, Arthur Declercq <arthur.declercq@ugent.be>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Development Status :: 5 - Production/Stable
+Requires-Dist: ms2rescore_rs
 Requires-Dist: numpy>=1.16.0; python_version != '3.11'
 Requires-Dist: numpy==1.24.3; python_version == '3.11'
 Requires-Dist: pandas>=1.0
 Requires-Dist: rich>=12
 Requires-Dist: pyteomics>=4.1.0
 Requires-Dist: lxml>=4.5
 Requires-Dist: ms2pip>=4.0.0-dev4
@@ -104,15 +105,15 @@
 
 ## Citing
 
 **Latest MS²Rescore publication:**
 
 > **MS²Rescore 3.0 is a modular, flexible, and user-friendly platform to boost peptide identifications, as showcased with MS Amanda 3.0.**
 > Louise Marie Buur*, Arthur Declercq*, Marina Strobl, Robbin Bouwmeester, Sven Degroeve, Lennart Martens, Viktoria Dorfer*, and Ralf Gabriels*.
-> _ChemRxiv_ (2023) [doi:10.26434/chemrxiv-2023-rvr9n](https://doi.org/10.26434/chemrxiv-2023-rvr9n) <br/> \*contributed equally <span class="__dimensions_badge_embed__" data-doi="10.26434/chemrxiv-2023-rvr9n" data-hide-zero-citations="true" data-style="small_rectangle"></span>
+> _Journal of Proteome Research_ (2024) [doi:10.1021/acs.jproteome.3c00785](https://doi.org/10.1021/acs.jproteome.3c00785) <br/> \*contributed equally <span class="__dimensions_badge_embed__" data-doi="10.1021/acs.jproteome.3c00785" data-hide-zero-citations="true" data-style="small_rectangle"></span>
 
 **MS²Rescore for immunopeptidomics:**
 
 > **MS2Rescore: Data-driven rescoring dramatically boosts immunopeptide identification rates.**
 > Arthur Declercq, Robbin Bouwmeester, Aurélie Hirschler, Christine Carapito, Sven Degroeve, Lennart Martens, and Ralf Gabriels.
 > _Molecular & Cellular Proteomics_ (2021) [doi:10.1016/j.mcpro.2022.100266](https://doi.org/10.1016/j.mcpro.2022.100266) <span class="__dimensions_badge_embed__" data-doi="10.1016/j.mcpro.2022.100266" data-hide-zero-citations="true" data-style="small_rectangle"></span>
```

