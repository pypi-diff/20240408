# Comparing `tmp/curated-transformers-2.0.0.dev0.tar.gz` & `tmp/curated-transformers-2.0.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curated-transformers-2.0.0.dev0.tar", last modified: Thu Oct  5 12:14:17 2023, max compression
+gzip compressed data, was "curated-transformers-2.0.0.dev1.tar", last modified: Mon Apr  8 11:39:52 2024, max compression
```

## Comparing `curated-transformers-2.0.0.dev0.tar` & `curated-transformers-2.0.0.dev1.tar`

### file list

```diff
@@ -1,229 +1,241 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-10-05 12:14:17.270802 curated-transformers-2.0.0.dev0/
--rw-r--r--   0 vsts      (1001) docker     (127)     1088 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)      116 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)     5279 2023-10-05 12:14:17.270802 curated-transformers-2.0.0.dev0/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     4606 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-10-05 12:14:17.250801 curated-transformers-2.0.0.dev0/curated_transformers/
--rw-r--r--   0 vsts      (1001) docker     (127)      533 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      757 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/_compat.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-10-05 12:14:17.250801 curated-transformers-2.0.0.dev0/curated_transformers/generation/
--rw-r--r--   0 vsts      (1001) docker     (127)     1346 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/generation/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2685 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/generation/auto_generator.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4000 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/generation/config.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3787 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/generation/default_generator.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1962 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/generation/dolly_v2.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1200 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/generation/falcon.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4303 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/generation/generator.py
--rw-r--r--   0 vsts      (1001) docker     (127)      791 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/generation/generator_wrapper.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1756 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/generation/hf_hub.py
--rw-r--r--   0 vsts      (1001) docker     (127)      753 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/generation/llama.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6591 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/generation/logits.py
--rw-r--r--   0 vsts      (1001) docker     (127)      631 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/generation/mpt.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4827 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/generation/state.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2794 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/generation/stop_conditions.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2105 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/generation/string_generator.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-10-05 12:14:17.254801 curated-transformers-2.0.0.dev0/curated_transformers/layers/
--rw-r--r--   0 vsts      (1001) docker     (127)     1335 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/layers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4055 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/layers/activations.py
--rw-r--r--   0 vsts      (1001) docker     (127)    35160 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/layers/attention.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2848 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/layers/cache.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10683 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/layers/embeddings.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3174 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/layers/feedforward.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1522 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/layers/normalization.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16063 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/layers/transformer.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-10-05 12:14:17.254801 curated-transformers-2.0.0.dev0/curated_transformers/models/
--rw-r--r--   0 vsts      (1001) docker     (127)     1921 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/models/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-10-05 12:14:17.254801 curated-transformers-2.0.0.dev0/curated_transformers/models/albert/
--rw-r--r--   0 vsts      (1001) docker     (127)      105 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/models/albert/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3093 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/models/albert/_hf.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4484 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/models/albert/config.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4177 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/models/albert/encoder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3650 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/models/albert/layer_group.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7766 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/models/auto_model.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-10-05 12:14:17.254801 curated-transformers-2.0.0.dev0/curated_transformers/models/bert/
--rw-r--r--   0 vsts      (1001) docker     (127)       64 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/models/bert/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3155 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/models/bert/_hf.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3473 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/models/bert/config.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4995 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/models/bert/encoder.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-10-05 12:14:17.254801 curated-transformers-2.0.0.dev0/curated_transformers/models/camembert/
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/models/camembert/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      831 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/models/camembert/encoder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3729 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/models/config.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-10-05 12:14:17.254801 curated-transformers-2.0.0.dev0/curated_transformers/models/falcon/
--rw-r--r--   0 vsts      (1001) docker     (127)      147 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/models/falcon/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5110 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/models/falcon/_hf.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2455 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/models/falcon/causal_lm.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3988 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/models/falcon/config.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6621 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/models/falcon/decoder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5637 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/models/falcon/layer.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-10-05 12:14:17.258802 curated-transformers-2.0.0.dev0/curated_transformers/models/gpt_neox/
--rw-r--r--   0 vsts      (1001) docker     (127)      109 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/models/gpt_neox/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2358 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/models/gpt_neox/_hf.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2419 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/models/gpt_neox/causal_lm.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3796 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/models/gpt_neox/config.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5466 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/models/gpt_neox/decoder.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-10-05 12:14:17.258802 curated-transformers-2.0.0.dev0/curated_transformers/models/hf_hub/
--rw-r--r--   0 vsts      (1001) docker     (127)       29 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/models/hf_hub/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3191 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/models/hf_hub/conversion.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8184 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/models/hf_hub/mixin.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-10-05 12:14:17.258802 curated-transformers-2.0.0.dev0/curated_transformers/models/llama/
--rw-r--r--   0 vsts      (1001) docker     (127)      103 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/models/llama/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2559 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/models/llama/_hf.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2507 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/models/llama/causal_lm.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3637 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/models/llama/config.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5729 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/models/llama/decoder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5468 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/models/module.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-10-05 12:14:17.258802 curated-transformers-2.0.0.dev0/curated_transformers/models/mpt/
--rw-r--r--   0 vsts      (1001) docker     (127)       97 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/models/mpt/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2412 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/models/mpt/_hf.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3781 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/models/mpt/causal_lm.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3395 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/models/mpt/config.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5205 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/models/mpt/decoder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2693 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/models/output.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-10-05 12:14:17.258802 curated-transformers-2.0.0.dev0/curated_transformers/models/roberta/
--rw-r--r--   0 vsts      (1001) docker     (127)       70 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/models/roberta/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3100 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/models/roberta/_hf.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1995 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/models/roberta/config.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3406 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/models/roberta/embeddings.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5023 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/models/roberta/encoder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4187 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/models/transformer.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-10-05 12:14:17.258802 curated-transformers-2.0.0.dev0/curated_transformers/models/xlm_roberta/
--rw-r--r--   0 vsts      (1001) docker     (127)       33 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/models/xlm_roberta/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      834 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/models/xlm_roberta/encoder.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-10-05 12:14:17.258802 curated-transformers-2.0.0.dev0/curated_transformers/quantization/
--rw-r--r--   0 vsts      (1001) docker     (127)      163 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/quantization/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-10-05 12:14:17.258802 curated-transformers-2.0.0.dev0/curated_transformers/quantization/bnb/
--rw-r--r--   0 vsts      (1001) docker     (127)      183 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/quantization/bnb/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2558 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/quantization/bnb/config.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5987 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/quantization/bnb/impl.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1118 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/quantization/helpers.py
--rw-r--r--   0 vsts      (1001) docker     (127)      676 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/quantization/quantizable.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-10-05 12:14:17.258802 curated-transformers-2.0.0.dev0/curated_transformers/repository/
--rw-r--r--   0 vsts      (1001) docker     (127)      419 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/repository/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1050 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/repository/_hf.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1767 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/repository/file.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3221 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/repository/fsspec.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3314 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/repository/hf_hub.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9183 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/repository/repository.py
--rw-r--r--   0 vsts      (1001) docker     (127)      605 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/semver.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-10-05 12:14:17.262802 curated-transformers-2.0.0.dev0/curated_transformers/tests/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      588 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/compat.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3332 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/conftest.py
--rw-r--r--   0 vsts      (1001) docker     (127)      133 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/enable_gpu.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-10-05 12:14:17.262802 curated-transformers-2.0.0.dev0/curated_transformers/tests/generation/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/generation/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      933 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/generation/test_auto_generator.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5058 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/generation/test_dolly_v2.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4514 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/generation/test_falcon.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5152 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/generation/test_generic.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5066 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/generation/test_logits.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2954 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/generation/test_stop.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-10-05 12:14:17.262802 curated-transformers-2.0.0.dev0/curated_transformers/tests/layers/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/layers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9040 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/layers/test_attention.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7176 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/layers/test_embeddings.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-10-05 12:14:17.262802 curated-transformers-2.0.0.dev0/curated_transformers/tests/models/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/models/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-10-05 12:14:17.262802 curated-transformers-2.0.0.dev0/curated_transformers/tests/models/albert/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/models/albert/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2330 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/models/albert/test_encoder.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-10-05 12:14:17.262802 curated-transformers-2.0.0.dev0/curated_transformers/tests/models/bert/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/models/bert/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2116 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/models/bert/test_encoder.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-10-05 12:14:17.262802 curated-transformers-2.0.0.dev0/curated_transformers/tests/models/camembert/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/models/camembert/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2166 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/models/camembert/test_encoder.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-10-05 12:14:17.262802 curated-transformers-2.0.0.dev0/curated_transformers/tests/models/falcon/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/models/falcon/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5639 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/models/falcon/test_decoder.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-10-05 12:14:17.262802 curated-transformers-2.0.0.dev0/curated_transformers/tests/models/gpt_neox/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/models/gpt_neox/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2271 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/models/gpt_neox/test_causal_lm.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2659 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/models/gpt_neox/test_decoder.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-10-05 12:14:17.262802 curated-transformers-2.0.0.dev0/curated_transformers/tests/models/llama/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/models/llama/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2442 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/models/llama/test_causal_lm.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2399 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/models/llama/test_decoder.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-10-05 12:14:17.262802 curated-transformers-2.0.0.dev0/curated_transformers/tests/models/mpt/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/models/mpt/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2129 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/models/mpt/test_causal_lm.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2598 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/models/mpt/test_decoder.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-10-05 12:14:17.266802 curated-transformers-2.0.0.dev0/curated_transformers/tests/models/roberta/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/models/roberta/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2146 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/models/roberta/test_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3081 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/models/test_auto_models.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4029 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/models/test_hf_hub.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13526 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/models/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-10-05 12:14:17.266802 curated-transformers-2.0.0.dev0/curated_transformers/tests/models/xlm_roberta/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/models/xlm_roberta/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2151 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/models/xlm_roberta/test_encoder.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-10-05 12:14:17.266802 curated-transformers-2.0.0.dev0/curated_transformers/tests/quantization/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/quantization/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3736 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/quantization/test_generation.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-10-05 12:14:17.266802 curated-transformers-2.0.0.dev0/curated_transformers/tests/tokenizers/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/tokenizers/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-10-05 12:14:17.266802 curated-transformers-2.0.0.dev0/curated_transformers/tests/tokenizers/legacy/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/tokenizers/legacy/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10775 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/tokenizers/legacy/test_bert_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10748 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/tokenizers/legacy/test_camembert_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)      734 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/tokenizers/legacy/test_llama_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10809 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/tokenizers/legacy/test_roberta_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10557 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/tokenizers/legacy/test_xlmr_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4690 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/tokenizers/legacy/toy-merges.txt
--rw-r--r--   0 vsts      (1001) docker     (127)    14493 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/tokenizers/legacy/toy-vocab.json
--rw-r--r--   0 vsts      (1001) docker     (127)   253270 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/tokenizers/legacy/toy.model
--rw-r--r--   0 vsts      (1001) docker     (127)     4968 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/tokenizers/legacy/toy.wordpieces
--rw-r--r--   0 vsts      (1001) docker     (127)     1419 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/tokenizers/test_auto_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1748 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/tokenizers/test_chunks.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1845 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/tokenizers/test_hf_hub.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3856 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/tokenizers/test_tokenizer.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-10-05 12:14:17.266802 curated-transformers-2.0.0.dev0/curated_transformers/tests/tokenizers/toy-roberta/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/tokenizers/toy-roberta/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    30593 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/tokenizers/toy-roberta/tokenizer.json
--rw-r--r--   0 vsts      (1001) docker     (127)     1939 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/tokenizers/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-10-05 12:14:17.266802 curated-transformers-2.0.0.dev0/curated_transformers/tests/util/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/util/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2640 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/util/test_dataclass.py
--rw-r--r--   0 vsts      (1001) docker     (127)      483 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tests/utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-10-05 12:14:17.270802 curated-transformers-2.0.0.dev0/curated_transformers/tokenizers/
--rw-r--r--   0 vsts      (1001) docker     (127)      370 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tokenizers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2924 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tokenizers/_hf_compat.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4932 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tokenizers/auto_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2661 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tokenizers/chunks.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4980 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tokenizers/hf_hub.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-10-05 12:14:17.270802 curated-transformers-2.0.0.dev0/curated_transformers/tokenizers/legacy/
--rw-r--r--   0 vsts      (1001) docker     (127)      812 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tokenizers/legacy/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2325 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tokenizers/legacy/_fairseq.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2903 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tokenizers/legacy/bbpe_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12006 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tokenizers/legacy/bert_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4508 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tokenizers/legacy/camembert_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7336 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tokenizers/legacy/legacy_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3011 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tokenizers/legacy/llama_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4255 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tokenizers/legacy/roberta_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2287 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tokenizers/legacy/sentencepiece_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3230 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tokenizers/legacy/wordpiece_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4017 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tokenizers/legacy/xlmr_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13108 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tokenizers/tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)      221 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/tokenizers/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-10-05 12:14:17.270802 curated-transformers-2.0.0.dev0/curated_transformers/util/
--rw-r--r--   0 vsts      (1001) docker     (127)       54 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/util/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4974 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/util/dataclass.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1445 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/util/profile.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1208 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/util/pytorch.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-10-05 12:14:17.270802 curated-transformers-2.0.0.dev0/curated_transformers/util/serde/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/util/serde/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2730 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/util/serde/checkpoint.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7302 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/util/serde/load.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7231 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/curated_transformers/util/string.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-10-05 12:14:17.250801 curated-transformers-2.0.0.dev0/curated_transformers.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     5279 2023-10-05 12:14:17.000000 curated-transformers-2.0.0.dev0/curated_transformers.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     8823 2023-10-05 12:14:17.000000 curated-transformers-2.0.0.dev0/curated_transformers.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2023-10-05 12:14:17.000000 curated-transformers-2.0.0.dev0/curated_transformers.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)     1123 2023-10-05 12:14:17.000000 curated-transformers-2.0.0.dev0/curated_transformers.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      159 2023-10-05 12:14:17.000000 curated-transformers-2.0.0.dev0/curated_transformers.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       21 2023-10-05 12:14:17.000000 curated-transformers-2.0.0.dev0/curated_transformers.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2023-10-05 12:14:17.000000 curated-transformers-2.0.0.dev0/curated_transformers.egg-info/zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)      134 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)     1986 2023-10-05 12:14:17.274802 curated-transformers-2.0.0.dev0/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)      204 2023-10-05 12:14:02.000000 curated-transformers-2.0.0.dev0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.358737 curated-transformers-2.0.0.dev1/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1088 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      116 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)     5279 2024-04-08 11:39:52.358737 curated-transformers-2.0.0.dev1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     4606 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.286736 curated-transformers-2.0.0.dev1/curated_transformers/
+-rw-r--r--   0 vsts      (1001) docker     (127)      728 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      757 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/_compat.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.294736 curated-transformers-2.0.0.dev1/curated_transformers/generation/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1346 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/generation/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2685 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/generation/auto_generator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4000 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/generation/config.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3787 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/generation/default_generator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1962 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/generation/dolly_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1200 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/generation/falcon.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4303 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/generation/generator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      791 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/generation/generator_wrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1756 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/generation/hf_hub.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      753 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/generation/llama.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6591 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/generation/logits.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      631 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/generation/mpt.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4827 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/generation/state.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2794 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/generation/stop_conditions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2105 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/generation/string_generator.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.298736 curated-transformers-2.0.0.dev1/curated_transformers/layers/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1335 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/layers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4055 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/layers/activations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    35234 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/layers/attention.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1437 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/layers/cache.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10495 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/layers/embeddings.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3174 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/layers/feedforward.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1522 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/layers/normalization.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16063 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/layers/transformer.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.298736 curated-transformers-2.0.0.dev1/curated_transformers/models/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1921 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.302736 curated-transformers-2.0.0.dev1/curated_transformers/models/albert/
+-rw-r--r--   0 vsts      (1001) docker     (127)      105 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/albert/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4065 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/albert/_hf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4484 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/albert/config.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4481 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/albert/encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3650 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/albert/layer_group.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7766 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/auto_model.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.302736 curated-transformers-2.0.0.dev1/curated_transformers/models/bert/
+-rw-r--r--   0 vsts      (1001) docker     (127)       64 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/bert/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3528 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/bert/_hf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3473 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/bert/config.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5325 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/bert/encoder.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.302736 curated-transformers-2.0.0.dev1/curated_transformers/models/camembert/
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/camembert/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      643 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/camembert/_hf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1159 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/camembert/encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3729 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/config.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.306736 curated-transformers-2.0.0.dev1/curated_transformers/models/electra/
+-rw-r--r--   0 vsts      (1001) docker     (127)       36 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/electra/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3881 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/electra/_hf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1369 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/electra/encoder.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.306736 curated-transformers-2.0.0.dev1/curated_transformers/models/falcon/
+-rw-r--r--   0 vsts      (1001) docker     (127)      147 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/falcon/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9313 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/falcon/_hf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2770 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/falcon/causal_lm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3988 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/falcon/config.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6930 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/falcon/decoder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5677 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/falcon/layer.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.310736 curated-transformers-2.0.0.dev1/curated_transformers/models/gpt_neox/
+-rw-r--r--   0 vsts      (1001) docker     (127)      109 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/gpt_neox/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3763 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/gpt_neox/_hf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2737 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/gpt_neox/causal_lm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3796 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/gpt_neox/config.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5763 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/gpt_neox/decoder.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.310736 curated-transformers-2.0.0.dev1/curated_transformers/models/hf_hub/
+-rw-r--r--   0 vsts      (1001) docker     (127)       29 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/hf_hub/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11545 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/hf_hub/conversion.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8623 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/hf_hub/mixin.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.310736 curated-transformers-2.0.0.dev1/curated_transformers/models/llama/
+-rw-r--r--   0 vsts      (1001) docker     (127)      103 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/llama/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4236 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/llama/_hf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2819 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/llama/causal_lm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3637 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/llama/config.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6035 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/llama/decoder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5468 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/module.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.314736 curated-transformers-2.0.0.dev1/curated_transformers/models/mpt/
+-rw-r--r--   0 vsts      (1001) docker     (127)       97 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/mpt/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4259 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/mpt/_hf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4081 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/mpt/causal_lm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3444 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/mpt/config.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5505 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/mpt/decoder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2629 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/output.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.314736 curated-transformers-2.0.0.dev1/curated_transformers/models/roberta/
+-rw-r--r--   0 vsts      (1001) docker     (127)       70 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/roberta/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3718 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/roberta/_hf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1995 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/roberta/config.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3406 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/roberta/embeddings.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5330 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/roberta/encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4187 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/transformer.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.318736 curated-transformers-2.0.0.dev1/curated_transformers/models/xlm_roberta/
+-rw-r--r--   0 vsts      (1001) docker     (127)       33 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/xlm_roberta/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      646 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/xlm_roberta/_hf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1162 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/models/xlm_roberta/encoder.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.318736 curated-transformers-2.0.0.dev1/curated_transformers/quantization/
+-rw-r--r--   0 vsts      (1001) docker     (127)      163 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/quantization/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.318736 curated-transformers-2.0.0.dev1/curated_transformers/quantization/bnb/
+-rw-r--r--   0 vsts      (1001) docker     (127)      183 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/quantization/bnb/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2558 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/quantization/bnb/config.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5987 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/quantization/bnb/impl.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1118 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/quantization/helpers.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      676 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/quantization/quantizable.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.322736 curated-transformers-2.0.0.dev1/curated_transformers/repository/
+-rw-r--r--   0 vsts      (1001) docker     (127)      517 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/repository/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1050 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/repository/_hf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2105 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/repository/file.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4362 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/repository/fsspec.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11957 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/repository/hf_hub.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9625 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/repository/repository.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1490 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/repository/transaction.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      605 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/semver.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.322736 curated-transformers-2.0.0.dev1/curated_transformers/tests/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      588 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/compat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3349 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/conftest.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      133 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/enable_gpu.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.326737 curated-transformers-2.0.0.dev1/curated_transformers/tests/generation/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/generation/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      933 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/generation/test_auto_generator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5058 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/generation/test_dolly_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4514 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/generation/test_falcon.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5152 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/generation/test_generic.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5066 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/generation/test_logits.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2954 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/generation/test_stop.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.326737 curated-transformers-2.0.0.dev1/curated_transformers/tests/layers/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/layers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9040 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/layers/test_attention.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7236 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/layers/test_embeddings.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.330736 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.330736 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/albert/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/albert/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1821 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/albert/test_encoder.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.330736 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/bert/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/bert/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1611 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/bert/test_encoder.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.330736 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/camembert/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/camembert/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1651 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/camembert/test_encoder.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.330736 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/electra/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/electra/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      722 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/electra/test_encoder.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.330736 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/falcon/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/falcon/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5424 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/falcon/test_decoder.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.334736 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/gpt_neox/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/gpt_neox/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1961 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/gpt_neox/test_causal_lm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2300 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/gpt_neox/test_decoder.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.334736 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/llama/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/llama/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2267 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/llama/test_causal_lm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2229 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/llama/test_decoder.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.334736 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/mpt/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/mpt/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1976 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/mpt/test_causal_lm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2395 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/mpt/test_decoder.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.334736 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/roberta/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/roberta/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1635 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/roberta/test_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3081 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/test_auto_models.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4029 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/test_hf_hub.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14286 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.338737 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/xlm_roberta/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/xlm_roberta/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1639 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/models/xlm_roberta/test_encoder.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.338737 curated-transformers-2.0.0.dev1/curated_transformers/tests/quantization/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/quantization/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3736 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/quantization/test_generation.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.338737 curated-transformers-2.0.0.dev1/curated_transformers/tests/repository/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/repository/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2648 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/repository/test_hf_hub.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.342737 curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.346737 curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/legacy/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/legacy/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10775 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/legacy/test_bert_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10748 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/legacy/test_camembert_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      653 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/legacy/test_electra_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      734 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/legacy/test_llama_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10809 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/legacy/test_roberta_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10557 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/legacy/test_xlmr_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4690 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/legacy/toy-merges.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)    14493 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/legacy/toy-vocab.json
+-rw-r--r--   0 vsts      (1001) docker     (127)   253270 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/legacy/toy.model
+-rw-r--r--   0 vsts      (1001) docker     (127)     4968 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/legacy/toy.wordpieces
+-rw-r--r--   0 vsts      (1001) docker     (127)     1419 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/test_auto_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1748 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/test_chunks.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1930 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/test_hf_hub.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3856 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/test_tokenizer.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.346737 curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/toy-roberta/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/toy-roberta/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    30593 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/toy-roberta/tokenizer.json
+-rw-r--r--   0 vsts      (1001) docker     (127)     1939 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.346737 curated-transformers-2.0.0.dev1/curated_transformers/tests/util/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/util/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      483 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tests/utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.350737 curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/
+-rw-r--r--   0 vsts      (1001) docker     (127)      370 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2924 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/_hf_compat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4904 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/auto_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2661 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/chunks.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4980 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/hf_hub.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.354737 curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/legacy/
+-rw-r--r--   0 vsts      (1001) docker     (127)      812 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/legacy/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2325 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/legacy/_fairseq.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2903 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/legacy/bbpe_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12006 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/legacy/bert_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4508 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/legacy/camembert_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7320 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/legacy/legacy_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3011 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/legacy/llama_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4255 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/legacy/roberta_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2287 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/legacy/sentencepiece_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3230 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/legacy/wordpiece_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4017 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/legacy/xlmr_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13473 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      221 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.354737 curated-transformers-2.0.0.dev1/curated_transformers/util/
+-rw-r--r--   0 vsts      (1001) docker     (127)       54 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/util/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1445 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/util/profile.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1208 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/util/pytorch.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.354737 curated-transformers-2.0.0.dev1/curated_transformers/util/serde/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/util/serde/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2730 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/util/serde/checkpoint.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7302 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/util/serde/load.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7231 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/curated_transformers/util/string.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 11:39:52.354737 curated-transformers-2.0.0.dev1/curated_transformers.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     5279 2024-04-08 11:39:52.000000 curated-transformers-2.0.0.dev1/curated_transformers.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     9297 2024-04-08 11:39:52.000000 curated-transformers-2.0.0.dev1/curated_transformers.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-08 11:39:52.000000 curated-transformers-2.0.0.dev1/curated_transformers.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)     1123 2024-04-08 11:39:52.000000 curated-transformers-2.0.0.dev1/curated_transformers.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      159 2024-04-08 11:39:52.000000 curated-transformers-2.0.0.dev1/curated_transformers.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       21 2024-04-08 11:39:52.000000 curated-transformers-2.0.0.dev1/curated_transformers.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-08 11:39:52.000000 curated-transformers-2.0.0.dev1/curated_transformers.egg-info/zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)      134 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)     1986 2024-04-08 11:39:52.358737 curated-transformers-2.0.0.dev1/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)      204 2024-04-08 11:39:42.000000 curated-transformers-2.0.0.dev1/setup.py
```

### Comparing `curated-transformers-2.0.0.dev0/LICENSE` & `curated-transformers-2.0.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/PKG-INFO` & `curated-transformers-2.0.0.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curated-transformers
-Version: 2.0.0.dev0
+Version: 2.0.0.dev1
 Summary: A PyTorch library of transformer models and components
 Home-page: https://github.com/explosion/curated-transformers
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `curated-transformers-2.0.0.dev0/README.md` & `curated-transformers-2.0.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/_compat.py` & `curated-transformers-2.0.0.dev1/curated_transformers/_compat.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/generation/__init__.py` & `curated-transformers-2.0.0.dev1/curated_transformers/generation/__init__.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/generation/auto_generator.py` & `curated-transformers-2.0.0.dev1/curated_transformers/generation/auto_generator.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/generation/config.py` & `curated-transformers-2.0.0.dev1/curated_transformers/generation/config.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/generation/default_generator.py` & `curated-transformers-2.0.0.dev1/curated_transformers/generation/default_generator.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/generation/dolly_v2.py` & `curated-transformers-2.0.0.dev1/curated_transformers/generation/dolly_v2.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/generation/falcon.py` & `curated-transformers-2.0.0.dev1/curated_transformers/generation/falcon.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/generation/generator.py` & `curated-transformers-2.0.0.dev1/curated_transformers/generation/generator.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/generation/generator_wrapper.py` & `curated-transformers-2.0.0.dev1/curated_transformers/generation/generator_wrapper.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/generation/hf_hub.py` & `curated-transformers-2.0.0.dev1/curated_transformers/generation/hf_hub.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/generation/llama.py` & `curated-transformers-2.0.0.dev1/curated_transformers/generation/llama.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/generation/logits.py` & `curated-transformers-2.0.0.dev1/curated_transformers/generation/logits.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/generation/mpt.py` & `curated-transformers-2.0.0.dev1/curated_transformers/generation/mpt.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/generation/state.py` & `curated-transformers-2.0.0.dev1/curated_transformers/generation/state.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/generation/stop_conditions.py` & `curated-transformers-2.0.0.dev1/curated_transformers/generation/stop_conditions.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/generation/string_generator.py` & `curated-transformers-2.0.0.dev1/curated_transformers/generation/string_generator.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/layers/__init__.py` & `curated-transformers-2.0.0.dev1/curated_transformers/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/layers/activations.py` & `curated-transformers-2.0.0.dev1/curated_transformers/layers/activations.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/layers/attention.py` & `curated-transformers-2.0.0.dev1/curated_transformers/layers/attention.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 import torch
 import torch.nn.functional as F
 from torch import Tensor
 from torch.nn import Dropout, Linear, Module
 
 from ..semver import Default, FutureMandatory
-from ..util.dataclass import DataclassAsDict
 from .cache import KeyValueCache
 from .embeddings import QueryKeyRotaryEmbeddings
 
 _TORCH_SDP: ContextVar[bool] = ContextVar("torch_sdp", default=False)
 
 
 @contextmanager
@@ -43,15 +42,15 @@
     try:
         yield
     finally:
         _TORCH_SDP.reset(token)
 
 
 @dataclass
-class AttentionMask(DataclassAsDict):
+class AttentionMask:
     """
     Mask for attention calculation. Sequence elements for which the
     corresponding mask element is set to ``False`` are ignored during
     attention calculation.
 
     :param bool_mask:
         The boolean mask.
@@ -70,41 +69,14 @@
             self.bool_mask = bool_mask
         else:
             raise ValueError(
                 "The attention mask must be a tensor of shape [batch, key_len] or "
                 "[batch_len, heads, query_len, key_len]"
             )
 
-        self.__post_init__()
-
-    @classmethod
-    def jit_rewrap(
-        cls: Type["AttentionMask"],
-        attention_mask: Union["AttentionMask", Dict[str, Tensor]],
-    ) -> "AttentionMask":
-        """
-        Rewrap TorchScript dictionary conversion of an attention mask
-        as an ``AttentionMask``.
-
-        :param attention_mask:
-            The attention mask or its dictionary representation. If the
-            value is an ``AttentionMask``, the value will be returned as-is.
-        :returns:
-            The attention mask.
-        """
-        if isinstance(attention_mask, AttentionMask):
-            return attention_mask
-
-        bool_mask = attention_mask.get("bool_mask")
-        if bool_mask is None:
-            raise ValueError(
-                "Attention mask is not of the `AttentionMask` type, nor a dict with 'bool_mask'."
-            )
-        return AttentionMask(bool_mask=bool_mask)
-
     def apply_logit_mask(self, input: Tensor) -> Tensor:
         """
         Use the attention mask to mask attention logits.
 
         :param input:
             Attention logits to apply the mask to.
 
@@ -642,14 +614,15 @@
     def forward(
         self,
         *,
         query: Tensor,
         key: Tensor,
         value: Tensor,
         attention_mask: AttentionMask,
+        use_causal_mask: bool,
     ) -> Tensor:
         """
         Apply attention scores to the given key, query and value.
 
         Sequence elements that are marked with ``False`` in the attention mask
         are ignored by the attention mechanism (if a mask is provided).
 
@@ -665,14 +638,16 @@
             Value tensor.
 
             *Shape:* ``(batch_size, heads, seq_len, width)``
         :param attention_mask:
 
             Attention mask. Sequence elements for which the corresponding mask
             element is set to ``False`` are ignored in attention.
+        :param use_causal_mask:
+            Mask out succeeding sequence elements when ``True``.
         :returns:
             Attention values.
 
             *Shape:* ``(batch_size, heads, seq_len, width)``
         """
         ...
 
@@ -708,44 +683,78 @@
     def forward(
         self,
         *,
         query: Tensor,
         key: Tensor,
         value: Tensor,
         attention_mask: AttentionMask,
+        use_causal_mask: bool,
     ) -> Tensor:
+        combined_mask = attention_mask
+        if use_causal_mask:
+            causal_mask = create_causal_mask(query, key)
+            combined_mask = combined_mask.merge_mask(causal_mask)
+
         if _TORCH_SDP.get():
-            attn_mask = attention_mask.logit_mask(query.dtype)
+            logit_mask = combined_mask.logit_mask(query.dtype)
 
             # Add AliBi to the logit mask
             if self.linear_biases is not None:
                 biases = self.linear_biases.calculate_biases(key.size(-2)).to(
                     dtype=query.dtype, device=query.device
                 )
-                bool_mask = attention_mask.bool_mask
-                attn_mask = torch.where(bool_mask, biases, attn_mask)
+                bool_mask = combined_mask.bool_mask
+                logit_mask = torch.where(bool_mask, biases, logit_mask)
 
             # We can't pass a bool mask, because it is currently broken:
             # https://github.com/pytorch/pytorch/issues/103749
-            return F.scaled_dot_product_attention(
+            attn_values = F.scaled_dot_product_attention(
                 query=query,
                 key=key,
                 value=value,
-                attn_mask=attn_mask,
+                attn_mask=logit_mask,
                 dropout_p=self.dropout_prob if self.training else 0.0,
             )
+
+            # Torch SDP returns NaNs for pieces where every is piece masked out.
+            # These errors propagate because zero attention times NaN is NaN.
+            # Since the representations of these pieces don't matter anyway, we
+            # will just zero them out.
+            #
+            # One issue is that values have shape
+            #
+            # [batch_len, n_heads, key_len, hidden_size]
+            #
+            # whereas masks have the shape
+            #
+            # [batch_len, 1, query_len, key_len]
+            #
+            # So we can only do this when we have attention masks where
+            # the query length it not specified, which are typically 'pure'
+            # attention masks (not causal maskes or combined masks):
+            #
+            # [batch_len, 1, 1, key_len]
+            #
+            # Doing this properly requires a redesign of our AttentionMask
+            # class.
+            assert (
+                attention_mask.bool_mask.size(-2) == 1
+            ), "Torch SDP does not support attention masks with non-broadcastable query length yet"
+            return torch.where(
+                attention_mask.bool_mask.transpose(-1, -2), attn_values, 0.0
+            )
         else:
             width = key.shape[-1]
             attn_scores = query @ key.transpose(-2, -1)
             attn_scores /= math.sqrt(width)
 
             if self.linear_biases is not None:
                 attn_scores = self.linear_biases(attention_scores=attn_scores)
 
-            attn_scores = attention_mask.apply_logit_mask(attn_scores)
+            attn_scores = combined_mask.apply_logit_mask(attn_scores)
             attn_weights = attn_scores.softmax(dim=-1)
             attn_values = self.dropout(attn_weights @ value)
 
             return attn_values
 
 
 class SelfAttention(Module):
@@ -878,53 +887,42 @@
 
             *Shape:* ``(batch_size, seq_len)``
         :returns:
             Layer output.
 
             *Shape:* ``(batch_size, seq_len, width)``
         """
-        # The attention mask is converted to a dict for traced models. Rewrap as
-        # AttentionMask to get validation and utility methods.
-        attention_mask = AttentionMask.jit_rewrap(attention_mask)
-
         query, key, value = self._query_key_value(input)
 
         if self.rotary_embeds is not None:
             query, key = self.rotary_embeds(
                 query=query, key=key, cache=cache, positions=positions
             )
 
-        # The key-value is converted to a dict for traced models. Rewrap as
-        # KeyValueCache to get validation and utility methods.
-        cache = KeyValueCache.jit_rewrap(cache)
         if cache is not None:
             cache_k = cache.key
             cache_v = cache.value
 
             key = torch.cat([cache_k, key], dim=-2)
             value = torch.cat([cache_v, value], dim=-2)
 
-        combined_mask = attention_mask
-        if use_causal_mask:
-            causal_mask = create_causal_mask(query, key)
-            combined_mask = combined_mask.merge_mask(causal_mask)
-
         attn = self.attention_scorer(
             query=query,
             key=key,
             value=value,
-            attention_mask=combined_mask,
+            attention_mask=attention_mask,
+            use_causal_mask=use_causal_mask,
         )
 
         attn = combine_heads(attn)
 
         output = self.output(attn)
 
         if store_cache:
-            return output, KeyValueCache(key, value)
+            return output, KeyValueCache(key=key, value=value)
         else:
             return output, None
 
     def _query_key_value(self, input: Tensor) -> Tuple[Tensor, Tensor, Tensor]:
         """
         Compute query, key and value representations for the input.
```

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/layers/embeddings.py` & `curated-transformers-2.0.0.dev1/curated_transformers/layers/embeddings.py`

 * *Files 1% similar despite different names*

```diff
@@ -274,18 +274,14 @@
             Query and key with the rotary embeddings applied.
 
             *Shape:* ``(batch_size, head, seq_len, width_per_head)``
         """
         head_width = self.head_width
         rotary_width = self.rotary_width
 
-        # The key-value is converted to a dict for traced models. Rewrap as
-        # KeyValueCache to get validation and utility methods.
-        cache = KeyValueCache.jit_rewrap(cache)
-
         # If a cache was provided, but no positions, assume that the
         # positions of the current batch continue from the cache.
         if cache is not None and positions is None:
             cache_len = cache.key.size(-2)
             seq_len = key.size(-2)
             positions = torch.arange(
                 cache_len,
```

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/layers/feedforward.py` & `curated-transformers-2.0.0.dev1/curated_transformers/layers/feedforward.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/layers/normalization.py` & `curated-transformers-2.0.0.dev1/curated_transformers/layers/normalization.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/layers/transformer.py` & `curated-transformers-2.0.0.dev1/curated_transformers/layers/transformer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/models/__init__.py` & `curated-transformers-2.0.0.dev1/curated_transformers/models/__init__.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/models/albert/config.py` & `curated-transformers-2.0.0.dev1/curated_transformers/models/albert/config.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/models/albert/encoder.py` & `curated-transformers-2.0.0.dev1/curated_transformers/models/albert/encoder.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,23 +10,23 @@
     EmbeddingLayerNorms,
     TransformerEmbeddings,
 )
 from ..hf_hub import FromHFHub
 from ..hf_hub.conversion import state_dict_from_hf, state_dict_to_hf
 from ..module import EncoderModule
 from ..output import ModelOutput
-from ._hf import HF_PARAM_KEY_TRANSFORMS, convert_hf_config
+from ._hf import HF_PARAM_KEY_TRANSFORMS, _config_from_hf, _config_to_hf
 from .config import ALBERTConfig
 from .layer_group import ALBERTLayerGroup
 
 # Only provided as typing.Self in Python 3.11+.
 Self = TypeVar("Self", bound="ALBERTEncoder")
 
 
-class ALBERTEncoder(EncoderModule[ALBERTConfig], FromHFHub):
+class ALBERTEncoder(EncoderModule[ALBERTConfig], FromHFHub[ALBERTConfig]):
     """
     ALBERT (`Lan et al., 2022`_) encoder.
 
     .. _Lan et al., 2022: https://arxiv.org/abs/1909.11942
     """
 
     def __init__(self, config: ALBERTConfig, *, device: Optional[torch.device] = None):
@@ -112,15 +112,23 @@
     @classmethod
     def state_dict_to_hf(
         cls: Type[Self], params: Mapping[str, Tensor]
     ) -> Mapping[str, Tensor]:
         return state_dict_to_hf(params, HF_PARAM_KEY_TRANSFORMS)
 
     @classmethod
+    def config_from_hf(cls, hf_config: Mapping[str, Any]) -> ALBERTConfig:
+        return _config_from_hf(hf_config)
+
+    @classmethod
+    def config_to_hf(cls, curated_config: ALBERTConfig) -> Mapping[str, Any]:
+        return _config_to_hf(curated_config)
+
+    @classmethod
     def from_hf_config(
         cls: Type[Self],
         *,
         hf_config: Any,
         device: Optional[torch.device] = None,
     ) -> Self:
-        config = convert_hf_config(hf_config)
+        config = cls.config_from_hf(hf_config)
         return cls(config, device=device)
```

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/models/albert/layer_group.py` & `curated-transformers-2.0.0.dev1/curated_transformers/models/albert/layer_group.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/models/auto_model.py` & `curated-transformers-2.0.0.dev1/curated_transformers/models/auto_model.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/models/bert/config.py` & `curated-transformers-2.0.0.dev1/curated_transformers/models/bert/config.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/models/bert/encoder.py` & `curated-transformers-2.0.0.dev1/curated_transformers/models/bert/encoder.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from functools import partial
-from typing import Any, Dict, Mapping, Optional, Tuple, Type, TypeVar
+from typing import Any, Dict, Mapping, Optional, Type, TypeVar
 
 import torch
 from torch import Tensor
 from torch.nn import Dropout, LayerNorm
 
 from ...layers.attention import (
     AttentionHeads,
@@ -19,29 +19,34 @@
     TransformerDropouts,
     TransformerEmbeddings,
     TransformerLayerNorms,
 )
 from ..hf_hub import FromHFHub
 from ..hf_hub.conversion import state_dict_from_hf, state_dict_to_hf
 from ..transformer import TransformerEncoder
-from ._hf import HF_PARAM_KEY_TRANSFORMS, convert_hf_config
+from ._hf import HF_PARAM_KEY_TRANSFORMS, _config_from_hf, _config_to_hf
 from .config import BERTConfig
 
 # Only provided as typing.Self in Python 3.11+.
 Self = TypeVar("Self", bound="BERTEncoder")
 
 
-class BERTEncoder(TransformerEncoder[BERTConfig], FromHFHub):
+class BERTEncoder(TransformerEncoder[BERTConfig], FromHFHub[BERTConfig]):
     """
     BERT (`Devlin et al., 2018`_) encoder.
 
     .. _Devlin et al., 2018 : https://arxiv.org/abs/1810.04805
     """
 
-    def __init__(self, config: BERTConfig, *, device: Optional[torch.device] = None):
+    def __init__(
+        self,
+        config: BERTConfig,
+        *,
+        device: Optional[torch.device] = None,
+    ):
         """
         Construct a BERT encoder.
 
         :param config:
             Encoder configuration.
         :param device:
             Device to which the module is to be moved.
