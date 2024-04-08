# Comparing `tmp/kimchima-0.3.0.tar.gz` & `tmp/kimchima-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kimchima-0.3.0.tar", max compression
+gzip compressed data, was "kimchima-0.3.1.tar", max compression
```

## Comparing `kimchima-0.3.0.tar` & `kimchima-0.3.1.tar`

### file list

```diff
@@ -1,23 +1,25 @@
--rw-r--r--   0        0        0    11343 2024-04-07 12:39:37.614397 kimchima-0.3.0/LICENSE
--rw-r--r--   0        0        0      908 2024-04-07 12:39:37.614397 kimchima-0.3.0/README.md
--rw-r--r--   0        0        0     2530 2024-04-07 12:39:37.614397 kimchima-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      991 2024-04-07 12:39:37.614397 kimchima-0.3.0/src/kimchima/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 12:39:37.614397 kimchima-0.3.0/src/kimchima/cmds/__init__.py
--rw-r--r--   0        0        0     1558 2024-04-07 12:39:37.614397 kimchima-0.3.0/src/kimchima/cmds/auto_cli.py
--rw-r--r--   0        0        0     1344 2024-04-07 12:39:37.614397 kimchima-0.3.0/src/kimchima/cmds/kimchima_cli.py
--rw-r--r--   0        0        0      674 2024-04-07 12:39:37.614397 kimchima-0.3.0/src/kimchima/pipelines/__init__.py
--rw-r--r--   0        0        0     1800 2024-04-07 12:39:37.614397 kimchima-0.3.0/src/kimchima/pipelines/pipelines_factory.py
--rw-r--r--   0        0        0     1014 2024-04-07 12:39:37.614397 kimchima-0.3.0/src/kimchima/pkg/__init__.py
--rw-r--r--   0        0        0     1596 2024-04-07 12:39:37.614397 kimchima-0.3.0/src/kimchima/pkg/devices.py
--rw-r--r--   0        0        0     3222 2024-04-07 12:39:37.614397 kimchima-0.3.0/src/kimchima/pkg/embedding_factory.py
--rw-r--r--   0        0        0     5564 2024-04-07 12:39:37.614397 kimchima-0.3.0/src/kimchima/pkg/logging.py
--rw-r--r--   0        0        0     4727 2024-04-07 12:39:37.614397 kimchima-0.3.0/src/kimchima/pkg/model_factory.py
--rw-r--r--   0        0        0     1659 2024-04-07 12:39:37.614397 kimchima-0.3.0/src/kimchima/pkg/quantization_factory.py
--rw-r--r--   0        0        0     2735 2024-04-07 12:39:37.614397 kimchima-0.3.0/src/kimchima/pkg/streamer_factory.py
--rw-r--r--   0        0        0     3475 2024-04-07 12:39:37.614397 kimchima-0.3.0/src/kimchima/pkg/tokenizer_factory.py
--rw-r--r--   0        0        0        0 2024-04-07 12:39:37.614397 kimchima-0.3.0/src/kimchima/tests/__init__.py
--rw-r--r--   0        0        0     1818 2024-04-07 12:39:37.614397 kimchima-0.3.0/src/kimchima/tests/test_devices.py
--rw-r--r--   0        0        0     2032 2024-04-07 12:39:37.614397 kimchima-0.3.0/src/kimchima/tests/test_embedding_factory.py
--rw-r--r--   0        0        0     1992 2024-04-07 12:39:37.614397 kimchima-0.3.0/src/kimchima/tests/test_pipelines_factory.py
--rw-r--r--   0        0        0     1084 2024-04-07 12:39:37.614397 kimchima-0.3.0/src/kimchima/tests/test_quantization_factory.py
--rw-r--r--   0        0        0     1689 1970-01-01 00:00:00.000000 kimchima-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11343 2024-04-08 12:45:03.927963 kimchima-0.3.1/LICENSE
+-rw-r--r--   0        0        0      908 2024-04-08 12:45:03.927963 kimchima-0.3.1/README.md
+-rw-r--r--   0        0        0     2576 2024-04-08 12:45:03.931963 kimchima-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1027 2024-04-08 12:45:03.931963 kimchima-0.3.1/src/kimchima/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 12:45:03.931963 kimchima-0.3.1/src/kimchima/cmds/__init__.py
+-rw-r--r--   0        0        0     1558 2024-04-08 12:45:03.931963 kimchima-0.3.1/src/kimchima/cmds/auto_cli.py
+-rw-r--r--   0        0        0     1344 2024-04-08 12:45:03.931963 kimchima-0.3.1/src/kimchima/cmds/kimchima_cli.py
+-rw-r--r--   0        0        0        0 2024-04-08 12:45:03.931963 kimchima-0.3.1/src/kimchima/models/__init__.py
+-rw-r--r--   0        0        0      674 2024-04-08 12:45:03.931963 kimchima-0.3.1/src/kimchima/pipelines/__init__.py
+-rw-r--r--   0        0        0     2004 2024-04-08 12:45:03.931963 kimchima-0.3.1/src/kimchima/pipelines/pipelines_factory.py
+-rw-r--r--   0        0        0     1072 2024-04-08 12:45:03.931963 kimchima-0.3.1/src/kimchima/pkg/__init__.py
+-rw-r--r--   0        0        0     1598 2024-04-08 12:45:03.931963 kimchima-0.3.1/src/kimchima/pkg/devices.py
+-rw-r--r--   0        0        0     3233 2024-04-08 12:45:03.931963 kimchima-0.3.1/src/kimchima/pkg/download_hub.py
+-rw-r--r--   0        0        0     3222 2024-04-08 12:45:03.931963 kimchima-0.3.1/src/kimchima/pkg/embedding_factory.py
+-rw-r--r--   0        0        0     5564 2024-04-08 12:45:03.931963 kimchima-0.3.1/src/kimchima/pkg/logging.py
+-rw-r--r--   0        0        0     4727 2024-04-08 12:45:03.931963 kimchima-0.3.1/src/kimchima/pkg/model_factory.py
+-rw-r--r--   0        0        0     1838 2024-04-08 12:45:03.931963 kimchima-0.3.1/src/kimchima/pkg/quantization_factory.py
+-rw-r--r--   0        0        0     2735 2024-04-08 12:45:03.931963 kimchima-0.3.1/src/kimchima/pkg/streamer_factory.py
+-rw-r--r--   0        0        0     3558 2024-04-08 12:45:03.931963 kimchima-0.3.1/src/kimchima/pkg/tokenizer_factory.py
+-rw-r--r--   0        0        0        0 2024-04-08 12:45:03.931963 kimchima-0.3.1/src/kimchima/tests/__init__.py
+-rw-r--r--   0        0        0     1818 2024-04-08 12:45:03.931963 kimchima-0.3.1/src/kimchima/tests/test_devices.py
+-rw-r--r--   0        0        0     2032 2024-04-08 12:45:03.931963 kimchima-0.3.1/src/kimchima/tests/test_embedding_factory.py
+-rw-r--r--   0        0        0     1992 2024-04-08 12:45:03.931963 kimchima-0.3.1/src/kimchima/tests/test_pipelines_factory.py
+-rw-r--r--   0        0        0     1084 2024-04-08 12:45:03.931963 kimchima-0.3.1/src/kimchima/tests/test_quantization_factory.py
+-rw-r--r--   0        0        0     1689 1970-01-01 00:00:00.000000 kimchima-0.3.1/PKG-INFO
```

### Comparing `kimchima-0.3.0/LICENSE` & `kimchima-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kimchima-0.3.0/README.md` & `kimchima-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `kimchima-0.3.0/pyproject.toml` & `kimchima-0.3.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kimchima"
-version = "0.3.0"
+version = "0.3.1"
 description = "The collections of tools for ML model development."
 authors = ["Aisuko <urakiny@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/Aisuko/kimchi"
 repository = "https://github.com/Aisuko/kimchi"
 keywords = ["transformers", "pytorch"]
@@ -19,14 +19,16 @@
 bitsandbytes = "0.43.0"
 accelerate = "0.28.0"
 
 [tool.poetry.group.dev.dependencies]
 torch = "2.2.2"
 transformers = "4.39.2"
 sentencepiece = "0.2.0"
+bitsandbytes = "0.43.0"
+accelerate = "0.28.0"
 
 
 [tool.ruff]
 # Exclude a variety of commonly ignored directories.
 exclude = [
     ".bzr",
     ".direnv",
```

