# Comparing `tmp/jaxonloader-0.3.4.tar.gz` & `tmp/jaxonloader-0.3.5.tar.gz`

## Comparing `jaxonloader-0.3.4.tar` & `jaxonloader-0.3.5.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 jaxonloader-0.3.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 jaxonloader-0.3.4/mkdocs.yml
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 jaxonloader-0.3.4/noxfile.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 jaxonloader-0.3.4/.github/workflows/nox.yaml
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 jaxonloader-0.3.4/.github/workflows/pre_commit.yaml
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 jaxonloader-0.3.4/docs/api.md
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 jaxonloader-0.3.4/docs/future.md
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 jaxonloader-0.3.4/docs/getting-started.md
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 jaxonloader-0.3.4/docs/index.md
--rw-r--r--   0        0        0   126325 2020-02-02 00:00:00.000000 jaxonloader-0.3.4/docs/images/performance.png
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 jaxonloader-0.3.4/jaxonloader/__init__.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 jaxonloader-0.3.4/jaxonloader/config.py
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 jaxonloader-0.3.4/jaxonloader/dataloader.py
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 jaxonloader-0.3.4/jaxonloader/dataset.py
--rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 jaxonloader-0.3.4/jaxonloader/utils.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jaxonloader-0.3.4/jaxonloader/datasets/__init__.py
--rw-r--r--   0        0        0     8878 2020-02-02 00:00:00.000000 jaxonloader-0.3.4/jaxonloader/datasets/_datasets.py
--rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 jaxonloader-0.3.4/jaxonloader/datasets/raw.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 jaxonloader-0.3.4/tests/test_mnist.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 jaxonloader-0.3.4/tests/test_slicing.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 jaxonloader-0.3.4/tests/test_tinyshakespeare.py
--rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 jaxonloader-0.3.4/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 jaxonloader-0.3.4/LICENSE
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 jaxonloader-0.3.4/README.md
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 jaxonloader-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     3681 2020-02-02 00:00:00.000000 jaxonloader-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 jaxonloader-0.3.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 jaxonloader-0.3.5/mkdocs.yml
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 jaxonloader-0.3.5/noxfile.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 jaxonloader-0.3.5/.github/workflows/nox.yaml
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 jaxonloader-0.3.5/.github/workflows/pre_commit.yaml
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 jaxonloader-0.3.5/docs/api.md
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 jaxonloader-0.3.5/docs/future.md
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 jaxonloader-0.3.5/docs/getting-started.md
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 jaxonloader-0.3.5/docs/index.md
+-rw-r--r--   0        0        0   126325 2020-02-02 00:00:00.000000 jaxonloader-0.3.5/docs/images/performance.png
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 jaxonloader-0.3.5/jaxonloader/__init__.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 jaxonloader-0.3.5/jaxonloader/boto_client.py
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 jaxonloader-0.3.5/jaxonloader/config.py
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 jaxonloader-0.3.5/jaxonloader/dataloader.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 jaxonloader-0.3.5/jaxonloader/dataset.py
+-rw-r--r--   0        0        0     4159 2020-02-02 00:00:00.000000 jaxonloader-0.3.5/jaxonloader/utils.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jaxonloader-0.3.5/jaxonloader/datasets/__init__.py
+-rw-r--r--   0        0        0     6912 2020-02-02 00:00:00.000000 jaxonloader-0.3.5/jaxonloader/datasets/_datasets.py
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 jaxonloader-0.3.5/jaxonloader/datasets/download.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 jaxonloader-0.3.5/tests/test_mnist.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 jaxonloader-0.3.5/tests/test_slicing.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 jaxonloader-0.3.5/tests/test_tinyshakespeare.py
+-rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 jaxonloader-0.3.5/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 jaxonloader-0.3.5/LICENSE
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 jaxonloader-0.3.5/README.md
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 jaxonloader-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     3707 2020-02-02 00:00:00.000000 jaxonloader-0.3.5/PKG-INFO
```

### Comparing `jaxonloader-0.3.4/.github/workflows/nox.yaml` & `jaxonloader-0.3.5/.github/workflows/nox.yaml`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.4/docs/getting-started.md` & `jaxonloader-0.3.5/docs/getting-started.md`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.4/docs/index.md` & `jaxonloader-0.3.5/docs/index.md`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.4/docs/images/performance.png` & `jaxonloader-0.3.5/docs/images/performance.png`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.4/jaxonloader/dataloader.py` & `jaxonloader-0.3.5/jaxonloader/dataloader.py`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.4/jaxonloader/dataset.py` & `jaxonloader-0.3.5/jaxonloader/dataset.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,38 +8,50 @@
 class JaxonDataset(ABC):
     @abstractmethod
     def __len__(self) -> int:
         raise NotImplementedError()
 
     @abstractmethod
     def __getitem__(
-        self, idx: Int[NDArray, " batch_size"] | slice
-    ) -> Union[NDArray, tuple[NDArray, ...], "JaxonDataset"]:
+        self, idx: Int[NDArray, " batch_size"] | slice | int
+    ) -> Union[NDArray, tuple[NDArray, ...]]:
+        raise NotImplementedError()
+
+    def split(self, ratio: float) -> tuple["JaxonDataset", "JaxonDataset"]:
         raise NotImplementedError()
 
 
 class SingleArrayDataset(JaxonDataset):
     def __init__(self, data: NDArray):
         self.data = data
 
     def __len__(self) -> int:
         return len(self.data)
 
     def __getitem__(self, idx):
         return self.data[idx]
 
+    def split(self, ratio: float) -> tuple["SingleArrayDataset", "SingleArrayDataset"]:
+        split = int(len(self.data) * ratio)
+        return SingleArrayDataset(self.data[:split]), SingleArrayDataset(
+            self.data[split:]
+        )
+
 
 class DataTargetDataset(JaxonDataset):
     def __init__(self, data: NDArray, target: NDArray):
         self.data = data
         self.target = target
         if len(data) != len(target):
             raise ValueError("data and target must have the same length")
 
     def __len__(self) -> int:
         return len(self.data)
 
     def __getitem__(self, idx):
-        if isinstance(idx, slice):
-            return DataTargetDataset(self.data[idx], self.target[idx])
-        else:
-            return self.data[idx], self.target[idx]
+        return self.data[idx], self.target[idx]
+
+    def split(self, ratio: float) -> tuple["DataTargetDataset", "DataTargetDataset"]:
+        split = int(len(self.data) * ratio)
+        return DataTargetDataset(
+            self.data[:split], self.target[:split]
+        ), DataTargetDataset(self.data[split:], self.target[split:])
```