@@ -126,15 +131,23 @@
     @classmethod
     def state_dict_to_hf(
         cls: Type[Self], params: Mapping[str, Tensor]
     ) -> Mapping[str, Tensor]:
         return state_dict_to_hf(params, HF_PARAM_KEY_TRANSFORMS)
 
     @classmethod
+    def config_from_hf(cls, hf_config: Mapping[str, Any]) -> BERTConfig:
+        return _config_from_hf(hf_config)
+
+    @classmethod
+    def config_to_hf(cls, curated_config: BERTConfig) -> Mapping[str, Any]:
+        return _config_to_hf(curated_config)
+
+    @classmethod
     def from_hf_config(
         cls: Type[Self],
         *,
         hf_config: Any,
         device: Optional[torch.device] = None,
     ) -> Self:
-        config = convert_hf_config(hf_config)
+        config = cls.config_from_hf(hf_config)
         return cls(config, device=device)
```

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/models/camembert/encoder.py` & `curated-transformers-2.0.0.dev1/curated_transformers/models/camembert/encoder.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-from typing import Any, Dict, Optional, Tuple
+from typing import Any, Dict, Mapping, Optional
 
 import torch
 
 from ..roberta.config import RoBERTaConfig
 from ..roberta.encoder import RoBERTaEncoder
+from ._hf import _config_from_hf, _config_to_hf
 
 
 class CamemBERTEncoder(RoBERTaEncoder):
     """
     CamemBERT (`Martin et al., 2020`_) encoder.
 
     .. _Martin et al., 2020: https://arxiv.org/abs/1911.03894
@@ -25,7 +26,15 @@
             The encoder.
         """
         super().__init__(config, device=device)
 
     @classmethod
     def is_supported(cls, config: Dict[str, Any]) -> bool:
         return config.get("model_type") == "camembert"
+
+    @classmethod
+    def config_from_hf(cls, hf_config: Mapping[str, Any]) -> RoBERTaConfig:
+        return _config_from_hf(hf_config)
+
+    @classmethod
+    def config_to_hf(cls, curated_config: RoBERTaConfig) -> Mapping[str, Any]:
+        return _config_to_hf(curated_config)
```

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/models/config.py` & `curated-transformers-2.0.0.dev1/curated_transformers/models/config.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/models/falcon/causal_lm.py` & `curated-transformers-2.0.0.dev1/curated_transformers/models/falcon/causal_lm.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,23 +4,25 @@
 from torch import Tensor
 from torch.nn import Linear
 
 from ...quantization.quantizable import Quantizable
 from ..hf_hub import FromHFHub
 from ..hf_hub.conversion import state_dict_from_hf, state_dict_to_hf
 from ..transformer import TransformerCausalLM
