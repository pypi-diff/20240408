# Comparing `tmp/pyreft-0.0.1.tar.gz` & `tmp/pyreft-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyreft-0.0.1.tar", last modified: Sat Apr  6 22:12:01 2024, max compression
+gzip compressed data, was "pyreft-0.0.2.tar", last modified: Sun Apr  7 23:17:48 2024, max compression
```

## Comparing `pyreft-0.0.1.tar` & `pyreft-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 22:12:01.814798 pyreft-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-06 22:11:52.000000 pyreft-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-06 22:11:52.000000 pyreft-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12845 2024-04-06 22:12:01.814798 pyreft-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11614 2024-04-06 22:11:52.000000 pyreft-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 22:12:01.814798 pyreft-0.0.1/pyreft/
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-06 22:11:52.000000 pyreft-0.0.1/pyreft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-06 22:11:52.000000 pyreft-0.0.1/pyreft/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    10455 2024-04-06 22:11:52.000000 pyreft-0.0.1/pyreft/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-04-06 22:11:52.000000 pyreft-0.0.1/pyreft/interventions.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-06 22:11:52.000000 pyreft-0.0.1/pyreft/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-06 22:11:52.000000 pyreft-0.0.1/pyreft/reft_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5711 2024-04-06 22:11:52.000000 pyreft-0.0.1/pyreft/reft_trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-06 22:11:52.000000 pyreft-0.0.1/pyreft/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 22:12:01.814798 pyreft-0.0.1/pyreft.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12845 2024-04-06 22:12:01.000000 pyreft-0.0.1/pyreft.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-06 22:12:01.000000 pyreft-0.0.1/pyreft.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 22:12:01.000000 pyreft-0.0.1/pyreft.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-06 22:12:01.000000 pyreft-0.0.1/pyreft.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-06 22:12:01.000000 pyreft-0.0.1/pyreft.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-06 22:11:52.000000 pyreft-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 22:12:01.814798 pyreft-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-06 22:11:52.000000 pyreft-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:17:48.059512 pyreft-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-07 23:17:43.000000 pyreft-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-07 23:17:43.000000 pyreft-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    13131 2024-04-07 23:17:48.059512 pyreft-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11869 2024-04-07 23:17:43.000000 pyreft-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:17:48.059512 pyreft-0.0.2/pyreft/
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-07 23:17:43.000000 pyreft-0.0.2/pyreft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-07 23:17:43.000000 pyreft-0.0.2/pyreft/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10455 2024-04-07 23:17:43.000000 pyreft-0.0.2/pyreft/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-04-07 23:17:43.000000 pyreft-0.0.2/pyreft/interventions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-07 23:17:43.000000 pyreft-0.0.2/pyreft/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-07 23:17:43.000000 pyreft-0.0.2/pyreft/reft_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5711 2024-04-07 23:17:43.000000 pyreft-0.0.2/pyreft/reft_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-07 23:17:43.000000 pyreft-0.0.2/pyreft/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 23:17:48.059512 pyreft-0.0.2/pyreft.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13131 2024-04-07 23:17:48.000000 pyreft-0.0.2/pyreft.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-07 23:17:48.000000 pyreft-0.0.2/pyreft.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 23:17:48.000000 pyreft-0.0.2/pyreft.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-07 23:17:48.000000 pyreft-0.0.2/pyreft.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-07 23:17:48.000000 pyreft-0.0.2/pyreft.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-07 23:17:43.000000 pyreft-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 23:17:48.059512 pyreft-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-07 23:17:43.000000 pyreft-0.0.2/setup.py
```

### Comparing `pyreft-0.0.1/LICENSE` & `pyreft-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyreft-0.0.1/PKG-INFO` & `pyreft-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyreft
-Version: 0.0.1
+Version: 0.0.2
 Summary: REFT: Representation Finetuning for Language Models
 Home-page: https://github.com/stanfordnlp/reft
 Author: Zhengxuan Wu
 Author-email: wuzhengx@stanford.edu
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -27,14 +27,15 @@
 Requires-Dist: ipywidgets>=8.1.1
 Requires-Dist: plotnine>=0.12.4
 Requires-Dist: huggingface-hub>=0.20.3
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: fsspec>=2023.6.0
 Requires-Dist: accelerate>=0.26.1
 Requires-Dist: sentencepiece>=0.1.96
+Requires-Dist: evaluate>=0.4.1
 Requires-Dist: wandb
 Requires-Dist: scikit-learn
 Requires-Dist: jupyter
 
 <h1 align="center"> <p>pyreft<sub> by <a href="https://github.com/stanfordnlp/pyvene">pyvene</a></sub></p></h1>
 <h3 align="center">
     <p>State-of-the-art Representation Fine-Tuning (ReFT) methods</p>