### Comparing `jaxonloader-0.3.4/jaxonloader/datasets/_datasets.py` & `jaxonloader-0.3.5/jaxonloader/datasets/_datasets.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,48 +1,49 @@
-import os
 import pathlib
 import pickle
 from collections.abc import Callable
+from typing import Optional
 
 import numpy as np
-import pandas as pd
 import polars as pl
-from loguru import logger
 from numpy import ndarray as NDArray
 
 from jaxonloader.dataset import DataTargetDataset, JaxonDataset, SingleArrayDataset
+from jaxonloader.datasets.download import (
+    download_cifar10,
+    download_cifar100,
+    download_mnist,
+    download_tinyshakespeare,
+    download_titanic,
+)
 from jaxonloader.utils import (
-    download_and_extract_zip,
-    jaxonloader_cache,
+    get_data_path,
     JAXONLOADER_PATH,
 )
 
 
-@jaxonloader_cache(dataset_name="mnist")
-def get_mnist() -> tuple[JaxonDataset, JaxonDataset]:
-    data_url = "https://omnisium.eu-central-1.linodeobjects.com/mnist/mnist.zip"
-    data_path = pathlib.Path(JAXONLOADER_PATH) / "mnist"
-    download_and_extract_zip(data_url, data_path)
-
+def get_mnist(
+    *, target_path: Optional[str] = None
+) -> tuple[JaxonDataset, JaxonDataset]:
+    download_mnist(target_path=target_path)
+    data_path = get_data_path("mnist", target_path)
     train_df = pl.read_csv(data_path / "mnist_train.csv")
     test_df = pl.read_csv(data_path / "mnist_test.csv")
 
     x_train = train_df.to_numpy()
     x_test = test_df.to_numpy()
 
     train_dataset = SingleArrayDataset(x_train)
     test_dataset = SingleArrayDataset(x_test)
     return train_dataset, test_dataset
 
 
-@jaxonloader_cache(dataset_name="cifar10")
-def get_cifar10() -> tuple[JaxonDataset, JaxonDataset]:
-    data_url = "https://omnisium.eu-central-1.linodeobjects.com/cifar10/cifar-10-batches-py.zip"
+def get_cifar10(target_path: Optional[str] = None) -> tuple[JaxonDataset, JaxonDataset]:
+    download_cifar10(target_path=target_path)
     data_path = pathlib.Path(JAXONLOADER_PATH) / "cifar10"
