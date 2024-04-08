# Comparing `tmp/scyan-1.5.4.tar.gz` & `tmp/scyan-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scyan-1.5.4.tar", max compression
+gzip compressed data, was "scyan-1.6.0.tar", max compression
```

## Comparing `scyan-1.5.4.tar` & `scyan-1.6.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1523 2024-01-08 14:06:00.690741 scyan-1.5.4/LICENSE
--rw-r--r--   0        0        0     4841 2024-01-08 14:06:00.690741 scyan-1.5.4/README.md
--rw-r--r--   0        0        0     2567 2024-01-08 14:06:00.734741 scyan-1.5.4/pyproject.toml
--rw-r--r--   0        0        0      428 2024-01-08 14:06:00.734741 scyan-1.5.4/scyan/__init__.py
--rw-r--r--   0        0        0     7320 2024-01-08 14:06:00.734741 scyan-1.5.4/scyan/_io.py
--rw-r--r--   0        0        0     4972 2024-01-08 14:06:00.734741 scyan-1.5.4/scyan/baseline.py
--rw-r--r--   0        0        0      105 2024-01-08 14:06:00.734741 scyan-1.5.4/scyan/data/__init__.py
--rw-r--r--   0        0        0    10800 2024-01-08 14:06:00.734741 scyan-1.5.4/scyan/data/datasets.py
--rw-r--r--   0        0        0     2247 2024-01-08 14:06:00.734741 scyan-1.5.4/scyan/data/tensors.py
--rw-r--r--   0        0        0    24098 2024-01-08 14:06:00.734741 scyan-1.5.4/scyan/model.py
--rw-r--r--   0        0        0      154 2024-01-08 14:06:00.734741 scyan-1.5.4/scyan/module/__init__.py
--rw-r--r--   0        0        0     3026 2024-01-08 14:06:00.734741 scyan-1.5.4/scyan/module/coupling_layer.py
--rw-r--r--   0        0        0     4505 2024-01-08 14:06:00.734741 scyan-1.5.4/scyan/module/distribution.py
--rw-r--r--   0        0        0     2295 2024-01-08 14:06:00.734741 scyan-1.5.4/scyan/module/real_nvp.py
--rw-r--r--   0        0        0     6263 2024-01-08 14:06:00.734741 scyan-1.5.4/scyan/module/scyan_module.py
--rw-r--r--   0        0        0      334 2024-01-08 14:06:00.734741 scyan-1.5.4/scyan/plot/__init__.py
--rw-r--r--   0        0        0      277 2024-01-08 14:06:00.734741 scyan-1.5.4/scyan/plot/_scanpy_plot/README.md
--rw-r--r--   0        0        0       80 2024-01-08 14:06:00.734741 scyan-1.5.4/scyan/plot/_scanpy_plot/__init__.py
--rw-r--r--   0        0        0     5600 2024-01-08 14:06:00.734741 scyan-1.5.4/scyan/plot/_scanpy_plot/palettes.py
--rw-r--r--   0        0        0     2082 2024-01-08 14:06:00.734741 scyan-1.5.4/scyan/plot/_scanpy_plot/plot_settings.py
--rw-r--r--   0        0        0    32523 2024-01-08 14:06:00.734741 scyan-1.5.4/scyan/plot/_scanpy_plot/umap.py
--rw-r--r--   0        0        0     3755 2024-01-08 14:06:00.734741 scyan-1.5.4/scyan/plot/density.py
--rw-r--r--   0        0        0     5369 2024-01-08 14:06:00.734741 scyan-1.5.4/scyan/plot/dot.py
--rw-r--r--   0        0        0     5886 2024-01-08 14:06:00.734741 scyan-1.5.4/scyan/plot/expressions.py
--rw-r--r--   0        0        0     2093 2024-01-08 14:06:00.734741 scyan-1.5.4/scyan/plot/graph.py
--rw-r--r--   0        0        0     1930 2024-01-08 14:06:00.734741 scyan-1.5.4/scyan/plot/heatmap.py
--rw-r--r--   0        0        0     5448 2024-01-08 14:06:00.734741 scyan-1.5.4/scyan/plot/ratios.py
--rw-r--r--   0        0        0     5116 2024-01-08 14:06:00.734741 scyan-1.5.4/scyan/plot/utils.py
--rw-r--r--   0        0        0     8721 2024-01-08 14:06:00.734741 scyan-1.5.4/scyan/preprocess.py
--rw-r--r--   0        0        0      206 2024-01-08 14:06:00.734741 scyan-1.5.4/scyan/tools/__init__.py
--rw-r--r--   0        0        0     5554 2024-01-08 14:06:00.734741 scyan-1.5.4/scyan/tools/biomarkers.py
--rw-r--r--   0        0        0     3717 2024-01-08 14:06:00.734741 scyan-1.5.4/scyan/tools/colors.py
--rw-r--r--   0        0        0     6992 2024-01-08 14:06:00.734741 scyan-1.5.4/scyan/tools/gating.py
--rw-r--r--   0        0        0     7756 2024-01-08 14:06:00.734741 scyan-1.5.4/scyan/tools/representation.py
--rw-r--r--   0        0        0     9855 2024-01-08 14:06:00.734741 scyan-1.5.4/scyan/utils.py
--rw-r--r--   0        0        0     7022 1970-01-01 00:00:00.000000 scyan-1.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1523 2024-04-08 13:14:54.305778 scyan-1.6.0/LICENSE
+-rw-r--r--   0        0        0     4841 2024-04-08 13:14:54.305778 scyan-1.6.0/README.md
+-rw-r--r--   0        0        0     2591 2024-04-08 13:14:54.349777 scyan-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0      428 2024-04-08 13:14:54.349777 scyan-1.6.0/scyan/__init__.py
+-rw-r--r--   0        0        0     8267 2024-04-08 13:14:54.349777 scyan-1.6.0/scyan/_io.py
+-rw-r--r--   0        0        0     4972 2024-04-08 13:14:54.349777 scyan-1.6.0/scyan/baseline.py
+-rw-r--r--   0        0        0      105 2024-04-08 13:14:54.349777 scyan-1.6.0/scyan/data/__init__.py
+-rw-r--r--   0        0        0    10800 2024-04-08 13:14:54.349777 scyan-1.6.0/scyan/data/datasets.py
+-rw-r--r--   0        0        0     2247 2024-04-08 13:14:54.349777 scyan-1.6.0/scyan/data/tensors.py
+-rw-r--r--   0        0        0    24386 2024-04-08 13:14:54.349777 scyan-1.6.0/scyan/model.py
+-rw-r--r--   0        0        0      154 2024-04-08 13:14:54.349777 scyan-1.6.0/scyan/module/__init__.py
+-rw-r--r--   0        0        0     3026 2024-04-08 13:14:54.349777 scyan-1.6.0/scyan/module/coupling_layer.py
+-rw-r--r--   0        0        0     4505 2024-04-08 13:14:54.349777 scyan-1.6.0/scyan/module/distribution.py
+-rw-r--r--   0        0        0     2295 2024-04-08 13:14:54.349777 scyan-1.6.0/scyan/module/real_nvp.py
+-rw-r--r--   0        0        0     6263 2024-04-08 13:14:54.349777 scyan-1.6.0/scyan/module/scyan_module.py
+-rw-r--r--   0        0        0      334 2024-04-08 13:14:54.349777 scyan-1.6.0/scyan/plot/__init__.py
+-rw-r--r--   0        0        0      277 2024-04-08 13:14:54.349777 scyan-1.6.0/scyan/plot/_scanpy_plot/README.md
+-rw-r--r--   0        0        0       80 2024-04-08 13:14:54.349777 scyan-1.6.0/scyan/plot/_scanpy_plot/__init__.py
+-rw-r--r--   0        0        0     5600 2024-04-08 13:14:54.349777 scyan-1.6.0/scyan/plot/_scanpy_plot/palettes.py
+-rw-r--r--   0        0        0     2082 2024-04-08 13:14:54.349777 scyan-1.6.0/scyan/plot/_scanpy_plot/plot_settings.py
+-rw-r--r--   0        0        0    32523 2024-04-08 13:14:54.349777 scyan-1.6.0/scyan/plot/_scanpy_plot/umap.py
+-rw-r--r--   0        0        0     3755 2024-04-08 13:14:54.349777 scyan-1.6.0/scyan/plot/density.py
+-rw-r--r--   0        0        0     5369 2024-04-08 13:14:54.349777 scyan-1.6.0/scyan/plot/dot.py
+-rw-r--r--   0        0        0     5886 2024-04-08 13:14:54.349777 scyan-1.6.0/scyan/plot/expressions.py
+-rw-r--r--   0        0        0     2093 2024-04-08 13:14:54.349777 scyan-1.6.0/scyan/plot/graph.py
+-rw-r--r--   0        0        0     1930 2024-04-08 13:14:54.349777 scyan-1.6.0/scyan/plot/heatmap.py
+-rw-r--r--   0        0        0     5794 2024-04-08 13:14:54.349777 scyan-1.6.0/scyan/plot/ratios.py
+-rw-r--r--   0        0        0     5116 2024-04-08 13:14:54.349777 scyan-1.6.0/scyan/plot/utils.py
+-rw-r--r--   0        0        0     9526 2024-04-08 13:14:54.349777 scyan-1.6.0/scyan/preprocess.py
+-rw-r--r--   0        0        0      206 2024-04-08 13:14:54.349777 scyan-1.6.0/scyan/tools/__init__.py
+-rw-r--r--   0        0        0     5554 2024-04-08 13:14:54.349777 scyan-1.6.0/scyan/tools/biomarkers.py
+-rw-r--r--   0        0        0     3717 2024-04-08 13:14:54.353777 scyan-1.6.0/scyan/tools/colors.py
+-rw-r--r--   0        0        0     6992 2024-04-08 13:14:54.353777 scyan-1.6.0/scyan/tools/gating.py
+-rw-r--r--   0        0        0     7756 2024-04-08 13:14:54.353777 scyan-1.6.0/scyan/tools/representation.py
+-rw-r--r--   0        0        0     9855 2024-04-08 13:14:54.353777 scyan-1.6.0/scyan/utils.py
+-rw-r--r--   0        0        0     6967 1970-01-01 00:00:00.000000 scyan-1.6.0/PKG-INFO
```

### Comparing `scyan-1.5.4/LICENSE` & `scyan-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scyan-1.5.4/README.md` & `scyan-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `scyan-1.5.4/pyproject.toml` & `scyan-1.6.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scyan"
-version = "1.5.4"
+version = "1.6.0"
 description = "Single-cell Cytometry Annotation Network"
 documentation = "https://mics-lab.github.io/scyan/"
 homepage = "https://mics-lab.github.io/scyan/"
 repository = "https://github.com/MICS-Lab/scyan"
 authors = ["Blampey Quentin <quentin.blampey@gmail.com>"]
 license = "BSD-3-Clause"
 readme = "README.md"
@@ -15,41 +15,41 @@
   "Operating System :: Microsoft :: Windows",
   "Programming Language :: Python :: 3",
   "Topic :: Scientific/Engineering",
 ]
 packages = [{ include = "scyan" }]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.11"
-anndata = "^0.8.0"
-torch = "^1.13"
-pytorch-lightning = "^1.6.4"
-seaborn = "^0.12.2"
-umap-learn = "^0.5.3"
-llvmlite = "^0.38.1"
-FlowUtils = "^1.0.0"
-fcsparser = "^0.2.4"
-fcswrite = "^0.6.2"
+python = ">=3.8,<3.13"
+anndata = ">=0.8.0"
+torch = ">=1.13"
+pytorch-lightning = ">=1.6.4"
+seaborn = ">=0.12.2"
+umap-learn = ">=0.5.3"
+llvmlite = ">=0.38.1"
+FlowUtils = ">=1.0.0"
+fcsparser = ">=0.2.4"
+fcswrite = ">=0.6.2"
 
-wandb = { version = "0.13.7", optional = true }
-hydra-core = { version = "^1.2.0", optional = true }
-hydra-colorlog = { version = "^1.2.0", optional = true }
-hydra-optuna-sweeper = { version = "^1.2.0", optional = true }
+wandb = { version = ">=0.13.7", optional = true }
+hydra-core = { version = ">=1.2.0", optional = true }
+hydra-colorlog = { version = ">=1.2.0", optional = true }
+hydra-optuna-sweeper = { version = ">=1.2.0", optional = true }
 
-pytest = { version = "^7.1.2", optional = true }
-ipykernel = { version = "^6.15.0", optional = true }
-ipywidgets = { version = "^7.7.1", optional = true }
-isort = { version = "^5.10.1", optional = true }
-black = { version = "^22.6.0", optional = true }
-mkdocs-material = { version = "^8.5.0", optional = true }
-mkdocstrings = { version = "^0.19.0", optional = true }
-mkdocstrings-python = { version = "^0.7.1", optional = true }
-mkdocs-jupyter = { version = "^0.21.0", optional = true }
+pytest = { version = ">=7.1.2", optional = true }
+ipykernel = { version = ">=6.15.0", optional = true }
+ipywidgets = { version = ">=7.7.1", optional = true }
+isort = { version = ">=5.10.1", optional = true }
+black = { version = ">=22.6.0", optional = true }
+mkdocs-material = { version = ">=8.5.0", optional = true }
+mkdocstrings = { version = ">=0.19.0", optional = true }
+mkdocstrings-python = { version = ">=0.7.1", optional = true }
+mkdocs-jupyter = { version = ">=0.21.0", optional = true }
 
-leidenalg = { version = "^0.8.10", optional = true }
+leidenalg = { version = ">=0.8.10", optional = true }
 
 [tool.poetry.extras]
 dev = [
   "pytest",
   "ipykernel",
   "ipywidgets",
   "isort",
```