-from ._hf import CAUSAL_LM_HF_PARAM_KEY_TRANSFORMS, convert_hf_config
+from ._hf import CAUSAL_LM_HF_PARAM_KEY_TRANSFORMS, _config_from_hf, _config_to_hf
 from .config import FalconConfig
 from .decoder import FalconDecoder
 
 # Only provided as typing.Self in Python 3.11+.
 Self = TypeVar("Self", bound="FalconCausalLM")
 
 
-class FalconCausalLM(TransformerCausalLM[FalconConfig], FromHFHub, Quantizable):
+class FalconCausalLM(
+    TransformerCausalLM[FalconConfig], FromHFHub[FalconConfig], Quantizable
+):
     """
     Falcon (`Penedo et al., 2019`_) causal language model.
 
     .. _Penedo et al., 2019: https://arxiv.org/abs/2306.01116
     """
 
     def __init__(
@@ -59,20 +61,28 @@
     @classmethod
     def state_dict_to_hf(
         cls: Type[Self], params: Mapping[str, Tensor]
     ) -> Mapping[str, Tensor]:
         return state_dict_to_hf(params, CAUSAL_LM_HF_PARAM_KEY_TRANSFORMS)
 
     @classmethod
+    def config_from_hf(cls, hf_config: Mapping[str, Any]) -> FalconConfig:
+        return _config_from_hf(hf_config)
+
+    @classmethod
+    def config_to_hf(cls, curated_config: FalconConfig) -> Mapping[str, Any]:
+        return _config_to_hf(cls, curated_config)
+
+    @classmethod
     def from_hf_config(
         cls: Type[Self],
         *,
         hf_config: Any,
         device: Optional[torch.device] = None,
     ) -> Self:
-        config = convert_hf_config(hf_config)
+        config = cls.config_from_hf(hf_config)
         return cls(config, device=device)
 
     @classmethod
     def modules_to_not_quantize(cls) -> Set[str]:
         # Ignore the output embedding matrix.
         return {"output_embeddings"}
```

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/models/falcon/config.py` & `curated-transformers-2.0.0.dev1/curated_transformers/models/falcon/config.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/models/falcon/decoder.py` & `curated-transformers-2.0.0.dev1/curated_transformers/models/gpt_neox/decoder.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 import torch
 from torch import Tensor
 from torch.nn import Dropout, LayerNorm, ModuleList
 
 from ...layers.attention import (
     AttentionHeads,
-    AttentionLinearBiases,
     QkvMode,
     ScaledDotProductAttention,
     SelfAttention,
 )
 from ...layers.embeddings import QueryKeyRotaryEmbeddings
 from ...layers.feedforward import PointwiseFeedForward
 from ...layers.transformer import (
@@ -21,34 +20,33 @@
     TransformerDropouts,
     TransformerEmbeddings,
     TransformerLayerNorms,
 )
 from ..hf_hub import FromHFHub
 from ..hf_hub.conversion import state_dict_from_hf, state_dict_to_hf
 from ..transformer import TransformerDecoder
-from ._hf import DECODER_HF_PARAM_KEY_TRANSFORMS, convert_hf_config
-from .config import FalconConfig
-from .layer import OldFalconDecoderLayer
+from ._hf import DECODER_HF_PARAM_KEY_TRANSFORMS, _config_from_hf, _config_to_hf
+from .config import GPTNeoXConfig
 
 # Only provided as typing.Self in Python 3.11+.
-Self = TypeVar("Self", bound="FalconDecoder")
+Self = TypeVar("Self", bound="GPTNeoXDecoder")
 
 
-class FalconDecoder(TransformerDecoder[FalconConfig], FromHFHub):
+class GPTNeoXDecoder(TransformerDecoder[GPTNeoXConfig], FromHFHub):
     """
-    Falcon (`Penedo et al., 2019`_) decoder.
+    GPT-NeoX (`Black et al., 2022`_) decoder.
 
-    .. _Penedo et al., 2019: https://arxiv.org/abs/2306.01116
+    .. _Black et al., 2022: https://arxiv.org/abs/2204.06745
     """
 
     def __init__(
-        self, config: FalconConfig, *, device: Optional[torch.device] = None
+        self, config: GPTNeoXConfig, *, device: Optional[torch.device] = None
     ) -> None:
         """
-        Construct a Falcon decoder.
+        Construct a GPT-NeoX decoder.
 
         :param config:
             Decoder configuration.
         :param device:
             Device to which the module is to be moved.
         :returns:
             The decoder.
@@ -64,126 +62,96 @@
             layer_norms=EmbeddingLayerNorms(),
             n_pieces=config.embedding.n_pieces,
             n_positions=None,
             n_types=None,
             device=device,
         )
 
-        if config.new_decoder_architecture:
-            decoder_layer = partial(
-                self._create_new_decoder_architecture_layer, config, device
-            )
-        else:
-            decoder_layer = partial(
-                self._create_old_decoder_architecture_layer, config, device
+        hidden_width = config.layer.feedforward.hidden_width
+        n_attention_heads = config.layer.attention.n_query_heads
+        layer_norm = partial(
+            LayerNorm,
+            hidden_width,
+            config.layer.layer_norm_eps,
+            device=device,
+        )
+        if config.layer.attention.rotary_embeddings is None:
+            raise ValueError(
+                "GPT-NeoX attention config does not contain rotary embedding parameters"
             )
-
         self.layers = ModuleList(
-            [decoder_layer() for _ in range(config.layer.n_hidden_layers)]
+            [
+                DecoderLayer(
+                    attention_layer=SelfAttention(
+                        attention_heads=AttentionHeads.uniform(n_attention_heads),
+                        attention_scorer=ScaledDotProductAttention(
+                            dropout_prob=config.layer.attention.dropout_prob,
+                            linear_biases=None,
+                        ),
+                        hidden_width=hidden_width,
+                        qkv_mode=QkvMode.MERGED_SPLIT_BEFORE,
+                        rotary_embeds=QueryKeyRotaryEmbeddings(
+                            fraction=config.layer.attention.rotary_embeddings.rotary_fraction,
+                            base=config.layer.attention.rotary_embeddings.rotary_base,
+                            head_width=hidden_width // n_attention_heads,
+                        ),
+                        use_bias=config.layer.attention.use_bias,
+                        device=device,
+                    ),
+                    feed_forward_layer=PointwiseFeedForward(
+                        activation=config.layer.feedforward.activation.module(),
+                        hidden_width=hidden_width,
+                        intermediate_width=config.layer.feedforward.intermediate_width,
+                        use_bias=config.layer.feedforward.use_bias,
+                        use_gate=config.layer.feedforward.use_gate,
+                        device=device,
+                    ),
+                    dropouts=TransformerDropouts.layer_output_dropouts(
+                        config.layer.dropout_prob
+                    ),
+                    layer_norms=TransformerLayerNorms(
+                        attn_input_layer_norm=layer_norm(),
+                        ffn_input_layer_norm=layer_norm(),
+                    ),
+                    use_parallel_attention=config.layer.attention.use_parallel_attention,
+                )
+                for _ in range(config.layer.n_hidden_layers)
+            ]
         )
 
         self.output_layer_norm = LayerNorm(
-            config.layer.feedforward.hidden_width,
-            config.layer.layer_norm_eps,
-            device=device,
+            hidden_width, config.layer.layer_norm_eps, device=device
         )
 
     @classmethod
     def is_supported(cls: Type[Self], config: Dict[str, Any]) -> bool:
-        return config.get("model_type") in ("falcon", "RefinedWeb", "RefinedWebModel")
+        return config.get("model_type") == "gpt_neox"
 
     @classmethod
     def state_dict_from_hf(
         cls: Type[Self], params: Mapping[str, Tensor]
     ) -> Mapping[str, Tensor]:
         return state_dict_from_hf(params, DECODER_HF_PARAM_KEY_TRANSFORMS)
 
     @classmethod
     def state_dict_to_hf(
         cls: Type[Self], params: Mapping[str, Tensor]
     ) -> Mapping[str, Tensor]:
         return state_dict_to_hf(params, DECODER_HF_PARAM_KEY_TRANSFORMS)
 
     @classmethod
+    def config_from_hf(cls, hf_config: Mapping[str, Any]) -> GPTNeoXConfig:
+        return _config_from_hf(hf_config)
+
+    @classmethod
+    def config_to_hf(cls, curated_config: GPTNeoXConfig) -> Mapping[str, Any]:
+        return _config_to_hf(cls, curated_config)
+
+    @classmethod
     def from_hf_config(
         cls: Type[Self],
         *,
         hf_config: Any,
         device: Optional[torch.device] = None,
     ) -> Self:
-        config = convert_hf_config(hf_config)
+        config = cls.config_from_hf(hf_config)
         return cls(config, device=device)
-
-    def _create_old_decoder_architecture_layer(
-        self, config: FalconConfig, device: Optional[torch.device]
-    ):
-        return OldFalconDecoderLayer(config.layer, device=device)
-
-    def _create_new_decoder_architecture_layer(
-        self, config: FalconConfig, device: Optional[torch.device]
-    ):
-        if config.layer.attention.rotary_embeddings is None:
-            raise ValueError(
-                "Falcon attention config does not contain rotary embedding parameters"
-            )
-
-        hidden_width = config.layer.feedforward.hidden_width
-        layer_norm = partial(
-            LayerNorm,
-            hidden_width,
-            config.layer.layer_norm_eps,
-            device=device,
-        )
-        n_attention_heads = config.layer.attention.n_query_heads
-        attention_biases = (
-            AttentionLinearBiases(
-                n_attention_heads=config.layer.attention.n_query_heads,
-                is_causal=True,
-                is_inverted=True,
-            )
-            if config.layer.attention.use_alibi
-            else None
-        )
-        # Rotary embeddings are disabled when using ALiBi.
-        rotary_embeds = (
-            QueryKeyRotaryEmbeddings(
-                fraction=config.layer.attention.rotary_embeddings.rotary_fraction,
-                base=config.layer.attention.rotary_embeddings.rotary_base,
-                head_width=hidden_width // n_attention_heads,
-            )
-            if not config.layer.attention.use_alibi
-            else None
-        )
-        return DecoderLayer(
-            attention_layer=SelfAttention(
-                attention_heads=AttentionHeads.key_value_broadcast(
-                    n_query_heads=n_attention_heads,
-                    n_key_value_heads=config.layer.attention.n_key_value_heads,
-                ),
-                attention_scorer=ScaledDotProductAttention(
-                    dropout_prob=config.layer.attention.dropout_prob,
-                    linear_biases=attention_biases,
-                ),
-                hidden_width=hidden_width,
-                qkv_mode=QkvMode.MERGED_SPLIT_AFTER,
-                rotary_embeds=rotary_embeds,
-                use_bias=config.layer.attention.use_bias,
-                device=device,
-            ),
-            feed_forward_layer=PointwiseFeedForward(
-                activation=config.layer.feedforward.activation.module(),
-                hidden_width=hidden_width,
-                intermediate_width=config.layer.feedforward.intermediate_width,
-                use_bias=config.layer.feedforward.use_bias,
-                use_gate=config.layer.feedforward.use_gate,
-                device=device,
-            ),
-            dropouts=TransformerDropouts.parallel_attention_dropout(
-                config.layer.dropout_prob
-            ),
-            layer_norms=TransformerLayerNorms(
-                attn_input_layer_norm=layer_norm(),
-                ffn_input_layer_norm=layer_norm(),
-            ),
-            # The new decoder uses parallel attention unconditionally.
-            use_parallel_attention=True,
-        )
```

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/models/falcon/layer.py` & `curated-transformers-2.0.0.dev1/curated_transformers/models/falcon/layer.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,17 +69,19 @@
             ),
             hidden_width=hidden_width,
             attention_heads=AttentionHeads.key_value_broadcast(
                 n_query_heads=attention_config.n_query_heads,
                 n_key_value_heads=attention_config.n_key_value_heads,
             ),
             rotary_embeds=rotary_embeds,
-            qkv_mode=QkvMode.MERGED_SPLIT_AFTER
-            if attention_config.n_key_value_heads == 1
-            else QkvMode.MERGED_SPLIT_BEFORE,
+            qkv_mode=(
+                QkvMode.MERGED_SPLIT_AFTER
+                if attention_config.n_key_value_heads == 1
+                else QkvMode.MERGED_SPLIT_BEFORE
+            ),
             use_bias=attention_config.use_bias,
             device=device,
         )
         self.attn_output_dropout = torch.nn.Dropout(p=layer_config.dropout_prob)
         self.attn_layer_norm = torch.nn.LayerNorm(
             hidden_width, eps=layer_config.layer_norm_eps, device=device
         )
```

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/models/gpt_neox/causal_lm.py` & `curated-transformers-2.0.0.dev1/curated_transformers/models/gpt_neox/causal_lm.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,23 +4,25 @@
 from torch import Tensor
 from torch.nn import Linear
 
 from ...quantization import Quantizable
 from ..hf_hub import FromHFHub
 from ..hf_hub.conversion import state_dict_from_hf, state_dict_to_hf
 from ..transformer import TransformerCausalLM
-from ._hf import CAUSAL_LM_HF_PARAM_KEY_TRANSFORMS, convert_hf_config
+from ._hf import CAUSAL_LM_HF_PARAM_KEY_TRANSFORMS, _config_from_hf, _config_to_hf
 from .config import GPTNeoXConfig
 from .decoder import GPTNeoXDecoder
 
 # Only provided as typing.Self in Python 3.11+.
 Self = TypeVar("Self", bound="GPTNeoXCausalLM")
 
 
-class GPTNeoXCausalLM(TransformerCausalLM[GPTNeoXConfig], FromHFHub, Quantizable):
+class GPTNeoXCausalLM(
+    TransformerCausalLM[GPTNeoXConfig], FromHFHub[GPTNeoXConfig], Quantizable
+):
     """
     GPT-NeoX (`Black et al., 2022`_) causal language model.
 
     .. _Black et al., 2022: https://arxiv.org/abs/2204.06745
     """
 
     def __init__(
@@ -59,20 +61,28 @@
     @classmethod
     def state_dict_to_hf(
         cls: Type[Self], params: Mapping[str, Tensor]
     ) -> Mapping[str, Tensor]:
         return state_dict_to_hf(params, CAUSAL_LM_HF_PARAM_KEY_TRANSFORMS)
 
     @classmethod
+    def config_from_hf(cls, hf_config: Mapping[str, Any]) -> GPTNeoXConfig:
+        return _config_from_hf(hf_config)
+
+    @classmethod
+    def config_to_hf(cls, curated_config: GPTNeoXConfig) -> Mapping[str, Any]:
+        return _config_to_hf(cls, curated_config)
+
+    @classmethod
     def from_hf_config(
         cls: Type[Self],
         *,
         hf_config: Any,
         device: Optional[torch.device] = None,
     ) -> Self:
-        config = convert_hf_config(hf_config)
+        config = cls.config_from_hf(hf_config)
         return cls(config, device=device)
 
     @classmethod
     def modules_to_not_quantize(cls) -> Set[str]:
         # Ignore the output embedding matrix.
         return {"output_embeddings"}
```

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/models/gpt_neox/config.py` & `curated-transformers-2.0.0.dev1/curated_transformers/models/gpt_neox/config.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/models/gpt_neox/decoder.py` & `curated-transformers-2.0.0.dev1/curated_transformers/models/llama/decoder.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,52 +1,54 @@
 from functools import partial
 from typing import Any, Dict, Mapping, Optional, Tuple, Type, TypeVar
 
 import torch
 from torch import Tensor
-from torch.nn import Dropout, LayerNorm, ModuleList
+from torch.nn import Dropout, ModuleList
 
 from ...layers.attention import (
     AttentionHeads,
     QkvMode,
     ScaledDotProductAttention,
     SelfAttention,
 )
 from ...layers.embeddings import QueryKeyRotaryEmbeddings
 from ...layers.feedforward import PointwiseFeedForward
+from ...layers.normalization import RMSNorm
 from ...layers.transformer import (
     DecoderLayer,
     EmbeddingDropouts,
     EmbeddingLayerNorms,
     TransformerDropouts,
     TransformerEmbeddings,
     TransformerLayerNorms,
 )
 from ..hf_hub import FromHFHub
 from ..hf_hub.conversion import state_dict_from_hf, state_dict_to_hf
 from ..transformer import TransformerDecoder
-from ._hf import DECODER_HF_PARAM_KEY_TRANSFORMS, convert_hf_config
-from .config import GPTNeoXConfig
+from ._hf import DECODER_HF_PARAM_KEY_TRANSFORMS, _config_from_hf, _config_to_hf
+from .config import LlamaConfig
 
 # Only provided as typing.Self in Python 3.11+.