### Comparing `kimchima-0.3.0/src/kimchima/__init__.py` & `kimchima-0.3.1/src/kimchima/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,29 +8,31 @@
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__="0.3.0"
+__version__="0.3.1"
 
 from kimchima.pkg import (
     ModelFactory,
     TokenizerFactory,
     EmbeddingsFactory,
     QuantizationFactory,
     StreamerFactory,
-    Devices
+    Devices,
+    DownloadHub
     )
 
 from kimchima.pipelines import PipelinesFactory
 
 __all__ = [
     'ModelFactory', 
     'TokenizerFactory', 
     'EmbeddingsFactory',
     'QuantizationFactory',
     'StreamerFactory',
     'Devices',
-    'PipelinesFactory'
+    'PipelinesFactory',
+    'DownloadHub'
     ]
```

### Comparing `kimchima-0.3.0/src/kimchima/cmds/auto_cli.py` & `kimchima-0.3.1/src/kimchima/cmds/auto_cli.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.3.0/src/kimchima/cmds/kimchima_cli.py` & `kimchima-0.3.1/src/kimchima/cmds/kimchima_cli.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.3.0/src/kimchima/pipelines/__init__.py` & `kimchima-0.3.1/src/kimchima/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.3.0/src/kimchima/pkg/__init__.py` & `kimchima-0.3.1/src/kimchima/pkg/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,16 +16,19 @@
 from .model_factory import ModelFactory
 from .tokenizer_factory import TokenizerFactory
 from .embedding_factory import EmbeddingsFactory
 from .quantization_factory import QuantizationFactory
 from .streamer_factory import StreamerFactory
 
 from .devices import Devices
