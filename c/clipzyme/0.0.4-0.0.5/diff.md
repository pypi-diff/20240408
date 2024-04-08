# Comparing `tmp/clipzyme-0.0.4.tar.gz` & `tmp/clipzyme-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clipzyme-0.0.4.tar", max compression
+gzip compressed data, was "clipzyme-0.0.5.tar", max compression
```

## Comparing `clipzyme-0.0.4.tar` & `clipzyme-0.0.5.tar`

### file list

```diff
@@ -1,56 +1,57 @@
--rw-r--r--   0        0        0    11358 2024-03-28 18:26:04.343837 clipzyme-0.0.4/LICENSE.txt
--rw-r--r--   0        0        0     4253 2024-03-29 06:25:59.143772 clipzyme-0.0.4/README.md
--rw-r--r--   0        0        0     1696 2024-03-29 17:09:45.001827 clipzyme-0.0.4/clipzyme/__init__.py
--rw-r--r--   0        0        0        0 2024-03-28 15:53:13.578850 clipzyme-0.0.4/clipzyme/callbacks/__init__.py
--rw-r--r--   0        0        0      948 2024-03-28 15:53:13.579321 clipzyme-0.0.4/clipzyme/callbacks/basic.py
--rw-r--r--   0        0        0        0 2024-03-28 15:53:13.579397 clipzyme-0.0.4/clipzyme/datasets/__init__.py
--rw-r--r--   0        0        0     8552 2024-03-28 15:53:13.579934 clipzyme-0.0.4/clipzyme/datasets/abstract.py
--rw-r--r--   0        0        0    12769 2024-03-28 15:53:13.580656 clipzyme-0.0.4/clipzyme/datasets/enzyme_screening.py
--rw-r--r--   0        0        0    59793 2024-03-28 18:04:43.401264 clipzyme-0.0.4/clipzyme/datasets/enzymemap.py
--rw-r--r--   0        0        0    11047 2024-03-28 21:19:33.372241 clipzyme-0.0.4/clipzyme/datasets/reaction.py
--rw-r--r--   0        0        0        0 2024-03-28 15:53:13.581466 clipzyme-0.0.4/clipzyme/learning/losses/__init__.py
--rw-r--r--   0        0        0    10857 2024-03-28 15:53:13.581946 clipzyme-0.0.4/clipzyme/learning/losses/basic.py
--rw-r--r--   0        0        0    17891 2024-03-28 18:04:43.398133 clipzyme-0.0.4/clipzyme/learning/losses/contrastive.py
--rw-r--r--   0        0        0        0 2024-03-28 15:53:13.582586 clipzyme-0.0.4/clipzyme/learning/metrics/__init__.py
--rw-r--r--   0        0        0    20086 2024-03-28 15:53:13.582961 clipzyme-0.0.4/clipzyme/learning/metrics/basic.py
--rw-r--r--   0        0        0     6590 2024-03-28 15:53:13.583284 clipzyme-0.0.4/clipzyme/learning/metrics/representation.py
--rw-r--r--   0        0        0        0 2024-03-28 15:53:13.583361 clipzyme-0.0.4/clipzyme/learning/optimizers/__init__.py
--rw-r--r--   0        0        0     2406 2024-03-28 15:53:13.583673 clipzyme-0.0.4/clipzyme/learning/optimizers/basic.py
--rw-r--r--   0        0        0        0 2024-03-28 15:53:13.583744 clipzyme-0.0.4/clipzyme/learning/schedulers/__init__.py
--rw-r--r--   0        0        0     1855 2024-03-28 15:53:13.583927 clipzyme-0.0.4/clipzyme/learning/schedulers/basic.py
--rw-r--r--   0        0        0     6835 2024-03-28 18:04:43.397866 clipzyme-0.0.4/clipzyme/learning/schedulers/warmup.py
--rw-r--r--   0        0        0      122 2024-03-28 15:53:13.584578 clipzyme-0.0.4/clipzyme/learning/utils.py
--rw-r--r--   0        0        0        0 2024-03-28 15:53:13.584651 clipzyme-0.0.4/clipzyme/lightning/__init__.py
--rw-r--r--   0        0        0    21181 2024-03-28 15:53:13.584896 clipzyme-0.0.4/clipzyme/lightning/base.py
--rw-r--r--   0        0        0    10369 2024-03-28 23:19:42.636488 clipzyme-0.0.4/clipzyme/lightning/clipzyme.py
--rw-r--r--   0        0        0        0 2024-03-28 15:53:13.585018 clipzyme-0.0.4/clipzyme/loggers/__init__.py
--rw-r--r--   0        0        0      637 2024-03-28 15:53:13.585360 clipzyme-0.0.4/clipzyme/loggers/tensorboard.py
--rw-r--r--   0        0        0     2254 2024-03-28 15:53:13.585569 clipzyme-0.0.4/clipzyme/loggers/wandb.py
--rw-r--r--   0        0        0        0 2024-03-28 15:53:13.585646 clipzyme-0.0.4/clipzyme/models/__init__.py
--rw-r--r--   0        0        0      300 2024-03-28 15:53:13.585810 clipzyme-0.0.4/clipzyme/models/abstract.py
--rw-r--r--   0        0        0     7144 2024-03-28 15:53:13.585987 clipzyme-0.0.4/clipzyme/models/chemprop.py
--rw-r--r--   0        0        0     7285 2024-03-28 15:53:13.586155 clipzyme-0.0.4/clipzyme/models/classifier.py
--rw-r--r--   0        0        0    29102 2024-03-28 15:53:13.586482 clipzyme-0.0.4/clipzyme/models/egnn.py
--rw-r--r--   0        0        0     6917 2024-03-28 15:53:13.586943 clipzyme-0.0.4/clipzyme/models/fair_esm.py
--rw-r--r--   0        0        0    10220 2024-03-28 15:53:13.587252 clipzyme-0.0.4/clipzyme/models/gat.py
--rw-r--r--   0        0        0    28669 2024-03-28 15:53:13.587614 clipzyme-0.0.4/clipzyme/models/protmol.py
--rw-r--r--   0        0        0     5331 2024-03-28 15:53:13.588426 clipzyme-0.0.4/clipzyme/models/seq2seq.py
--rw-r--r--   0        0        0    24182 2024-03-28 15:53:13.588821 clipzyme-0.0.4/clipzyme/models/wln.py
--rw-r--r--   0        0        0        0 2024-03-28 15:53:13.588932 clipzyme-0.0.4/clipzyme/utils/__init__.py
--rw-r--r--   0        0        0     1891 2024-03-28 15:53:13.589041 clipzyme-0.0.4/clipzyme/utils/amino_acids.py
--rw-r--r--   0        0        0     1679 2024-03-28 15:53:13.589238 clipzyme-0.0.4/clipzyme/utils/callbacks.py
--rw-r--r--   0        0        0     3669 2024-03-28 15:53:13.589424 clipzyme-0.0.4/clipzyme/utils/classes.py
--rw-r--r--   0        0        0     8793 2024-03-28 18:04:43.397858 clipzyme-0.0.4/clipzyme/utils/colabfold_msa.py
--rw-r--r--   0        0        0    11554 2024-03-28 15:53:13.589737 clipzyme-0.0.4/clipzyme/utils/loading.py
--rw-r--r--   0        0        0      154 2024-03-28 15:53:13.589922 clipzyme-0.0.4/clipzyme/utils/messages.py
--rw-r--r--   0        0        0    22189 2024-03-28 15:53:13.590443 clipzyme-0.0.4/clipzyme/utils/parsing.py
--rw-r--r--   0        0        0    10752 2024-03-28 18:04:43.398921 clipzyme-0.0.4/clipzyme/utils/protein_utils.py
--rw-r--r--   0        0        0    15629 2024-03-28 18:04:43.398175 clipzyme-0.0.4/clipzyme/utils/proteins.py
--rw-r--r--   0        0        0    13289 2024-03-28 15:53:13.591225 clipzyme-0.0.4/clipzyme/utils/pyg.py
--rw-r--r--   0        0        0    17957 2024-03-28 18:04:43.399109 clipzyme-0.0.4/clipzyme/utils/reactions.py
--rw-r--r--   0        0        0     1187 2024-03-28 15:53:13.591465 clipzyme-0.0.4/clipzyme/utils/registry.py
--rw-r--r--   0        0        0     4638 2024-03-28 15:53:13.591739 clipzyme-0.0.4/clipzyme/utils/sampler.py
--rw-r--r--   0        0        0    22325 2024-03-28 15:53:13.591875 clipzyme-0.0.4/clipzyme/utils/smiles.py
--rw-r--r--   0        0        0    48101 2024-03-28 18:04:43.399645 clipzyme-0.0.4/clipzyme/utils/wln_processing.py
--rw-r--r--   0        0        0      623 2024-03-29 17:10:35.897902 clipzyme-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     4778 1970-01-01 00:00:00.000000 clipzyme-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-03-28 18:26:04.343837 clipzyme-0.0.5/LICENSE.txt
+-rw-r--r--   0        0        0     7694 2024-04-08 16:54:12.469585 clipzyme-0.0.5/README.md
+-rw-r--r--   0        0        0     1788 2024-03-29 19:24:34.636971 clipzyme-0.0.5/clipzyme/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-28 15:53:13.578850 clipzyme-0.0.5/clipzyme/callbacks/__init__.py
+-rw-r--r--   0        0        0      948 2024-03-28 15:53:13.579321 clipzyme-0.0.5/clipzyme/callbacks/basic.py
+-rw-r--r--   0        0        0        0 2024-03-28 15:53:13.579397 clipzyme-0.0.5/clipzyme/datasets/__init__.py
+-rw-r--r--   0        0        0     8552 2024-03-28 15:53:13.579934 clipzyme-0.0.5/clipzyme/datasets/abstract.py
+-rw-r--r--   0        0        0    12769 2024-03-28 15:53:13.580656 clipzyme-0.0.5/clipzyme/datasets/enzyme_screening.py
+-rw-r--r--   0        0        0    43705 2024-04-08 16:54:12.470132 clipzyme-0.0.5/clipzyme/datasets/enzymemap.py
+-rw-r--r--   0        0        0    11816 2024-04-08 02:52:05.338533 clipzyme-0.0.5/clipzyme/datasets/reaction.py
+-rw-r--r--   0        0        0        0 2024-03-28 15:53:13.581466 clipzyme-0.0.5/clipzyme/learning/losses/__init__.py
+-rw-r--r--   0        0        0    10857 2024-03-28 15:53:13.581946 clipzyme-0.0.5/clipzyme/learning/losses/basic.py
+-rw-r--r--   0        0        0    17891 2024-03-28 18:04:43.398133 clipzyme-0.0.5/clipzyme/learning/losses/contrastive.py
+-rw-r--r--   0        0        0        0 2024-03-28 15:53:13.582586 clipzyme-0.0.5/clipzyme/learning/metrics/__init__.py
+-rw-r--r--   0        0        0    20086 2024-03-28 15:53:13.582961 clipzyme-0.0.5/clipzyme/learning/metrics/basic.py
+-rw-r--r--   0        0        0     6590 2024-03-28 15:53:13.583284 clipzyme-0.0.5/clipzyme/learning/metrics/representation.py
+-rw-r--r--   0        0        0        0 2024-03-28 15:53:13.583361 clipzyme-0.0.5/clipzyme/learning/optimizers/__init__.py
+-rw-r--r--   0        0        0     2406 2024-03-28 15:53:13.583673 clipzyme-0.0.5/clipzyme/learning/optimizers/basic.py
+-rw-r--r--   0        0        0        0 2024-03-28 15:53:13.583744 clipzyme-0.0.5/clipzyme/learning/schedulers/__init__.py
+-rw-r--r--   0        0        0     1855 2024-03-28 15:53:13.583927 clipzyme-0.0.5/clipzyme/learning/schedulers/basic.py
+-rw-r--r--   0        0        0     6835 2024-03-28 18:04:43.397866 clipzyme-0.0.5/clipzyme/learning/schedulers/warmup.py
+-rw-r--r--   0        0        0      122 2024-03-28 15:53:13.584578 clipzyme-0.0.5/clipzyme/learning/utils.py
+-rw-r--r--   0        0        0        0 2024-03-28 15:53:13.584651 clipzyme-0.0.5/clipzyme/lightning/__init__.py
+-rw-r--r--   0        0        0    21181 2024-03-28 15:53:13.584896 clipzyme-0.0.5/clipzyme/lightning/base.py
+-rw-r--r--   0        0        0    12584 2024-04-08 17:02:34.466944 clipzyme-0.0.5/clipzyme/lightning/clipzyme.py
+-rw-r--r--   0        0        0        0 2024-03-28 15:53:13.585018 clipzyme-0.0.5/clipzyme/loggers/__init__.py
+-rw-r--r--   0        0        0      637 2024-03-28 15:53:13.585360 clipzyme-0.0.5/clipzyme/loggers/tensorboard.py
+-rw-r--r--   0        0        0     2254 2024-03-28 15:53:13.585569 clipzyme-0.0.5/clipzyme/loggers/wandb.py
+-rw-r--r--   0        0        0        0 2024-03-28 15:53:13.585646 clipzyme-0.0.5/clipzyme/models/__init__.py
+-rw-r--r--   0        0        0      300 2024-03-28 15:53:13.585810 clipzyme-0.0.5/clipzyme/models/abstract.py
+-rw-r--r--   0        0        0     7144 2024-03-28 15:53:13.585987 clipzyme-0.0.5/clipzyme/models/chemprop.py
+-rw-r--r--   0        0        0     7285 2024-03-28 15:53:13.586155 clipzyme-0.0.5/clipzyme/models/classifier.py
+-rw-r--r--   0        0        0    29102 2024-03-28 15:53:13.586482 clipzyme-0.0.5/clipzyme/models/egnn.py
+-rw-r--r--   0        0        0     6917 2024-03-28 15:53:13.586943 clipzyme-0.0.5/clipzyme/models/fair_esm.py
+-rw-r--r--   0        0        0    10220 2024-03-28 15:53:13.587252 clipzyme-0.0.5/clipzyme/models/gat.py
+-rw-r--r--   0        0        0    28859 2024-03-29 19:38:31.847201 clipzyme-0.0.5/clipzyme/models/protmol.py
+-rw-r--r--   0        0        0     5331 2024-03-28 15:53:13.588426 clipzyme-0.0.5/clipzyme/models/seq2seq.py
+-rw-r--r--   0        0        0    24182 2024-03-28 15:53:13.588821 clipzyme-0.0.5/clipzyme/models/wln.py
+-rw-r--r--   0        0        0        0 2024-03-28 15:53:13.588932 clipzyme-0.0.5/clipzyme/utils/__init__.py
+-rw-r--r--   0        0        0     1891 2024-03-28 15:53:13.589041 clipzyme-0.0.5/clipzyme/utils/amino_acids.py
+-rw-r--r--   0        0        0     1679 2024-03-28 15:53:13.589238 clipzyme-0.0.5/clipzyme/utils/callbacks.py
+-rw-r--r--   0        0        0     3669 2024-03-28 15:53:13.589424 clipzyme-0.0.5/clipzyme/utils/classes.py
+-rw-r--r--   0        0        0     8793 2024-03-28 18:04:43.397858 clipzyme-0.0.5/clipzyme/utils/colabfold_msa.py
+-rw-r--r--   0        0        0    11554 2024-03-28 15:53:13.589737 clipzyme-0.0.5/clipzyme/utils/loading.py
+-rw-r--r--   0        0        0      154 2024-03-28 15:53:13.589922 clipzyme-0.0.5/clipzyme/utils/messages.py
+-rw-r--r--   0        0        0    22189 2024-03-28 15:53:13.590443 clipzyme-0.0.5/clipzyme/utils/parsing.py
+-rw-r--r--   0        0        0    13604 2024-04-08 17:00:53.080799 clipzyme-0.0.5/clipzyme/utils/protein_utils.py
+-rw-r--r--   0        0        0    15629 2024-03-28 18:04:43.398175 clipzyme-0.0.5/clipzyme/utils/proteins.py
+-rw-r--r--   0        0        0    13289 2024-03-28 15:53:13.591225 clipzyme-0.0.5/clipzyme/utils/pyg.py
+-rw-r--r--   0        0        0    17957 2024-03-28 18:04:43.399109 clipzyme-0.0.5/clipzyme/utils/reactions.py
+-rw-r--r--   0        0        0     1187 2024-03-28 15:53:13.591465 clipzyme-0.0.5/clipzyme/utils/registry.py
+-rw-r--r--   0        0        0     4638 2024-03-28 15:53:13.591739 clipzyme-0.0.5/clipzyme/utils/sampler.py
+-rw-r--r--   0        0        0     4897 2024-04-08 16:56:54.314023 clipzyme-0.0.5/clipzyme/utils/screening.py
+-rw-r--r--   0        0        0    22325 2024-03-28 15:53:13.591875 clipzyme-0.0.5/clipzyme/utils/smiles.py
+-rw-r--r--   0        0        0    48101 2024-03-28 18:04:43.399645 clipzyme-0.0.5/clipzyme/utils/wln_processing.py
+-rw-r--r--   0        0        0      623 2024-04-08 17:03:00.807007 clipzyme-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     8219 1970-01-01 00:00:00.000000 clipzyme-0.0.5/PKG-INFO
```

### Comparing `clipzyme-0.0.4/LICENSE.txt` & `clipzyme-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.4/clipzyme/__init__.py` & `clipzyme-0.0.5/clipzyme/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -59,9 +59,10 @@
 # comet
 import clipzyme.loggers.wandb
 import clipzyme.loggers.tensorboard
 
 from clipzyme.datasets.reaction import ReactionDataset
 from clipzyme.lightning.clipzyme import CLIPZyme
 from clipzyme.utils.registry import get_object