-    download_and_extract_zip(data_url, data_path)
     n_batches = 5
     train_data = []
     train_labels = []
     for i in range(1, n_batches + 1):
         with open(data_path / f"cifar-10-batches-py/data_batch_{i}", "rb") as f:
             data = pickle.load(f, encoding="bytes")
             train_data.append(data[b"data"])
@@ -57,27 +58,19 @@
 
     train_dataset = DataTargetDataset(train_data, train_labels)
     test_dataset = DataTargetDataset(test_data, test_labels)
 
     return train_dataset, test_dataset
 
 
-@jaxonloader_cache(dataset_name="cifar100")
-def get_cifar100() -> tuple[JaxonDataset, JaxonDataset]:
-    dataset_url = (
-        "https://omnisium.eu-central-1.linodeobjects.com/cifar100/cifar-100-python.zip"
-    )
-    data_path = pathlib.Path(JAXONLOADER_PATH) / "cifar100"
-    download_and_extract_zip(dataset_url, data_path)
-
-    if os.path.exists(data_path) and not os.path.exists(data_path / "cifar-100-python"):
-        raise FileNotFoundError(
-            f"The data folder {data_path} exists but the dataset is missing. "
-            + "If this error persists, please delete the data folder and try again."
-        )
+def get_cifar100(
+    target_path: Optional[str] = None,
+) -> tuple[JaxonDataset, JaxonDataset]:
+    download_cifar100(target_path=target_path)
+    data_path = get_data_path("cifar100", target_path)
 
     with open(data_path / "cifar-100-python/train", "rb") as f:
         train_data = pickle.load(f, encoding="bytes")
     with open(data_path / "cifar-100-python/test", "rb") as f:
         test_data = pickle.load(f, encoding="bytes")
 
     class CiFar100Dataset(JaxonDataset):
@@ -100,21 +93,20 @@
     test_dataset = CiFar100Dataset(
         test_data[b"data"], test_data[b"fine_labels"], test_data[b"coarse_labels"]
     )
 
     return train_dataset, test_dataset
 
 
-def get_fashion_mnist():
+def get_fashion_mnist(target_path: Optional[str]):
     raise NotImplementedError("get_fashion_mnist is not implemented yet.")
 
 
-@jaxonloader_cache(dataset_name="tinyshakespeare")
 def get_tiny_shakespeare(
-    block_size: int = 8, train_ratio: float = 0.8
+    block_size: int = 8, train_ratio: float = 0.8, *, target_path: Optional[str] = None
 ) -> tuple[
     JaxonDataset, JaxonDataset, int, Callable[[str], NDArray], Callable[[NDArray], str]
 ]:
     """
     Get the tiny shakespeare dataset from Andrej Karpathy's char-rnn repository.
 
     Args:
@@ -132,24 +124,18 @@
     Example:
     ```python
     from jaxonloader import get_tiny_shakespeare
 
     train_dataset, test_dataset, vocab_size, encoder, decoder = get_tiny_shakespeare()
     ```
     """
+    download_tinyshakespeare(target_path=target_path)
+    data_path = get_data_path("tinyshakespeare", target_path)
 
     def get_text():
-        data_path = pathlib.Path(JAXONLOADER_PATH) / "tinyshakespeare/"
-        if not os.path.exists(data_path / "input.txt"):
-            import urllib.request
-
-            url = "https://raw.githubusercontent.com/karpathy/char-rnn/master/data/tinyshakespeare/input.txt"  # noqa
-            logger.info(f"Downloading the dataset from {url}")
-            urllib.request.urlretrieve(url, data_path / "input.txt")
-
         with open(data_path / "input.txt", "r") as f:
             text = f.read()
         return text
 
     text = get_text()
     chars = sorted(list(set(text)))
     vocab_size = len(chars)
@@ -181,19 +167,17 @@
     y_test = np.roll(x_test, -1)
     test_data = np.concatenate((x_test, y_test), axis=1)
     test_dataset = SingleArrayDataset(test_data)
 
     return train_dataset, test_dataset, vocab_size, encoder, decoder
 
 