-Self = TypeVar("Self", bound="GPTNeoXDecoder")
+Self = TypeVar("Self", bound="LlamaDecoder")
 
 
-class GPTNeoXDecoder(TransformerDecoder[GPTNeoXConfig], FromHFHub):
+class LlamaDecoder(TransformerDecoder[LlamaConfig], FromHFHub[LlamaConfig]):
     """
-    GPT-NeoX (`Black et al., 2022`_) decoder.
+    Llama (`Touvron et al., 2023 [a]`_, `Touvron et al., 2023 [b]`_) decoder.
 
-    .. _Black et al., 2022: https://arxiv.org/abs/2204.06745
+    .. _Touvron et al., 2023 [a]: https://arxiv.org/abs/2302.13971
+    .. _Touvron et al., 2023 [b]: https://arxiv.org/abs/2307.09288
     """
 
     def __init__(
-        self, config: GPTNeoXConfig, *, device: Optional[torch.device] = None
+        self, config: LlamaConfig, *, device: Optional[torch.device] = None
     ) -> None:
         """
-        Construct a GPT-NeoX decoder.
+        Construct a Llama decoder.
 
         :param config:
             Decoder configuration.
         :param device:
             Device to which the module is to be moved.
         :returns:
             The decoder.
@@ -63,40 +65,44 @@
             n_pieces=config.embedding.n_pieces,
             n_positions=None,
             n_types=None,
             device=device,
         )
 
         hidden_width = config.layer.feedforward.hidden_width
-        n_attention_heads = config.layer.attention.n_query_heads
+        n_query_heads = config.layer.attention.n_query_heads
+        attention_heads = AttentionHeads.key_value_broadcast(
+            n_query_heads=n_query_heads,
+            n_key_value_heads=config.layer.attention.n_key_value_heads,
+        )
         layer_norm = partial(
-            LayerNorm,
+            RMSNorm,
             hidden_width,
-            config.layer.layer_norm_eps,
+            eps=config.layer.layer_norm_eps,
             device=device,
         )
         if config.layer.attention.rotary_embeddings is None:
             raise ValueError(
-                "GPT-NeoX attention config does not contain rotary embedding parameters"
+                "Llama attention config does not contain rotary embedding parameters"
             )
         self.layers = ModuleList(
             [
                 DecoderLayer(
                     attention_layer=SelfAttention(
-                        attention_heads=AttentionHeads.uniform(n_attention_heads),
+                        attention_heads=attention_heads,
                         attention_scorer=ScaledDotProductAttention(
                             dropout_prob=config.layer.attention.dropout_prob,
                             linear_biases=None,
                         ),
                         hidden_width=hidden_width,
-                        qkv_mode=QkvMode.MERGED_SPLIT_BEFORE,
+                        qkv_mode=QkvMode.SEPARATE,
                         rotary_embeds=QueryKeyRotaryEmbeddings(
                             fraction=config.layer.attention.rotary_embeddings.rotary_fraction,
                             base=config.layer.attention.rotary_embeddings.rotary_base,
-                            head_width=hidden_width // n_attention_heads,
+                            head_width=hidden_width // n_query_heads,
                         ),
                         use_bias=config.layer.attention.use_bias,
                         device=device,
                     ),
                     feed_forward_layer=PointwiseFeedForward(
                         activation=config.layer.feedforward.activation.module(),
                         hidden_width=hidden_width,
@@ -114,36 +120,44 @@
                     ),
                     use_parallel_attention=config.layer.attention.use_parallel_attention,
                 )
                 for _ in range(config.layer.n_hidden_layers)
             ]
         )
 
-        self.output_layer_norm = LayerNorm(
-            hidden_width, config.layer.layer_norm_eps, device=device
+        self.output_layer_norm = RMSNorm(
+            hidden_width, eps=config.layer.layer_norm_eps, device=device
         )
 
     @classmethod
     def is_supported(cls: Type[Self], config: Dict[str, Any]) -> bool:
-        return config.get("model_type") == "gpt_neox"
+        return config.get("model_type") == "llama"
 
     @classmethod
     def state_dict_from_hf(
         cls: Type[Self], params: Mapping[str, Tensor]
     ) -> Mapping[str, Tensor]:
         return state_dict_from_hf(params, DECODER_HF_PARAM_KEY_TRANSFORMS)
 
     @classmethod
     def state_dict_to_hf(
         cls: Type[Self], params: Mapping[str, Tensor]
     ) -> Mapping[str, Tensor]:
         return state_dict_to_hf(params, DECODER_HF_PARAM_KEY_TRANSFORMS)
 
     @classmethod
+    def config_from_hf(cls, hf_config: Mapping[str, Any]) -> LlamaConfig:
+        return _config_from_hf(hf_config)
+
+    @classmethod
+    def config_to_hf(cls, curated_config: LlamaConfig) -> Mapping[str, Any]:
+        return _config_to_hf(cls, curated_config)
+
+    @classmethod
     def from_hf_config(
         cls: Type[Self],
         *,
         hf_config: Any,
         device: Optional[torch.device] = None,
     ) -> Self:
-        config = convert_hf_config(hf_config)
+        config = cls.config_from_hf(hf_config)
         return cls(config, device=device)
```

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/models/hf_hub/mixin.py` & `curated-transformers-2.0.0.dev1/curated_transformers/models/hf_hub/mixin.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from abc import ABC, abstractmethod
-from typing import Any, Dict, Mapping, Optional, Tuple, Type, TypeVar
+from typing import Any, Dict, Generic, Mapping, Optional, Type, TypeVar
 
 import torch
 from fsspec import AbstractFileSystem
 from torch import Tensor
+from torch.nn import Module
 
 from ...quantization import prepare_module_for_quantization
 from ...quantization.bnb.config import BitsAndBytesConfig
 from ...repository.fsspec import FsspecArgs, FsspecRepository
 from ...repository.hf_hub import HfHubRepository
 from ...repository.repository import ModelRepository, Repository
 from ...util.serde.load import load_model_from_checkpoints
-from ..module import TransformerModule
+from ..module import ConfigT, TransformerModule
 
 # Only provided as typing.Self in Python 3.11+.
 Self = TypeVar("Self", bound="FromHFHub")
 
 
-class FromHFHub(ABC):
+class FromHFHub(ABC, Generic[ConfigT]):
     """
     Mixin class for downloading models from Hugging Face Hub.
 
     A module using this mixin can implement the ``convert_hf_state_dict``
     and ``from_hf_config`` methods. The mixin will then provide the
     ``from_hf_hub`` method to download a model from the Hugging Face Hub.
     """
@@ -61,14 +62,43 @@
         :returns:
             The converted state dict.
         """
         ...
 
     @classmethod
     @abstractmethod
+    def config_from_hf(cls, hf_config: Mapping[str, Any]) -> ConfigT:
+        """
+        Convert a Hugging Face model configuration to the
+        module's configuration.
+
+        :param hf_config:
+            The Hugging Face model configuration.
+        :returns:
+            The converted Curated Transformer
+            configuration.
+        """
+        ...
+
+    @classmethod
+    @abstractmethod
+    def config_to_hf(cls, curated_config: ConfigT) -> Mapping[str, Any]:
+        """
+        Convert the module's  configuration to the a
+        Hugging Face model configuration.
+
+        :param curated_config:
+            The Curated Transformer model configuration.
+        :returns:
+            The converted Hugging Face configuration.
+        """
+        ...
+
+    @classmethod
+    @abstractmethod
     def from_hf_config(
         cls: Type[Self],
         *,
         hf_config: Any,
         device: Optional[torch.device] = None,
     ) -> Self:
         """
@@ -178,30 +208,14 @@
         :param config:
             Hugging Face model configuration.
         :returns:
             Whether the model is supported by this class.
         """
         raise NotImplementedError
 
-    @abstractmethod
-    def to(
-        self,
-        device: Optional[torch.device] = None,
-        dtype: Optional[torch.dtype] = None,
-        non_blocking: bool = False,
-    ):
-        """
-        Moves and/or casts the parameters and buffers.
-
-        This method is automatically implemented by also deriving from
-        ``torch.nn.Module``. This mixin does not derive from ``Module`` in
-        order to be an abstract base class.
-        """
-        ...
-
     @classmethod
     def from_repo(
         cls: Type[Self],
         *,
         repo: Repository,
         device: Optional[torch.device] = None,
         quantization_config: Optional[BitsAndBytesConfig] = None,
@@ -217,14 +231,15 @@
             Configuration for loading quantized weights.
         :returns:
             Loaded model.
         """
         model_repo = ModelRepository(repo)
         config = model_repo.model_config()
         model = cls.from_hf_config(hf_config=config, device=torch.device("meta"))
+        assert isinstance(model, Module)
 
         # Convert the model to the expected dtype.
         assert isinstance(model, TransformerModule)
         dtype: torch.dtype = model.config.dtype
         serialized_dtype_str = config.get("torch_dtype")
         if serialized_dtype_str is not None:
             serialized_dtype = getattr(torch, serialized_dtype_str, None)
```

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/models/llama/causal_lm.py` & `curated-transformers-2.0.0.dev1/curated_transformers/models/llama/causal_lm.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,23 +4,25 @@
 from torch import Tensor
 from torch.nn import Linear
 
 from ...quantization import Quantizable
 from ..hf_hub import FromHFHub
 from ..hf_hub.conversion import state_dict_from_hf, state_dict_to_hf
 from ..transformer import TransformerCausalLM
-from ._hf import CAUSAL_LM_HF_PARAM_KEY_TRANSFORMS, convert_hf_config
+from ._hf import CAUSAL_LM_HF_PARAM_KEY_TRANSFORMS, _config_from_hf, _config_to_hf
 from .config import LlamaConfig
 from .decoder import LlamaDecoder
 
 # Only provided as typing.Self in Python 3.11+.
 Self = TypeVar("Self", bound="LlamaCausalLM")
 
 
-class LlamaCausalLM(TransformerCausalLM[LlamaConfig], FromHFHub, Quantizable):
+class LlamaCausalLM(
+    TransformerCausalLM[LlamaConfig], FromHFHub[LlamaConfig], Quantizable
+):
     """
     Llama (`Touvron et al., 2023 [a]`_, `Touvron et al., 2023 [b]`_) causal language model.
 
     .. _Touvron et al., 2023 [a]: https://arxiv.org/abs/2302.13971
     .. _Touvron et al., 2023 [b]: https://arxiv.org/abs/2307.09288
     """
 
@@ -60,20 +62,28 @@
     @classmethod
     def state_dict_to_hf(
         cls: Type[Self], params: Mapping[str, Tensor]
     ) -> Mapping[str, Tensor]:
         return state_dict_to_hf(params, CAUSAL_LM_HF_PARAM_KEY_TRANSFORMS)
 
     @classmethod
+    def config_from_hf(cls, hf_config: Mapping[str, Any]) -> LlamaConfig:
+        return _config_from_hf(hf_config)
+
+    @classmethod
+    def config_to_hf(cls, curated_config: LlamaConfig) -> Mapping[str, Any]:
+        return _config_to_hf(cls, curated_config)
+
+    @classmethod
     def from_hf_config(
         cls: Type[Self],
         *,
         hf_config: Any,
         device: Optional[torch.device] = None,
     ) -> Self:
-        config = convert_hf_config(hf_config)
+        config = cls.config_from_hf(hf_config)
         return cls(config, device=device)
 
     @classmethod
     def modules_to_not_quantize(cls) -> Set[str]:
         # Ignore the LM output embedding matrix.
         return {"output_embeddings"}
```

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/models/llama/config.py` & `curated-transformers-2.0.0.dev1/curated_transformers/models/llama/config.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/models/llama/decoder.py` & `curated-transformers-2.0.0.dev1/curated_transformers/models/mpt/decoder.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,52 @@
-from functools import partial
 from typing import Any, Dict, Mapping, Optional, Tuple, Type, TypeVar
 
 import torch
 from torch import Tensor
-from torch.nn import Dropout, ModuleList
+from torch.nn import Dropout, LayerNorm, ModuleList
 
 from ...layers.attention import (
     AttentionHeads,
+    AttentionLinearBiases,
     QkvMode,
+    QkvSplitGroupedByHead,
     ScaledDotProductAttention,
     SelfAttention,
 )
-from ...layers.embeddings import QueryKeyRotaryEmbeddings
 from ...layers.feedforward import PointwiseFeedForward
-from ...layers.normalization import RMSNorm
 from ...layers.transformer import (
     DecoderLayer,
     EmbeddingDropouts,
     EmbeddingLayerNorms,
     TransformerDropouts,
     TransformerEmbeddings,
     TransformerLayerNorms,
 )
 from ..hf_hub import FromHFHub
 from ..hf_hub.conversion import state_dict_from_hf, state_dict_to_hf
 from ..transformer import TransformerDecoder
-from ._hf import DECODER_HF_PARAM_KEY_TRANSFORMS, convert_hf_config
-from .config import LlamaConfig
+from ._hf import DECODER_HF_PARAM_KEY_TRANSFORMS, _config_from_hf, _config_to_hf
+from .config import MPTConfig
 
 # Only provided as typing.Self in Python 3.11+.
-Self = TypeVar("Self", bound="LlamaDecoder")
+Self = TypeVar("Self", bound="MPTDecoder")
 
 
-class LlamaDecoder(TransformerDecoder[LlamaConfig], FromHFHub):
+class MPTDecoder(TransformerDecoder[MPTConfig], FromHFHub[MPTConfig]):
     """
-    Llama (`Touvron et al., 2023 [a]`_, `Touvron et al., 2023 [b]`_) decoder.
+    `MosaicML MPT`_ decoder.
 
-    .. _Touvron et al., 2023 [a]: https://arxiv.org/abs/2302.13971
-    .. _Touvron et al., 2023 [b]: https://arxiv.org/abs/2307.09288
+    .. _MosaicML MPT: https://www.mosaicml.com/blog/mpt-7b
     """
 
     def __init__(
-        self, config: LlamaConfig, *, device: Optional[torch.device] = None
+        self, config: MPTConfig, *, device: Optional[torch.device] = None
     ) -> None:
         """
-        Construct a Llama decoder.
+        Construct an MPT decoder.
 
         :param config:
             Decoder configuration.
         :param device:
             Device to which the module is to be moved.
         :returns:
             The decoder.
@@ -65,45 +63,44 @@
             n_pieces=config.embedding.n_pieces,
             n_positions=None,
             n_types=None,
             device=device,
         )
 
         hidden_width = config.layer.feedforward.hidden_width
-        n_query_heads = config.layer.attention.n_query_heads
-        attention_heads = AttentionHeads.key_value_broadcast(
-            n_query_heads=n_query_heads,
-            n_key_value_heads=config.layer.attention.n_key_value_heads,
-        )
-        layer_norm = partial(
-            RMSNorm,
-            hidden_width,
-            eps=config.layer.layer_norm_eps,
-            device=device,
-        )
-        if config.layer.attention.rotary_embeddings is None:
-            raise ValueError(
-                "Llama attention config does not contain rotary embedding parameters"
+        n_attention_heads = config.layer.attention.n_query_heads
+
+        def layer_norm():
+            layer_norm = LayerNorm(
+                hidden_width, config.layer.layer_norm_eps, device=device
             )
+            if not config.layer.feedforward.use_bias:
+                layer_norm.bias = None
+            return layer_norm
+
+        attention_biases = AttentionLinearBiases(
+            n_attention_heads=config.layer.attention.n_query_heads,
+            is_causal=True,
+            is_inverted=False,
+        )
+
         self.layers = ModuleList(
             [
                 DecoderLayer(
                     attention_layer=SelfAttention(
-                        attention_heads=attention_heads,
+                        attention_heads=AttentionHeads.uniform(
+                            n_attention_heads, QkvSplitGroupedByHead()
+                        ),
                         attention_scorer=ScaledDotProductAttention(
                             dropout_prob=config.layer.attention.dropout_prob,
-                            linear_biases=None,
+                            linear_biases=attention_biases,
                         ),
                         hidden_width=hidden_width,
-                        qkv_mode=QkvMode.SEPARATE,
-                        rotary_embeds=QueryKeyRotaryEmbeddings(
-                            fraction=config.layer.attention.rotary_embeddings.rotary_fraction,
-                            base=config.layer.attention.rotary_embeddings.rotary_base,
-                            head_width=hidden_width // n_query_heads,
-                        ),
+                        qkv_mode=QkvMode.MERGED_SPLIT_AFTER,
+                        rotary_embeds=None,
                         use_bias=config.layer.attention.use_bias,
                         device=device,
                     ),
                     feed_forward_layer=PointwiseFeedForward(
                         activation=config.layer.feedforward.activation.module(),
                         hidden_width=hidden_width,
                         intermediate_width=config.layer.feedforward.intermediate_width,
@@ -120,36 +117,42 @@
                     ),
                     use_parallel_attention=config.layer.attention.use_parallel_attention,
                 )
                 for _ in range(config.layer.n_hidden_layers)
             ]
         )
 
-        self.output_layer_norm = RMSNorm(
-            hidden_width, eps=config.layer.layer_norm_eps, device=device
-        )
+        self.output_layer_norm = layer_norm()
 
     @classmethod
     def is_supported(cls: Type[Self], config: Dict[str, Any]) -> bool:
-        return config.get("model_type") == "llama"
+        return config.get("model_type") == "mpt"
 
     @classmethod
     def state_dict_from_hf(
         cls: Type[Self], params: Mapping[str, Tensor]
     ) -> Mapping[str, Tensor]:
         return state_dict_from_hf(params, DECODER_HF_PARAM_KEY_TRANSFORMS)
 
     @classmethod
     def state_dict_to_hf(
         cls: Type[Self], params: Mapping[str, Tensor]
     ) -> Mapping[str, Tensor]:
         return state_dict_to_hf(params, DECODER_HF_PARAM_KEY_TRANSFORMS)
 
     @classmethod
+    def config_from_hf(cls, hf_config: Mapping[str, Any]) -> MPTConfig:
+        return _config_from_hf(hf_config)
+
+    @classmethod
+    def config_to_hf(cls, curated_config: MPTConfig) -> Mapping[str, Any]:
+        return _config_to_hf(cls, curated_config)
+
+    @classmethod
     def from_hf_config(
         cls: Type[Self],
         *,
         hf_config: Any,
         device: Optional[torch.device] = None,
     ) -> Self:
-        config = convert_hf_config(hf_config)
+        config = cls.config_from_hf(hf_config)
         return cls(config, device=device)
```

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/models/module.py` & `curated-transformers-2.0.0.dev1/curated_transformers/models/module.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/models/mpt/causal_lm.py` & `curated-transformers-2.0.0.dev1/curated_transformers/models/mpt/causal_lm.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 from ...layers.attention import AttentionMask
 from ...layers.cache import KeyValueCache
 from ...quantization import Quantizable
 from ..hf_hub import FromHFHub
 from ..hf_hub.conversion import state_dict_from_hf, state_dict_to_hf
 from ..output import CausalLMOutputWithCache
 from ..transformer import TransformerCausalLM
-from ._hf import CAUSAL_LM_HF_PARAM_KEY_TRANSFORMS, convert_hf_config
+from ._hf import CAUSAL_LM_HF_PARAM_KEY_TRANSFORMS, _config_from_hf, _config_to_hf
 from .config import MPTConfig
 from .decoder import MPTDecoder
 
 # Only provided as typing.Self in Python 3.11+.
 Self = TypeVar("Self", bound="MPTCausalLM")
 
 
-class MPTCausalLM(TransformerCausalLM[MPTConfig], FromHFHub, Quantizable):
+class MPTCausalLM(TransformerCausalLM[MPTConfig], FromHFHub[MPTConfig], Quantizable):
     """
     `MosaicML MPT`_ causal language model.
 
     .. _MosaicML MPT: https://www.mosaicml.com/blog/mpt-7b
     """
 
     def __init__(
@@ -97,20 +97,28 @@
     @classmethod
     def state_dict_to_hf(
         cls: Type[Self], params: Mapping[str, Tensor]
     ) -> Mapping[str, Tensor]:
         return state_dict_to_hf(params, CAUSAL_LM_HF_PARAM_KEY_TRANSFORMS)
 
     @classmethod
+    def config_from_hf(cls, hf_config: Mapping[str, Any]) -> MPTConfig:
+        return _config_from_hf(hf_config)
+
+    @classmethod
+    def config_to_hf(cls, curated_config: MPTConfig) -> Mapping[str, Any]:
+        return _config_to_hf(cls, curated_config)
+
+    @classmethod
     def from_hf_config(
         cls: Type[Self],
         *,
         hf_config: Any,
         device: Optional[torch.device] = None,
     ) -> Self:
-        config = convert_hf_config(hf_config)
+        config = cls.config_from_hf(hf_config)
         return cls(config, device=device)
 
     @classmethod
     def modules_to_not_quantize(cls) -> Set[str]:
         # Ignore the output embedding matrix.
         return {"output_embeddings"}
```

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/models/mpt/config.py` & `curated-transformers-2.0.0.dev1/curated_transformers/models/mpt/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,7 +91,8 @@
                 use_gate=False,
             ),
             dropout_prob=hidden_dropout_prob,
             layer_norm_eps=layer_norm_eps,
             n_hidden_layers=n_hidden_layers,
         )
         self.dtype = torch.bfloat16
