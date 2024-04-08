# Comparing `tmp/cg_hermes-4.2.1.tar.gz` & `tmp/cg_hermes-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cg_hermes-4.2.1.tar", max compression
+gzip compressed data, was "cg_hermes-4.3.0.tar", max compression
```

## Comparing `cg_hermes-4.2.1.tar` & `cg_hermes-4.3.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0       22 2024-03-18 15:21:56.523149 cg_hermes-4.2.1/cg_hermes/__init__.py
--rw-r--r--   0        0        0      289 2024-03-18 15:21:56.523149 cg_hermes-4.2.1/cg_hermes/__main__.py
--rw-r--r--   0        0        0        0 2024-03-18 15:21:56.523149 cg_hermes-4.2.1/cg_hermes/cli/__init__.py
--rw-r--r--   0        0        0     1025 2024-03-18 15:21:56.523149 cg_hermes-4.2.1/cg_hermes/cli/base.py
--rw-r--r--   0        0        0      946 2024-03-18 15:21:56.523149 cg_hermes-4.2.1/cg_hermes/cli/common.py
--rw-r--r--   0        0        0     1568 2024-03-18 15:21:56.523149 cg_hermes-4.2.1/cg_hermes/cli/convert.py
--rw-r--r--   0        0        0     3533 2024-03-18 15:21:56.523149 cg_hermes-4.2.1/cg_hermes/cli/export.py
--rw-r--r--   0        0        0     3090 2024-03-18 15:21:56.523149 cg_hermes-4.2.1/cg_hermes/cli/validate.py
--rw-r--r--   0        0        0    28216 2024-03-18 15:21:56.523149 cg_hermes-4.2.1/cg_hermes/config/balsamic.py
--rw-r--r--   0        0        0     1590 2024-03-18 15:21:56.523149 cg_hermes-4.2.1/cg_hermes/config/balsamic_qc.py
--rw-r--r--   0        0        0     5551 2024-03-18 15:21:56.523149 cg_hermes-4.2.1/cg_hermes/config/balsamic_umi.py
--rw-r--r--   0        0        0      846 2024-03-18 15:21:56.523149 cg_hermes-4.2.1/cg_hermes/config/fluffy.py
--rw-r--r--   0        0        0     2166 2024-03-18 15:21:56.523149 cg_hermes-4.2.1/cg_hermes/config/microsalt.py
--rw-r--r--   0        0        0     8540 2024-03-18 15:21:56.523149 cg_hermes-4.2.1/cg_hermes/config/mip_dna.py
--rw-r--r--   0        0        0     4551 2024-03-18 15:21:56.523149 cg_hermes-4.2.1/cg_hermes/config/mip_rna.py
--rw-r--r--   0        0        0     4354 2024-03-18 15:21:56.523149 cg_hermes-4.2.1/cg_hermes/config/mutant.py
--rw-r--r--   0        0        0      498 2024-03-18 15:21:56.523149 cg_hermes-4.2.1/cg_hermes/config/nextflow.py
--rw-r--r--   0        0        0     4156 2024-03-18 15:21:56.523149 cg_hermes-4.2.1/cg_hermes/config/rnafusion.py
--rw-r--r--   0        0        0    16492 2024-03-18 15:21:56.523149 cg_hermes-4.2.1/cg_hermes/config/tags.py
--rw-r--r--   0        0        0     2527 2024-03-18 15:21:56.523149 cg_hermes-4.2.1/cg_hermes/config/taxprofiler.py
--rw-r--r--   0        0        0      204 2024-03-18 15:21:56.523149 cg_hermes-4.2.1/cg_hermes/config/workflows.py
--rw-r--r--   0        0        0      527 2024-03-18 15:21:56.523149 cg_hermes-4.2.1/cg_hermes/constants/workflow.py
--rw-r--r--   0        0        0    13219 2024-03-18 15:21:56.523149 cg_hermes-4.2.1/cg_hermes/deliverables.py
--rw-r--r--   0        0        0      338 2024-03-18 15:21:56.523149 cg_hermes-4.2.1/cg_hermes/exceptions.py
--rw-r--r--   0        0        0        0 2024-03-18 15:21:56.523149 cg_hermes-4.2.1/cg_hermes/models/__init__.py
--rw-r--r--   0        0        0      651 2024-03-18 15:21:56.527149 cg_hermes-4.2.1/cg_hermes/models/tags.py
--rw-r--r--   0        0        0     2768 2024-03-18 15:21:56.527149 cg_hermes-4.2.1/cg_hermes/models/workflow_deliverables.py
--rw-r--r--   0        0        0     1805 2024-03-18 15:21:56.527149 cg_hermes-4.2.1/cg_hermes/validate.py
--rw-r--r--   0        0        0      773 2024-03-18 15:21:56.527149 cg_hermes-4.2.1/pyproject.toml
--rw-r--r--   0        0        0      599 1970-01-01 00:00:00.000000 cg_hermes-4.2.1/PKG-INFO
+-rw-r--r--   0        0        0       22 2024-04-08 07:01:36.181836 cg_hermes-4.3.0/cg_hermes/__init__.py
+-rw-r--r--   0        0        0      289 2024-04-08 07:01:36.181836 cg_hermes-4.3.0/cg_hermes/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-08 07:01:36.181836 cg_hermes-4.3.0/cg_hermes/cli/__init__.py
+-rw-r--r--   0        0        0     1025 2024-04-08 07:01:36.181836 cg_hermes-4.3.0/cg_hermes/cli/base.py
+-rw-r--r--   0        0        0      946 2024-04-08 07:01:36.181836 cg_hermes-4.3.0/cg_hermes/cli/common.py
+-rw-r--r--   0        0        0     1542 2024-04-08 07:01:36.181836 cg_hermes-4.3.0/cg_hermes/cli/convert.py
+-rw-r--r--   0        0        0     3520 2024-04-08 07:01:36.181836 cg_hermes-4.3.0/cg_hermes/cli/export.py
+-rw-r--r--   0        0        0     3176 2024-04-08 07:01:36.181836 cg_hermes-4.3.0/cg_hermes/cli/validate.py
+-rw-r--r--   0        0        0    28216 2024-04-08 07:01:36.181836 cg_hermes-4.3.0/cg_hermes/config/balsamic.py
+-rw-r--r--   0        0        0     1590 2024-04-08 07:01:36.181836 cg_hermes-4.3.0/cg_hermes/config/balsamic_qc.py
+-rw-r--r--   0        0        0     5551 2024-04-08 07:01:36.181836 cg_hermes-4.3.0/cg_hermes/config/balsamic_umi.py
+-rw-r--r--   0        0        0      846 2024-04-08 07:01:36.181836 cg_hermes-4.3.0/cg_hermes/config/fluffy.py
+-rw-r--r--   0        0        0     2166 2024-04-08 07:01:36.181836 cg_hermes-4.3.0/cg_hermes/config/microsalt.py
+-rw-r--r--   0        0        0     8540 2024-04-08 07:01:36.181836 cg_hermes-4.3.0/cg_hermes/config/mip_dna.py
+-rw-r--r--   0        0        0     4551 2024-04-08 07:01:36.181836 cg_hermes-4.3.0/cg_hermes/config/mip_rna.py
+-rw-r--r--   0        0        0     4354 2024-04-08 07:01:36.181836 cg_hermes-4.3.0/cg_hermes/config/mutant.py
+-rw-r--r--   0        0        0      519 2024-04-08 07:01:36.181836 cg_hermes-4.3.0/cg_hermes/config/nextflow.py
+-rw-r--r--   0        0        0     4156 2024-04-08 07:01:36.181836 cg_hermes-4.3.0/cg_hermes/config/rnafusion.py
+-rw-r--r--   0        0        0     2527 2024-04-08 07:01:36.181836 cg_hermes-4.3.0/cg_hermes/config/taxprofiler.py
+-rw-r--r--   0        0        0     4836 2024-04-08 07:01:36.181836 cg_hermes-4.3.0/cg_hermes/config/tomte.py
+-rw-r--r--   0        0        0    27879 2024-04-08 07:01:36.181836 cg_hermes-4.3.0/cg_hermes/constants/tags.py
+-rw-r--r--   0        0        0      872 2024-04-08 07:01:36.181836 cg_hermes-4.3.0/cg_hermes/constants/workflow.py
+-rw-r--r--   0        0        0    12727 2024-04-08 07:01:36.181836 cg_hermes-4.3.0/cg_hermes/deliverables.py
+-rw-r--r--   0        0        0      338 2024-04-08 07:01:36.181836 cg_hermes-4.3.0/cg_hermes/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-08 07:01:36.181836 cg_hermes-4.3.0/cg_hermes/models/__init__.py
+-rw-r--r--   0        0        0      642 2024-04-08 07:01:36.181836 cg_hermes-4.3.0/cg_hermes/models/tags.py
+-rw-r--r--   0        0        0     2476 2024-04-08 07:01:36.181836 cg_hermes-4.3.0/cg_hermes/models/workflow_deliverables.py
+-rw-r--r--   0        0        0      997 2024-04-08 07:01:36.181836 cg_hermes-4.3.0/cg_hermes/validate.py
+-rw-r--r--   0        0        0      773 2024-04-08 07:01:36.185836 cg_hermes-4.3.0/pyproject.toml
+-rw-r--r--   0        0        0      599 1970-01-01 00:00:00.000000 cg_hermes-4.3.0/PKG-INFO
```

### Comparing `cg_hermes-4.2.1/cg_hermes/cli/base.py` & `cg_hermes-4.3.0/cg_hermes/cli/base.py`

 * *Files identical despite different names*

### Comparing `cg_hermes-4.2.1/cg_hermes/cli/common.py` & `cg_hermes-4.3.0/cg_hermes/cli/common.py`

 * *Files identical despite different names*

### Comparing `cg_hermes-4.2.1/cg_hermes/cli/convert.py` & `cg_hermes-4.3.0/cg_hermes/cli/convert.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,31 +4,30 @@
 import logging
 from pathlib import Path
 
 import typer
 from pydantic import ValidationError
 
 from cg_hermes.cli.common import get_deliverables