### Comparing `scyan-1.5.4/scyan/_io.py` & `scyan-1.6.0/scyan/_io.py`

 * *Files 25% similar despite different names*

```diff
@@ -40,29 +40,54 @@
         `AnnData` object containing the FCS data.
     """
     meta, data = fcsparser.parse(path)
 
     names = pd.Series(
         [meta.get(f"$P{i + 1}{channel_suffix}") for i in range(data.shape[1])]
     )
-    fallback_names = [meta[f"$P{i + 1}N"] for i in range(data.shape[1])]
+    fallback_names = pd.Series([meta[f"$P{i + 1}N"] for i in range(data.shape[1])])
     data.columns = np.where(names.isna() | names.duplicated(False), fallback_names, names)
 
     exclude_markers = _check_exlude_markers(data, exclude_markers)
     is_marker = data.columns.str.lower().str.contains(marker_regex) & ~np.isin(
         data.columns, exclude_markers
     )
 
-    return AnnData(
-        X=data.loc[:, is_marker].values,
+    adata = AnnData(
+        X=data.loc[:, is_marker].values.astype(np.float32),
         var=pd.DataFrame(index=data.columns[is_marker]),
         obs=data.loc[:, ~is_marker],
-        dtype=np.float32,
     )
 
+    if "$SPILLOVER" in meta:
+        df_spillover = _read_spillover_matrix(meta["$SPILLOVER"])
+        fallback_var_names = fallback_names[is_marker].values
+        is_in = np.isin(fallback_var_names, df_spillover.index)
+        if is_in.all():
+            adata.varp["spillover_matrix"] = df_spillover.loc[
+                fallback_var_names, fallback_var_names
+            ]
+        else:
+            log.warn(
+                f"Missing var names inside spillover matrix: {fallback_var_names[~is_in]}. The spillover matrix will be saved in adata.uns instead of adata.varp"
+            )
+            adata.uns["spillover_matrix"] = df_spillover
+
+    return adata
+
+
+def _read_spillover_matrix(spillover_string):
+    ncol, *elements = spillover_string.split(",")
+    ncol = int(ncol)
+
+    names = elements[:ncol]
+    X = np.array(elements[ncol:]).reshape((-1, ncol)).astype(float)
+
+    return pd.DataFrame(data=X, columns=names, index=names)
+
 
 def read_csv(
     path: str,
     marker_regex: str = "^cd|^hla|epcam|^ccr",
     exclude_markers: Optional[List[str]] = None,
     **pandas_kwargs: int,
 ) -> AnnData:
```