+        self.model_max_length = model_max_length
```

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/models/mpt/decoder.py` & `curated-transformers-2.0.0.dev1/curated_transformers/models/roberta/encoder.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,105 +1,97 @@
+from functools import partial
 from typing import Any, Dict, Mapping, Optional, Tuple, Type, TypeVar
 
 import torch
 from torch import Tensor
-from torch.nn import Dropout, LayerNorm, ModuleList
+from torch.nn import Dropout, LayerNorm
 
 from ...layers.attention import (
     AttentionHeads,
-    AttentionLinearBiases,
     QkvMode,
-    QkvSplitGroupedByHead,
     ScaledDotProductAttention,
     SelfAttention,
 )
 from ...layers.feedforward import PointwiseFeedForward
 from ...layers.transformer import (
-    DecoderLayer,
     EmbeddingDropouts,
     EmbeddingLayerNorms,
+    EncoderLayer,
     TransformerDropouts,
-    TransformerEmbeddings,
     TransformerLayerNorms,
 )
 from ..hf_hub import FromHFHub
 from ..hf_hub.conversion import state_dict_from_hf, state_dict_to_hf
-from ..transformer import TransformerDecoder
-from ._hf import DECODER_HF_PARAM_KEY_TRANSFORMS, convert_hf_config
-from .config import MPTConfig
+from ..transformer import TransformerEncoder
+from ._hf import HF_PARAM_KEY_TRANSFORMS, _config_from_hf, _config_to_hf
+from .config import RoBERTaConfig
+from .embeddings import RoBERTaEmbeddings
 
 # Only provided as typing.Self in Python 3.11+.
-Self = TypeVar("Self", bound="MPTDecoder")
+Self = TypeVar("Self", bound="RoBERTaEncoder")
 
 
-class MPTDecoder(TransformerDecoder[MPTConfig], FromHFHub):
+class RoBERTaEncoder(TransformerEncoder[RoBERTaConfig], FromHFHub[RoBERTaConfig]):
     """
-    `MosaicML MPT`_ decoder.
+    RoBERTa (`Liu et al., 2019`_) encoder.
 
-    .. _MosaicML MPT: https://www.mosaicml.com/blog/mpt-7b
+    .. _Liu et al., 2019: https://arxiv.org/abs/1907.11692
     """
 
-    def __init__(
-        self, config: MPTConfig, *, device: Optional[torch.device] = None
-    ) -> None:
+    def __init__(self, config: RoBERTaConfig, *, device: Optional[torch.device] = None):
         """
-        Construct an MPT decoder.
+        Construct a RoBERTa encoder.
 
         :param config:
-            Decoder configuration.
+            Encoder configuration.
         :param device:
             Device to which the module is to be moved.
         :returns:
-            The decoder.
+            The encoder.
         """
         super().__init__(config)
 
-        self.embeddings = TransformerEmbeddings(
+        self.embeddings = RoBERTaEmbeddings(
             dropouts=EmbeddingDropouts(
                 embed_output_dropout=Dropout(config.embedding.dropout_prob)
             ),
             embedding_width=config.embedding.embedding_width,
             hidden_width=config.layer.feedforward.hidden_width,
-            layer_norms=EmbeddingLayerNorms(),
+            layer_norms=EmbeddingLayerNorms(
+                embed_output_layer_norm=LayerNorm(
+                    config.embedding.embedding_width, config.embedding.layer_norm_eps
+                )
+            ),
             n_pieces=config.embedding.n_pieces,
-            n_positions=None,
-            n_types=None,
-            device=device,
+            n_positions=config.embedding.n_positions,
+            n_types=config.embedding.n_types,
+            padding_id=config.padding_id,
         )
+        self.max_seq_len = config.model_max_length
 
         hidden_width = config.layer.feedforward.hidden_width
-        n_attention_heads = config.layer.attention.n_query_heads
-
-        def layer_norm():
-            layer_norm = LayerNorm(
-                hidden_width, config.layer.layer_norm_eps, device=device
-            )
-            if not config.layer.feedforward.use_bias:
-                layer_norm.bias = None
-            return layer_norm
-
-        attention_biases = AttentionLinearBiases(
-            n_attention_heads=config.layer.attention.n_query_heads,
-            is_causal=True,
-            is_inverted=False,
+        layer_norm = partial(
+            LayerNorm,
+            hidden_width,
+            config.layer.layer_norm_eps,
+            device=device,
         )
-
-        self.layers = ModuleList(
+        self.layers = torch.nn.ModuleList(
             [
-                DecoderLayer(
+                EncoderLayer(
                     attention_layer=SelfAttention(
                         attention_heads=AttentionHeads.uniform(
-                            n_attention_heads, QkvSplitGroupedByHead()
+                            config.layer.attention.n_query_heads
                         ),
                         attention_scorer=ScaledDotProductAttention(
                             dropout_prob=config.layer.attention.dropout_prob,
-                            linear_biases=attention_biases,
+                            linear_biases=None,
                         ),
                         hidden_width=hidden_width,
-                        qkv_mode=QkvMode.MERGED_SPLIT_AFTER,
+                        qkv_mode=QkvMode.SEPARATE,
                         rotary_embeds=None,
                         use_bias=config.layer.attention.use_bias,
                         device=device,
                     ),
                     feed_forward_layer=PointwiseFeedForward(
                         activation=config.layer.feedforward.activation.module(),
                         hidden_width=hidden_width,
@@ -108,43 +100,49 @@
                         use_gate=config.layer.feedforward.use_gate,
                         device=device,
                     ),
                     dropouts=TransformerDropouts.layer_output_dropouts(
                         config.layer.dropout_prob
                     ),
                     layer_norms=TransformerLayerNorms(
-                        attn_input_layer_norm=layer_norm(),
-                        ffn_input_layer_norm=layer_norm(),
+                        attn_residual_layer_norm=layer_norm(),
+                        ffn_residual_layer_norm=layer_norm(),
                     ),
                     use_parallel_attention=config.layer.attention.use_parallel_attention,
                 )
                 for _ in range(config.layer.n_hidden_layers)
             ]
         )
 
-        self.output_layer_norm = layer_norm()
-
     @classmethod
     def is_supported(cls: Type[Self], config: Dict[str, Any]) -> bool:
-        return config.get("model_type") == "mpt"
+        return config.get("model_type") == "roberta"
 
     @classmethod
     def state_dict_from_hf(
         cls: Type[Self], params: Mapping[str, Tensor]
     ) -> Mapping[str, Tensor]:
-        return state_dict_from_hf(params, DECODER_HF_PARAM_KEY_TRANSFORMS)
+        return state_dict_from_hf(params, HF_PARAM_KEY_TRANSFORMS)
 
     @classmethod
     def state_dict_to_hf(
         cls: Type[Self], params: Mapping[str, Tensor]
     ) -> Mapping[str, Tensor]:
-        return state_dict_to_hf(params, DECODER_HF_PARAM_KEY_TRANSFORMS)
+        return state_dict_to_hf(params, HF_PARAM_KEY_TRANSFORMS)
+
+    @classmethod
+    def config_from_hf(cls, hf_config: Mapping[str, Any]) -> RoBERTaConfig:
+        return _config_from_hf(hf_config)
+
+    @classmethod
+    def config_to_hf(cls, curated_config: RoBERTaConfig) -> Mapping[str, Any]:
+        return _config_to_hf(curated_config)
 
     @classmethod
     def from_hf_config(
         cls: Type[Self],
         *,
         hf_config: Any,
         device: Optional[torch.device] = None,
     ) -> Self:
-        config = convert_hf_config(hf_config)
+        config = cls.config_from_hf(hf_config)
         return cls(config, device=device)
```

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/models/output.py` & `curated-transformers-2.0.0.dev1/curated_transformers/models/output.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from dataclasses import dataclass
 from typing import Generic, List, Optional, TypeVar
 
 from torch import Tensor
 
 from ..layers.cache import CacheProtocol
-from ..util.dataclass import DataclassAsTuple
 
 CacheT = TypeVar("CacheT", bound=CacheProtocol)
 
 
 @dataclass
-class ModelOutput(DataclassAsTuple):
+class ModelOutput:
     """
     Base class for model outputs.
 
     :param all_outputs:
         The first element is the output of the embedding layer. The
         rest of the elements are the states of each encoder hidden
         layer respectively.
```

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/models/roberta/config.py` & `curated-transformers-2.0.0.dev1/curated_transformers/models/roberta/config.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/models/roberta/embeddings.py` & `curated-transformers-2.0.0.dev1/curated_transformers/models/roberta/embeddings.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/models/transformer.py` & `curated-transformers-2.0.0.dev1/curated_transformers/models/transformer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/quantization/bnb/config.py` & `curated-transformers-2.0.0.dev1/curated_transformers/quantization/bnb/config.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/quantization/bnb/impl.py` & `curated-transformers-2.0.0.dev1/curated_transformers/quantization/bnb/impl.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/quantization/helpers.py` & `curated-transformers-2.0.0.dev1/curated_transformers/quantization/helpers.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/quantization/quantizable.py` & `curated-transformers-2.0.0.dev1/curated_transformers/quantization/quantizable.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/repository/_hf.py` & `curated-transformers-2.0.0.dev1/curated_transformers/repository/_hf.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/repository/file.py` & `curated-transformers-2.0.0.dev1/curated_transformers/repository/file.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 from abc import ABC, abstractmethod
 from typing import IO, Optional
 
 
 class RepositoryFile(ABC):
     """
     A repository file.
@@ -18,14 +19,16 @@
 
         :param mode:
             Mode to open the file with (see Python ``open``).
         :param encoding:
             Encoding to use when the file is opened as text.
         :returns:
             An I/O stream.
+        :raises FileNotFoundError:
+            When the file cannot be found.
         :raises OSError:
             When the file cannot be opened.
         """
         ...
 
     @property
     @abstractmethod
@@ -36,14 +39,22 @@
         :returns:
             The repository file. If the file is not available as a local
             path, the value of this property is ``None``. In these cases
             ``open`` can be used to get the file as a file-like object.
         """
         ...
 
+    @abstractmethod
+    def exists(self) -> bool:
+        """
+        Returns if the file exists. This can cause the file
+        to be cached locally.
+        """
+        ...
+
 
 class LocalFile(RepositoryFile):
     """
     Repository file on the local machine.
     """
 
     def __init__(self, path: str):
@@ -59,7 +70,10 @@
     def open(self, mode: str = "rb", encoding: Optional[str] = None) -> IO:
         # Raises OSError, so we don't have to do any rewrapping.
         return open(self._path, mode=mode, encoding=encoding)
 
     @property
     def path(self) -> Optional[str]:
         return self._path
+
+    def exists(self) -> bool:
+        return os.path.isfile(self._path)
```

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/repository/fsspec.py` & `curated-transformers-2.0.0.dev1/curated_transformers/repository/fsspec.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+import warnings
 from dataclasses import dataclass
 from typing import IO, Any, Dict, Optional
 
 from fsspec import AbstractFileSystem
 
 from .repository import Repository, RepositoryFile
+from .transaction import TransactionContext
 
 
 @dataclass
 class FsspecArgs:
     """
     Convenience wrapper for additional fsspec arguments.
     """
@@ -51,27 +53,35 @@
         """
         super().__init__()
         self._fs = fs
         self._path = path
         self._fsspec_args = FsspecArgs() if fsspec_args is None else fsspec_args
 
     def open(self, mode: str = "rb", encoding: Optional[str] = None) -> IO:
+        if ("r" in mode or "+" in mode) and not self.exists():
+            raise FileNotFoundError(
+                f"Cannot find fsspec path {self._fs.unstrip_protocol(self._path)}"
+            )
+
         try:
             return self._fs.open(
                 self._path, mode=mode, encoding=encoding, **self._fsspec_args.kwargs
             )
         except Exception as e:
             raise OSError(
-                f"Cannot open fsspec path {self._fs.unstrip_protocol(self.path)}"
-            )
+                f"Cannot open fsspec path {self._fs.unstrip_protocol(self._path)}"
+            ) from e
 
     @property
     def path(self) -> Optional[str]:
         return None
 
+    def exists(self) -> bool:
+        return self._fs.exists(self._path, **self._fsspec_args.kwargs)
+
 
 class FsspecRepository(Repository):
     """
     Repository using a filesystem that uses the `fsspec`_ interface.
 
     .. _fsspec: https://filesystem-spec.readthedocs.io/en/latest/
 
@@ -93,19 +103,51 @@
         super().__init__()
         self.fs = fs
         self.repo_path = path
         self.fsspec_args = FsspecArgs() if fsspec_args is None else fsspec_args
 
     def file(self, path: str) -> RepositoryFile:
         full_path = f"{self.repo_path}/{path}"
-        if not self.fs.exists(full_path, **self.fsspec_args.kwargs):
-            raise FileNotFoundError(f"Cannot find file in repository: {path}")
         return FsspecFile(self.fs, full_path, self.fsspec_args)
 
     def pretty_path(self, path: Optional[str] = None) -> str:
         if not path:
             return self._protocol
         return f"{self._protocol}/{path}"
 
+    def transaction(self) -> TransactionContext:
+        return FsspecTransactionContext(self)
+
     @property
     def _protocol(self) -> str:
         return self.fs.unstrip_protocol(self.repo_path)
+
+
+class FsspecTransactionContext(TransactionContext):
+    """
+    `fsspec`_ transaction context manager.
+    TODO: Implement/currently a noop
+
+    .. _fsspec: https://filesystem-spec.readthedocs.io/en/latest/
+    """
+
+    def __init__(self, repo: FsspecRepository):
+        """
+        :param repo:
+            The parent repository.
+        """
+        super().__init__()
+        self._repo = repo
+
+    def open(self, path: str, mode: str, encoding: Optional[str] = None) -> IO:
+        return self._repo.file(path).open(mode=mode, encoding=encoding)
+
+    @property
+    def repo(self) -> Repository:
+        return self._repo
+
+    def __enter__(self):
+        warnings.warn("Transaction support is currently not implemented for fsspec")
+        return self
+
+    def __exit__(self, exc_type, exc_value, exc_tb):
+        pass
```

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/repository/repository.py` & `curated-transformers-2.0.0.dev1/curated_transformers/repository/repository.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,34 +11,31 @@
     PRIMARY_CHECKPOINT_FILENAMES,
     SHARDED_CHECKPOINT_INDEX_FILENAMES,
     SHARDED_CHECKPOINT_INDEX_WEIGHTS_KEY,
     SPECIAL_TOKENS_MAP,
     TOKENIZER_JSON,
 )
 from .file import RepositoryFile
+from .transaction import TransactionContext
 
 
 class Repository(ABC):
     """
     A repository that contains a model or tokenizer.
     """
 
     @abstractmethod
     def file(self, path: str) -> RepositoryFile:
         """
-        Get a repository file.
+        Get a lazily-loaded repository file.
 
         :param path:
             The path of the file within the repository.
         :returns:
             The file.
-        :raises FileNotFoundError:
-            When the file cannot be found.
-        :raises OSError:
-            When the file cannot be opened.
         """
         ...
 
     def json_file(self, path: str) -> Dict[str, Any]:
         """
         Get and parse a JSON file.
 
@@ -49,16 +46,16 @@
         :raises FileNotFoundError:
             When the file cannot be found.
         :raises OSError:
             When the file cannot be opened.
         :raises json.JSONDecodeError:
             When the JSON cannot be decoded.
         """
-        f = self.file(path)
-        with f.open("r", encoding="utf-8") as f:
+        file = self.file(path)
+        with file.open("r", encoding="utf-8") as f:
             return json.load(f)
 
     @abstractmethod
     def pretty_path(self, path: Optional[str] = None) -> str:
         """
         Get a user-consumable path representation (e.g. for error messages).
 
@@ -66,14 +63,25 @@
             The path of a file within the repository. The repository path
             will be returned if ``path`` is falsy.
         :returns:
             The path representation.
         """
         ...
 
+    @abstractmethod
+    def transaction(self) -> TransactionContext:
+        """
+        Begins a new transaction. File operations performed on the transaction
+        context will be deferred until the transaction completes successfully.
+
+        :returns:
+            The transaction context manager.
+        """
+        ...
+
 
 class ModelRepository(Repository):
     """
     Repository wrapper that exposes some methods that are useful for working
     with repositories that contain a model.
     """
 
@@ -107,18 +115,17 @@
             When the checkpoint paths files could not be retrieved.
         """
 
         def get_checkpoint_paths(
             checkpoint_type: ModelCheckpointType,
         ) -> List[RepositoryFile]:
             # Attempt to download a non-sharded checkpoint first.
-            try:
-                return [self.file(PRIMARY_CHECKPOINT_FILENAMES[checkpoint_type])]
-            except:
-                pass
+            primary_ckpt = self.file(PRIMARY_CHECKPOINT_FILENAMES[checkpoint_type])
+            if primary_ckpt.exists():
+                return [primary_ckpt]
 
             # Try sharded checkpoint.
             index_filename = SHARDED_CHECKPOINT_INDEX_FILENAMES[checkpoint_type]
 
             try:
                 index = self.json_file(index_filename)
             except (FileNotFoundError, JSONDecodeError, OSError) as e:
@@ -132,21 +139,21 @@
                 raise OSError(
                     f"Invalid index file in sharded {checkpoint_type.pretty_name} "
                     f"checkpoint for model at `{self.pretty_path()}`"
                 )
 
             checkpoint_paths = []
             for filename in sorted(set(weight_map.values())):
-                try:
-                    checkpoint_paths.append(self.file(filename))
-                except FileNotFoundError:
+                ckpt = self.file(filename)
+                if not ckpt.exists():
                     raise OSError(
                         f"File for sharded checkpoint type {checkpoint_type.pretty_name} "
                         f"could not be found at `{self.pretty_path(index_filename)}`"
                     )
+                checkpoint_paths.append(ckpt)
 
             return checkpoint_paths
 
         # Precedence: Safetensors > PyTorch
         checkpoint_type = ModelCheckpointType.SAFE_TENSORS
         checkpoint_paths: Optional[List[RepositoryFile]] = None
         if has_safetensors:
@@ -195,14 +202,17 @@
             When the model config cannot be opened.
         """
         return self.model_config()["model_type"]
 
     def pretty_path(self, path: Optional[str] = None) -> str:
         return self.repo.pretty_path(path)
 
+    def transaction(self) -> TransactionContext:
+        return self.repo.transaction()
+
 
 class TokenizerRepository(Repository):
     """
     Repository wrapper that exposes some methods that are useful for working
     with repositories that contain a tokenizer.
     """
 
@@ -286,7 +296,10 @@
         """
         Return the HF tokenizers' ``tokenizer.json``.
 
         :returns:
             The tokenizer file.
         """
         return self.repo.file(TOKENIZER_JSON)