-from cg_hermes.config.workflows import AnalysisType
-from cg_hermes.constants.workflow import Workflow
+from cg_hermes.constants.workflow import CancerAnalysisType, Workflow
 from cg_hermes.deliverables import Deliverables
 from cg_hermes.exceptions import MissingFileError
 from cg_hermes.models.workflow_deliverables import CGDeliverables
 from cg_hermes.validate import get_deliverables_obj
 
 LOG = logging.getLogger(__name__)
 
 app = typer.Typer()
 
 
 @app.command(name="deliverables")
 def convert_cmd(
     infile: Path,
     workflow: Workflow = typer.Option(..., help="Specify the workflow"),
-    analysis_type: AnalysisType = typer.Option(None, help="Specify the analysis type"),
+    analysis_type: CancerAnalysisType = typer.Option(None, help="Specify the analysis type"),
 ):
     LOG.info(f"Convert deliverable file: {infile} from workflow {workflow} to CG format")
 
     raw_deliverables: dict[str, list[dict[str, str]]] = get_deliverables(infile)
     try:
         deliverables: Deliverables = get_deliverables_obj(
             deliverables=raw_deliverables, workflow=workflow, analysis_type=analysis_type
```

### Comparing `cg_hermes-4.2.1/cg_hermes/cli/export.py` & `cg_hermes-4.3.0/cg_hermes/cli/export.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 from cg_hermes.config.fluffy import FLUFFY_COMMON_TAGS
 from cg_hermes.config.microsalt import MICROSALT_COMMON_TAGS
 from cg_hermes.config.mip_dna import MIP_DNA_TAGS
 from cg_hermes.config.mip_rna import MIP_RNA_TAGS
 from cg_hermes.config.mutant import MUTANT_COMMON_TAGS
 from cg_hermes.config.rnafusion import RNAFUSION_TAGS
 from cg_hermes.config.taxprofiler import TAXPROFILER_TAGS
-from cg_hermes.config.tags import COMMON_TAG_CATEGORIES
+from cg_hermes.config.tomte import TOMTE_TAGS
+from cg_hermes.constants.tags import COMMON_TAG_CATEGORIES
 from cg_hermes.constants.workflow import Workflow
 
 app = typer.Typer()
 
 LOG = logging.getLogger(__name__)
 
 
@@ -70,42 +71,39 @@
         "header": ["Rnafusion tags", "Mandatory", "HK tags", "Used by"],
         "tags": RNAFUSION_TAGS,
     },
     Workflow.TAXPROFILER: {
         "header": ["Taxprofiler tags", "Mandatory", "HK tags", "Used by"],
         "tags": TAXPROFILER_TAGS,
     },