### Comparing `scyan-1.5.4/scyan/baseline.py` & `scyan-1.6.0/scyan/baseline.py`

 * *Files identical despite different names*

### Comparing `scyan-1.5.4/scyan/data/datasets.py` & `scyan-1.6.0/scyan/data/datasets.py`

 * *Files identical despite different names*

### Comparing `scyan-1.5.4/scyan/data/tensors.py` & `scyan-1.6.0/scyan/data/tensors.py`

 * *Files identical despite different names*

### Comparing `scyan-1.5.4/scyan/model.py` & `scyan-1.6.0/scyan/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -403,36 +403,33 @@
             >>> model.load('scyan_state_dict.pt')
             ```
 
         Args:
             path: Path where the parameters were saved, i.e. the argument of `model.save(path)`.
         """
         self.load_state_dict(torch.load(path))
-        self.dataset = TensorDataset(self.x, self.covariates)
         self._is_fitted = True
 
     @property
     def _batch_size(self):
         return min(self.hparams.batch_size, self.adata.n_obs)
 
     def train_dataloader(self):
         """PyTorch lightning `train_dataloader` implementation"""
-        self.dataset = TensorDataset(self.x, self.covariates)
-
         return DataLoader(
-            self.dataset,
+            TensorDataset(self.x, self.covariates),
             batch_size=self._batch_size,
             sampler=RandomSampler(self.adata.n_obs, self._n_samples),
             num_workers=self._num_workers,
         )
 
     def predict_dataloader(self):
         """PyTorch lightning `predict_dataloader` implementation"""
         return DataLoader(
-            self.dataset,
+            TensorDataset(self.x, self.covariates),
             batch_size=self._batch_size,
             num_workers=self._num_workers,
         )
 
     def dataset_apply(self, func: Callable, data: Tuple[Tensor] = None) -> Tensor:
         """Apply a function on a dataset using a PyTorch DataLoader and with a progress bar display. It concatenates the results along the first axis.
 
@@ -492,31 +489,36 @@
             self.module.prior.fill_rho(means)
 
         self.fit(patience=patience, min_delta=min_delta, **fit_kwargs)
 
     def fit(
         self,
         max_epochs: int = 100,
+        accelerator: str = "cpu",
         min_delta: float = 1,
         patience: int = 4,
         num_workers: int = 0,
         log_every_n_steps: int = 10,
         callbacks: Optional[List[pl.Callback]] = None,
         logger: Union[bool, "pl.Logger"] = False,
         enable_checkpointing: bool = False,
         trainer: Optional[pl.Trainer] = None,
         **trainer_args: int,
     ) -> "Scyan":
         """Train the `Scyan` model. On interactive Python (e.g., Jupyter Notebooks), training can be interrupted at any time without crashing.
 
         !!! note
+            The Pytorch Lightning training is used under the hood (see the corresponding API [here](https://lightning.ai/docs/pytorch/stable/common/trainer.html#trainer-class-api))
+
+        !!! note
             Depending on your machine, you may have a warning about some performance issues. You can simply set `num_workers` to the number indicated by the warning.
 
         Args:
             max_epochs: Maximum number of epochs.
+            accelerator: Accelerator used during training. See Pytorch Lightning docs.
             min_delta: min_delta parameters used for `EarlyStopping`. See Pytorch Lightning docs.
             patience: Number of epochs with no loss improvement before stopping training.
             num_workers: Pytorch DataLoader `num_workers` argument, i.e. how many subprocesses to use for data loading. 0 means that the data will be loaded in the main process.
             log_every_n_steps: How often to log within steps (see Pytorch Lightning Trainer API).
             callbacks: Optional list of Pytorch Lightning callbacks (see their Trainer API). They will be added to our EarlyStopping callback.
             logger: Pytorch Lightning logger argument (see their Trainer API).
             enable_checkpointing: If `True`, enables Pytorch Lightning checkpointing.
@@ -537,14 +539,15 @@
                 patience=patience,
                 check_on_train_epoch_end=True,
             )
 
             log_every_n_steps = min(log_every_n_steps, len(self.x) // self._batch_size)
             trainer = pl.Trainer(
                 max_epochs=max_epochs,
+                accelerator=accelerator,
                 callbacks=[esc] + (callbacks or []),
                 log_every_n_steps=log_every_n_steps,
                 enable_checkpointing=enable_checkpointing,
                 logger=logger,
                 **trainer_args,
             )
```