+
+    def transaction(self) -> TransactionContext:
+        return self.repo.transaction()
```

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/semver.py` & `curated-transformers-2.0.0.dev1/curated_transformers/semver.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/tests/compat.py` & `curated-transformers-2.0.0.dev1/curated_transformers/tests/compat.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/tests/conftest.py` & `curated-transformers-2.0.0.dev1/curated_transformers/tests/conftest.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,48 +5,47 @@
 
 TORCH_DEVICES = [torch.device("cpu")]
 GPU_TESTS_ENABLED = False
 
 
 def pytest_addoption(parser):
     try:
+        parser.addoption("--slow", action="store_true", help="include slow tests")
         parser.addoption(
-            "--hf-head",
+            "--upload-tests",
             action="store_true",
-            help="include tests that require `transformers` development version",
+            help="include tests that upload test artifacts to remote repos",
         )
-        parser.addoption("--slow", action="store_true", help="include slow tests")
     # Options are already added, e.g. if conftest is copied in a build pipeline
     # and runs twice
     except ValueError:
         pass
 
 
 def pytest_configure(config):
     config.addinivalue_line("markers", "slow: include slow tests")
     config.addinivalue_line(
-        "markers",
-        "hf-head: include tests that require `transformers` development version",
+        "markers", "upload-tests: tests that upload test artifacts to remote repos"
     )
 
 
 def pytest_runtest_setup(item):
     def getopt(opt):
         # When using 'pytest --pyargs spacy' to test an installed copy of
         # spacy, pytest skips running our pytest_addoption() hook. Later, when
         # we call getoption(), pytest raises an error, because it doesn't
         # recognize the option we're asking about. To avoid this, we need to
         # pass a default value. We default to False, i.e., we act like all the
         # options weren't given.
         return item.config.getoption(f"--{opt}", False)
 
     # Integration of boolean flags
-    for opt in ["slow"]:
+    for opt in ["upload_tests", "slow"]:
         if opt in item.keywords and not getopt(opt.replace("_", "-")):
-            pytest.skip(f"need --{opt} option to run")
+            pytest.skip(f"need --{opt.replace('_', '-')} option to run")
 
 
 @pytest.fixture
 def test_dir(request):
     return Path(request.fspath).parent
```

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/tests/generation/test_auto_generator.py` & `curated-transformers-2.0.0.dev1/curated_transformers/tests/generation/test_auto_generator.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/tests/generation/test_dolly_v2.py` & `curated-transformers-2.0.0.dev1/curated_transformers/tests/generation/test_dolly_v2.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/tests/generation/test_falcon.py` & `curated-transformers-2.0.0.dev1/curated_transformers/tests/generation/test_falcon.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/tests/generation/test_generic.py` & `curated-transformers-2.0.0.dev1/curated_transformers/tests/generation/test_generic.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/tests/generation/test_logits.py` & `curated-transformers-2.0.0.dev1/curated_transformers/tests/generation/test_logits.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/tests/generation/test_stop.py` & `curated-transformers-2.0.0.dev1/curated_transformers/tests/generation/test_stop.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/tests/layers/test_attention.py` & `curated-transformers-2.0.0.dev1/curated_transformers/tests/layers/test_attention.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/tests/layers/test_embeddings.py` & `curated-transformers-2.0.0.dev1/curated_transformers/tests/layers/test_embeddings.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,16 @@
     )
 
     re = RotaryEmbeddings(768).to(device)
     hf_re = LlamaRotaryEmbedding(768, device=device)
 
     X = torch.rand(16, 12, 64, 768, device=device)
     Y = re(X)
-    hf_re_cos, hf_re_sin = hf_re(X, seq_len=X.shape[-2])
+    positions = torch.arange(X.shape[2], device=device).view([1, -1])
+    hf_re_cos, hf_re_sin = hf_re(X, positions)
     Y_hf = hf_re_cos * X + hf_re_sin * rotate_half(X)
 
     torch_assertclose(Y, Y_hf)
 
 
 def test_rotary_embeddings_rejects_uneven_width():
     with pytest.raises(ValueError, match=r"must be even"):
```

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/tests/models/albert/test_encoder.py` & `curated-transformers-2.0.0.dev1/curated_transformers/tests/models/xlm_roberta/test_encoder.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,66 +1,46 @@
 import pytest
 
-from curated_transformers.models.albert import ALBERTConfig, ALBERTEncoder
+from curated_transformers.models.xlm_roberta.encoder import XLMREncoder
 
 from ...compat import has_hf_transformers, has_torch_compile
 from ...conftest import TORCH_DEVICES
 from ..util import (
     JITMethod,
     assert_encoder_output_equals_hf,
     assert_model_hf_serialization_roundtrip,
 )
 
 
-def test_rejects_incorrect_number_of_groups():
-    config = ALBERTConfig(n_hidden_groups=5)
-    with pytest.raises(ValueError, match=r"must be divisable"):
-        ALBERTEncoder(config)
-
-
 @pytest.mark.skipif(not has_hf_transformers, reason="requires huggingface transformers")
 @pytest.mark.parametrize("torch_device", TORCH_DEVICES)
 @pytest.mark.parametrize("with_torch_sdp", [False, True])
 def test_encoder(torch_device, with_torch_sdp):
     assert_encoder_output_equals_hf(
-        ALBERTEncoder,
-        "explosion-testing/albert-test",
+        XLMREncoder,
+        "explosion-testing/xlm-roberta-test",
         torch_device,
         with_torch_sdp=with_torch_sdp,
     )
 
 
 @pytest.mark.slow
 @pytest.mark.skipif(not has_hf_transformers, reason="requires huggingface transformers")
 @pytest.mark.skipif(not has_torch_compile, reason="requires torch.compile")
 @pytest.mark.parametrize("torch_device", TORCH_DEVICES)
 @pytest.mark.parametrize("with_torch_sdp", [False, True])
 def test_encoder_with_torch_compile(torch_device, with_torch_sdp):
     assert_encoder_output_equals_hf(
-        ALBERTEncoder,
-        "explosion-testing/albert-test",
+        XLMREncoder,
+        "explosion-testing/xlm-roberta-test",
         torch_device,
         jit_method=JITMethod.TorchCompile,
         with_torch_sdp=with_torch_sdp,
     )
 
 
-@pytest.mark.slow
-@pytest.mark.skipif(not has_hf_transformers, reason="requires huggingface transformers")
-@pytest.mark.parametrize("torch_device", TORCH_DEVICES)
-@pytest.mark.parametrize("with_torch_sdp", [False, True])
-def test_encoder_with_torchscript_trace(torch_device, with_torch_sdp):
-    assert_encoder_output_equals_hf(
-        ALBERTEncoder,
-        "explosion-testing/albert-test",
-        torch_device,
-        jit_method=JITMethod.TorchScriptTrace,
-        with_torch_sdp=with_torch_sdp,
-    )
-
-
 @pytest.mark.skipif(not has_hf_transformers, reason="requires huggingface transformers")
 @pytest.mark.parametrize("torch_device", TORCH_DEVICES)
 def test_encoder_hf_serializtion_roundtrip(torch_device):
     assert_model_hf_serialization_roundtrip(
-        ALBERTEncoder, "explosion-testing/albert-test", torch_device
+        XLMREncoder, "explosion-testing/xlm-roberta-test", torch_device
     )
```

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/tests/models/bert/test_encoder.py` & `curated-transformers-2.0.0.dev1/curated_transformers/tests/models/bert/test_encoder.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,27 +34,13 @@
         "explosion-testing/bert-test",
         torch_device,
         jit_method=JITMethod.TorchCompile,
         with_torch_sdp=with_torch_sdp,
     )
 
 
-@pytest.mark.slow
-@pytest.mark.skipif(not has_hf_transformers, reason="requires huggingface transformers")
-@pytest.mark.parametrize("torch_device", TORCH_DEVICES)
-@pytest.mark.parametrize("with_torch_sdp", [False, True])
-def test_encoder_with_torchscript_trace(torch_device, with_torch_sdp):
-    assert_encoder_output_equals_hf(
-        BERTEncoder,
-        "explosion-testing/bert-test",
-        torch_device,
-        jit_method=JITMethod.TorchScriptTrace,
-        with_torch_sdp=with_torch_sdp,
-    )
-
-
 @pytest.mark.skipif(not has_hf_transformers, reason="requires huggingface transformers")
 @pytest.mark.parametrize("torch_device", TORCH_DEVICES)
 def test_encoder_hf_serializtion_roundtrip(torch_device):
     assert_model_hf_serialization_roundtrip(
         BERTEncoder, "explosion-testing/bert-test", torch_device
     )
```

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/tests/models/camembert/test_encoder.py` & `curated-transformers-2.0.0.dev1/curated_transformers/tests/models/camembert/test_encoder.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,27 +34,13 @@
         "explosion-testing/camembert-test",
         torch_device,
         jit_method=JITMethod.TorchCompile,
         with_torch_sdp=with_torch_sdp,
     )
 
 
-@pytest.mark.slow
-@pytest.mark.skipif(not has_hf_transformers, reason="requires huggingface transformers")
-@pytest.mark.parametrize("torch_device", TORCH_DEVICES)
-@pytest.mark.parametrize("with_torch_sdp", [False, True])
-def test_encoder_with_torchscript_trace(torch_device, with_torch_sdp):
-    assert_encoder_output_equals_hf(
-        CamemBERTEncoder,
-        "explosion-testing/camembert-test",
-        torch_device,
-        jit_method=JITMethod.TorchScriptTrace,
-        with_torch_sdp=with_torch_sdp,
-    )
-
-
 @pytest.mark.skipif(not has_hf_transformers, reason="requires huggingface transformers")
 @pytest.mark.parametrize("torch_device", TORCH_DEVICES)
 def test_encoder_hf_serializtion_roundtrip(torch_device):
     assert_model_hf_serialization_roundtrip(
         CamemBERTEncoder, "explosion-testing/camembert-test", torch_device
     )
```

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/tests/models/falcon/test_decoder.py` & `curated-transformers-2.0.0.dev1/curated_transformers/tests/models/falcon/test_decoder.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import pytest
 import torch
 
 from curated_transformers.layers.attention import AttentionMask
+from curated_transformers.models.falcon._hf import HFConfigKeys
 from curated_transformers.models.falcon.decoder import FalconDecoder
+from curated_transformers.models.hf_hub.conversion import CommonHFKeys
 
 from ...compat import has_hf_transformers, has_torch_compile
 from ...conftest import TORCH_DEVICES
 from ...utils import torch_assertclose
 from ..util import (
     JITMethod,
     assert_decoder_output_equals_hf,
@@ -94,35 +96,14 @@
         with_mask=False,
         with_positions=False,
         jit_method=JITMethod.TorchCompile,
         with_torch_sdp=with_torch_sdp,
     )
 
 
-@pytest.mark.slow
-@pytest.mark.skipif(not has_hf_transformers, reason="requires huggingface transformers")
-@pytest.mark.parametrize("torch_device", TORCH_DEVICES)
-@pytest.mark.parametrize("model_revision", FALCON_TEST_MODELS)
-@pytest.mark.parametrize("with_torch_sdp", [False, True])
-def test_decoder_with_torchscript_trace(torch_device, model_revision, with_torch_sdp):
-    model, revision = model_revision
-    assert_decoder_output_equals_hf(
-        FalconDecoder,
-        model,
-        torch_device,
-        model_revision=revision,
-        trust_remote_code=True,
-        with_cache=False,
-        with_mask=False,
-        with_positions=False,
-        jit_method=JITMethod.TorchScriptTrace,
-        with_torch_sdp=with_torch_sdp,
-    )
-
-
 @pytest.mark.skipif(not has_hf_transformers, reason="requires huggingface transformers")
 @pytest.mark.parametrize("torch_device", TORCH_DEVICES)
 @pytest.mark.parametrize("model_revision", FALCON_TEST_MODELS)
 def test_decoder_with_cache(torch_device, model_revision):
     model, revision = model_revision
 
     model = FalconDecoder.from_hf_hub(
@@ -146,17 +127,25 @@
         ).last_hidden_layer_state
 
     torch_assertclose(Y, Y_no_cache[:, 10:, :])
 
 
 @pytest.mark.skipif(not has_hf_transformers, reason="requires huggingface transformers")
 @pytest.mark.parametrize("torch_device", TORCH_DEVICES)
-@pytest.mark.parametrize("model_revision", FALCON_TEST_MODELS)
-def test_decoder_hf_serializtion_roundtrip(torch_device, model_revision):
-    model, revision = model_revision
+def test_decoder_hf_serializtion_roundtrip(torch_device):
+    # We only support round-trip serialization for the non-RWM models.
     assert_model_hf_serialization_roundtrip(
         FalconDecoder,
-        model,
+        "explosion-testing/falcon-test",
         torch_device,
-        model_revision=revision,
+        model_revision="24ff3d5fd83b4d174888356f20e61349f6cbf467",
         trust_remote_code=True,
+        optional_hf_config_keys={
+            HFConfigKeys.N_HEAD_KV.name,
+            HFConfigKeys.NUM_HEAD_KV.name,
+            HFConfigKeys.MULTI_QUERY.name,
+            HFConfigKeys.N_HEAD_KV.name,
+            HFConfigKeys.NEW_DECODER_ARCHITECTURE.name,
+            CommonHFKeys.ATTENTION_PROBS_DROPOUT_PROB.name,
+            CommonHFKeys.HIDDEN_DROPOUT_PROB.name,
+        },
     )
```

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/tests/models/gpt_neox/test_causal_lm.py` & `curated-transformers-2.0.0.dev1/curated_transformers/tests/models/gpt_neox/test_causal_lm.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import pytest
 
 from curated_transformers.models.gpt_neox.causal_lm import GPTNeoXCausalLM
+from curated_transformers.models.hf_hub.conversion import CommonHFKeys
 
 from ...compat import has_hf_transformers, has_torch_compile
 from ...conftest import TORCH_DEVICES
 from ..util import (
     JITMethod,
     assert_causal_lm_output_equals_hf,
     assert_model_hf_serialization_roundtrip,
@@ -34,29 +35,19 @@
         "trl-internal-testing/tiny-random-GPTNeoXForCausalLM",
         torch_device,
         jit_method=JITMethod.TorchCompile,
         with_torch_sdp=with_torch_sdp,
     )
 
 
-@pytest.mark.slow
-@pytest.mark.skipif(not has_hf_transformers, reason="requires huggingface transformers")
-@pytest.mark.parametrize("torch_device", TORCH_DEVICES)
-@pytest.mark.parametrize("with_torch_sdp", [False, True])
-def test_causal_lm_with_torchscript_trace(torch_device, with_torch_sdp):
-    assert_causal_lm_output_equals_hf(
-        GPTNeoXCausalLM,
-        "trl-internal-testing/tiny-random-GPTNeoXForCausalLM",
-        torch_device,
-        jit_method=JITMethod.TorchScriptTrace,
-        with_torch_sdp=with_torch_sdp,
-    )
-
-
 @pytest.mark.skipif(not has_hf_transformers, reason="requires huggingface transformers")
 @pytest.mark.parametrize("torch_device", TORCH_DEVICES)
 def test_causal_lm_hf_serializtion_roundtrip(torch_device):
     assert_model_hf_serialization_roundtrip(
         GPTNeoXCausalLM,
         "trl-internal-testing/tiny-random-GPTNeoXForCausalLM",
         torch_device,
+        optional_hf_config_keys={
+            CommonHFKeys.ATTENTION_PROBS_DROPOUT_PROB.name,
+            CommonHFKeys.HIDDEN_DROPOUT_PROB.name,
+        },
     )
```

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/tests/models/gpt_neox/test_decoder.py` & `curated-transformers-2.0.0.dev1/curated_transformers/tests/models/gpt_neox/test_decoder.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import pytest
 
 from curated_transformers.models.gpt_neox.decoder import GPTNeoXDecoder
+from curated_transformers.models.hf_hub.conversion import CommonHFKeys
 
 from ...compat import has_hf_transformers, has_torch_compile
 from ...conftest import TORCH_DEVICES
 from ..util import (
     JITMethod,
     assert_decoder_output_equals_hf,
     assert_model_hf_serialization_roundtrip,
@@ -40,31 +41,19 @@
         with_cache=False,
         with_positions=False,
         jit_method=JITMethod.TorchCompile,
         with_torch_sdp=with_torch_sdp,
     )
 
 
-@pytest.mark.slow
-@pytest.mark.skipif(not has_hf_transformers, reason="requires huggingface transformers")
-@pytest.mark.parametrize("torch_device", TORCH_DEVICES)
-@pytest.mark.parametrize("with_torch_sdp", [False, True])
-def test_decoder_with_torchscript_trace(torch_device, with_torch_sdp):
-    assert_decoder_output_equals_hf(
-        GPTNeoXDecoder,
-        "trl-internal-testing/tiny-random-GPTNeoXForCausalLM",
-        torch_device,
-        with_cache=True,
-        with_positions=True,
-        jit_method=JITMethod.TorchScriptTrace,
-        with_torch_sdp=with_torch_sdp,
-    )
-
-
 @pytest.mark.skipif(not has_hf_transformers, reason="requires huggingface transformers")
 @pytest.mark.parametrize("torch_device", TORCH_DEVICES)
 def test_decoder_hf_serializtion_roundtrip(torch_device):
     assert_model_hf_serialization_roundtrip(
         GPTNeoXDecoder,
         "trl-internal-testing/tiny-random-GPTNeoXForCausalLM",
         torch_device,
+        optional_hf_config_keys={
+            CommonHFKeys.ATTENTION_PROBS_DROPOUT_PROB.name,
+            CommonHFKeys.HIDDEN_DROPOUT_PROB.name,
+        },
     )
```

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/tests/models/llama/test_causal_lm.py` & `curated-transformers-2.0.0.dev1/curated_transformers/tests/models/mpt/test_decoder.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,68 +1,63 @@
 import pytest
 
-from curated_transformers.models.llama.causal_lm import LlamaCausalLM
+from curated_transformers.models.hf_hub.conversion import CommonHFKeys
+from curated_transformers.models.mpt._hf import HFConfigKeys
+from curated_transformers.models.mpt.decoder import MPTDecoder
 
 from ...compat import has_hf_transformers, has_torch_compile
 from ...conftest import TORCH_DEVICES
 from ..util import (
     JITMethod,
-    assert_causal_lm_output_equals_hf,
+    assert_decoder_output_equals_hf,
     assert_model_hf_serialization_roundtrip,
 )
 
-LLAMA_TEST_MODELS = [
-    "trl-internal-testing/tiny-random-LlamaForCausalLM",
-    "explosion-testing/llama2-fewer-kv-heads",
-    "explosion-testing/llama2-kv-sharing",
-]
-
 
 @pytest.mark.skipif(not has_hf_transformers, reason="requires huggingface transformers")
 @pytest.mark.parametrize("torch_device", TORCH_DEVICES)
 @pytest.mark.parametrize("with_torch_sdp", [False, True])
-@pytest.mark.parametrize("model", LLAMA_TEST_MODELS)
-def test_causal_lm(torch_device, model, with_torch_sdp):
-    assert_causal_lm_output_equals_hf(
-        LlamaCausalLM,
-        model,
+def test_decoder(torch_device, with_torch_sdp):
+    assert_decoder_output_equals_hf(
+        MPTDecoder,
+        "explosion-testing/mpt-test",
         torch_device,
+        # HF model does not support position IDs.
+        with_positions=False,
         with_torch_sdp=with_torch_sdp,
     )
 
 
 @pytest.mark.slow
 @pytest.mark.skipif(not has_hf_transformers, reason="requires huggingface transformers")
 @pytest.mark.skipif(not has_torch_compile, reason="requires torch.compile")
 @pytest.mark.parametrize("torch_device", TORCH_DEVICES)
-@pytest.mark.parametrize("model", LLAMA_TEST_MODELS)
 @pytest.mark.parametrize("with_torch_sdp", [False, True])
-def test_causal_lm_torch_compile(torch_device, model, with_torch_sdp):
-    assert_causal_lm_output_equals_hf(
-        LlamaCausalLM,
-        model,
+def test_decoder_with_torch_compile(torch_device, with_torch_sdp):
+    # NOTE: testing with cache/positions fails. All outputs seems ok until
+    # the concatenation of the vectors with/without rotary embeddings:
+    #
+    # https://github.com/explosion/curated-transformers/blob/6de9b9828b1d6f8f52dba8b87b4e00a9732a2d5f/curated_transformers/layers/embeddings.py#L308
+    assert_decoder_output_equals_hf(
+        MPTDecoder,
+        "explosion-testing/mpt-test",
         torch_device,
+        with_cache=False,
+        with_positions=False,
         jit_method=JITMethod.TorchCompile,
         with_torch_sdp=with_torch_sdp,
     )
 
 
-@pytest.mark.slow
 @pytest.mark.skipif(not has_hf_transformers, reason="requires huggingface transformers")
 @pytest.mark.parametrize("torch_device", TORCH_DEVICES)
-@pytest.mark.parametrize("model", LLAMA_TEST_MODELS)
-@pytest.mark.parametrize("with_torch_sdp", [False, True])
-def test_causal_lm_with_torchscript_trace(torch_device, model, with_torch_sdp):
-    assert_causal_lm_output_equals_hf(
-        LlamaCausalLM,
-        model,
+def test_decoder_hf_serializtion_roundtrip(torch_device):
+    assert_model_hf_serialization_roundtrip(
+        MPTDecoder,
+        "explosion-testing/mpt-test",
         torch_device,
-        jit_method=JITMethod.TorchScriptTrace,
-        with_torch_sdp=with_torch_sdp,
+        optional_hf_config_keys={
+            HFConfigKeys.LAYER_NORM_EPSILON.name,
+            CommonHFKeys.ATTENTION_PROBS_DROPOUT_PROB.name,
+            CommonHFKeys.HIDDEN_DROPOUT_PROB.name,
+        },
     )
-
-
-@pytest.mark.skipif(not has_hf_transformers, reason="requires huggingface transformers")
-@pytest.mark.parametrize("model", LLAMA_TEST_MODELS)
-@pytest.mark.parametrize("torch_device", TORCH_DEVICES)
-def test_causal_lm_hf_serializtion_roundtrip(model, torch_device):
-    assert_model_hf_serialization_roundtrip(LlamaCausalLM, model, torch_device)
```

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/tests/models/llama/test_decoder.py` & `curated-transformers-2.0.0.dev1/curated_transformers/tests/models/llama/test_decoder.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import pytest
 