+    Workflow.TOMTE: {
+        "header": ["Tomte tags", "Mandatory", "HK tags", "Used by"],
+        "tags": TOMTE_TAGS,
+    },
 }
 
 
 @app.command(name="tags")
 def export_tags_cmd(
     output: OutputFormat = typer.Option(OutputFormat.github),
     workflow: Workflow = None,
 ):
     """Export tag definitions from Hermes."""
     LOG.info(f"Running export tags for workflow: {workflow}")
 
     if not workflow:
         header = ["Tag name", "Description"]
         for category in COMMON_TAG_CATEGORIES:
-            table_name = category.upper().replace("_", " ")
+            table_name: str = category.name()
             if output == "github":
                 typer.echo(f"## {table_name}")
             else:
                 typer.echo(table_name)
             typer.echo()
-            table = [
-                [
-                    tag_name,
-                    COMMON_TAG_CATEGORIES[category][tag_name]["description"],
-                ]
-                for tag_name in COMMON_TAG_CATEGORIES[category]
-            ]
-
+            table = [[tag.value, tag.description] for tag in category]
             typer.echo(tabulate(table, headers=header, tablefmt=output))
             typer.echo()
         raise typer.Exit()
     if workflow not in WORKFLOW_MAP:
         LOG.info("Could not recognize workflow")
         raise typer.Exit(code=1)