+from .download_hub import DownloadHub
 
 __all__ = [
     'ModelFactory', 
     'TokenizerFactory', 
     'EmbeddingsFactory',
     'QuantizationFactory',
     'StreamerFactory',
-    'Devices'
+
+    'Devices',
+    'DownloadHub'
     ]
```

### Comparing `kimchima-0.3.0/src/kimchima/pkg/devices.py` & `kimchima-0.3.1/src/kimchima/pkg/devices.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,26 +26,26 @@
     CPU = 'cpu'
     # only Nvidia GPU is supported currently
     GPU = 'cuda'
 
 
     @classmethod
     def get_device(cls)-> Devices:
-        """
+        r"""
         Only support Single GPU for now
         """
         if platform.system() == 'Darwin':
             return Devices.Silicon
         elif torch.cuda.is_available():
             return Devices.GPU
         return Devices.CPU
 
     @classmethod
     def get_capability(cls)-> Tuple[int, int]:
-        """
+        r"""
         Get the capability of the device(GPU) for current env, this is used for support latest quantization techniques like: Marlin
         
         Returns:
             tuple: The capability of the device(GPU) for current env.
 
         For not GPU env, return (0, 0)
         """
```

### Comparing `kimchima-0.3.0/src/kimchima/pkg/embedding_factory.py` & `kimchima-0.3.1/src/kimchima/pkg/embedding_factory.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.3.0/src/kimchima/pkg/logging.py` & `kimchima-0.3.1/src/kimchima/pkg/logging.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.3.0/src/kimchima/pkg/model_factory.py` & `kimchima-0.3.1/src/kimchima/pkg/model_factory.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.3.0/src/kimchima/pkg/quantization_factory.py` & `kimchima-0.3.1/src/kimchima/pkg/quantization_factory.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,38 +19,41 @@
 import torch
 from transformers import BitsAndBytesConfig
 
 logger = logging.get_logger(__name__)
 
 class QuantizationFactory:
     r"""
+    A factory class for creating Huggingface Transformers quantization configurations for different quantization techniques.
     """
 
     def __init__(self):
         raise EnvironmentError(
             "QuantizationFactory is designed to be instantiated "
             "using the `QuantizationFactory.from_pretrained(pretrained_model_name_or_path)` method."
         )
     
     @classmethod
     def quantization_4bit(cls, *args, **kwargs)-> BitsAndBytesConfig:
         r"""
+        4 bit quantization
         """
         #TODO support more parameters
         config=BitsAndBytesConfig(
             load_in_4bit=True,
             bnb_4bit_compute_dtype=torch.bfloat16,
             **kwargs
             )
 
         return config
     
     @classmethod
     def quantization_8bit(cls, *args, **kwargs)-> BitsAndBytesConfig:
         r"""
+        8 bit quantization
         """
         config=BitsAndBytesConfig(
             load_in_8bit=True,
             bnb_8bit_compute_dtype=torch.bfloat16,
             **kwargs
             )
```

### Comparing `kimchima-0.3.0/src/kimchima/pkg/streamer_factory.py` & `kimchima-0.3.1/src/kimchima/pkg/streamer_factory.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.3.0/src/kimchima/pkg/tokenizer_factory.py` & `kimchima-0.3.1/src/kimchima/pkg/tokenizer_factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,15 @@
             "TokenizerFactory is designed to be instantiated "
             "using the `TokenizerFactory.from_pretrained(pretrained_model_name_or_path)` method."
         )
 
     @classmethod                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  
     def auto_tokenizer(cls, pretrained_model_name_or_path, **kwargs)-> AutoTokenizer:
         r"""
+        Create a tokenizer using the Huggingface Transformers AutoTokenizer class.
         """
         if pretrained_model_name_or_path is None:
             raise ValueError("pretrained_model_name_or_path cannot be None")
 
         tokenizer = AutoTokenizer.from_pretrained(pretrained_model_name_or_path, **kwargs)
         logger.debug(f"Loaded tokenizer: {pretrained_model_name_or_path}")
         return tokenizer
```

### Comparing `kimchima-0.3.0/src/kimchima/tests/test_devices.py` & `kimchima-0.3.1/src/kimchima/tests/test_devices.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.3.0/src/kimchima/tests/test_embedding_factory.py` & `kimchima-0.3.1/src/kimchima/tests/test_embedding_factory.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.3.0/src/kimchima/tests/test_pipelines_factory.py` & `kimchima-0.3.1/src/kimchima/tests/test_pipelines_factory.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.3.0/src/kimchima/tests/test_quantization_factory.py` & `kimchima-0.3.1/src/kimchima/tests/test_quantization_factory.py`

 * *Files identical despite different names*

### Comparing `kimchima-0.3.0/PKG-INFO` & `kimchima-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kimchima
-Version: 0.3.0
+Version: 0.3.1
 Summary: The collections of tools for ML model development.
 Home-page: https://github.com/Aisuko/kimchi
 License: Apache-2.0
 Keywords: transformers,pytorch
 Author: Aisuko
 Author-email: urakiny@gmail.com
 Requires-Python: >=3.11,<4.0
```