+from clipzyme.utils.screening import collect_screening_results
 
-__all__ = ["CLIPZyme", "ReactionDataset", "get_object"]
+__all__ = ["CLIPZyme", "ReactionDataset", "get_object", "collect_screening_results"]
```

### Comparing `clipzyme-0.0.4/clipzyme/callbacks/basic.py` & `clipzyme-0.0.5/clipzyme/callbacks/basic.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.4/clipzyme/datasets/abstract.py` & `clipzyme-0.0.5/clipzyme/datasets/abstract.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.4/clipzyme/datasets/enzyme_screening.py` & `clipzyme-0.0.5/clipzyme/datasets/enzyme_screening.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.4/clipzyme/datasets/enzymemap.py` & `clipzyme-0.0.5/clipzyme/datasets/enzymemap.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,27 +16,24 @@
 import Bio
 from Bio.Data.IUPACData import protein_letters_3to1
 import Bio.PDB
 from esm import pretrained
 from clipzyme.utils.registry import register_object
 from clipzyme.datasets.abstract import AbstractDataset
 
-from clipzyme.utils.smiles import (
-    generate_scaffold,
-)
+
 from clipzyme.utils.protein_utils import (
     read_structure_file,
     filter_resolution,
     build_graph,
     compute_graph_edges,
     compute_node_embedding,
 )
 from clipzyme.utils.pyg import from_mapped_smiles
 from clipzyme.utils.wln_processing import get_bond_changes