```

### Comparing `cg_hermes-4.2.1/cg_hermes/cli/validate.py` & `cg_hermes-4.3.0/cg_hermes/cli/validate.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,30 +10,30 @@
 from cg_hermes.config.balsamic_umi import BALSAMIC_UMI_TAGS
 from cg_hermes.config.fluffy import FLUFFY_COMMON_TAGS
 from cg_hermes.config.mip_dna import MIP_DNA_TAGS
 from cg_hermes.config.mip_rna import MIP_RNA_TAGS
 from cg_hermes.config.mutant import MUTANT_COMMON_TAGS
 from cg_hermes.config.rnafusion import RNAFUSION_TAGS
 from cg_hermes.config.taxprofiler import TAXPROFILER_TAGS
-from cg_hermes.config.workflows import AnalysisType
-from cg_hermes.constants.workflow import Workflow
+from cg_hermes.config.tomte import TOMTE_TAGS
+from cg_hermes.constants.workflow import CancerAnalysisType, Workflow
 from cg_hermes.deliverables import Deliverables
 from cg_hermes.exceptions import MissingFileError
 from cg_hermes.validate import get_deliverables_obj, validate_tag_map
 
 LOG = logging.getLogger(__name__)
 
 app = typer.Typer()
 
 
 @app.command("deliverables")
 def validate_deliverables(
     infile: Path,
     workflow: Workflow = typer.Option(Workflow.FLUFFY, help="Specify workflow"),
-    analysis_type: AnalysisType = typer.Option(None, help="Specify the analysis type"),
+    analysis_type: CancerAnalysisType = typer.Option(None, help="Specify the analysis type"),
 ):
     """Validate a deliverables file."""
     LOG.info(f"Validating file: {infile} from workflow: {workflow}")
 
     raw_deliverables: dict[str, list[dict[str, str]]] = get_deliverables(infile)
 
     try:
@@ -70,14 +70,16 @@
         tag_map = FLUFFY_COMMON_TAGS
     elif workflow == Workflow.MUTANT:
         tag_map = MUTANT_COMMON_TAGS
     elif workflow == Workflow.RNAFUSION:
         tag_map = RNAFUSION_TAGS
     elif workflow == Workflow.TAXPROFILER:
         tag_map = TAXPROFILER_TAGS
+    elif workflow == Workflow.TOMTE:
+        tag_map = TOMTE_TAGS
     else:
         LOG.info(f"Could not find workflow tags for {workflow}")
         raise typer.Exit(code=exit_code)
 
     try:
         validate_tag_map(tag_map=tag_map)
         LOG.info("Tag map looks fine")
```

### Comparing `cg_hermes-4.2.1/cg_hermes/config/balsamic.py` & `cg_hermes-4.3.0/cg_hermes/config/balsamic.py`

 * *Files identical despite different names*

### Comparing `cg_hermes-4.2.1/cg_hermes/config/balsamic_qc.py` & `cg_hermes-4.3.0/cg_hermes/config/balsamic_qc.py`

 * *Files identical despite different names*

### Comparing `cg_hermes-4.2.1/cg_hermes/config/balsamic_umi.py` & `cg_hermes-4.3.0/cg_hermes/config/balsamic_umi.py`

 * *Files identical despite different names*

### Comparing `cg_hermes-4.2.1/cg_hermes/config/fluffy.py` & `cg_hermes-4.3.0/cg_hermes/config/fluffy.py`

 * *Files identical despite different names*

### Comparing `cg_hermes-4.2.1/cg_hermes/config/microsalt.py` & `cg_hermes-4.3.0/cg_hermes/config/microsalt.py`

 * *Files identical despite different names*

### Comparing `cg_hermes-4.2.1/cg_hermes/config/mip_dna.py` & `cg_hermes-4.3.0/cg_hermes/config/mip_dna.py`

 * *Files identical despite different names*

### Comparing `cg_hermes-4.2.1/cg_hermes/config/mip_rna.py` & `cg_hermes-4.3.0/cg_hermes/config/mip_rna.py`

 * *Files identical despite different names*

### Comparing `cg_hermes-4.2.1/cg_hermes/config/mutant.py` & `cg_hermes-4.3.0/cg_hermes/config/mutant.py`

 * *Files identical despite different names*

### Comparing `cg_hermes-4.2.1/cg_hermes/config/rnafusion.py` & `cg_hermes-4.3.0/cg_hermes/config/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg_hermes-4.2.1/cg_hermes/config/taxprofiler.py` & `cg_hermes-4.3.0/cg_hermes/config/taxprofiler.py`

 * *Files identical despite different names*

### Comparing `cg_hermes-4.2.1/cg_hermes/deliverables.py` & `cg_hermes-4.3.0/cg_hermes/deliverables.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Class to represent deliverables file."""
+
 import copy
 import logging
 from typing import FrozenSet
 
 from cg_hermes.config.balsamic import (
     BALSAMIC_TAGS,
     TUMOR_NORMAL_PANEL_TAGS,
@@ -23,49 +24,47 @@
 from cg_hermes.config.fluffy import FLUFFY_COMMON_TAGS
 from cg_hermes.config.microsalt import MICROSALT_COMMON_TAGS
 from cg_hermes.config.mip_dna import MIP_DNA_TAGS
 from cg_hermes.config.mip_rna import MIP_RNA_TAGS
 from cg_hermes.config.mutant import MUTANT_COMMON_TAGS
 from cg_hermes.config.rnafusion import RNAFUSION_TAGS
 from cg_hermes.config.taxprofiler import TAXPROFILER_TAGS
-from cg_hermes.config.workflows import AnalysisType
-from cg_hermes.constants.workflow import Workflow
+from cg_hermes.config.tomte import TOMTE_TAGS
+from cg_hermes.constants.workflow import CancerAnalysisType, Workflow
 from cg_hermes.exceptions import MissingFileError
 from cg_hermes.models.tags import CGTag, TagMap
 from cg_hermes.models.workflow_deliverables import (
     BalsamicDeliverables,
     BalsamicFile,
     CGDeliverables,
     FileBase,
     FluffyDeliverables,
     MicrosaltDeliverables,
     MicrosaltFile,
     MipDeliverables,
     MipFile,
     MutantDeliverables,
     MutantFile,
-    RnafusionDeliverables,
-    RnafusionFile,
+    NfAnalysisDeliverables,
+    NfAnalysisFile,
     TagBase,
-    TaxprofilerDeliverables,
-    TaxprofilerFile,
     WorkflowDeliverables,
 )
 
 LOG = logging.getLogger(__name__)
 
 
 class Deliverables:
     """Class with functionality to validate deliverables"""
 
     def __init__(
         self,
         deliverables: dict[str, list[dict[str, str]]],
         workflow: Workflow,
-        analysis_type: AnalysisType | None = None,
+        analysis_type: CancerAnalysisType | None = None,
     ):
         self.raw_deliverables = deliverables
         self.workflow = workflow
         self.analysis_type = analysis_type
         self.bundle_id: str | None = None
         self.configs: dict[FrozenSet[str], TagMap]
         self.files: list[TagBase]
@@ -98,26 +97,25 @@
             self.model: MipDeliverables = MipDeliverables.parse_obj(self.raw_deliverables)
             self.files = self.get_mip_files()
             self.configs = Deliverables.build_internal_tag_map(MIP_DNA_TAGS)
         elif self.workflow == Workflow.MIP_RNA:
             self.model: MipDeliverables = MipDeliverables.parse_obj(self.raw_deliverables)
             self.files = self.get_mip_files()
             self.configs = Deliverables.build_internal_tag_map(MIP_RNA_TAGS)
-        elif self.workflow == Workflow.RNAFUSION:
-            self.model: RnafusionDeliverables = RnafusionDeliverables.parse_obj(
-                self.raw_deliverables
-            )
-            self.files = self.get_rnafusion_files()
-            self.configs = Deliverables.build_internal_tag_map(RNAFUSION_TAGS)
-        elif self.workflow == Workflow.TAXPROFILER:
-            self.model: TaxprofilerDeliverables = TaxprofilerDeliverables.parse_obj(
+        elif self.workflow in Workflow.get_nf_workflows():
+            self.model: NfAnalysisDeliverables = NfAnalysisDeliverables.parse_obj(
                 self.raw_deliverables
             )
-            self.files = self.get_taxprofiler_files()
-            self.configs = Deliverables.build_internal_tag_map(TAXPROFILER_TAGS)
+            self.files = self.get_nf_analysis_files()
+            if self.workflow == Workflow.RNAFUSION:
+                self.configs = Deliverables.build_internal_tag_map(RNAFUSION_TAGS)
+            elif self.workflow == Workflow.TAXPROFILER:
+                self.configs = Deliverables.build_internal_tag_map(TAXPROFILER_TAGS)
+            elif self.workflow == Workflow.TOMTE:
+                self.configs = Deliverables.build_internal_tag_map(TOMTE_TAGS)
         else:
             raise Exception(
                 "Invalid workflow ({}) set for Deliverables object".format(self.workflow)
             )
 
     @staticmethod
     def build_internal_tag_map(tag_map: dict[FrozenSet[str], dict]) -> dict[FrozenSet[str], TagMap]:
@@ -171,31 +169,31 @@
     def get_balsamic_analysis_configs(self) -> dict[FrozenSet[str], dict]:
         """Extracts all the BALSAMIC mandatory files depending on the analysis workflow and type executed"""
 
         BALSAMIC_COMMON_TAGS = []
         tag_set = []
         if self.workflow == Workflow.BALSAMIC:
             BALSAMIC_COMMON_TAGS = BALSAMIC_TAGS
-            if self.analysis_type == AnalysisType.tumor_wgs:
+            if self.analysis_type == CancerAnalysisType.TUMOR_WGS:
                 tag_set = TUMOR_ONLY_WGS_TAGS
-            elif self.analysis_type == AnalysisType.tumor_normal_wgs:
+            elif self.analysis_type == CancerAnalysisType.TUMOR_NORMAL_WGS:
                 tag_set = TUMOR_NORMAL_WGS_TAGS
-            elif self.analysis_type == AnalysisType.tumor_panel:
+            elif self.analysis_type == CancerAnalysisType.TUMOR_PANEL:
                 tag_set = TUMOR_ONLY_PANEL_TAGS
             else:
                 tag_set = TUMOR_NORMAL_PANEL_TAGS
         elif self.workflow == Workflow.BALSAMIC_QC:
             BALSAMIC_COMMON_TAGS = BALSAMIC_QC_TAGS
-            if self.analysis_type == AnalysisType.tumor_normal_wgs:
+            if self.analysis_type == CancerAnalysisType.TUMOR_NORMAL_WGS:
                 tag_set = QC_TUMOR_NORMAL_WGS_TAGS
-            elif self.analysis_type == AnalysisType.tumor_normal_panel:
+            elif self.analysis_type == CancerAnalysisType.TUMOR_NORMAL_PANEL:
                 tag_set = QC_TUMOR_NORMAL_PANEL_TAGS
         elif self.workflow == Workflow.BALSAMIC_UMI:
             BALSAMIC_COMMON_TAGS = BALSAMIC_UMI_TAGS
-            if self.analysis_type == AnalysisType.tumor_panel:
+            if self.analysis_type == CancerAnalysisType.TUMOR_PANEL:
                 tag_set = UMI_TUMOR_ONLY_PANEL_TAGS
             else:
                 tag_set = UMI_TUMOR_NORMAL_PANEL_TAGS
 
         updated_tags = copy.deepcopy(BALSAMIC_COMMON_TAGS)
         for tag_name in tag_set:
             tag_info = tag_set[tag_name]
@@ -286,32 +284,16 @@
                 tag_sample_id: str = "-".join(split_id)
             identifier = frozenset(tag.lower() for tag in file_obj.tag if tag != tag_sample_id)
 
             LOG.debug("Found tag %s", identifier)
             files.append(TagBase(tags=identifier, subject_id=sample_id, path=file_obj.path))
         return files
 
-    def get_rnafusion_files(self) -> list[TagBase]:
-        file_obj: RnafusionFile
-        files: list[TagBase] = []
-        for file_obj in self.model.files:
-            identifier = [file_obj.step]
-            if file_obj.tag:
-                identifier.append(file_obj.tag)
-            files.append(
-                TagBase(
-                    tags=frozenset(identifier),
-                    subject_id=file_obj.id,
-                    path=file_obj.path,
-                )
-            )
-        return files
-
-    def get_taxprofiler_files(self) -> list[TagBase]:
-        file_obj: TaxprofilerFile
+    def get_nf_analysis_files(self) -> list[TagBase]:
+        file_obj: NfAnalysisFile
         files: list[TagBase] = []
         for file_obj in self.model.files:
             identifier = [file_obj.step]
             if file_obj.tag:
                 identifier.append(file_obj.tag)
             files.append(
                 TagBase(
```

### Comparing `cg_hermes-4.2.1/cg_hermes/models/tags.py` & `cg_hermes-4.3.0/cg_hermes/models/tags.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pydantic import validator
 from pydantic.main import BaseModel
 
-from cg_hermes.config.tags import ALL_TAGS, AVAILABLE_USAGES
+from cg_hermes.constants.tags import ALL_TAGS, USAGE_TAGS
 
 
 class TagMap(BaseModel):
     tags: list[str]
     is_mandatory: bool
     used_by: list[str]
     bundle_id: bool | None = False
@@ -13,15 +13,15 @@
     @validator("tags", each_item=True)
     def check_tags(cls, tag):
         assert tag in ALL_TAGS, f"{tag} not a valid tag"
         return tag
 
     @validator("used_by", each_item=True)
     def check_usage(cls, usage):
-        assert usage in AVAILABLE_USAGES, f"{usage} not a valid usage"
+        assert usage in USAGE_TAGS, f"{usage} not a valid usage"
         return usage
 
 
 class CGTag(BaseModel):
     path: str
     tags: list[str]
     mandatory: bool
```

### Comparing `cg_hermes-4.2.1/cg_hermes/models/workflow_deliverables.py` & `cg_hermes-4.3.0/cg_hermes/models/workflow_deliverables.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,16 +33,16 @@
 class MutantFile(FileBase):
     """Definition for elements in Mutant deliverables"""
 
     format: str
     step: str
 
 
-class RnafusionFile(FileBase):
-    """Definition for elements in Rnafusion deliverables"""
+class NfAnalysisFile(FileBase):
+    """Definition for elements in deliverables for nextflow workflows."""
 
     format: str
     path_index: str | None
     step: str
 
 
 class BalsamicFile(FileBase):
@@ -54,22 +54,14 @@
     @validator("tag", pre=True)
     def split_str(cls, v):
         if isinstance(v, str):
             return v.split(",")
         return v
 
 
-class TaxprofilerFile(FileBase):
-    """Definition for elements in Taxprofiler deliverables."""
-
-    format: str
-    path_index: str | None
-    step: str
-
-
 # Classes to represent deliverable files
 
 
 class WorkflowDeliverables(BaseModel):
     """Specification for a general deliverables file"""
 
     files: list[FileBase]
@@ -101,24 +93,18 @@
 
 class MutantDeliverables(WorkflowDeliverables):
     """Specification for a MUTANT specific deliverables file"""
 
     files: list[MutantFile]
 
 
-class RnafusionDeliverables(WorkflowDeliverables):
-    """Specification for a RNAFUSION specific deliverables file"""
-
-    files: list[RnafusionFile]
-
-
-class TaxprofilerDeliverables(WorkflowDeliverables):
-    """Specification for a Taxprofiler specific deliverables file."""
+class NfAnalysisDeliverables(WorkflowDeliverables):
+    """Specification for a deliverables file for a nextflow workflow."""
 
-    files: list[TaxprofilerFile]
+    files: list[NfAnalysisFile]
 
 
 class CGDeliverables(WorkflowDeliverables):
     """Class that specifies the output to CG"""
 
     workflow: str
     bundle_id: str
```

### Comparing `cg_hermes-4.2.1/pyproject.toml` & `cg_hermes-4.3.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cg-hermes"
-version = "4.2.1"
+version = "4.3.0"
 description = "Convert information between pipelines and CG"
 authors = ["Måns Magnusson <mans.magnusson@scilifelab.se>"]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 pydantic = "^1.7.3"
 coloredlogs = "^14.0"
```

### Comparing `cg_hermes-4.2.1/PKG-INFO` & `cg_hermes-4.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cg-hermes
-Version: 4.2.1
+Version: 4.3.0
 Summary: Convert information between pipelines and CG
 Author: Måns Magnusson
 Author-email: mans.magnusson@scilifelab.se
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bump2version (>=1.0.1,<2.0.0)
```