@@ -64,15 +65,22 @@
 > **Powerful and Parameter-Efficient:** Read [Our ReFT paper](https://arxiv.org/abs/2404.03592) for an introduction of representation fine-tuning (ReFT) and its performance.
 
 > [!TIP]
 > **Intepretable Finetuning:** Read [Composable ReFT](https://github.com/frankaging/pyreft/tree/main/examples/composition) for a sneak-peek of the interpretable nature of ReFT.
 
 ## Quickstart
 
-Install **pyreft** from pip+git:
+Here is one verified conda env setup steps:
+
+```bash
+conda create --name awesome-reft python=3.10
+conda activate awesome-reft
+```
+
+Then, install **pyreft** from pip+git:
 
 ```bash
 pip install git+https://github.com/frankaging/pyreft.git
 ```
 
 Or install **pyreft** from pip (coming soon):
 
@@ -173,15 +181,15 @@
 science. We also develop a wide variety of educational materials
 on NLP and many tools for the community to use, including the Stanza
 toolkit which processes text in over 60 human languages."""
 ```
 
 We successfully compress the text into 4,097 parameters! We perform more rigious memorisation test like this one in [ReFT Interp](https://github.com/frankaging/pyreft/tree/main/examples/memorisation). 
 
-You can do ReFT with any language modeling tasks or SFT. Check out our [`examples`](https://github.com/frankaging/pyreft/tree/main/examples) folder! **You can train a 7B chat-model as good as ChatGPT-3.5-1103 under 18 mins with a single A100 GPU + ReFT** by following steps here [`train.py`](https://github.com/frankaging/pyreft/blob/main/examples/loreft/train.py).
+You can do ReFT with any language modeling tasks or SFT. Check out our [`examples`](https://github.com/frankaging/pyreft/tree/main/examples) folder! **You can train a 7B chat-model close to ChatGPT-3.5-1103 (81.9 v.s. 86.3 Alpaca-eval scores) under 18 mins with a single A100 GPU + ReFT** by following steps here [`train.py`](https://github.com/frankaging/pyreft/blob/main/examples/loreft/train.py) training Llama-2 with the [Ultrafeedback dataset](https://arxiv.org/abs/2310.01377).
 
 ## Loading our 18 min-cooked `Loreft1k-Llama-2-7b-hf` from HuggingFace
 
 For full tutorial, please take a look at [`chat_model.ipynb`](https://github.com/frankaging/pyreft/blob/main/examples/chat/chat_model.ipynb).
 
 Loading the base LM first:
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1 Name: pyreft Version: 0.0.1 Summary: REFT: Representation
+Metadata-Version: 2.1 Name: pyreft Version: 0.0.2 Summary: REFT: Representation
 Finetuning for Language Models Home-page: https://github.com/stanfordnlp/reft
 Author: Zhengxuan Wu Author-email: wuzhengx@stanford.edu License: Apache
 License 2.0 Classifier: Development Status :: 3 - Alpha Classifier: Intended
 Audience :: Science/Research Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Requires-Python: >=3.8 Description-
 Content-Type: text/markdown License-File: LICENSE Requires-Dist: torch>=2.2.1
 Requires-Dist: flash-attn>=2.5.6 Requires-Dist: transformers>=4.39.2 Requires-
 Dist: pyvene>=0.0.8 Requires-Dist: datasets>=2.16.1 Requires-Dist:
 protobuf>=3.20.0 Requires-Dist: matplotlib>=3.7.4 Requires-Dist:
 seaborn>=0.13.1 Requires-Dist: ipywidgets>=8.1.1 Requires-Dist:
 plotnine>=0.12.4 Requires-Dist: huggingface-hub>=0.20.3 Requires-Dist:
 numpy>=1.26.4 Requires-Dist: fsspec>=2023.6.0 Requires-Dist: accelerate>=0.26.1
-Requires-Dist: sentencepiece>=0.1.96 Requires-Dist: wandb Requires-Dist:
-scikit-learn Requires-Dist: jupyter
+Requires-Dist: sentencepiece>=0.1.96 Requires-Dist: evaluate>=0.4.1 Requires-
+Dist: wandb Requires-Dist: scikit-learn Requires-Dist: jupyter
                         ************ ppyyrreefftt bbyy _pp_yy_vv_ee_nn_ee ************
      ******** SSttaattee--ooff--tthhee--aarrtt RReepprreesseennttaattiioonn FFiinnee--TTuunniinngg ((RReeFFTT)) mmeetthhooddss ********
 > [!WARNING] > **Hey hey! Corrections to the preprint:** We or members of the
 community have identified a few typos. - (1) Hyperparameter settings presented
 in Table 5 and 6 in the Appendix should be swapped, i.e., GSM8K should be the
 one where we apply interventions to all layers. We release our training wandb
 logs in our [LoReFT](https://github.com/frankaging/pyreft/tree/main/examples/
@@ -36,19 +36,21 @@
 parameters. **pyreft** supports - Fine tuning any pretrained LMs on HuggingFace
 with ReFT - Setting ReFT hyperparameters via configs - Sharing the fine-tuned
 results easily to HuggingFace > [!TIP] > **Powerful and Parameter-Efficient:**
 Read [Our ReFT paper](https://arxiv.org/abs/2404.03592) for an introduction of
 representation fine-tuning (ReFT) and its performance. > [!TIP] >
 **Intepretable Finetuning:** Read [Composable ReFT](https://github.com/
 frankaging/pyreft/tree/main/examples/composition) for a sneak-peek of the
-interpretable nature of ReFT. ## Quickstart Install **pyreft** from pip+git:
-```bash pip install git+https://github.com/frankaging/pyreft.git ``` Or install
-**pyreft** from pip (coming soon): ```bash pip install pyreft ``` Prepare a
-model for training with a ReFT method by wrapping the base model and ReFT
-configuration with `get_reft_model`. In the following example, we are using
+interpretable nature of ReFT. ## Quickstart Here is one verified conda env
+setup steps: ```bash conda create --name awesome-reft python=3.10 conda
+activate awesome-reft ``` Then, install **pyreft** from pip+git: ```bash pip
+install git+https://github.com/frankaging/pyreft.git ``` Or install **pyreft**
+from pip (coming soon): ```bash pip install pyreft ``` Prepare a model for
+training with a ReFT method by wrapping the base model and ReFT configuration
+with `get_reft_model`. In the following example, we are using
 [`ConsreftIntervention`](https://github.com/stanfordnlp/pyreft/blob/main/
 pyreft/interventions.py#L85) (Constant LoReFT Intervention) which is even more
 parameter-efficient than the original LoReFT described in the paper: ```python
 import torch import transformers from pyreft import ( get_reft_model,
 ReftConfig, ConsreftIntervention ) # loading huggingface model
 model_name_or_path = "yahma/llama-7b-hf" model =
 transformers.AutoModelForCausalLM.from_pretrained( model_name_or_path,
@@ -100,27 +102,29 @@
 cognitive science. We also develop a wide variety of educational materials on
 NLP and many tools for the community to use, including the Stanza toolkit which
 processes text in over 60 human languages.""" ``` We successfully compress the
 text into 4,097 parameters! We perform more rigious memorisation test like this
 one in [ReFT Interp](https://github.com/frankaging/pyreft/tree/main/examples/
 memorisation). You can do ReFT with any language modeling tasks or SFT. Check
 out our [`examples`](https://github.com/frankaging/pyreft/tree/main/examples)
-folder! **You can train a 7B chat-model as good as ChatGPT-3.5-1103 under 18
-mins with a single A100 GPU + ReFT** by following steps here [`train.py`]
-(https://github.com/frankaging/pyreft/blob/main/examples/loreft/train.py). ##
-Loading our 18 min-cooked `Loreft1k-Llama-2-7b-hf` from HuggingFace For full
-tutorial, please take a look at [`chat_model.ipynb`](https://github.com/
-frankaging/pyreft/blob/main/examples/chat/chat_model.ipynb). Loading the base
-LM first: ```py import torch, transformers from pyreft import ( ReftModel,
-get_intervention_locations ) prompt_no_input_template = """Below is an
-instruction that \ describes a task. Write a response that appropriately \
-completes the request. ### Instruction: %s ### Response: """ device = "cuda" if
-torch.cuda.is_available() else "cpu" model_name_or_path = "meta-llama/Llama-2-
-7b-hf" reft_model_name_or_path = "zhengxuanzenwu/Loreft1k-Llama-2-7b-hf"
-tokenizer = transformers.AutoTokenizer.from_pretrained( model_name_or_path,
+folder! **You can train a 7B chat-model close to ChatGPT-3.5-1103 (81.9 v.s.
+86.3 Alpaca-eval scores) under 18 mins with a single A100 GPU + ReFT** by
+following steps here [`train.py`](https://github.com/frankaging/pyreft/blob/
+main/examples/loreft/train.py) training Llama-2 with the [Ultrafeedback
+dataset](https://arxiv.org/abs/2310.01377). ## Loading our 18 min-cooked
+`Loreft1k-Llama-2-7b-hf` from HuggingFace For full tutorial, please take a look
+at [`chat_model.ipynb`](https://github.com/frankaging/pyreft/blob/main/
+examples/chat/chat_model.ipynb). Loading the base LM first: ```py import torch,
+transformers from pyreft import ( ReftModel, get_intervention_locations )
+prompt_no_input_template = """Below is an instruction that \ describes a task.
+Write a response that appropriately \ completes the request. ### Instruction:
+%s ### Response: """ device = "cuda" if torch.cuda.is_available() else "cpu"
+model_name_or_path = "meta-llama/Llama-2-7b-hf" reft_model_name_or_path =
+"zhengxuanzenwu/Loreft1k-Llama-2-7b-hf" tokenizer =
+transformers.AutoTokenizer.from_pretrained( model_name_or_path,
 model_max_length=2048, padding_side="right", use_fast=False)
 tokenizer.pad_token = tokenizer.unk_token model =
 transformers.AutoModelForCausalLM.from_pretrained( model_name_or_path,
 torch_dtype=torch.bfloat16, device_map=device) ``` Then, loading ReFT
 artifacts: ```py reft_model = ReftModel.load( "zhengxuanzenwu/Loreft1k-Llama-2-
 7b-hf", model, from_huggingface_hub=True) reft_model.set_device(device) ```
 Start chatting with it: ```py instruction = "Tell me about the NLP Group at
```

### Comparing `pyreft-0.0.1/README.md` & `pyreft-0.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,22 @@
 > **Powerful and Parameter-Efficient:** Read [Our ReFT paper](https://arxiv.org/abs/2404.03592) for an introduction of representation fine-tuning (ReFT) and its performance.
 
 > [!TIP]
 > **Intepretable Finetuning:** Read [Composable ReFT](https://github.com/frankaging/pyreft/tree/main/examples/composition) for a sneak-peek of the interpretable nature of ReFT.
 
 ## Quickstart
 
-Install **pyreft** from pip+git:
+Here is one verified conda env setup steps:
+
+```bash
+conda create --name awesome-reft python=3.10
+conda activate awesome-reft
+```
+
+Then, install **pyreft** from pip+git:
 
 ```bash
 pip install git+https://github.com/frankaging/pyreft.git
 ```
 
 Or install **pyreft** from pip (coming soon):
 
@@ -136,15 +143,15 @@
 science. We also develop a wide variety of educational materials
 on NLP and many tools for the community to use, including the Stanza
 toolkit which processes text in over 60 human languages."""
 ```
 
 We successfully compress the text into 4,097 parameters! We perform more rigious memorisation test like this one in [ReFT Interp](https://github.com/frankaging/pyreft/tree/main/examples/memorisation). 
 
-You can do ReFT with any language modeling tasks or SFT. Check out our [`examples`](https://github.com/frankaging/pyreft/tree/main/examples) folder! **You can train a 7B chat-model as good as ChatGPT-3.5-1103 under 18 mins with a single A100 GPU + ReFT** by following steps here [`train.py`](https://github.com/frankaging/pyreft/blob/main/examples/loreft/train.py).
+You can do ReFT with any language modeling tasks or SFT. Check out our [`examples`](https://github.com/frankaging/pyreft/tree/main/examples) folder! **You can train a 7B chat-model close to ChatGPT-3.5-1103 (81.9 v.s. 86.3 Alpaca-eval scores) under 18 mins with a single A100 GPU + ReFT** by following steps here [`train.py`](https://github.com/frankaging/pyreft/blob/main/examples/loreft/train.py) training Llama-2 with the [Ultrafeedback dataset](https://arxiv.org/abs/2310.01377).
 
 ## Loading our 18 min-cooked `Loreft1k-Llama-2-7b-hf` from HuggingFace
 
 For full tutorial, please take a look at [`chat_model.ipynb`](https://github.com/frankaging/pyreft/blob/main/examples/chat/chat_model.ipynb).
 
 Loading the base LM first:
```

#### html2text {}

```diff
@@ -19,19 +19,21 @@
 parameters. **pyreft** supports - Fine tuning any pretrained LMs on HuggingFace
 with ReFT - Setting ReFT hyperparameters via configs - Sharing the fine-tuned
 results easily to HuggingFace > [!TIP] > **Powerful and Parameter-Efficient:**
 Read [Our ReFT paper](https://arxiv.org/abs/2404.03592) for an introduction of
 representation fine-tuning (ReFT) and its performance. > [!TIP] >
 **Intepretable Finetuning:** Read [Composable ReFT](https://github.com/
 frankaging/pyreft/tree/main/examples/composition) for a sneak-peek of the
-interpretable nature of ReFT. ## Quickstart Install **pyreft** from pip+git:
-```bash pip install git+https://github.com/frankaging/pyreft.git ``` Or install
-**pyreft** from pip (coming soon): ```bash pip install pyreft ``` Prepare a
-model for training with a ReFT method by wrapping the base model and ReFT
-configuration with `get_reft_model`. In the following example, we are using
+interpretable nature of ReFT. ## Quickstart Here is one verified conda env
+setup steps: ```bash conda create --name awesome-reft python=3.10 conda
+activate awesome-reft ``` Then, install **pyreft** from pip+git: ```bash pip
+install git+https://github.com/frankaging/pyreft.git ``` Or install **pyreft**
+from pip (coming soon): ```bash pip install pyreft ``` Prepare a model for
+training with a ReFT method by wrapping the base model and ReFT configuration
+with `get_reft_model`. In the following example, we are using
 [`ConsreftIntervention`](https://github.com/stanfordnlp/pyreft/blob/main/
 pyreft/interventions.py#L85) (Constant LoReFT Intervention) which is even more
 parameter-efficient than the original LoReFT described in the paper: ```python
 import torch import transformers from pyreft import ( get_reft_model,
 ReftConfig, ConsreftIntervention ) # loading huggingface model
 model_name_or_path = "yahma/llama-7b-hf" model =
 transformers.AutoModelForCausalLM.from_pretrained( model_name_or_path,
@@ -83,27 +85,29 @@
 cognitive science. We also develop a wide variety of educational materials on
 NLP and many tools for the community to use, including the Stanza toolkit which
 processes text in over 60 human languages.""" ``` We successfully compress the
 text into 4,097 parameters! We perform more rigious memorisation test like this
 one in [ReFT Interp](https://github.com/frankaging/pyreft/tree/main/examples/
 memorisation). You can do ReFT with any language modeling tasks or SFT. Check
 out our [`examples`](https://github.com/frankaging/pyreft/tree/main/examples)
-folder! **You can train a 7B chat-model as good as ChatGPT-3.5-1103 under 18
-mins with a single A100 GPU + ReFT** by following steps here [`train.py`]
-(https://github.com/frankaging/pyreft/blob/main/examples/loreft/train.py). ##
-Loading our 18 min-cooked `Loreft1k-Llama-2-7b-hf` from HuggingFace For full
-tutorial, please take a look at [`chat_model.ipynb`](https://github.com/
-frankaging/pyreft/blob/main/examples/chat/chat_model.ipynb). Loading the base
-LM first: ```py import torch, transformers from pyreft import ( ReftModel,
-get_intervention_locations ) prompt_no_input_template = """Below is an
-instruction that \ describes a task. Write a response that appropriately \
-completes the request. ### Instruction: %s ### Response: """ device = "cuda" if
-torch.cuda.is_available() else "cpu" model_name_or_path = "meta-llama/Llama-2-
-7b-hf" reft_model_name_or_path = "zhengxuanzenwu/Loreft1k-Llama-2-7b-hf"
-tokenizer = transformers.AutoTokenizer.from_pretrained( model_name_or_path,
+folder! **You can train a 7B chat-model close to ChatGPT-3.5-1103 (81.9 v.s.
+86.3 Alpaca-eval scores) under 18 mins with a single A100 GPU + ReFT** by
+following steps here [`train.py`](https://github.com/frankaging/pyreft/blob/
+main/examples/loreft/train.py) training Llama-2 with the [Ultrafeedback
+dataset](https://arxiv.org/abs/2310.01377). ## Loading our 18 min-cooked
+`Loreft1k-Llama-2-7b-hf` from HuggingFace For full tutorial, please take a look
+at [`chat_model.ipynb`](https://github.com/frankaging/pyreft/blob/main/
+examples/chat/chat_model.ipynb). Loading the base LM first: ```py import torch,
+transformers from pyreft import ( ReftModel, get_intervention_locations )
+prompt_no_input_template = """Below is an instruction that \ describes a task.
+Write a response that appropriately \ completes the request. ### Instruction:
+%s ### Response: """ device = "cuda" if torch.cuda.is_available() else "cpu"
+model_name_or_path = "meta-llama/Llama-2-7b-hf" reft_model_name_or_path =
+"zhengxuanzenwu/Loreft1k-Llama-2-7b-hf" tokenizer =
+transformers.AutoTokenizer.from_pretrained( model_name_or_path,
 model_max_length=2048, padding_side="right", use_fast=False)
 tokenizer.pad_token = tokenizer.unk_token model =
 transformers.AutoModelForCausalLM.from_pretrained( model_name_or_path,
 torch_dtype=torch.bfloat16, device_map=device) ``` Then, loading ReFT
 artifacts: ```py reft_model = ReftModel.load( "zhengxuanzenwu/Loreft1k-Llama-2-
 7b-hf", model, from_huggingface_hub=True) reft_model.set_device(device) ```
 Start chatting with it: ```py instruction = "Tell me about the NLP Group at
```

### Comparing `pyreft-0.0.1/pyreft/__init__.py` & `pyreft-0.0.2/pyreft/__init__.py`

 * *Files identical despite different names*

### Comparing `pyreft-0.0.1/pyreft/dataset.py` & `pyreft-0.0.2/pyreft/dataset.py`

 * *Files identical despite different names*

### Comparing `pyreft-0.0.1/pyreft/interventions.py` & `pyreft-0.0.2/pyreft/interventions.py`

 * *Files identical despite different names*

### Comparing `pyreft-0.0.1/pyreft/reft_model.py` & `pyreft-0.0.2/pyreft/reft_model.py`

 * *Files identical despite different names*

### Comparing `pyreft-0.0.1/pyreft/reft_trainer.py` & `pyreft-0.0.2/pyreft/reft_trainer.py`

 * *Files identical despite different names*

### Comparing `pyreft-0.0.1/pyreft/utils.py` & `pyreft-0.0.2/pyreft/utils.py`

 * *Files identical despite different names*

### Comparing `pyreft-0.0.1/pyreft.egg-info/PKG-INFO` & `pyreft-0.0.2/pyreft.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyreft
-Version: 0.0.1
+Version: 0.0.2
 Summary: REFT: Representation Finetuning for Language Models
 Home-page: https://github.com/stanfordnlp/reft
 Author: Zhengxuan Wu
 Author-email: wuzhengx@stanford.edu
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -27,14 +27,15 @@
 Requires-Dist: ipywidgets>=8.1.1
 Requires-Dist: plotnine>=0.12.4
 Requires-Dist: huggingface-hub>=0.20.3
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: fsspec>=2023.6.0
 Requires-Dist: accelerate>=0.26.1
 Requires-Dist: sentencepiece>=0.1.96
+Requires-Dist: evaluate>=0.4.1
 Requires-Dist: wandb
 Requires-Dist: scikit-learn
 Requires-Dist: jupyter
 
 <h1 align="center"> <p>pyreft<sub> by <a href="https://github.com/stanfordnlp/pyvene">pyvene</a></sub></p></h1>
 <h3 align="center">
     <p>State-of-the-art Representation Fine-Tuning (ReFT) methods</p>
@@ -64,15 +65,22 @@
 > **Powerful and Parameter-Efficient:** Read [Our ReFT paper](https://arxiv.org/abs/2404.03592) for an introduction of representation fine-tuning (ReFT) and its performance.
 
 > [!TIP]
 > **Intepretable Finetuning:** Read [Composable ReFT](https://github.com/frankaging/pyreft/tree/main/examples/composition) for a sneak-peek of the interpretable nature of ReFT.
 
 ## Quickstart
 
-Install **pyreft** from pip+git:
+Here is one verified conda env setup steps:
+
+```bash
+conda create --name awesome-reft python=3.10
+conda activate awesome-reft
+```
+
+Then, install **pyreft** from pip+git:
 
 ```bash
 pip install git+https://github.com/frankaging/pyreft.git
 ```
 
 Or install **pyreft** from pip (coming soon):
 
@@ -173,15 +181,15 @@
 science. We also develop a wide variety of educational materials
 on NLP and many tools for the community to use, including the Stanza
 toolkit which processes text in over 60 human languages."""
 ```
 
 We successfully compress the text into 4,097 parameters! We perform more rigious memorisation test like this one in [ReFT Interp](https://github.com/frankaging/pyreft/tree/main/examples/memorisation). 
 
-You can do ReFT with any language modeling tasks or SFT. Check out our [`examples`](https://github.com/frankaging/pyreft/tree/main/examples) folder! **You can train a 7B chat-model as good as ChatGPT-3.5-1103 under 18 mins with a single A100 GPU + ReFT** by following steps here [`train.py`](https://github.com/frankaging/pyreft/blob/main/examples/loreft/train.py).
+You can do ReFT with any language modeling tasks or SFT. Check out our [`examples`](https://github.com/frankaging/pyreft/tree/main/examples) folder! **You can train a 7B chat-model close to ChatGPT-3.5-1103 (81.9 v.s. 86.3 Alpaca-eval scores) under 18 mins with a single A100 GPU + ReFT** by following steps here [`train.py`](https://github.com/frankaging/pyreft/blob/main/examples/loreft/train.py) training Llama-2 with the [Ultrafeedback dataset](https://arxiv.org/abs/2310.01377).
 
 ## Loading our 18 min-cooked `Loreft1k-Llama-2-7b-hf` from HuggingFace
 
 For full tutorial, please take a look at [`chat_model.ipynb`](https://github.com/frankaging/pyreft/blob/main/examples/chat/chat_model.ipynb).
 
 Loading the base LM first:
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1 Name: pyreft Version: 0.0.1 Summary: REFT: Representation
+Metadata-Version: 2.1 Name: pyreft Version: 0.0.2 Summary: REFT: Representation
 Finetuning for Language Models Home-page: https://github.com/stanfordnlp/reft
 Author: Zhengxuan Wu Author-email: wuzhengx@stanford.edu License: Apache
 License 2.0 Classifier: Development Status :: 3 - Alpha Classifier: Intended
 Audience :: Science/Research Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Requires-Python: >=3.8 Description-
 Content-Type: text/markdown License-File: LICENSE Requires-Dist: torch>=2.2.1
 Requires-Dist: flash-attn>=2.5.6 Requires-Dist: transformers>=4.39.2 Requires-
 Dist: pyvene>=0.0.8 Requires-Dist: datasets>=2.16.1 Requires-Dist:
 protobuf>=3.20.0 Requires-Dist: matplotlib>=3.7.4 Requires-Dist:
 seaborn>=0.13.1 Requires-Dist: ipywidgets>=8.1.1 Requires-Dist:
 plotnine>=0.12.4 Requires-Dist: huggingface-hub>=0.20.3 Requires-Dist:
 numpy>=1.26.4 Requires-Dist: fsspec>=2023.6.0 Requires-Dist: accelerate>=0.26.1
-Requires-Dist: sentencepiece>=0.1.96 Requires-Dist: wandb Requires-Dist:
-scikit-learn Requires-Dist: jupyter
+Requires-Dist: sentencepiece>=0.1.96 Requires-Dist: evaluate>=0.4.1 Requires-
+Dist: wandb Requires-Dist: scikit-learn Requires-Dist: jupyter
                         ************ ppyyrreefftt bbyy _pp_yy_vv_ee_nn_ee ************
      ******** SSttaattee--ooff--tthhee--aarrtt RReepprreesseennttaattiioonn FFiinnee--TTuunniinngg ((RReeFFTT)) mmeetthhooddss ********
 > [!WARNING] > **Hey hey! Corrections to the preprint:** We or members of the
 community have identified a few typos. - (1) Hyperparameter settings presented
 in Table 5 and 6 in the Appendix should be swapped, i.e., GSM8K should be the
 one where we apply interventions to all layers. We release our training wandb
 logs in our [LoReFT](https://github.com/frankaging/pyreft/tree/main/examples/
@@ -36,19 +36,21 @@
 parameters. **pyreft** supports - Fine tuning any pretrained LMs on HuggingFace
 with ReFT - Setting ReFT hyperparameters via configs - Sharing the fine-tuned
 results easily to HuggingFace > [!TIP] > **Powerful and Parameter-Efficient:**
 Read [Our ReFT paper](https://arxiv.org/abs/2404.03592) for an introduction of
 representation fine-tuning (ReFT) and its performance. > [!TIP] >
 **Intepretable Finetuning:** Read [Composable ReFT](https://github.com/
 frankaging/pyreft/tree/main/examples/composition) for a sneak-peek of the
-interpretable nature of ReFT. ## Quickstart Install **pyreft** from pip+git:
-```bash pip install git+https://github.com/frankaging/pyreft.git ``` Or install
-**pyreft** from pip (coming soon): ```bash pip install pyreft ``` Prepare a
-model for training with a ReFT method by wrapping the base model and ReFT
-configuration with `get_reft_model`. In the following example, we are using
+interpretable nature of ReFT. ## Quickstart Here is one verified conda env
+setup steps: ```bash conda create --name awesome-reft python=3.10 conda
+activate awesome-reft ``` Then, install **pyreft** from pip+git: ```bash pip
+install git+https://github.com/frankaging/pyreft.git ``` Or install **pyreft**
+from pip (coming soon): ```bash pip install pyreft ``` Prepare a model for
+training with a ReFT method by wrapping the base model and ReFT configuration
+with `get_reft_model`. In the following example, we are using
 [`ConsreftIntervention`](https://github.com/stanfordnlp/pyreft/blob/main/
 pyreft/interventions.py#L85) (Constant LoReFT Intervention) which is even more
 parameter-efficient than the original LoReFT described in the paper: ```python
 import torch import transformers from pyreft import ( get_reft_model,
 ReftConfig, ConsreftIntervention ) # loading huggingface model
 model_name_or_path = "yahma/llama-7b-hf" model =
 transformers.AutoModelForCausalLM.from_pretrained( model_name_or_path,
@@ -100,27 +102,29 @@
 cognitive science. We also develop a wide variety of educational materials on
 NLP and many tools for the community to use, including the Stanza toolkit which
 processes text in over 60 human languages.""" ``` We successfully compress the
 text into 4,097 parameters! We perform more rigious memorisation test like this
 one in [ReFT Interp](https://github.com/frankaging/pyreft/tree/main/examples/
 memorisation). You can do ReFT with any language modeling tasks or SFT. Check
 out our [`examples`](https://github.com/frankaging/pyreft/tree/main/examples)
-folder! **You can train a 7B chat-model as good as ChatGPT-3.5-1103 under 18
-mins with a single A100 GPU + ReFT** by following steps here [`train.py`]
-(https://github.com/frankaging/pyreft/blob/main/examples/loreft/train.py). ##
-Loading our 18 min-cooked `Loreft1k-Llama-2-7b-hf` from HuggingFace For full
-tutorial, please take a look at [`chat_model.ipynb`](https://github.com/
-frankaging/pyreft/blob/main/examples/chat/chat_model.ipynb). Loading the base
-LM first: ```py import torch, transformers from pyreft import ( ReftModel,
-get_intervention_locations ) prompt_no_input_template = """Below is an
-instruction that \ describes a task. Write a response that appropriately \
-completes the request. ### Instruction: %s ### Response: """ device = "cuda" if
-torch.cuda.is_available() else "cpu" model_name_or_path = "meta-llama/Llama-2-
-7b-hf" reft_model_name_or_path = "zhengxuanzenwu/Loreft1k-Llama-2-7b-hf"
-tokenizer = transformers.AutoTokenizer.from_pretrained( model_name_or_path,
+folder! **You can train a 7B chat-model close to ChatGPT-3.5-1103 (81.9 v.s.
+86.3 Alpaca-eval scores) under 18 mins with a single A100 GPU + ReFT** by
+following steps here [`train.py`](https://github.com/frankaging/pyreft/blob/
+main/examples/loreft/train.py) training Llama-2 with the [Ultrafeedback
+dataset](https://arxiv.org/abs/2310.01377). ## Loading our 18 min-cooked
+`Loreft1k-Llama-2-7b-hf` from HuggingFace For full tutorial, please take a look
+at [`chat_model.ipynb`](https://github.com/frankaging/pyreft/blob/main/
+examples/chat/chat_model.ipynb). Loading the base LM first: ```py import torch,
+transformers from pyreft import ( ReftModel, get_intervention_locations )
+prompt_no_input_template = """Below is an instruction that \ describes a task.
+Write a response that appropriately \ completes the request. ### Instruction:
+%s ### Response: """ device = "cuda" if torch.cuda.is_available() else "cpu"
+model_name_or_path = "meta-llama/Llama-2-7b-hf" reft_model_name_or_path =
+"zhengxuanzenwu/Loreft1k-Llama-2-7b-hf" tokenizer =
+transformers.AutoTokenizer.from_pretrained( model_name_or_path,
 model_max_length=2048, padding_side="right", use_fast=False)
 tokenizer.pad_token = tokenizer.unk_token model =
 transformers.AutoModelForCausalLM.from_pretrained( model_name_or_path,
 torch_dtype=torch.bfloat16, device_map=device) ``` Then, loading ReFT
 artifacts: ```py reft_model = ReftModel.load( "zhengxuanzenwu/Loreft1k-Llama-2-
 7b-hf", model, from_huggingface_hub=True) reft_model.set_device(device) ```
 Start chatting with it: ```py instruction = "Tell me about the NLP Group at
```

### Comparing `pyreft-0.0.1/setup.py` & `pyreft-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Read the content of the requirements.txt file
 with open('requirements.txt', 'r', encoding='utf-8') as f:
     requirements = f.read().splitlines()
 
 setup(
     name="pyreft",
-    version="0.0.1",
+    version="0.0.2",
     description="REFT: Representation Finetuning for Language Models",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/stanfordnlp/reft",
     author="Zhengxuan Wu",
     author_email="wuzhengx@stanford.edu",
     license="Apache License 2.0",
@@ -27,8 +27,8 @@
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
     ],
-)
+)
```