### Comparing `scyan-1.5.4/scyan/module/coupling_layer.py` & `scyan-1.6.0/scyan/module/coupling_layer.py`

 * *Files identical despite different names*

### Comparing `scyan-1.5.4/scyan/module/distribution.py` & `scyan-1.6.0/scyan/module/distribution.py`

 * *Files identical despite different names*

### Comparing `scyan-1.5.4/scyan/module/real_nvp.py` & `scyan-1.6.0/scyan/module/real_nvp.py`

 * *Files identical despite different names*

### Comparing `scyan-1.5.4/scyan/module/scyan_module.py` & `scyan-1.6.0/scyan/module/scyan_module.py`

 * *Files identical despite different names*

### Comparing `scyan-1.5.4/scyan/plot/_scanpy_plot/palettes.py` & `scyan-1.6.0/scyan/plot/_scanpy_plot/palettes.py`

 * *Files identical despite different names*

### Comparing `scyan-1.5.4/scyan/plot/_scanpy_plot/plot_settings.py` & `scyan-1.6.0/scyan/plot/_scanpy_plot/plot_settings.py`

 * *Files identical despite different names*

### Comparing `scyan-1.5.4/scyan/plot/_scanpy_plot/umap.py` & `scyan-1.6.0/scyan/plot/_scanpy_plot/umap.py`

 * *Files identical despite different names*