+from curated_transformers.models.hf_hub.conversion import CommonHFKeys
+from curated_transformers.models.llama._hf import HFConfigKeys
 from curated_transformers.models.llama.decoder import LlamaDecoder
 
 from ...compat import has_hf_transformers, has_torch_compile
 from ...conftest import TORCH_DEVICES
 from ..util import (
     JITMethod,
     assert_decoder_output_equals_hf,
@@ -39,27 +41,21 @@
         model,
         torch_device,
         jit_method=JITMethod.TorchCompile,
         with_torch_sdp=with_torch_sdp,
     )
 
 
-@pytest.mark.slow
 @pytest.mark.skipif(not has_hf_transformers, reason="requires huggingface transformers")
-@pytest.mark.parametrize("torch_device", TORCH_DEVICES)
 @pytest.mark.parametrize("model", LLAMA_TEST_MODELS)
-@pytest.mark.parametrize("with_torch_sdp", [False, True])
-def test_decoder_with_torchscript_trace(torch_device, model, with_torch_sdp):
-    assert_decoder_output_equals_hf(
+@pytest.mark.parametrize("torch_device", TORCH_DEVICES)
+def test_decoder_hf_serializtion_roundtrip(model, torch_device):
+    assert_model_hf_serialization_roundtrip(
         LlamaDecoder,
         model,
         torch_device,
-        jit_method=JITMethod.TorchScriptTrace,
-        with_torch_sdp=with_torch_sdp,
+        optional_hf_config_keys={
+            HFConfigKeys.NUM_KEY_VALUE_HEADS.name,
+            CommonHFKeys.ATTENTION_PROBS_DROPOUT_PROB.name,
+            CommonHFKeys.HIDDEN_DROPOUT_PROB.name,
+        },
     )
-
-
-@pytest.mark.skipif(not has_hf_transformers, reason="requires huggingface transformers")
-@pytest.mark.parametrize("model", LLAMA_TEST_MODELS)
-@pytest.mark.parametrize("torch_device", TORCH_DEVICES)
-def test_decoder_hf_serializtion_roundtrip(model, torch_device):
-    assert_model_hf_serialization_roundtrip(LlamaDecoder, model, torch_device)
```

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/tests/models/mpt/test_causal_lm.py` & `curated-transformers-2.0.0.dev1/curated_transformers/tests/models/roberta/test_encoder.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,60 +1,46 @@
 import pytest
 
-from curated_transformers.models.mpt.causal_lm import MPTCausalLM
+from curated_transformers.models.roberta.encoder import RoBERTaEncoder
 
 from ...compat import has_hf_transformers, has_torch_compile
 from ...conftest import TORCH_DEVICES
 from ..util import (
     JITMethod,
-    assert_causal_lm_output_equals_hf,
+    assert_encoder_output_equals_hf,
     assert_model_hf_serialization_roundtrip,
 )
 
 
 @pytest.mark.skipif(not has_hf_transformers, reason="requires huggingface transformers")
 @pytest.mark.parametrize("torch_device", TORCH_DEVICES)
 @pytest.mark.parametrize("with_torch_sdp", [False, True])
-def test_causal_lm(torch_device, with_torch_sdp):
-    assert_causal_lm_output_equals_hf(
-        MPTCausalLM,
-        "explosion-testing/mpt-test",
+def test_encoder(torch_device, with_torch_sdp):
+    assert_encoder_output_equals_hf(
+        RoBERTaEncoder,
+        "explosion-testing/roberta-test",
         torch_device,
         with_torch_sdp=with_torch_sdp,
     )
 
 
 @pytest.mark.slow
 @pytest.mark.skipif(not has_hf_transformers, reason="requires huggingface transformers")
 @pytest.mark.skipif(not has_torch_compile, reason="requires torch.compile")
 @pytest.mark.parametrize("torch_device", TORCH_DEVICES)
 @pytest.mark.parametrize("with_torch_sdp", [False, True])
-def test_causal_lm_with_torch_compile(torch_device, with_torch_sdp):
-    assert_causal_lm_output_equals_hf(
-        MPTCausalLM,
-        "explosion-testing/mpt-test",
+def test_encoder_with_torch_compile(torch_device, with_torch_sdp):
+    assert_encoder_output_equals_hf(
+        RoBERTaEncoder,
+        "explosion-testing/roberta-test",
         torch_device,
         jit_method=JITMethod.TorchCompile,
         with_torch_sdp=with_torch_sdp,
     )
 
 
-@pytest.mark.slow
-@pytest.mark.skipif(not has_hf_transformers, reason="requires huggingface transformers")
-@pytest.mark.parametrize("torch_device", TORCH_DEVICES)
-@pytest.mark.parametrize("with_torch_sdp", [False, True])
-def test_causal_lm_with_torchscript_trace(torch_device, with_torch_sdp):
-    assert_causal_lm_output_equals_hf(
-        MPTCausalLM,
-        "explosion-testing/mpt-test",
-        torch_device,
-        jit_method=JITMethod.TorchScriptTrace,
-        with_torch_sdp=with_torch_sdp,
-    )
-
-
 @pytest.mark.skipif(not has_hf_transformers, reason="requires huggingface transformers")
 @pytest.mark.parametrize("torch_device", TORCH_DEVICES)
-def test_causal_lm_hf_serializtion_roundtrip(torch_device):
+def test_encoder_hf_serializtion_roundtrip(torch_device):
     assert_model_hf_serialization_roundtrip(
-        MPTCausalLM, "explosion-testing/mpt-test", torch_device
+        RoBERTaEncoder, "explosion-testing/roberta-test", torch_device
     )
```

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/tests/models/mpt/test_decoder.py` & `curated-transformers-2.0.0.dev1/curated_transformers/tests/models/mpt/test_causal_lm.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,70 +1,55 @@
 import pytest
 
-from curated_transformers.models.mpt.decoder import MPTDecoder
+from curated_transformers.models.hf_hub.conversion import CommonHFKeys
+from curated_transformers.models.mpt._hf import HFConfigKeys
+from curated_transformers.models.mpt.causal_lm import MPTCausalLM
 
 from ...compat import has_hf_transformers, has_torch_compile
 from ...conftest import TORCH_DEVICES
 from ..util import (
     JITMethod,
-    assert_decoder_output_equals_hf,
+    assert_causal_lm_output_equals_hf,
     assert_model_hf_serialization_roundtrip,
 )
 
 
 @pytest.mark.skipif(not has_hf_transformers, reason="requires huggingface transformers")
 @pytest.mark.parametrize("torch_device", TORCH_DEVICES)
 @pytest.mark.parametrize("with_torch_sdp", [False, True])
-def test_decoder(torch_device, with_torch_sdp):
-    assert_decoder_output_equals_hf(
-        MPTDecoder,
+def test_causal_lm(torch_device, with_torch_sdp):
+    assert_causal_lm_output_equals_hf(
+        MPTCausalLM,
         "explosion-testing/mpt-test",
         torch_device,
-        # HF model does not support position IDs.
-        with_positions=False,
         with_torch_sdp=with_torch_sdp,
     )
 
 
 @pytest.mark.slow
 @pytest.mark.skipif(not has_hf_transformers, reason="requires huggingface transformers")
 @pytest.mark.skipif(not has_torch_compile, reason="requires torch.compile")
 @pytest.mark.parametrize("torch_device", TORCH_DEVICES)
 @pytest.mark.parametrize("with_torch_sdp", [False, True])
-def test_decoder_with_torch_compile(torch_device, with_torch_sdp):
-    # NOTE: testing with cache/positions fails. All outputs seems ok until
-    # the concatenation of the vectors with/without rotary embeddings:
-    #
-    # https://github.com/explosion/curated-transformers/blob/6de9b9828b1d6f8f52dba8b87b4e00a9732a2d5f/curated_transformers/layers/embeddings.py#L308
-    assert_decoder_output_equals_hf(
-        MPTDecoder,
+def test_causal_lm_with_torch_compile(torch_device, with_torch_sdp):
+    assert_causal_lm_output_equals_hf(
+        MPTCausalLM,
         "explosion-testing/mpt-test",
         torch_device,
-        with_cache=False,
-        with_positions=False,
         jit_method=JITMethod.TorchCompile,
         with_torch_sdp=with_torch_sdp,
     )
 
 
-@pytest.mark.slow
 @pytest.mark.skipif(not has_hf_transformers, reason="requires huggingface transformers")
 @pytest.mark.parametrize("torch_device", TORCH_DEVICES)
-@pytest.mark.parametrize("with_torch_sdp", [False, True])
-def test_decoder_with_torchscript_trace(torch_device, with_torch_sdp):
-    assert_decoder_output_equals_hf(
-        MPTDecoder,
+def test_causal_lm_hf_serializtion_roundtrip(torch_device):
+    assert_model_hf_serialization_roundtrip(
+        MPTCausalLM,
         "explosion-testing/mpt-test",
         torch_device,
-        with_cache=True,
-        with_positions=False,
-        jit_method=JITMethod.TorchScriptTrace,
-        with_torch_sdp=with_torch_sdp,
-    )
-
-
-@pytest.mark.skipif(not has_hf_transformers, reason="requires huggingface transformers")
-@pytest.mark.parametrize("torch_device", TORCH_DEVICES)
-def test_decoder_hf_serializtion_roundtrip(torch_device):
-    assert_model_hf_serialization_roundtrip(
-        MPTDecoder, "explosion-testing/mpt-test", torch_device
+        optional_hf_config_keys={
+            HFConfigKeys.LAYER_NORM_EPSILON.name,
+            CommonHFKeys.ATTENTION_PROBS_DROPOUT_PROB.name,
+            CommonHFKeys.HIDDEN_DROPOUT_PROB.name,
+        },
     )
```

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/tests/models/test_auto_models.py` & `curated-transformers-2.0.0.dev1/curated_transformers/tests/models/test_auto_models.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/tests/models/test_hf_hub.py` & `curated-transformers-2.0.0.dev1/curated_transformers/tests/models/test_hf_hub.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/tests/models/util.py` & `curated-transformers-2.0.0.dev1/curated_transformers/tests/models/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from enum import Enum
-from typing import Callable, Dict, List, Tuple, Type, Union
+from typing import Callable, Dict, List, Set, Tuple, Type, Union
 
 import torch
 from huggingface_hub import HfFileSystem
 from torch import Tensor
 from torch.nn import Module
 
 from curated_transformers.layers.attention import AttentionMask, enable_torch_sdp
@@ -12,14 +12,16 @@
 from curated_transformers.models.module import (
     CausalLMModule,
     DecoderModule,
     EncoderModule,
     TransformerModule,
 )
 from curated_transformers.models.output import ModelOutput, ModelOutputWithCache
+from curated_transformers.repository.hf_hub import HfHubRepository
+from curated_transformers.repository.repository import ModelRepository
 
 from ..compat import transformers
 from ..utils import torch_assertclose
 
 
 class DecoderWithCache(Module):
     def __init__(self, decoder: DecoderModule):
@@ -52,38 +54,24 @@
             piece_ids=piece_ids, attention_mask=attention_mask, positions=positions
         )
 
 
 class JITMethod(Enum):
     Disable = 0
     TorchCompile = 1
-    TorchScriptTrace = 2
 
-    def convert(
-        self, model: Module, with_torch_sdp: bool, *args
-    ) -> Tuple[
-        Union[Module, torch.ScriptModule],
+    def convert(self, model: Module, with_torch_sdp: bool, *args) -> Tuple[
+        Module,
         Callable[[Union[ModelOutput, Dict[str, torch.Tensor]]], Tensor],
     ]:
         with enable_torch_sdp(with_torch_sdp):
-            if self == JITMethod.Disable:
-                return model, lambda s: s
-            elif self == JITMethod.TorchCompile:
+            if self == JITMethod.TorchCompile:
                 return torch.compile(model), lambda s: s
-            else:
-                if isinstance(model, EncoderModule):
-                    cls = ModelOutput
-                elif isinstance(model, DecoderModule):
-                    cls = ModelOutputWithCache
-                elif isinstance(model, CausalLMModule):
-                    cls = ModelOutputWithCache
-                return (
-                    torch.jit.trace(model, tuple(args)),
-                    lambda s: s,
-                )
+            else:  # JITMethod.Disable
+                return model, lambda s: s
 
 
 def assert_causal_lm_output_equals_hf(
     model_class: Type[FromHFHub],
     model_name: str,
     torch_device: torch.device,
     *,
@@ -94,16 +82,15 @@
     with_torch_sdp=False,
 ):
     orig_model = model_class.from_hf_hub(
         name=model_name, revision=model_revision, device=torch_device
     )
     orig_model.eval()
 
-    for _, param in orig_model.state_dict().items():
-        assert param.device == torch_device
+    check_params_buffers(orig_model, torch_device)
 
     hf_model = transformers.AutoModelForCausalLM.from_pretrained(
         model_name,
         revision=model_revision,
     )
     hf_model.eval()
     hf_model.to(torch_device)
@@ -114,26 +101,26 @@
     model, get_output = jit_method.convert(
         orig_model, with_torch_sdp, X_jit, AttentionMask(mask_jit)
     )
 
     X = torch.randint(0, hf_model.config.vocab_size, (2, 10), device=torch_device)
     mask = torch.ones_like(X, dtype=torch.bool)
     with torch.no_grad():
-        Y = get_output(model(X, AttentionMask(mask)))[1]
+        Y = get_output(model(X, AttentionMask(mask))).logits
         Y_hf = hf_model(X).logits
     torch_assertclose(Y, Y_hf, atol=atol, rtol=rtol)
 
     mask_jit = torch.rand_like(X_jit, dtype=torch.float32) < 0.5
     model, get_output = jit_method.convert(
         orig_model, with_torch_sdp, X_jit, AttentionMask(mask_jit)
     )
 
     mask = torch.rand((2, 10), dtype=torch.float, device=torch_device) < 0.5
     with torch.no_grad():
-        Y = get_output(model(X, AttentionMask(mask)))[1] * mask.unsqueeze(-1)
+        Y = get_output(model(X, AttentionMask(mask))).logits * mask.unsqueeze(-1)
         Y_hf = hf_model(X, attention_mask=mask).logits * mask.unsqueeze(-1)
     torch_assertclose(Y, Y_hf, atol=atol, rtol=rtol)
 
 
 def assert_decoder_output_equals_hf(
     model_class: Type[FromHFHub],
     model_name: str,
@@ -151,16 +138,15 @@
     check_config=True,
 ):
     orig_model = model_class.from_hf_hub(
         name=model_name, revision=model_revision, device=torch_device
     )
     orig_model.eval()
 
-    for _, param in orig_model.state_dict().items():
-        assert param.device == torch_device
+    check_params_buffers(orig_model, torch_device)
 
     hf_model = transformers.AutoModel.from_pretrained(
         model_name, revision=model_revision, trust_remote_code=trust_remote_code
     )
     hf_model.to(torch_device)
     hf_model.eval()
 
@@ -171,15 +157,15 @@
     model, output = jit_method.convert(
         orig_model, with_torch_sdp, X_jit, AttentionMask(mask_jit)
     )
 
     X = torch.randint(0, hf_model.config.vocab_size, (2, 10), device=torch_device)
     mask = torch.ones_like(X, dtype=torch.bool)
     with torch.no_grad():
-        Y = output(model(X, AttentionMask(mask)))[0][-1]
+        Y = output(model(X, AttentionMask(mask))).last_hidden_layer_state
         Y_hf = hf_model(X).last_hidden_state
 
     torch_assertclose(Y, Y_hf, atol=atol, rtol=rtol)
 
     if with_cache:
         assert_decoder_with_cache_output_equals_hf(
             orig_model, hf_model, torch_device, atol, rtol, jit_method
@@ -215,16 +201,15 @@
         orig_model = model_class.from_fsspec(
             fs=HfFileSystem(), model_path=model_name, device=torch_device
         )
     else:
         orig_model = model_class.from_hf_hub(name=model_name, device=torch_device)
     orig_model.eval()
 
-    for _, param in orig_model.state_dict().items():
-        assert param.device == torch_device
+    check_params_buffers(orig_model, torch_device)
 
     hf_model = transformers.AutoModel.from_pretrained(model_name)
     hf_model.to(torch_device)
     hf_model.eval()
 
     X_jit = torch.randint(0, hf_model.config.vocab_size, (3, 5), device=torch_device)
     mask_jit = torch.ones_like(X_jit, dtype=torch.bool)
@@ -233,15 +218,15 @@
     )
 
     torch.manual_seed(0)
     X = torch.randint(0, hf_model.config.vocab_size, (2, 10), device=torch_device)
     mask = torch.ones_like(X, dtype=torch.bool)
 
     with torch.no_grad():
-        Y = output(model(X, AttentionMask(mask)))[0][-1]
+        Y = output(model(X, AttentionMask(mask))).last_hidden_layer_state
         Y_hf = hf_model(X).last_hidden_state
 
     torch_assertclose(Y, Y_hf, atol=atol, rtol=rtol)
 
     assert_with_mask_output_equals_hf(
         orig_model, hf_model, torch_device, atol, rtol, jit_method
     )
@@ -275,25 +260,27 @@
     _, n_heads, _, head_width = cache_jit[0].key.shape
     empty_kv_jit = torch.zeros(
         (2, n_heads, 0, head_width),
         dtype=cache_jit[0].key.dtype,
         device=torch_device,
     )
     empty_cache_jit = [
-        KeyValueCache(empty_kv_jit, empty_kv_jit)
+        KeyValueCache(key=empty_kv_jit, value=empty_kv_jit)
     ] * hf_model.config.num_hidden_layers
 
     X = torch.randint(0, hf_model.config.vocab_size, (2, 10), device=torch_device)
     mask = torch.ones_like(X, dtype=torch.bool)
     X_rest = torch.randint(0, hf_model.config.vocab_size, (2, 10), device=torch_device)
     mask_rest = torch.cat([mask, torch.ones_like(X_rest, dtype=torch.bool)], dim=1)
     with torch.no_grad():
         Y = model(X, AttentionMask(mask), empty_cache_jit)
         Y_hf = hf_model(X, use_cache=True)
-        Y = output(model(X_rest, AttentionMask(mask_rest), cache=output(Y)[1]))[0][-1]
+        Y = output(
+            model(X_rest, AttentionMask(mask_rest), cache=output(Y).cache)
+        ).last_hidden_layer_state
         Y_hf = hf_model(X_rest, past_key_values=Y_hf.past_key_values).last_hidden_state
 
     torch_assertclose(Y, Y_hf, atol=atol, rtol=rtol)
 
 
 def assert_with_mask_output_equals_hf(
     orig_model: Union[DecoderModule, EncoderModule],
@@ -309,15 +296,17 @@
     model, output = jit_method.convert(
         orig_model, with_torch_sdp, X_jit, AttentionMask(mask_jit)
     )
 
     X = torch.randint(0, hf_model.config.vocab_size, (2, 10), device=torch_device)
     mask = torch.rand((2, 10), dtype=torch.float, device=torch_device) < 0.5
     with torch.no_grad():
-        Y = output(model(X, AttentionMask(mask)))[0][-1] * mask.unsqueeze(-1)
+        Y = output(
+            model(X, AttentionMask(mask))
+        ).last_hidden_layer_state * mask.unsqueeze(-1)
         Y_hf = hf_model(X, attention_mask=mask).last_hidden_state * mask.unsqueeze(-1)
     torch_assertclose(Y, Y_hf, atol=atol, rtol=rtol)
 
 
 def assert_decoder_with_positions_equals_hf(
     orig_model: DecoderModule,
     hf_model: "transformers.AutoModel",
@@ -348,15 +337,17 @@
         positions_jit,
     )
 
     X = torch.randint(0, hf_model.config.vocab_size, (2, 10), device=torch_device)
     mask = torch.ones_like(X, dtype=torch.bool)
     positions = torch.randint(0, 10, (2, 10), device=torch_device)
     with torch.no_grad():
-        Y = output(model(X, AttentionMask(mask), positions=positions))[0][-1]
+        Y = output(
+            model(X, AttentionMask(mask), positions=positions)
+        ).last_hidden_layer_state
         Y_hf = hf_model(X, position_ids=positions).last_hidden_state
 
     torch_assertclose(Y, Y_hf, atol=atol, rtol=rtol)
 
 
 def assert_model_config(model: TransformerModule, model_output: Tensor):
     assert isinstance(model, TransformerModule)
@@ -371,24 +362,24 @@
     model_name: str,
     torch_device: torch.device,
     *,
     model_revision: str = "main",
     atol: float = 1e-5,
     rtol: float = 1e-5,
     trust_remote_code: bool = False,
+    optional_hf_config_keys: Set[str] = set(),
 ):
     orig_model = model_class.from_hf_hub(
         name=model_name,
         revision=model_revision,
         device=torch_device,
     )
     orig_model.eval()
 
-    for _, param in orig_model.state_dict().items():
-        assert param.device == torch_device
+    check_params_buffers(orig_model, torch_device)
 
     auto_cls = (
         transformers.AutoModelForCausalLM
         if isinstance(orig_model, CausalLMModule)
         else transformers.AutoModel
     )
 
@@ -401,7 +392,38 @@
     hf_model.eval()
 
     hf_model_statedict = hf_model.state_dict()
     orig_model_hf_statedict = orig_model.state_dict_to_hf(orig_model.state_dict())
     for name in orig_model_hf_statedict.keys():
         assert name in hf_model_statedict.keys(), f"{name} not found in HF state dict"
         torch_assertclose(orig_model_hf_statedict[name], hf_model_statedict[name])
+
+    hf_config = ModelRepository(
+        HfHubRepository(name=model_name, revision=model_revision)
+    ).model_config()
+    orig_model_hf_config = orig_model.config_to_hf(orig_model.config)
+
+    # These won't be the same anyway, so we can skip them.
+    ignored_keys = ("architectures", "transformers_version")
+
+    for k, v in orig_model_hf_config.items():
+        if k in ignored_keys:
+            continue
+        elif k in optional_hf_config_keys and k not in hf_config:
+            continue
+        assert k in hf_config, f"Key '{k}' is missing in the Hugging Face model config"
+        assert (
+            hf_config[k] == v
+        ), f"Key '{k}' value '{v}' is different in the Hugging Face model config ('{hf_config[k]}')"
+
+
+def check_params_buffers(model: Module, device: torch.device):
+    """
+    Check that parameters/buffers are placed on the correct device and that
+    parameters are leaf nodes.
+    """
+    for buffer in model.buffers():
+        assert buffer.device == device
+
+    for param in model.parameters():
+        assert param.device == device
+        assert param.is_leaf
```

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/tests/quantization/test_generation.py` & `curated-transformers-2.0.0.dev1/curated_transformers/tests/quantization/test_generation.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/tests/tokenizers/legacy/test_bert_tokenizer.py` & `curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/legacy/test_bert_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/tests/tokenizers/legacy/test_camembert_tokenizer.py` & `curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/legacy/test_camembert_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/tests/tokenizers/legacy/test_llama_tokenizer.py` & `curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/legacy/test_llama_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/tests/tokenizers/legacy/test_roberta_tokenizer.py` & `curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/legacy/test_roberta_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/tests/tokenizers/legacy/test_xlmr_tokenizer.py` & `curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/legacy/test_xlmr_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/tests/tokenizers/legacy/toy-merges.txt` & `curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/legacy/toy-merges.txt`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/tests/tokenizers/legacy/toy-vocab.json` & `curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/legacy/toy-vocab.json`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/tests/tokenizers/legacy/toy.model` & `curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/legacy/toy.model`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/tests/tokenizers/legacy/toy.wordpieces` & `curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/legacy/toy.wordpieces`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/tests/tokenizers/test_auto_tokenizer.py` & `curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/test_auto_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/tests/tokenizers/test_chunks.py` & `curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/test_chunks.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/tests/tokenizers/test_hf_hub.py` & `curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/test_hf_hub.py`

 * *Files 22% similar despite different names*

```diff
@@ -47,14 +47,15 @@
                 filename=name,
                 revision="1dbc166cf8765166998eff31ade2eb64c8a40076",
             )
             != _CACHED_NO_EXIST
         )
 
 
+@pytest.mark.xfail(reason="HfFileSystem calls safetensors with incorrect arguments")
 @pytest.mark.skipif(not has_hf_transformers, reason="requires huggingface transformers")
 def test_fsspec(sample_texts):
     # We only test one model, since using fsspec downloads the model
     # each time.
     compare_tokenizer_outputs_with_hf_tokenizer(
         sample_texts,
         "EleutherAI/gpt-neox-20b",
```

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/tests/tokenizers/test_tokenizer.py` & `curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/tests/tokenizers/toy-roberta/tokenizer.json` & `curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/toy-roberta/tokenizer.json`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/tests/tokenizers/util.py` & `curated-transformers-2.0.0.dev1/curated_transformers/tests/tokenizers/util.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/tokenizers/_hf_compat.py` & `curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/_hf_compat.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/tokenizers/auto_tokenizer.py` & `curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/auto_tokenizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -135,30 +135,27 @@
     """
     return HF_TOKENIZER_MAPPING.get(tokenizer_config.get("tokenizer_class", None), None)
 
 
 def _resolve_tokenizer_class(
     repo: TokenizerRepository,
 ) -> Type[FromHFHub]:
+    tokenizer_file = repo.tokenizer_json()
+    if tokenizer_file.exists():
+        return Tokenizer
+
     cls: Optional[Type[FromHFHub]] = None
     try:
-        repo.tokenizer_json()
-        cls = Tokenizer
+        tokenizer_config = repo.tokenizer_config()
+        cls = _get_tokenizer_class_from_config(tokenizer_config)
     except:
         pass
 
     if cls is None:
         try:
-            tokenizer_config = repo.tokenizer_config()
-            cls = _get_tokenizer_class_from_config(tokenizer_config)
-        except:
-            pass
-
-    if cls is None:
-        try:
             model_type = repo.model_type()
             print(model_type)
             cls = HF_MODEL_MAPPING.get(model_type)
         except:
             pass
 
     if cls is None:
```

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/tokenizers/chunks.py` & `curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/chunks.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/tokenizers/hf_hub.py` & `curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/hf_hub.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/tokenizers/legacy/__init__.py` & `curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/tokenizers/legacy/_fairseq.py` & `curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/legacy/_fairseq.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/tokenizers/legacy/bbpe_tokenizer.py` & `curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/legacy/bbpe_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/tokenizers/legacy/bert_tokenizer.py` & `curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/legacy/bert_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/tokenizers/legacy/camembert_tokenizer.py` & `curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/legacy/camembert_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/tokenizers/legacy/legacy_tokenizer.py` & `curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/legacy/legacy_tokenizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,20 +151,18 @@
             InputChunks([TextChunk(seq)]) if isinstance(seq, str) else seq
             for seq in input
         ]
 
     @abstractmethod
     def _decode(
         self, input: Iterable[Iterable[int]], skip_special_pieces: bool
-    ) -> List[str]:
-        ...
+    ) -> List[str]: ...
 
     @abstractmethod
-    def _encode(self, input: Iterable[MergedInputChunks]) -> PiecesWithIds:
-        ...
+    def _encode(self, input: Iterable[MergedInputChunks]) -> PiecesWithIds: ...
 
 
 class AddBosEosPreEncoder(PreEncoder):
     """
     Adds beginning/end of sequence markers before the encoding process.
     """
```

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/tokenizers/legacy/llama_tokenizer.py` & `curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/legacy/llama_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/tokenizers/legacy/roberta_tokenizer.py` & `curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/legacy/roberta_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/tokenizers/legacy/sentencepiece_tokenizer.py` & `curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/legacy/sentencepiece_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/tokenizers/legacy/wordpiece_tokenizer.py` & `curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/legacy/wordpiece_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/tokenizers/legacy/xlmr_tokenizer.py` & `curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/legacy/xlmr_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/tokenizers/tokenizer.py` & `curated-transformers-2.0.0.dev1/curated_transformers/tokenizers/tokenizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import torch
 from fsspec.implementations.local import LocalFileSystem
 from huggingface_hub import Repository
 from tokenizers import Tokenizer as HFTokenizer
 from torch import Tensor
 
 from ..layers.attention import AttentionMask
+from ..repository.file import RepositoryFile
 from ..repository.fsspec import FsspecRepository
 from ..repository.hf_hub import HfHubRepository
 from ..repository.repository import Repository, TokenizerRepository
 from ._hf_compat import clean_up_decoded_string_like_hf
 from .chunks import InputChunks, MergedSpecialPieceChunk
 from .hf_hub import FromHFHub
 
@@ -333,21 +334,26 @@
         try:
             _ = repo.special_tokens_map()
         except:
             pass
 
     @classmethod
     def from_repo(cls: Type[Self], repo: Repository) -> Self:
+        def initialize_hf_tokenizer(tokenizer_file: RepositoryFile) -> HFTokenizer:
+            with tokenizer_file.open(mode="rb") as f:
+                # We have to open the file once before checking the local
+                # file's existence (since the repo files are loaded lazily).
+                if tokenizer_file.path is not None:
+                    return HFTokenizer.from_file(tokenizer_file.path)
+                else:
+                    return HFTokenizer.from_buffer(f.read())
+
         repo = TokenizerRepository(repo)
         tokenizer_file = repo.tokenizer_json()
-        if tokenizer_file.path is not None:
-            hf_tokenizer = HFTokenizer.from_file(tokenizer_file.path)
-        else:
-            with tokenizer_file.open() as f:
-                hf_tokenizer = HFTokenizer.from_buffer(f.read())
+        hf_tokenizer = initialize_hf_tokenizer(tokenizer_file)
 
         try:
             config = repo.tokenizer_config()
         except OSError:
             config = None
         try:
             special_tokens_map = repo.special_tokens_map()
```

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/util/profile.py` & `curated-transformers-2.0.0.dev1/curated_transformers/util/profile.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/util/pytorch.py` & `curated-transformers-2.0.0.dev1/curated_transformers/util/pytorch.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/util/serde/checkpoint.py` & `curated-transformers-2.0.0.dev1/curated_transformers/util/serde/checkpoint.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/util/serde/load.py` & `curated-transformers-2.0.0.dev1/curated_transformers/util/serde/load.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
         Device to which the converted parameter is moved.
     :returns:
         Converted parameter.
     """
     old_param = module._parameters[parameter_name]
     assert old_param is not None
     _validate_replacement(old_param, tensor, module_prefix)
-    return Parameter(tensor, requires_grad=old_param.requires_grad).to(device=device)  # type: ignore
+    return Parameter(tensor.to(device=device), requires_grad=old_param.requires_grad)  # type: ignore
 
 
 def _emplace_module_state_dict(
     module: Module,
     state_dict: Mapping[str, torch.Tensor],
     *,
     tensor_to_param_converter: Optional[TensorToParameterConverterT] = None,
```

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers/util/string.py` & `curated-transformers-2.0.0.dev1/curated_transformers/util/string.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers.egg-info/PKG-INFO` & `curated-transformers-2.0.0.dev1/curated_transformers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curated-transformers
-Version: 2.0.0.dev0
+Version: 2.0.0.dev1
 Summary: A PyTorch library of transformer models and components
 Home-page: https://github.com/explosion/curated-transformers
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers.egg-info/SOURCES.txt` & `curated-transformers-2.0.0.dev1/curated_transformers.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,19 @@
 curated_transformers/models/albert/encoder.py
 curated_transformers/models/albert/layer_group.py
 curated_transformers/models/bert/__init__.py
 curated_transformers/models/bert/_hf.py
 curated_transformers/models/bert/config.py
 curated_transformers/models/bert/encoder.py
 curated_transformers/models/camembert/__init__.py
+curated_transformers/models/camembert/_hf.py
 curated_transformers/models/camembert/encoder.py
+curated_transformers/models/electra/__init__.py
+curated_transformers/models/electra/_hf.py
+curated_transformers/models/electra/encoder.py
 curated_transformers/models/falcon/__init__.py
 curated_transformers/models/falcon/_hf.py
 curated_transformers/models/falcon/causal_lm.py
 curated_transformers/models/falcon/config.py
 curated_transformers/models/falcon/decoder.py
 curated_transformers/models/falcon/layer.py
 curated_transformers/models/gpt_neox/__init__.py
@@ -80,27 +84,29 @@
 curated_transformers/models/mpt/decoder.py
 curated_transformers/models/roberta/__init__.py
 curated_transformers/models/roberta/_hf.py
 curated_transformers/models/roberta/config.py
 curated_transformers/models/roberta/embeddings.py
 curated_transformers/models/roberta/encoder.py
 curated_transformers/models/xlm_roberta/__init__.py
+curated_transformers/models/xlm_roberta/_hf.py
 curated_transformers/models/xlm_roberta/encoder.py
 curated_transformers/quantization/__init__.py
 curated_transformers/quantization/helpers.py
 curated_transformers/quantization/quantizable.py
 curated_transformers/quantization/bnb/__init__.py
 curated_transformers/quantization/bnb/config.py
 curated_transformers/quantization/bnb/impl.py
 curated_transformers/repository/__init__.py
 curated_transformers/repository/_hf.py
 curated_transformers/repository/file.py
 curated_transformers/repository/fsspec.py
 curated_transformers/repository/hf_hub.py
 curated_transformers/repository/repository.py
+curated_transformers/repository/transaction.py
 curated_transformers/tests/__init__.py
 curated_transformers/tests/compat.py
 curated_transformers/tests/conftest.py
 curated_transformers/tests/enable_gpu.py
 curated_transformers/tests/utils.py
 curated_transformers/tests/generation/__init__.py
 curated_transformers/tests/generation/test_auto_generator.py
@@ -118,14 +124,16 @@
 curated_transformers/tests/models/util.py
 curated_transformers/tests/models/albert/__init__.py
 curated_transformers/tests/models/albert/test_encoder.py
 curated_transformers/tests/models/bert/__init__.py
 curated_transformers/tests/models/bert/test_encoder.py
 curated_transformers/tests/models/camembert/__init__.py
 curated_transformers/tests/models/camembert/test_encoder.py
+curated_transformers/tests/models/electra/__init__.py
+curated_transformers/tests/models/electra/test_encoder.py
 curated_transformers/tests/models/falcon/__init__.py
 curated_transformers/tests/models/falcon/test_decoder.py
 curated_transformers/tests/models/gpt_neox/__init__.py
 curated_transformers/tests/models/gpt_neox/test_causal_lm.py
 curated_transformers/tests/models/gpt_neox/test_decoder.py
 curated_transformers/tests/models/llama/__init__.py
 curated_transformers/tests/models/llama/test_causal_lm.py
@@ -135,34 +143,36 @@
 curated_transformers/tests/models/mpt/test_decoder.py
 curated_transformers/tests/models/roberta/__init__.py
 curated_transformers/tests/models/roberta/test_encoder.py
 curated_transformers/tests/models/xlm_roberta/__init__.py
 curated_transformers/tests/models/xlm_roberta/test_encoder.py
 curated_transformers/tests/quantization/__init__.py
 curated_transformers/tests/quantization/test_generation.py
+curated_transformers/tests/repository/__init__.py
+curated_transformers/tests/repository/test_hf_hub.py
 curated_transformers/tests/tokenizers/__init__.py
 curated_transformers/tests/tokenizers/test_auto_tokenizer.py
 curated_transformers/tests/tokenizers/test_chunks.py
 curated_transformers/tests/tokenizers/test_hf_hub.py
 curated_transformers/tests/tokenizers/test_tokenizer.py
 curated_transformers/tests/tokenizers/util.py
 curated_transformers/tests/tokenizers/legacy/__init__.py
 curated_transformers/tests/tokenizers/legacy/test_bert_tokenizer.py
 curated_transformers/tests/tokenizers/legacy/test_camembert_tokenizer.py
+curated_transformers/tests/tokenizers/legacy/test_electra_tokenizer.py
 curated_transformers/tests/tokenizers/legacy/test_llama_tokenizer.py
 curated_transformers/tests/tokenizers/legacy/test_roberta_tokenizer.py
 curated_transformers/tests/tokenizers/legacy/test_xlmr_tokenizer.py
 curated_transformers/tests/tokenizers/legacy/toy-merges.txt
 curated_transformers/tests/tokenizers/legacy/toy-vocab.json
 curated_transformers/tests/tokenizers/legacy/toy.model
 curated_transformers/tests/tokenizers/legacy/toy.wordpieces
 curated_transformers/tests/tokenizers/toy-roberta/__init__.py
 curated_transformers/tests/tokenizers/toy-roberta/tokenizer.json
 curated_transformers/tests/util/__init__.py
-curated_transformers/tests/util/test_dataclass.py
 curated_transformers/tokenizers/__init__.py
 curated_transformers/tokenizers/_hf_compat.py
 curated_transformers/tokenizers/auto_tokenizer.py
 curated_transformers/tokenizers/chunks.py
 curated_transformers/tokenizers/hf_hub.py
 curated_transformers/tokenizers/tokenizer.py
 curated_transformers/tokenizers/util.py
@@ -174,14 +184,13 @@
 curated_transformers/tokenizers/legacy/legacy_tokenizer.py
 curated_transformers/tokenizers/legacy/llama_tokenizer.py
 curated_transformers/tokenizers/legacy/roberta_tokenizer.py
 curated_transformers/tokenizers/legacy/sentencepiece_tokenizer.py
 curated_transformers/tokenizers/legacy/wordpiece_tokenizer.py
 curated_transformers/tokenizers/legacy/xlmr_tokenizer.py
 curated_transformers/util/__init__.py
-curated_transformers/util/dataclass.py
 curated_transformers/util/profile.py
 curated_transformers/util/pytorch.py
 curated_transformers/util/string.py
 curated_transformers/util/serde/__init__.py
 curated_transformers/util/serde/checkpoint.py
 curated_transformers/util/serde/load.py
```

### Comparing `curated-transformers-2.0.0.dev0/curated_transformers.egg-info/entry_points.txt` & `curated-transformers-2.0.0.dev1/curated_transformers.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev0/setup.cfg` & `curated-transformers-2.0.0.dev1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 2.0.0.dev0
+version = 2.0.0.dev1
 description = A PyTorch library of transformer models and components
 url = https://github.com/explosion/curated-transformers
 author = Explosion
 author_email = contact@explosion.ai
 license = MIT
 license_file = LICENSE
 long_description = file: README.md
```