-from clipzyme.models.wln import WLDN_Cache
 
 ESM_MODEL2HIDDEN_DIM = {
     "esm2_t48_15B_UR50D": 5120,
     "esm2_t36_3B_UR50D": 2560,
     "esm2_t33_650M_UR50D": 1280,
     "esm2_t30_150M_UR50D": 640,
     "esm2_t12_35M_UR50D": 480,
@@ -68,55 +65,37 @@
             self.esm_dir = args.esm_dir
             model, alphabet = pretrained.load_model_and_alphabet(args.esm_dir)
             self.esm_model = model
             self.alphabet = alphabet
             self.batch_converter = alphabet.get_batch_converter()
         super(EnzymeMap, EnzymeMap).__init__(self, args, split_group)
         self.metadata_json = None  # overwrite for memory
-        if args.load_wln_cache_in_dataset:
-            self.cache = WLDN_Cache(args.cache_path)
 
     def init_class(self, args: argparse.ArgumentParser, split_group: str) -> None:
         """Perform Class-Specific init methods
            Default is to load JSON dataset
 
         Args:
             args (argparse.ArgumentParser)
             split_group (str)
         """
         self.version = args.version
         self.load_dataset(args)
 
         self.valid_ec2uniprot = defaultdict(set)
 
-        self.ec2uniprot = pickle.load(
-            open(
-                "/home/datasets/EnzymeMap/ec2uniprot.p",
-                "rb",
-            )
-        )
-        self.uniprot2sequence = pickle.load(
-            open(
-                "/home/datasets/EnzymeMap/uniprot2sequence.p",
-                "rb",
-            )
-        )
+        self.ec2uniprot = pickle.load(open("files/ec2uniprot.p", "rb"))
+        self.uniprot2sequence = pickle.load(open("files/uniprot2sequence.p", "rb"))
         self.uniprot2sequence_len = {
             k: 0 if v is None else len(v) for k, v in self.uniprot2sequence.items()
         }
-        self.uniprot2cluster = pickle.load(
-            open(
-                args.uniprot2cluster_path,
-                "rb",
-            )
-        )
 
         # products to remove based on smiles or pattern
-        remove_patterns_path = "/home/datasets/ECReact/patterns.txt"
-        remove_molecules_path = "/home/datasets/ECReact/molecules.txt"
+        remove_patterns_path = "files/ecreact/patterns.txt"
+        remove_molecules_path = "files/ecreact/molecules.txt"
 
         self.remove_patterns = []
         self.remove_molecules = []
 
         for line in open(remove_patterns_path):
             if not line.startswith("//") and line.strip():
                 self.remove_patterns.append(line.split("//")[0].strip())
@@ -133,25 +112,14 @@
                     self.remove_molecules.append(rdk.MolToSmiles(mol))
                     self.remove_molecules.append(
                         Chem.CanonSmiles(
                             self.remove_molecules[-1].replace("[O-]", "[OH]")
                         )
                     )
 
-        if (
-            not hasattr(self.args, "use_all_sequences")
-            or not self.args.use_all_sequences
-        ):
-            self.uniprot2split = pickle.load(
-                open(
-                    "/home/datasets/EnzymeMap/mmseq_splits_precomputed.p",
-                    "rb",
-                )
-            )
-
     def create_dataset(
         self, split_group: Literal["train", "dev", "test"]
     ) -> List[dict]:
         # if removing top K
         if self.args.topk_byproducts_to_remove is not None:
             raw_byproducts = Counter(
                 [r for d in self.metadata_json for r in d["products"]]
@@ -373,21 +341,14 @@
                 "quality": sample["quality"],
             }
 
             split_ec = ec.split(".")
             for k, v in self.args.ec_levels.items():
                 item[f"ec{k}"] = v.get(".".join(split_ec[: int(k)]), -1)
 
-            if self.args.use_pesto_scores:
-                scores = self.get_pesto_scores(item["protein_id"])
-                if (scores is None) or (scores.shape[0] != len(item["sequence"])):
-                    # make all zeros of length sequence
-                    scores = torch.zeros(len(item["sequence"]))
-                item["sequence_annotation"] = scores
-
             return item
 
         except Exception as e:
             print(
                 f"Getitem enzymemap: Could not load sample {sample['uniprot_id']} because of exception {e}"
             )
 
@@ -408,322 +369,45 @@
         """
         # get all samples
         self.to_split = {}
 
         # set seed
         np.random.seed(seed)
 
-        # assign groups
-        if self.args.split_type in [
-            "mmseqs",
-            "sequence",
-            "ec",
-            "product",
-            "mmseqs_precomputed",
-        ]:
-            if (
-                self.args.split_type == "mmseqs"
-                or self.args.split_type == "mmseqs_precomputed"
-            ):
-                samples = [
-                    self.uniprot2cluster[reaction["uniprot_id"]]
-                    for reaction in metadata_json
-                ]
-                # samples = list(self.uniprot2cluster.values())
-
-            if self.args.split_type == "sequence":
-                # split based on uniprot_id
-                samples = [
-                    u
-                    for reaction in metadata_json
-                    for u in self.ec2uniprot.get(reaction["ec"], [])
-                ]
-                if "protein_id" in metadata_json[0]:
-                    samples += [r["protein_id"] for r in metadata_json]
-
-            elif self.args.split_type == "ec":
-                # split based on ec number
-                samples = [reaction["ec"] for reaction in metadata_json]
-
-                # option to change level of ec categorization based on which to split
-                samples = [
-                    ".".join(e.split(".")[: self.args.ec_level + 1]) for e in samples
-                ]
-
-            elif self.args.split_type == "product":
-                # split by reaction product (splits share no products)
-                samples = [".".join(s["products"]) for s in metadata_json]
-
-            sample2count = Counter(samples)
-            samples = sorted(list(set(samples)))
-            np.random.shuffle(samples)
-            samples_cumsum = np.cumsum([sample2count[s] for s in samples])
-            # Find the indices for each quantile
-            split_indices = [
-                np.searchsorted(
-                    samples_cumsum, np.round(q, 3) * samples_cumsum[-1], side="right"
-                )
-                for q in np.cumsum(split_probs)
-            ]
-            split_indices[-1] = len(samples)
-            split_indices = np.concatenate([[0], split_indices])
-            for i in range(len(split_indices) - 1):
-                self.to_split.update(
-                    {
-                        sample: ["train", "dev", "test"][i]
-                        for sample in samples[split_indices[i] : split_indices[i + 1]]
-                    }
-                )
-
-        elif self.args.split_type == "rule_id":
-            # rule id
-            rules = [reaction["rule_id"] for reaction in metadata_json]
-            rule2count = Counter(rules)
-            samples = sorted(list(set(rules)))
-            np.random.shuffle(samples)
-            samples_cumsum = np.cumsum([rule2count[s] for s in samples])
-            # Find the indices for each quantile
-            split_indices = [
-                np.searchsorted(
-                    samples_cumsum, np.round(q, 3) * samples_cumsum[-1], side="right"
-                )
-                for q in np.cumsum(split_probs)
-            ]
-            split_indices[-1] = len(samples)
-            split_indices = np.concatenate([[0], split_indices])
-            for i in range(len(split_indices) - 1):
-                self.to_split.update(
-                    {
-                        sample: ["train", "dev", "test"][i]
-                        for sample in samples[split_indices[i] : split_indices[i + 1]]
-                    }
-                )
-
-        elif self.args.split_type == "ec_hold_out":
-            unique_products = set(
-                [
-                    ".".join(sample["products"])
-                    for sample in self.metadata_json
-                    if sample["ec"].split(".")[0] != str(self.args.held_out_ec_num)
-                ]
+        # rule id
+        rules = [reaction["rule_id"] for reaction in metadata_json]
+        rule2count = Counter(rules)
+        samples = sorted(list(set(rules)))
+        np.random.shuffle(samples)
+        samples_cumsum = np.cumsum([rule2count[s] for s in samples])
+        # Find the indices for each quantile
+        split_indices = [
+            np.searchsorted(
+                samples_cumsum, np.round(q, 3) * samples_cumsum[-1], side="right"
             )
-            # ! ENSURE REPRODUCIBLE SETS FOR SAME SEED
-            unique_products = sorted(list(unique_products))
-            np.random.shuffle(unique_products)
-
-            dev_probs = split_probs[1] / (split_probs[0] + split_probs[1])
-            train_probs = split_probs[0] / (split_probs[0] + split_probs[1])
-            if not self.args.split_multiproduct_samples:
-                products2split = {
-                    p: np.random.choice(["train", "dev"], p=[train_probs, dev_probs])
-                    for p in unique_products
+            for q in np.cumsum(split_probs)
+        ]
+        split_indices[-1] = len(samples)
+        split_indices = np.concatenate([[0], split_indices])
+        for i in range(len(split_indices) - 1):
+            self.to_split.update(
+                {
+                    sample: ["train", "dev", "test"][i]
+                    for sample in samples[split_indices[i] : split_indices[i + 1]]
                 }
-            else:
-                products2split = {}
-                for p_list in unique_products:
-                    for p in p_list.split("."):
-                        products2split[p] = np.random.choice(
-                            ["train", "dev"], p=[train_probs, dev_probs]
-                        )
-
-            for sample in self.metadata_json:
-                ec = sample["ec"]
-                rkey = (
-                    "mapped_reactants"
-                    if "mapped_reactants" in self.metadata_json[0]
-                    else "reactants"
-                )
-                pkey = (
-                    "mapped_products"
-                    if "mapped_products" in self.metadata_json[0]
-                    else "products"
-                )
-                reactants = sorted([s for s in sample[rkey] if s != "[H+]"])
-                products = sorted([s for s in sample[pkey] if s != "[H+]"])
-                products = [p for p in products if p not in reactants]
-
-                if self.args.topk_byproducts_to_remove is not None:
-                    products = [p for p in products if p not in self.common_byproducts]
-
-                reaction_string = "{}>>{}".format(
-                    ".".join(reactants), ".".join(products)
-                )
-
-                if self.args.version == "1":
-                    alluniprots = self.ec2uniprot.get(ec, [])
-                    protein_refs = []
-                elif self.args.version == "2":
-                    protein_refs = eval(sample["protein_refs"])
-                    alluniprots = protein_refs
-                    if (len(alluniprots) == 0) and self.args.sample_uniprot_per_ec:
-                        alluniprots = self.ec2uniprot.get(ec, [])
-
-                if (
-                    self.args.create_sample_per_sequence
-                    or self.args.sample_uniprot_per_ec
-                ):
-                    valid_uniprots = []
-                    for uniprot in alluniprots:
-                        if self.args.split_multiproduct_samples:
-                            for product_id, p in enumerate(products):
-                                psample = copy.deepcopy(sample)
-                                psample["products"] = [p]
-                                # psample["sample_id"] += f"_{product_id}"
-                                preaction_string = "{}>>{}".format(
-                                    ".".join(psample["reactants"]), p
-                                )
-                                # uniprot = psample["uniprot_id"]
-                                punique_sample_content = f"{preaction_string}{uniprot}{psample.get('organism', '')}"
-                                phashed_sample_content = hashlib.sha256(
-                                    punique_sample_content.encode("utf-8")
-                                ).hexdigest()
-                                psample["hash_sample_id"] = phashed_sample_content
-                                if str(self.args.held_out_ec_num) == ec:
-                                    self.to_split[psample["hash_sample_id"]] = "test"
-                                else:
-                                    self.to_split[psample["hash_sample_id"]] = (
-                                        products2split[p]
-                                    )
-
-                        else:
-                            unique_sample_content = f"{reaction_string}{uniprot}{sample.get('organism', '')}"
-                            hashed_sample_content = hashlib.sha256(
-                                unique_sample_content.encode("utf-8")
-                            ).hexdigest()
-                            sample["hash_sample_id"] = hashed_sample_content
-                            if sample["ec"].split(".")[0] == str(
-                                self.args.held_out_ec_num
-                            ):
-                                self.to_split[sample["hash_sample_id"]] = "test"
-                            else:
-                                self.to_split[sample["hash_sample_id"]] = (
-                                    products2split[".".join(sample["products"])]
-                                )
-
-        # random splitting
-        elif self.args.split_type == "random":
-            for sample in self.metadata_json:
-                reaction_string = (
-                    ".".join(sample["reactants"]) + ">>" + ".".join(sample["products"])
-                )
-                self.to_split.update(
-                    {
-                        reaction_string: np.random.choice(
-                            ["train", "dev", "test"], p=split_probs
-                        )
-                    }
-                )
-        elif self.args.split_type == "scaffold":
-            # split based on scaffold
-            self.scaffold_split(metadata_json, split_probs, seed)
-        else:
-            raise ValueError("Split type not supported")
-
-    def scaffold_split(self, meta: List[dict], split_probs: List[float], seed):
-        scaffold_to_indices = defaultdict(list)
-        for m_i, m in enumerate(meta):
-            scaffold = generate_scaffold(m["smiles"])
-            scaffold_to_indices[scaffold].append(m_i)
-
-        # Split
-        train_size, val_size, test_size = (
-            split_probs[0] * len(meta),
-            split_probs[1] * len(meta),
-            split_probs[2] * len(meta),
-        )
-        train, val, test = [], [], []
-        train_scaffold_count, val_scaffold_count, test_scaffold_count = 0, 0, 0
-
-        # Seed randomness
-        random = Random(seed)
-
-        if self.args.scaffold_balanced:  # Put stuff that's bigger than half the val/test size into train, rest just order randomly
-            index_sets = list(scaffold_to_indices.values())
-            big_index_sets = []
-            small_index_sets = []
-            for index_set in index_sets:
-                if len(index_set) > val_size / 2 or len(index_set) > test_size / 2:
-                    big_index_sets.append(index_set)
-                else:
-                    small_index_sets.append(index_set)
-            random.seed(seed)
-            random.shuffle(big_index_sets)
-            random.shuffle(small_index_sets)
-            index_sets = big_index_sets + small_index_sets
-        else:  # Sort from largest to smallest scaffold sets
-            index_sets = sorted(
-                list(scaffold_to_indices.values()),
-                key=lambda index_set: len(index_set),
-                reverse=True,
             )
 
-        for index_set in index_sets:
-            if len(train) + len(index_set) <= train_size:
-                train += index_set
-                train_scaffold_count += 1
-            elif len(val) + len(index_set) <= val_size:
-                val += index_set
-                val_scaffold_count += 1
-            else:
-                test += index_set
-                test_scaffold_count += 1
-
-        for idx_list, split in [(train, "train"), (val, "dev"), (test, "test")]:
-            for idx in idx_list:
-                meta[idx]["split"] = split
-                if (
-                    meta[idx]["smiles"] in self.to_split
-                    and self.to_split[meta[idx]["smiles"]] != split
-                ):
-                    raise Exception("Smile exists in to_split but with different split")
-                self.to_split[meta[idx]["smiles"]] = split
-
     def get_split_group_dataset(
         self, processed_dataset, split_group: Literal["train", "dev", "test"]
     ) -> List[dict]:
         dataset = []
         for sample in processed_dataset:
             # check right split
-            if self.args.split_type == "ec":
-                split_ec = sample[f"ec{self.args.ec_level + 1}"]
-                if self.to_split[split_ec] != split_group:
-                    continue
-
-            elif self.args.split_type == "rule_id":
-                if self.to_split[sample["rule_id"]] != split_group:
-                    continue
-
-            elif self.args.split_type == "mmseqs":
-                cluster = self.uniprot2cluster.get(sample["protein_id"], None)
-                if (cluster is None) or (self.to_split[cluster] != split_group):
-                    continue
-            elif (
-                self.args.split_type == "mmseqs_precomputed"
-                or self.args.split_type == "scaffold"
-            ):
-                if sample["split"] != split_group:
-                    continue
-            elif self.args.split_type in ["product"]:
-                products = ".".join(sample["products"])
-                if self.to_split[products] != split_group:
-                    continue
-
-            elif self.args.split_type == "sequence":
-                uniprot = sample["protein_id"]
-                if self.to_split[uniprot] != split_group:
-                    continue
-
-            elif self.args.split_type == "ec_hold_out":
-                sample_id = sample["hash_sample_id"]
-                if self.to_split[sample_id] != split_group:
-                    continue
-
-            elif sample["split"] is not None:
-                if sample["split"] != split_group:
-                    continue
+            if self.to_split[sample["rule_id"]] != split_group:
+                continue
             dataset.append(sample)
         return dataset
 
     def post_process(self, args):
         # add all possible products
         reaction_to_products = defaultdict(set)
         for sample in self.dataset:
@@ -835,31 +519,19 @@
     @staticmethod
     def add_args(parser) -> None:
         """Add class specific args
 
         Args:
             parser (argparse.ArgumentParser): argument parser
         """
-        super(EnzymeMap, EnzymeMap).add_args(parser)
-        parser.add_argument(
-            "--held_out_ec_num",
-            type=int,
-            default=None,
-            help="EC number to hold out",
-        )
-        parser.add_argument(
-            "--uniprot2cluster_path",
-            type=str,
-            default="/home/datasets/EnzymeMap/mmseq_clusters_updated.p",
-            help="path to uniprot2cluster pickle",
-        )
+        AbstractDataset.add_args(parser)
         parser.add_argument(
             "--esm_dir",
             type=str,
-            default="/home/snapshots/metabolomics/esm2/checkpoints/esm2_t33_650M_UR50D.pt",
+            default="/home/esm2/checkpoints/esm2_t33_650M_UR50D.pt",
             help="directory to load esm model from",
         )
         parser.add_argument(
             "--use_protein_graphs",
             action="store_true",
             default=False,
             help="whether to use and generate protein graphs",
@@ -946,26 +618,14 @@
         parser.add_argument(
             "--topk_byproducts_to_remove",
             type=int,
             default=None,
             help="remove common byproducts",
         )
         parser.add_argument(
-            "--use_pesto_scores",
-            action="store_true",
-            default=False,
-            help="use pesto scores",
-        )
-        parser.add_argument(
-            "--pesto_scores_directory",
-            type=str,
-            default="/home/datasets/ECReact/pesto_ligands",
-            help="load pesto scores from directory predictions",
-        )
-        parser.add_argument(
             "--create_sample_per_sequence",
             action="store_true",
             default=False,
             help="create a sample for each protein sequence annotated for given EC",
         )
         parser.add_argument(
             "--sample_uniprot_per_ec",
@@ -982,56 +642,32 @@
         parser.add_argument(
             "--min_reaction_quality",
             type=float,
             default=-1,
             help="minimum threshold to use for filtering reactions based on quality score",
         )
         parser.add_argument(
-            "--load_wln_cache_in_dataset",
-            action="store_true",
-            default=False,
-            help="load cache for wln in getitem",
-        )
-        parser.add_argument(
             "--split_multiproduct_samples",
             action="store_true",
             default=False,
             help="split products into different samples",
         )
         parser.add_argument(
             "--use_one_hot_mol_features",
             action="store_true",
             default=False,
             help="encode node and edge features of molecule as one-hot",
         )
         parser.add_argument(
-            "--scaffold_balanced",
-            action="store_true",
-            default=False,
-            help="balance the scaffold sets",
-        )
-        parser.add_argument(
             "--version",
             type=str,
             default="1",
             help="enzyme map version number",
         )
         parser.add_argument(
-            "--convert_graph_to_smiles",
-            action="store_true",
-            default=False,
-            help="for sequence based methods",
-        )
-        parser.add_argument(
-            "--reaction_to_products_dir",
-            type=str,
-            default=None,
-            help="cache for post process step",
-        )
-        parser.add_argument(
             "--remove_duplicate_reactions",
             action="store_true",
             default=False,
             help="remove duplicates",
         )
 
     @property
@@ -1059,29 +695,14 @@
         """
         return statement
 
 
 @register_object("enzymemap_reaction_graph", "dataset")
 class EnzymeMapGraph(EnzymeMap):
     def post_process(self, args):
-        def make_reaction_to_products():
-            reaction_to_products = defaultdict(set)
-            if args.create_sample_per_sequence:
-                key = lambda sample: f"{sample['ec']}{'.'.join(sample['reactants'])}"
-            else:
-                key = lambda sample: ".".join(sample["reactants"])
-            for sample in tqdm(self.dataset, desc="post-processing", ncols=100):
-                reaction_to_products[key(sample)].add(
-                    (
-                        ".".join(sample["products"]),
-                        stringify_sets(sorted(sample["bond_changes"])),
-                    )
-                )
-            return reaction_to_products
-
         # set ec levels to id for use in modeling
         ecs = set(d["ec"] for d in self.dataset)
         ecs = [e.split(".") for e in ecs]
         args.ec_levels = {}
         for level in range(1, 5, 1):
             unique_classes = sorted(list(set(".".join(ec[:level]) for ec in ecs)))
             args.ec_levels[str(level)] = {c: i for i, c in enumerate(unique_classes)}
@@ -1419,21 +1040,14 @@
                     yvec = torch.zeros(len(v))
                     yvec[v[".".join(split_ec[: int(k)])]] = 1
                     item[f"ec{k}"] = yvec
 
             if self.args.load_wln_cache_in_dataset:
                 item["product_candidates"] = self.cache.get(rowid)
 
-            if self.args.use_pesto_scores:
-                scores = self.get_pesto_scores(item["protein_id"])
-                if (scores is None) or (scores.shape[0] != len(item["sequence"])):
-                    # make all zeros of length sequence
-                    scores = torch.zeros(len(item["sequence"]))
-                item["sequence_annotation"] = scores
-
             if self.args.use_protein_graphs:
                 if self.args.cache_path:
                     try:
                         graph_path_cache = os.path.join(
                             self.args.cache_path,
                             f"{item['uniprot_id']}_graph.pt",
                         )
```

### Comparing `clipzyme-0.0.4/clipzyme/datasets/reaction.py` & `clipzyme-0.0.5/clipzyme/datasets/reaction.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,56 +1,86 @@
 import os
+import argparse
 from typing import List, Union
 from rich import print
 from tqdm import tqdm
 import copy
 import pandas as pd
 import Bio
 import Bio.PDB
 from Bio.Data.IUPACData import protein_letters_3to1
 import torch
 from torch.utils import data
 from torch_geometric.data import Data as pygData
 from esm import pretrained
 from clipzyme.utils.registry import register_object
 from clipzyme.utils.wln_processing import get_bond_changes
-from clipzyme.utils.pyg import from_mapped_smiles
+from clipzyme.utils.screening import process_mapped_reaction
 from clipzyme.utils.protein_utils import (
     read_structure_file,
     filter_resolution,
     build_graph,
     compute_graph_edges,
     compute_node_embedding,
 )
 
 
 protein_letters_3to1.update({k.upper(): v for k, v in protein_letters_3to1.items()})
 
 
 @register_object("reactions_dataset", "dataset")
 class ReactionDataset(data.Dataset):
-    def __init__(self, args) -> None:
+    def __init__(
+        self,
+        args: argparse.Namespace = None,
+        dataset_file_path: str = None,
+        esm_dir: str = None,
+        protein_cache_dir: str = None,
+        use_as_protein_encoder: bool = False,
+        use_as_reaction_encoder: bool = False,
+    ) -> None:
         """
         Create a dataset of reactions and proteins from a CSV file
 
         Parameters
         ----------
         args: argparse.Namespace
+            Arguments from command line
+        dataset_file_path: str
+            Path to CSV file with headers ['reaction', 'sequence', 'protein_id', 'cif']
+        esm_dir: str
+            Path to ESM model directory
+        protein_cache_dir: str
+            Directory to save/load protein graphs
+        use_as_protein_encoder: bool
+            Use dataset as protein encoder and do not consider reactions in data filtering
+        use_as_reaction_encoder: bool
+            Use dataset as reaction encoder and do not consider proteins in data filtering
 
         Raises
         ------
         ValueError
             If CSV file does not have headers ['reaction', 'sequence', 'protein_id', 'cif']
         """
         super(ReactionDataset, self).__init__()
-        # check if csv file has correct headers
-        csv_path = args.dataset_file_path
-        esm_dir = args.esm_dir
-        protein_cache_dir = args.protein_cache_dir
 
+        if args is None:
+            csv_path = dataset_file_path
+            esm_dir = esm_dir
+            protein_cache_dir = protein_cache_dir
+            self.use_as_protein_encoder = use_as_protein_encoder
+            self.use_as_reaction_encoder = use_as_reaction_encoder
+        else:
+            csv_path = args.dataset_file_path
+            esm_dir = args.esm_dir
+            protein_cache_dir = args.protein_cache_dir
+            self.use_as_protein_encoder = args.use_as_protein_encoder
+            self.use_as_reaction_encoder = args.use_as_reaction_encoder
+
+        # check if csv file has correct headers
         with open(csv_path, "r") as f:
             headers = f.readline().strip().split(",")
             if (
                 "reaction" not in headers
                 or "protein_id" not in headers
                 or "sequence" not in headers
                 or "cif" not in headers
@@ -133,29 +163,33 @@
             Sample dictionary from dataset
 
         Returns
         -------
         bool
             True if sample should be skipped
         """
-        # if sequence is unknown
-        sequence = sample["sequence"]
-        if len(sequence) == 0:
-            return True
-
-        if len(sequence) > 650:
-            return True
-
-        # check if cif file exists
-        if not os.path.exists(sample["cif_path"]):
-            return True
-
-        # if no bond changes
-        if len(sample["bond_changes"]) == 0:
-            return True
+        # if dataset is not used only as reaction encoder
+        if not self.use_as_reaction_encoder:
+            # if sequence is unknown
+            sequence = sample["sequence"]
+            if len(sequence) == 0:
+                return True
+
+            if len(sequence) > 650:
+                return True
+
+            # check if cif file exists
+            if not os.path.exists(sample["cif_path"]):
+                return True
+
+        # if dataset is not used only as protein encoder
+        if not self.use_as_protein_encoder:
+            # if no bond changes
+            if len(sample["bond_changes"]) == 0:
+                return True
 
         return False
 
     def create_protein_graph(self, sample: dict) -> Union[pygData, None]:
         """
         Create pyg protein graph from CIF file
 
@@ -198,15 +232,15 @@
                 data.center = center
 
             sequence = sample["sequence"]
             data.structure_sequence = sequence
 
             node_embeddings_args = {
                 "model": self.esm_model,
-                "model_location": self.esm_dir,
+                "model_location": "",
                 "alphabet": self.alphabet,
                 "batch_converter": self.batch_converter,
             }
             node_embedding = compute_node_embedding(data, **node_embeddings_args)
             # Fix sequence length mismatches
             if len(data["receptor"].seq) != node_embedding.shape[0]:
                 print("Computing seq embedding for mismatched seq length")
@@ -264,41 +298,23 @@
             return None
 
     def __len__(self):
         return len(self.dataset)
 
     def __getitem__(self, index):
         sample = self.dataset[index]
+        sample_id = sample["sample_id"]
 
         try:
-            reactants, products = (
-                copy.deepcopy(sample["reactants"]),
-                copy.deepcopy(sample["products"]),
+            reactants, products = process_mapped_reaction(
+                sample["reaction"],
+                sample["bond_changes"],
             )
             protein_id = sample["protein_id"]
 
-            reactants, atom_map2new_index = from_mapped_smiles(
-                ".".join(reactants),
-                encode_no_edge=True,
-                use_one_hot_encoding=self.args.use_one_hot_mol_features,
-            )
-            products, _ = from_mapped_smiles(
-                ".".join(products),
-                encode_no_edge=True,
-                use_one_hot_encoding=self.args.use_one_hot_mol_features,
-            )
-
-            bond_changes = [
-                (atom_map2new_index[int(u)], atom_map2new_index[int(v)], btype)
-                for u, v, btype in sample["bond_changes"]
-            ]
-            bond_changes = [(min(x, y), max(x, y), t) for x, y, t in bond_changes]
-            reactants.bond_changes = bond_changes
-            sample_id = sample["sample_id"]
-
             item = {
                 "reactants": reactants,
                 "products": products,
                 "protein_id": protein_id,
                 "sample_id": sample_id,
                 "cif_path": sample["cif_path"],
                 "sequence": sample["sequence"],
```

### Comparing `clipzyme-0.0.4/clipzyme/learning/losses/basic.py` & `clipzyme-0.0.5/clipzyme/learning/losses/basic.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.4/clipzyme/learning/losses/contrastive.py` & `clipzyme-0.0.5/clipzyme/learning/losses/contrastive.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.4/clipzyme/learning/metrics/basic.py` & `clipzyme-0.0.5/clipzyme/learning/metrics/basic.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.4/clipzyme/learning/metrics/representation.py` & `clipzyme-0.0.5/clipzyme/learning/metrics/representation.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.4/clipzyme/learning/optimizers/basic.py` & `clipzyme-0.0.5/clipzyme/learning/optimizers/basic.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.4/clipzyme/learning/schedulers/basic.py` & `clipzyme-0.0.5/clipzyme/learning/schedulers/basic.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.4/clipzyme/learning/schedulers/warmup.py` & `clipzyme-0.0.5/clipzyme/learning/schedulers/warmup.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.4/clipzyme/lightning/base.py` & `clipzyme-0.0.5/clipzyme/lightning/base.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.4/clipzyme/lightning/clipzyme.py` & `clipzyme-0.0.5/clipzyme/lightning/clipzyme.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,24 @@
-from typing import Optional, List, NamedTuple
+from typing import Optional, List, NamedTuple, Union
 from io import BytesIO
+import shutil
 from zipfile import ZipFile
 from urllib.request import urlopen
 from pathlib import Path
 import os
 import torch
 from rich import print
 import pytorch_lightning as pl
 import argparse
 from clipzyme.models.protmol import EnzymeReactionCLIP
+from clipzyme.utils.screening import process_mapped_reaction
+from clipzyme.utils.protein_utils import create_protein_graph
+from clipzyme.utils.loading import default_collate
 
-CHECKPOINT_URL = "https://github.com/pgmikhael/clipzyme/releases/download/v1.0.0/clipzyme_checkpoints.zip"  # TODO: Update this
+CHECKPOINT_URL = "https://github.com/pgmikhael/clipzyme/releases/download/v0.0.5/clipzyme_files.zip"  # TODO: Update this
 
 
 def download_and_extract(remote_model_url: str, local_model_dir) -> List[str]:
     resp = urlopen(remote_model_url)
     os.makedirs(local_model_dir, exist_ok=True)
     with ZipFile(BytesIO(resp.read())) as zip_file:
         all_files_and_dirs = zip_file.namelist()
@@ -47,82 +51,91 @@
     return model_path
 
 
 class CLIPZymeOutput(NamedTuple):
     scores: torch.Tensor
     protein_hiddens: torch.Tensor
     reaction_hiddens: torch.Tensor
+    sample_ids: List[str]
 
 
 class CLIPZyme(pl.LightningModule):
-    def __init__(self, args: argparse.Namespace, device: Optional[str] = None) -> None:
+    def __init__(
+        self,
+        args: argparse.Namespace = None,
+        checkpoint_path: str = None,
+        device: Optional[str] = None,
+    ) -> None:
         """
         Initialize a trained clipzyme model for inference.
 
         Parameters
         ----------
+        args: argparse.Namespace
+            Arguments from command line.
         checkpoint_path: str
             Path to a clipzyme checkpoint.
         device: str
             If provided, will run inference using this device.
             By default uses GPU, if available.
         """
-        checkpoint_path = args.checkpoint_path
+        super(CLIPZyme, self).__init__()
+        if args is not None:
+            checkpoint_path = args.checkpoint_path
         # Check if path exists
         if (checkpoint_path is None) or (not os.path.exists(checkpoint_path)):
             try:
                 # download model
                 print(f"Model checkpoint not found at {checkpoint_path}")
                 checkpoint_path = download_model(checkpoint_path)
             except Exception as e:
                 raise FileNotFoundError(
                     f"Model checkpoint not found at {checkpoint_path} and failed to download model. {e}"
                 )
 
-        # Set device
-        if device is not None:
-            self.device = device
-        elif self.device is not None:  # set in lightning module
-            pass
-        else:
-            self.device = "cuda" if torch.cuda.is_available() else "cpu"
-
         # Load model
-        self.model = self.load_model(checkpoint_path)
+        self.model = self.load_model(checkpoint_path, args)
 
         # prep directories
         self.prepare_directories(args)
 
+        # Set device
+        if device is not None:
+            self.device = device
+            self.model = self.model.to(self.device)
+
     def prepare_directories(self, args: argparse.Namespace) -> None:
         """
         Prepare directories for saving hiddens and predictions.
 
         Parameters
         ----------
         args : argparse.Namespace
             Arguments from command line.
         """
-        self.save_hiddens = args.save_hiddens
-        self.save_predictions = args.save_predictions
-        if args.save_hiddens or args.save_predictions:
+        self.save_hiddens = getattr(args, "save_hiddens", False)
+        self.save_predictions = getattr(args, "save_predictions", False)
+        if self.save_hiddens or self.save_predictions:
             checkpoint_path = Path(args.checkpoint_path)
             dataset_path = Path(args.dataset_file_path)
             hiddens_dir = os.path.join(
                 args.inference_dir, checkpoint_path.stem, dataset_path.stem
             )
             os.makedirs(hiddens_dir, exist_ok=True)
             self.hiddens_dir = Path(hiddens_dir)
 
-        if args.save_predictions:
+        if self.save_predictions:
             self.predictions_dir = os.path.join(hiddens_dir, "predictions")
             os.makedirs(self.predictions_dir, exist_ok=True)
             self.predictions_dir = Path(self.predictions_dir)
             self.predictions_path = os.path.join(self.hiddens_dir, "predictions.csv")
 
-    def load_model(self, path: str) -> EnzymeReactionCLIP:
+    def load_model(
+        self, path: str, screen_args: argparse.Namespace
+    ) -> EnzymeReactionCLIP:
         """
         Load model from path.
 
         Parameters
         ----------
         path : str
             Path to a clipzyme model checkpoint.
@@ -130,48 +143,44 @@
         Returns
         -------
         model
             Pretrained clipzyme model
         """
         # Load checkpoint
         checkpoint = torch.load(path, map_location="cpu")
-        args = checkpoint["args"]
+        args = checkpoint["hyper_parameters"]["args"]
+        # set relevant args
+        for key in ["use_as_protein_encoder", "use_as_reaction_encoder"]:
+            setattr(args, key, getattr(screen_args, key, False))
+            setattr(self, key, getattr(screen_args, key, False))
         model = EnzymeReactionCLIP(args)
 
         # Remove model from param names
         state_dict = {k[6:]: v for k, v in checkpoint["state_dict"].items()}
         model.load_state_dict(state_dict)  # type: ignore
-        if self.device == "cuda":
-            model.to("cuda")
 
         # Set eval
         model.eval()
-        print(f"Loaded model from {path}")
+        print(f"[bold] Loaded model from {path}")
         return model
 
     def forward(
         self,
         batch,
         batch_idx: int = 0,
-        extract_protein_features: bool = False,
-        extract_reaction_features: bool = False,
     ) -> CLIPZymeOutput:
         """
         Forward pass of the model.
 
         Parameters
         ----------
         batch : dict
             Batch of data.
         batch_idx : int, optional
             batch id, by default 0
-        extract_protein_features : bool, optional
-            whether to return protein features, by default False
-        extract_reaction_features : bool, optional
-            whether to return reaction features, by default False
 
         Returns
         -------
         CLIPZymeOutput
             Output of the model.
         """
         reaction_scores = None
@@ -187,26 +196,19 @@
         # want paired scores
         if not (self.use_as_protein_encoder or self.use_as_reaction_encoder):
             reaction_hiddens = model_output["substrate_hiddens"]
             protein_hiddens = model_output["protein_hiddens"]
             reaction_scores = torch.einsum(
                 "bx,bx->b", reaction_hiddens, protein_hiddens
             )
-        if extract_protein_features:
-            protein_hiddens = (
-                model_output["hidden"]
-                if self.use_as_protein_encoder
-                else model_output["protein_hiddens"]
-            )
-        if extract_reaction_features:
-            reaction_hiddens = (
-                model_output["hidden"]
-                if self.use_as_protein_encoder
-                else model_output["substrate_hiddens"]
-            )
+
+        if self.use_as_protein_encoder:
+            protein_hiddens = model_output["hidden"]
+        if self.use_as_reaction_encoder:
+            reaction_hiddens = model_output["hidden"]
 
         output = CLIPZymeOutput(
             scores=reaction_scores,
             protein_hiddens=protein_hiddens,
             reaction_hiddens=reaction_hiddens,
             sample_ids=batch["sample_id"],
         )
@@ -228,96 +230,163 @@
         -------
         ClipZymeOutput
             Output of the model.
         """
         output = self.forward(batch, batch_idx)
         if self.save_hiddens or self.save_predictions:
             self.save_outputs(output)
-        return output
+        return
 
     def on_test_epoch_end(self) -> None:
         self.clean_up()
 
     def save_outputs(self, outputs: CLIPZymeOutput) -> None:
         """
         Save outputs to disk.
 
         Parameters
         ----------
         outputs : ClipZymeOutput
             Output of the model.
         """
-        if outputs.protein_hiddens is not None:
-            protein_hiddens = outputs.protein_hiddens.cpu()
-            for idx, protein_hidden in enumerate(protein_hiddens):
-                predictions_filename = self.hiddens_dir.joinpath(
-                    f"sample_{outputs.sample_ids[idx]}.protein.pt"
-                )
-                torch.save(protein_hidden, predictions_filename)
+        if self.save_hiddens:
+            if outputs.protein_hiddens is not None:
+                protein_hiddens = outputs.protein_hiddens.cpu()
+                for idx, protein_hidden in enumerate(protein_hiddens):
+                    predictions_filename = self.hiddens_dir.joinpath(
+                        f"sample_{outputs.sample_ids[idx]}.protein.pt"
+                    )
+                    torch.save(protein_hidden, predictions_filename)
+
+            if outputs.reaction_hiddens is not None:
+                reaction_hiddens = outputs.reaction_hiddens.cpu()
+                for idx, reaction_hidden in enumerate(reaction_hiddens):
+                    predictions_filename = self.hiddens_dir.joinpath(
+                        f"sample_{outputs.sample_ids[idx]}.reaction.pt"
+                    )
+                    torch.save(reaction_hidden, predictions_filename)
 
-        if outputs.reaction_hidden is not None:
-            reaction_hiddens = outputs.reaction_hidden.cpu()
-            for idx, reaction_hidden in enumerate(reaction_hiddens):
-                predictions_filename = self.hiddens_dir.joinpath(
-                    f"sample_{outputs.sample_ids[idx]}.reaction.pt"
-                )
-                torch.save(reaction_hidden, predictions_filename)
-
-        if outputs.scores is not None:
+        if self.save_predictions:
             scores = outputs.scores.cpu()
             for idx, score in enumerate(scores):
                 predictions_filename = self.predictions_dir.joinpath(
                     f"sample_{outputs.sample_ids[idx]}.score.pt"
                 )
                 torch.save(score.item(), predictions_filename)
 
-    def extract_protein_features(self, batch: dict) -> torch.Tensor:
+    def extract_protein_features(
+        self,
+        batch: dict = None,
+        cif_path: Union[str, List[str]] = None,
+        esm_dir: str = None,
+    ) -> torch.Tensor:
         """
         Extract protein features from model.
 
         Parameters
         ----------
         batch : dict
             Batch of data.
+        cif_path : Union[str, List[str]], optional
+            Path to CIF file, by default None
+        esm_dir : str, optional
+            Path to ESM model (esm2_t33_650M_UR50D), by default None
 
         Returns
         -------
         torch.Tensor
             Protein features.
         """
-        self.use_as_protein_encoder = True
+        self.model.args.use_as_protein_encoder = True
+
+        if cif_path is not None:
+            assert (
+                esm_dir is not None
+            ), "If manually extracting protein embedding, then `esm_dir` must be provided"
+            if isinstance(cif_path, str):
+                cif_path = [cif_path]
+            protein_graphs = [
+                create_protein_graph(
+                    cif_path=cpath,
+                    esm_path=os.path.join(esm_dir, "esm2_t33_650M_UR50D.pt"),
+                )
+                for cpath in cif_path
+            ]
+            batch = default_collate([{"graph": g} for g in protein_graphs])
+
         model_output = self.model(batch)
-        return model_output["protein_hiddens"]
+        return model_output["hidden"]
 
-    def extract_reaction_features(self, batch: dict) -> torch.Tensor:
+    def extract_reaction_features(
+        self, batch: dict = None, reaction: Union[str, List[str]] = None
+    ) -> torch.Tensor:
         """
         Extract reaction features from model.
 
         Parameters
         ----------
         batch : dict
             Batch of data.
+        reaction : Union[str, List[str]], optional
+            Mapped raction string, by default None
 
         Returns
         -------
         torch.Tensor
             Reaction features.
         """
-        self.use_as_reaction_encoder = True
+        self.model.args.use_as_reaction_encoder = True
+        if reaction is not None:
+            if isinstance(reaction, str):
+                reaction = [reaction]
+            reactions = [process_mapped_reaction(rxn) for rxn in reaction]
+            batch = default_collate(
+                [
+                    {
+                        "reactants": rxn[0],
+                        "products": rxn[1],
+                    }
+                    for rxn in reactions
+                ]
+            )
         model_output = self.model(batch)
-        return model_output["substrate_hiddens"]
+
+        return model_output["hidden"]
+
+    def store_in_predictions(self, preds: dict, storage_dict: dict) -> dict:
+        """
+        Store values in predictions.
+
+        Parameters
+        ----------
+        preds : dict
+            prediction dictionary
+        storage_dict : dict
+            dictionary from which to get values
+
+        Returns
+        -------
+        dict
+            updated predictions dictionary
+        """
+        for key, val in storage_dict.items():
+            if torch.is_tensor(val) and val.requires_grad:
+                preds[key] = val.detach()
+            else:
+                preds[key] = val
+        return preds
 
     def clean_up(self):
         """
         Clean up directories after inference.
         """
         if self.save_predictions:
             print("Collecting predictions files")
 
             with open(self.predictions_path, "w") as f:
                 f.write("sample_id,score\n")
                 for score_file in self.predictions_dir.iterdir():
-                    score = torch.load(self.predictions_dir.joinpath(score_file))
-                    f.write(f"{score_file.stem},{score}\n")
+                    score = torch.load(score_file)
+                    f.write(f"{score_file.stem.split('.')[0]},{score}\n")
 
-            self.predictions_dir.rmdir()
+            shutil.rmtree(self.predictions_dir)
         print("Done")
```

### Comparing `clipzyme-0.0.4/clipzyme/loggers/tensorboard.py` & `clipzyme-0.0.5/clipzyme/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.4/clipzyme/loggers/wandb.py` & `clipzyme-0.0.5/clipzyme/loggers/wandb.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.4/clipzyme/models/chemprop.py` & `clipzyme-0.0.5/clipzyme/models/chemprop.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.4/clipzyme/models/classifier.py` & `clipzyme-0.0.5/clipzyme/models/classifier.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.4/clipzyme/models/egnn.py` & `clipzyme-0.0.5/clipzyme/models/egnn.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.4/clipzyme/models/fair_esm.py` & `clipzyme-0.0.5/clipzyme/models/fair_esm.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.4/clipzyme/models/gat.py` & `clipzyme-0.0.5/clipzyme/models/gat.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.4/clipzyme/models/protmol.py` & `clipzyme-0.0.5/clipzyme/models/protmol.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,17 @@
 @register_object("enzyme_reaction_clip", "model")
 class EnzymeReactionCLIP(AbstractModel):
     def __init__(self, args):
         super(EnzymeReactionCLIP, self).__init__()
         self.args = args
         self.reaction_clip_model_path = copy.copy(args.reaction_clip_model_path)
         self.use_as_protein_encoder = getattr(args, "use_as_protein_encoder", False)
-        self.use_as_mol_encoder = getattr(args, "use_as_mol_encoder", False)
+        self.use_as_mol_encoder = getattr(args, "use_as_mol_encoder", False) or getattr(
+            args, "use_as_reaction_encoder", False
+        )  # keep mol for backward compatibility
         args.train_esm_with_graph = getattr(args, "train_esm_with_graph", False)
 
         if args.reaction_clip_model_path is not None:
             state_dict = torch.load(args.reaction_clip_model_path)
             state_dict_copy = {
                 k.replace("model.", "", 1): v
                 for k, v in state_dict["state_dict"].items()
@@ -196,15 +198,17 @@
             output.update(
                 {
                     "hidden": protein_features,
                 }
             )
             return output
 
-        if getattr(self.args, "use_as_mol_encoder", False):
+        if getattr(self.args, "use_as_mol_encoder", False) or getattr(
+            self.args, "use_as_reaction_encoder", False
+        ):
             substrate_features = self.encode_reaction(batch)
             substrate_features = substrate_features / substrate_features.norm(
                 dim=1, keepdim=True
             )
             output.update(
                 {
                     "hidden": substrate_features,
```

### Comparing `clipzyme-0.0.4/clipzyme/models/seq2seq.py` & `clipzyme-0.0.5/clipzyme/models/seq2seq.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.4/clipzyme/models/wln.py` & `clipzyme-0.0.5/clipzyme/models/wln.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.4/clipzyme/utils/amino_acids.py` & `clipzyme-0.0.5/clipzyme/utils/amino_acids.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.4/clipzyme/utils/callbacks.py` & `clipzyme-0.0.5/clipzyme/utils/callbacks.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.4/clipzyme/utils/classes.py` & `clipzyme-0.0.5/clipzyme/utils/classes.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.4/clipzyme/utils/colabfold_msa.py` & `clipzyme-0.0.5/clipzyme/utils/colabfold_msa.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.4/clipzyme/utils/loading.py` & `clipzyme-0.0.5/clipzyme/utils/loading.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.4/clipzyme/utils/parsing.py` & `clipzyme-0.0.5/clipzyme/utils/parsing.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.4/clipzyme/utils/protein_utils.py` & `clipzyme-0.0.5/clipzyme/utils/protein_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,22 @@
-from torch_cluster import knn_graph
-from torch_geometric.data import HeteroData
-from rich import print
-from Bio.Data.IUPACData import protein_letters_3to1
-from esm import FastaBatchedDataset, pretrained
+from typing import Union
+import os, hashlib
 from collections import defaultdict
 from tqdm import tqdm
+from rich import print
+import Bio
+import Bio.PDB
+from Bio.Data.IUPACData import protein_letters_3to1
 import torch
-import os, sys, pickle, hashlib
+from torch_geometric.data import Data as pygData
+from torch_geometric.data import HeteroData
+from torch_cluster import knn_graph
+from esm import FastaBatchedDataset, pretrained
+
+protein_letters_3to1.update({k.upper(): v for k, v in protein_letters_3to1.items()})
 
 
 # Read PDB and CIF files
 def read_structure_file(protein_parser, raw_path, sample_id):
     structure = protein_parser.get_structure(sample_id, raw_path)
     all_res, all_pos, all_atom = [], [], []
     for chains in structure:
@@ -283,21 +289,101 @@
             sequence = seq
         else:
             sequence += ":" + seq
 
     return sequence
 
 
-# Process SDF files and SMILES
-# def read_ligand_files():
-#     pass
-# # add ligand graphs or other protein graphs to existing graph
-# def combine_graphs():
-#     pass
-# - Parallel processing
-# #     - Complex generation
-# #     - ESM embeddings
-# #     - AF downloading
-# - Can compute intelligent splits
-#     - mmseqs split
-#     - random split
-#     - easy to add additional splitting
+def create_protein_graph(cif_path: str, esm_path: str) -> Union[pygData, None]:
+    """
+    Create pyg protein graph from CIF file
+
+    Parameters
+    ----------
+    cif_path : str
+        Path to CIF file
+    esm_path : str
+        Path to ESM model (esm2_t33_650M_UR50D.pt)
+
+    Returns
+    -------
+    data
+        pygData object with protein graph
+    """
+    assert esm_path.endswith(
+        "esm2_t33_650M_UR50D.pt"
+    ), "ESM model filename must end with esm2_t33_650M_UR50D.pt"
+    esm_model, alphabet = pretrained.load_model_and_alphabet(esm_path)
+    batch_converter = alphabet.get_batch_converter()
+
+    try:
+        raw_path = cif_path
+        sample_id = "proteinX"
+        protein_parser = Bio.PDB.MMCIFParser()
+        protein_resolution = "residue"
+        graph_edge_args = {"knn_size": 10}
+        center_protein = True
+
+        # parse pdb
+        all_res, all_atom, all_pos = read_structure_file(
+            protein_parser, raw_path, sample_id
+        )
+        # filter resolution of protein (backbone, atomic, etc.)
+        atom_names, seq, pos = filter_resolution(
+            all_res,
+            all_atom,
+            all_pos,
+            protein_resolution=protein_resolution,
+        )
+        # generate graph
+        data = build_graph(atom_names, seq, pos, sample_id)
+        # kNN graph
+        data = compute_graph_edges(data, **graph_edge_args)
+        if center_protein:
+            center = data["receptor"].pos.mean(dim=0, keepdim=True)
+            data["receptor"].pos = data["receptor"].pos - center
+            data.center = center
+
+        # get sequence
+        AA_seq = ""
+        for char in seq:
+            AA_seq += protein_letters_3to1[char]
+
+        data.structure_sequence = AA_seq
+
+        node_embeddings_args = {
+            "model": esm_model,
+            "model_location": "",
+            "alphabet": alphabet,
+            "batch_converter": batch_converter,
+        }
+
+        # compute embeddings
+        data["receptor"].x = compute_node_embedding(data, **node_embeddings_args)
+
+        if len(data["receptor"].seq) != data["receptor"].x.shape[0]:
+            return None
+
+        if hasattr(data, "x") and not hasattr(data["receptor"], "x"):
+            data["receptor"].x = data.x
+
+        if not hasattr(data, "structure_sequence"):
+            data.structure_sequence = "".join(
+                [protein_letters_3to1[char] for char in data["receptor"].seq]
+            )
+
+        coors = data["receptor"].pos
+        feats = data["receptor"].x
+        edge_index = data["receptor", "contact", "receptor"].edge_index
+        assert (
+            coors.shape[0] == feats.shape[0]
+        ), f"Number of nodes do not match between coors ({coors.shape[0]}) and feats ({feats.shape[0]})"
+
+        assert (
+            max(edge_index[0]) < coors.shape[0] and max(edge_index[1]) < coors.shape[0]
+        ), "Edge index contains node indices not present in coors"
+
+        return data
+
+    except Exception as e:
+        print(f"Could not create protein graph because of the exception: {e}")
+        return None
```

### Comparing `clipzyme-0.0.4/clipzyme/utils/proteins.py` & `clipzyme-0.0.5/clipzyme/utils/proteins.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.4/clipzyme/utils/pyg.py` & `clipzyme-0.0.5/clipzyme/utils/pyg.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.4/clipzyme/utils/reactions.py` & `clipzyme-0.0.5/clipzyme/utils/reactions.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.4/clipzyme/utils/registry.py` & `clipzyme-0.0.5/clipzyme/utils/registry.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.4/clipzyme/utils/sampler.py` & `clipzyme-0.0.5/clipzyme/utils/sampler.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.4/clipzyme/utils/smiles.py` & `clipzyme-0.0.5/clipzyme/utils/smiles.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.4/clipzyme/utils/wln_processing.py` & `clipzyme-0.0.5/clipzyme/utils/wln_processing.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.4/pyproject.toml` & `clipzyme-0.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clipzyme"
-version = "0.0.4"
+version = "0.0.5"
 description = "Reaction-Conditioned Virtual Screening of Enzymes"
 authors = ["Peter G Mikhael <pgmikhael@csail.mit.edu>"]
 license = "Apache 2.0"
 readme = "README.md"
 repository = "https://github.com/pgmikhael/clipzyme"
```