### Comparing `scyan-1.5.4/scyan/plot/density.py` & `scyan-1.6.0/scyan/plot/density.py`

 * *Files identical despite different names*

### Comparing `scyan-1.5.4/scyan/plot/dot.py` & `scyan-1.6.0/scyan/plot/dot.py`

 * *Files identical despite different names*

### Comparing `scyan-1.5.4/scyan/plot/expressions.py` & `scyan-1.6.0/scyan/plot/expressions.py`

 * *Files identical despite different names*

### Comparing `scyan-1.5.4/scyan/plot/graph.py` & `scyan-1.6.0/scyan/plot/graph.py`

 * *Files identical despite different names*

### Comparing `scyan-1.5.4/scyan/plot/heatmap.py` & `scyan-1.6.0/scyan/plot/heatmap.py`

 * *Files identical despite different names*

### Comparing `scyan-1.5.4/scyan/plot/ratios.py` & `scyan-1.6.0/scyan/plot/ratios.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,44 +3,53 @@
 from typing import List, Optional, Union
 
 import matplotlib.pyplot as plt
 import numpy as np
 import seaborn as sns
 from anndata import AnnData
 from matplotlib.lines import Line2D
+from scipy.cluster import hierarchy
 
 from ..tools import cell_type_ratios
 from .utils import plot_decorator
 
 log = logging.getLogger(__name__)
 
 
 @plot_decorator(adata=True)
 def pop_percentage(
     adata: AnnData,
     groupby: Union[str, List[str], None] = None,
     key: str = "scyan_pop",
     figsize: tuple[float, float] = None,
+    dendogram: bool = False,
     show: bool = True,
 ):
     """Show populations percentages. Depending on `groupby`, this is either done globally, or as a stacked bar plot (one bar for each group).
 
     Args:
         adata: An `AnnData` object.
         groupby: Key(s) of `adata.obs` used to create groups (e.g. the patient ID).
         key: Key of `adata.obs` containing the population names (or the values) for which percentage will be displayed.
         figsize: matplotlib figure size.
+        dendogram: If True, the groups are sorted based on a dendogram clustering.
         show: Whether or not to display the figure.
     """
     if groupby is None:
         adata.obs[key].value_counts(normalize=True).mul(100).plot.bar(figsize=figsize)
     else:
-        adata.obs.groupby(groupby)[key].value_counts(normalize=True).mul(
-            100
-        ).unstack().plot.bar(stacked=True, figsize=figsize)
+        df = adata.obs.groupby(groupby)[key].value_counts(normalize=True)
+        df = df.mul(100).unstack()
+
+        if dendogram:
+            Z = hierarchy.linkage(df.values, method="ward")
+            dendrogram = hierarchy.dendrogram(Z, no_plot=True)
+            df = df.iloc[dendrogram["leaves"]]
+
+        df.plot.bar(stacked=True, figsize=figsize)
         plt.legend(
             bbox_to_anchor=(1.04, 0.5), loc="center left", borderaxespad=0, frameon=False
         )
 
     plt.ylabel(f"{key} percentage")
     sns.despine(offset=10, trim=True)
     plt.xticks(rotation=90)
@@ -77,15 +86,15 @@
 
     if groupby is None:
         groupby = [time_key]
     else:
         groupby = ([groupby] if isinstance(groupby, str) else groupby) + [time_key]
 
     df = cell_type_ratios(adata, groupby=groupby, key=key, normalize="%", among=among)
-    df.index = df.index.set_levels(df.index.levels[-1].astype(str), level=-1)
+    df.index = df.index.set_levels(df.index.levels[-1].codes, level=-1)
     df_log_count = np.log(
         1 + cell_type_ratios(adata, groupby=groupby, key=key, normalize=False)
     )
 
     n_pops = df.shape[1]
     n_rows = ceil(n_pops / n_cols)
     fig, axes = plt.subplots(n_rows, n_cols, figsize=figsize or (12, 3 * n_rows))