-@jaxonloader_cache(dataset_name="titanic")
-def get_titanic() -> JaxonDataset:
-    data_url = "https://omnisium.eu-central-1.linodeobjects.com/titanic/titanic.zip"
+def get_titanic(target_path: Optional[str] = None) -> JaxonDataset:
+    download_titanic(target_path=target_path)
     data_path = pathlib.Path(JAXONLOADER_PATH) / "titanic"
-    download_and_extract_zip(data_url, data_path)
     train_df = pl.read_csv(data_path / "train.csv")
 
     def _gender_to_int(df: pl.DataFrame) -> pl.DataFrame:
         df = df.with_columns(
             pl.when(pl.col("Sex") == "male").then(0).otherwise(1).alias("Sex")
         )
         return df
@@ -218,44 +202,7 @@
     train = _fill_nans(train)
     train_data = train.select(pl.exclude("Survived")).to_numpy()
     train_target = train.select(pl.col("Survived")).to_numpy()
 
     train_dataset = DataTargetDataset(train_data, train_target)
 
     return train_dataset
-
-
-def from_dataframe(dataframe: pl.DataFrame | pd.DataFrame) -> JaxonDataset:
-    """
-    Convert a polars.DataFrame (or pandas.DataFrame) to a JaxonDataset.
-
-    Args:
-    dataframe: A polars.DataFrame (or pandas.DataFrame).
-
-    Returns:
-    A JaxonDataset.
-    """
-    df: pl.DataFrame = (
-        pl.from_pandas(dataframe) if isinstance(dataframe, pd.DataFrame) else dataframe
-    )
-    data = df.to_numpy()
-    return SingleArrayDataset(data)
-
-
-def from_dataframes(*dataframes: pl.DataFrame | pd.DataFrame) -> list[JaxonDataset]:
-    """
-    Convert a list of polars.DataFrame (or pandas.DataFrame) to a list of JaxonDataset.
-
-    Args:
-        dataframes: A list of polars.DataFrame (or pandas.DataFrame).
-
-    Returns:
-        A list of JaxonDataset.
-    """
-    datasets: list[JaxonDataset] = []
-    for df in dataframes:
-        dataframe: pl.DataFrame = (
-            pl.from_pandas(df) if isinstance(df, pd.DataFrame) else df
-        )
-        data = dataframe.to_numpy()
-        datasets.append(SingleArrayDataset(data))
-    return datasets
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `jaxonloader-0.3.4/tests/test_tinyshakespeare.py` & `jaxonloader-0.3.5/tests/test_tinyshakespeare.py`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.4/.gitignore` & `jaxonloader-0.3.5/.gitignore`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.4/LICENSE` & `jaxonloader-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.4/README.md` & `jaxonloader-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.4/pyproject.toml` & `jaxonloader-0.3.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "jaxonloader"
-version = "0.3.4"
+version = "0.3.5"
 description = "A dataloader, but for JAX"
 readme = "README.md"
 requires-python ="~=3.10"
 license = {file = "LICENSE"}
 authors = [
   {name = "Artur A. Galstyan", email = "mail@arturgalstyan.dev"},
 ]
@@ -13,16 +13,17 @@
   "jaxtyping",
   "progressbar",
   "polars",
   "beartype",
   "typing_extensions",
   "loguru",
   "kaggle",
-  "pandas",
   "pyarrow",
+  "boto3",
+  "boto3-stubs"
 ]
 [project.optional-dependencies]
 dev = [
     "nox",
     "pre-commit",
     "pytest",
     "mkdocs",
```

### Comparing `jaxonloader-0.3.4/PKG-INFO` & `jaxonloader-0.3.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jaxonloader
-Version: 0.3.4
+Version: 0.3.5
 Summary: A dataloader, but for JAX
 Author-email: "Artur A. Galstyan" <mail@arturgalstyan.dev>
 License: MIT License
         
         Copyright (c) 2024 Artur A. Galstyan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -23,18 +23,19 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 License-File: LICENSE
 Requires-Python: ~=3.10
 Requires-Dist: beartype
+Requires-Dist: boto3
+Requires-Dist: boto3-stubs
 Requires-Dist: jaxtyping
 Requires-Dist: kaggle
 Requires-Dist: loguru
-Requires-Dist: pandas
 Requires-Dist: polars
 Requires-Dist: progressbar
 Requires-Dist: pyarrow
 Requires-Dist: tqdm
 Requires-Dist: typing-extensions
 Provides-Extra: dev
 Requires-Dist: mkdocs; extra == 'dev'
```