```

### Comparing `scyan-1.5.4/scyan/plot/utils.py` & `scyan-1.6.0/scyan/plot/utils.py`

 * *Files identical despite different names*

### Comparing `scyan-1.5.4/scyan/preprocess.py` & `scyan-1.6.0/scyan/preprocess.py`

 * *Files 7% similar despite different names*

```diff
@@ -60,17 +60,16 @@
             f"Auto logicle transformation failed for the following markers (logicle was used instead): {', '.join(markers_failed)}.\nIt can happen when expressions are all positive or all negative."
         )
 
 
 def _logicle_inverse_one(adata: AnnData, obsm: Optional[str], marker: str) -> np.ndarray:
     column = adata[:, marker].X if obsm is None else adata[:, marker].obsm[obsm]
     column = column.flatten()
-    return flowutils.transforms.logicle_inverse(
-        column, None, *adata.uns["scyan_logicle"][marker]
-    )
+    t, m, w = adata.uns["scyan_logicle"][marker]
+    return flowutils.transforms.logicle_inverse(column, None, t=t, m=m, w=w)
 
 
 def asinh_transform(adata: AnnData, translation: float = 0, cofactor: float = 5) -> None:
     """Asinh transformation for cell-expressions: $asinh((x - translation)/cofactor)$.
 
     Args:
         adata: An `AnnData` object.
@@ -211,7 +210,30 @@
         n_obs: Number of cell to keep.
 
     Returns:
         A view `AnnData` object with `n_obs` cells.
     """
     indices = _subset(np.arange(adata.n_obs), n_obs)
     return adata[indices]
+
+
+def correct_spillover(adata: AnnData, key_added: Optional[str] = None):
+    """Use the spillover matrix in `adata.varp["spillover_matrix"]` to correct spillover
+
+    Args:
+        adata: An `AnnData` object
+        key_added: Optional key in `adata.layers` information is saved to. By default, saved in `adata.X`
+    """
+    assert "spillover_matrix" in adata.varp, f"No 'spillover_matrix' found in adata.varp"
+
+    if any(
+        name in adata.uns
+        for name in ["scyan_asinh", "scyan_logicle", "scyan_scaling_means"]
+    ):
+        log.warn("It is recommended to apply spillover only on raw data (unprocessed)")
+
+    corrected = adata.X @ adata.varp["spillover_matrix"].T
+
+    if key_added is None:
+        adata.X = corrected
+    else:
+        adata.layers[key_added] = corrected
```

### Comparing `scyan-1.5.4/scyan/tools/biomarkers.py` & `scyan-1.6.0/scyan/tools/biomarkers.py`

 * *Files identical despite different names*

### Comparing `scyan-1.5.4/scyan/tools/colors.py` & `scyan-1.6.0/scyan/tools/colors.py`

 * *Files identical despite different names*

### Comparing `scyan-1.5.4/scyan/tools/gating.py` & `scyan-1.6.0/scyan/tools/gating.py`

 * *Files identical despite different names*

### Comparing `scyan-1.5.4/scyan/tools/representation.py` & `scyan-1.6.0/scyan/tools/representation.py`

 * *Files identical despite different names*

### Comparing `scyan-1.5.4/scyan/utils.py` & `scyan-1.6.0/scyan/utils.py`

 * *Files identical despite different names*

### Comparing `scyan-1.5.4/PKG-INFO` & `scyan-1.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,51 +1,53 @@
 Metadata-Version: 2.1
 Name: scyan
-Version: 1.5.4
+Version: 1.6.0
 Summary: Single-cell Cytometry Annotation Network
 Home-page: https://mics-lab.github.io/scyan/
 License: BSD-3-Clause
 Author: Blampey Quentin
 Author-email: quentin.blampey@gmail.com
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.8,<3.13
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Provides-Extra: dev
 Provides-Extra: discovery
 Provides-Extra: hydra
-Requires-Dist: FlowUtils (>=1.0.0,<2.0.0)
-Requires-Dist: anndata (>=0.8.0,<0.9.0)
-Requires-Dist: black (>=22.6.0,<23.0.0) ; extra == "dev"
-Requires-Dist: fcsparser (>=0.2.4,<0.3.0)
-Requires-Dist: fcswrite (>=0.6.2,<0.7.0)
-Requires-Dist: hydra-colorlog (>=1.2.0,<2.0.0) ; extra == "hydra"
-Requires-Dist: hydra-core (>=1.2.0,<2.0.0) ; extra == "hydra"
-Requires-Dist: hydra-optuna-sweeper (>=1.2.0,<2.0.0) ; extra == "hydra"
-Requires-Dist: ipykernel (>=6.15.0,<7.0.0) ; extra == "dev"
-Requires-Dist: ipywidgets (>=7.7.1,<8.0.0) ; extra == "dev"
-Requires-Dist: isort (>=5.10.1,<6.0.0) ; extra == "dev"
-Requires-Dist: leidenalg (>=0.8.10,<0.9.0) ; extra == "discovery"
-Requires-Dist: llvmlite (>=0.38.1,<0.39.0)
-Requires-Dist: mkdocs-jupyter (>=0.21.0,<0.22.0) ; extra == "dev"
-Requires-Dist: mkdocs-material (>=8.5.0,<9.0.0) ; extra == "dev"
-Requires-Dist: mkdocstrings (>=0.19.0,<0.20.0) ; extra == "dev"
-Requires-Dist: mkdocstrings-python (>=0.7.1,<0.8.0) ; extra == "dev"
-Requires-Dist: pytest (>=7.1.2,<8.0.0) ; extra == "dev"
-Requires-Dist: pytorch-lightning (>=1.6.4,<2.0.0)
-Requires-Dist: seaborn (>=0.12.2,<0.13.0)
-Requires-Dist: torch (>=1.13,<2.0)
-Requires-Dist: umap-learn (>=0.5.3,<0.6.0)
-Requires-Dist: wandb (==0.13.7) ; extra == "hydra"
+Requires-Dist: FlowUtils (>=1.0.0)
+Requires-Dist: anndata (>=0.8.0)
+Requires-Dist: black (>=22.6.0) ; extra == "dev"
+Requires-Dist: fcsparser (>=0.2.4)
+Requires-Dist: fcswrite (>=0.6.2)
+Requires-Dist: hydra-colorlog (>=1.2.0) ; extra == "hydra"
+Requires-Dist: hydra-core (>=1.2.0) ; extra == "hydra"
+Requires-Dist: hydra-optuna-sweeper (>=1.2.0) ; extra == "hydra"
+Requires-Dist: ipykernel (>=6.15.0) ; extra == "dev"
+Requires-Dist: ipywidgets (>=7.7.1) ; extra == "dev"
+Requires-Dist: isort (>=5.10.1) ; extra == "dev"
+Requires-Dist: leidenalg (>=0.8.10) ; extra == "discovery"
+Requires-Dist: llvmlite (>=0.38.1)
+Requires-Dist: mkdocs-jupyter (>=0.21.0) ; extra == "dev"
+Requires-Dist: mkdocs-material (>=8.5.0) ; extra == "dev"
+Requires-Dist: mkdocstrings (>=0.19.0) ; extra == "dev"
+Requires-Dist: mkdocstrings-python (>=0.7.1) ; extra == "dev"
+Requires-Dist: pytest (>=7.1.2) ; extra == "dev"
+Requires-Dist: pytorch-lightning (>=1.6.4)
+Requires-Dist: seaborn (>=0.12.2)
+Requires-Dist: torch (>=1.13)
+Requires-Dist: umap-learn (>=0.5.3)
+Requires-Dist: wandb (>=0.13.7) ; extra == "hydra"
 Project-URL: Documentation, https://mics-lab.github.io/scyan/
 Project-URL: Repository, https://github.com/MICS-Lab/scyan
 Description-Content-Type: text/markdown
 
 <p align="center">
   <img src="https://github.com/MICS-Lab/scyan/raw/master/docs/assets/logo.png" alt="scyan_logo" width="400"/>
 </p>
```

