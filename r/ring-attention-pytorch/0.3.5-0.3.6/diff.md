# Comparing `tmp/ring-attention-pytorch-0.3.5.tar.gz` & `tmp/ring-attention-pytorch-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ring-attention-pytorch-0.3.5.tar", last modified: Sun Apr  7 18:00:06 2024, max compression
+gzip compressed data, was "ring-attention-pytorch-0.3.6.tar", last modified: Sun Apr  7 18:36:22 2024, max compression
```

## Comparing `ring-attention-pytorch-0.3.5.tar` & `ring-attention-pytorch-0.3.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:00:06.626834 ring-attention-pytorch-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-07 18:00:02.000000 ring-attention-pytorch-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-07 18:00:06.626834 ring-attention-pytorch-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6871 2024-04-07 18:00:02.000000 ring-attention-pytorch-0.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:00:06.622834 ring-attention-pytorch-0.3.5/ring_attention_pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-07 18:00:02.000000 ring-attention-pytorch-0.3.5/ring_attention_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-04-07 18:00:02.000000 ring-attention-pytorch-0.3.5/ring_attention_pytorch/distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-04-07 18:00:02.000000 ring-attention-pytorch-0.3.5/ring_attention_pytorch/ring.py
--rw-r--r--   0 runner    (1001) docker     (127)    18348 2024-04-07 18:00:02.000000 ring-attention-pytorch-0.3.5/ring_attention_pytorch/ring_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    12229 2024-04-07 18:00:02.000000 ring-attention-pytorch-0.3.5/ring_attention_pytorch/ring_flash_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    25436 2024-04-07 18:00:02.000000 ring-attention-pytorch-0.3.5/ring_attention_pytorch/ring_flash_attention_cuda.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:00:06.626834 ring-attention-pytorch-0.3.5/ring_attention_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-07 18:00:06.000000 ring-attention-pytorch-0.3.5/ring_attention_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-07 18:00:06.000000 ring-attention-pytorch-0.3.5/ring_attention_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 18:00:06.000000 ring-attention-pytorch-0.3.5/ring_attention_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-07 18:00:06.000000 ring-attention-pytorch-0.3.5/ring_attention_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-07 18:00:06.000000 ring-attention-pytorch-0.3.5/ring_attention_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 18:00:06.626834 ring-attention-pytorch-0.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-07 18:00:02.000000 ring-attention-pytorch-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:36:22.132604 ring-attention-pytorch-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-07 18:36:18.000000 ring-attention-pytorch-0.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-07 18:36:22.132604 ring-attention-pytorch-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7302 2024-04-07 18:36:18.000000 ring-attention-pytorch-0.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:36:22.132604 ring-attention-pytorch-0.3.6/ring_attention_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-07 18:36:18.000000 ring-attention-pytorch-0.3.6/ring_attention_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-04-07 18:36:18.000000 ring-attention-pytorch-0.3.6/ring_attention_pytorch/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-04-07 18:36:18.000000 ring-attention-pytorch-0.3.6/ring_attention_pytorch/ring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18348 2024-04-07 18:36:18.000000 ring-attention-pytorch-0.3.6/ring_attention_pytorch/ring_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12229 2024-04-07 18:36:18.000000 ring-attention-pytorch-0.3.6/ring_attention_pytorch/ring_flash_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25731 2024-04-07 18:36:18.000000 ring-attention-pytorch-0.3.6/ring_attention_pytorch/ring_flash_attention_cuda.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:36:22.132604 ring-attention-pytorch-0.3.6/ring_attention_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-07 18:36:22.000000 ring-attention-pytorch-0.3.6/ring_attention_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-07 18:36:22.000000 ring-attention-pytorch-0.3.6/ring_attention_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 18:36:22.000000 ring-attention-pytorch-0.3.6/ring_attention_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-07 18:36:22.000000 ring-attention-pytorch-0.3.6/ring_attention_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-07 18:36:22.000000 ring-attention-pytorch-0.3.6/ring_attention_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 18:36:22.132604 ring-attention-pytorch-0.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-07 18:36:18.000000 ring-attention-pytorch-0.3.6/setup.py
```

### Comparing `ring-attention-pytorch-0.3.5/LICENSE` & `ring-attention-pytorch-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ring-attention-pytorch-0.3.5/PKG-INFO` & `ring-attention-pytorch-0.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ring-attention-pytorch
-Version: 0.3.5
+Version: 0.3.6
 Summary: Ring Attention - Pytorch
 Home-page: https://github.com/lucidrains/ring-attention-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,distributed attention
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ring-attention-pytorch-0.3.5/README.md` & `ring-attention-pytorch-0.3.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,18 @@
 
 In addition, the repository also contains the logic for <a href="https://arxiv.org/abs/2311.09431">Striped Attention</a>, a follow up paper that permutes the sequence for better workload balancing for autoregressive transformers.
 
 ## Appreciation
 
 - <a href="https://a16z.com/supporting-the-open-source-ai-community/">A16Z Open Source AI Grant Program</a> for the generous sponsorship, as well as my other sponsors, for affording me the independence to open source current artificial intelligence research
 
+- <a href="https://tridao.me/">Tri Dao</a> for all his tremendous hard work maintaining <a href="https://github.com/Dao-AILab/flash-attention">Flash Attention</a> over the last year or two, from which the CUDA version in this repository depends on
+
+- Phil Tillet for <a href="https://github.com/openai/triton">Triton</a>, without which the forward ring flash attention CUDA kernel would have taken a magnitude of order more work.
+
 ## Install
 
 ```bash
 $ pip install ring-attention-pytorch
 ```
 
 ## Usage
```

#### html2text {}

```diff
@@ -5,16 +5,20 @@
 being used for the 1-10 million tokens for the latest Gemini. At least some
 form of it; the other possibility would be unpublished improvements on top of
 _R_M_T. In addition, the repository also contains the logic for _S_t_r_i_p_e_d_ _A_t_t_e_n_t_i_o_n,
 a follow up paper that permutes the sequence for better workload balancing for
 autoregressive transformers. ## Appreciation - _A_1_6_Z_ _O_p_e_n_ _S_o_u_r_c_e_ _A_I_ _G_r_a_n_t
 _P_r_o_g_r_a_m for the generous sponsorship, as well as my other sponsors, for
 affording me the independence to open source current artificial intelligence
-research ## Install ```bash $ pip install ring-attention-pytorch ``` ## Usage
-```python import torch from ring_attention_pytorch import RingAttention attn =
+research - _T_r_i_ _D_a_o for all his tremendous hard work maintaining _F_l_a_s_h_ _A_t_t_e_n_t_i_o_n
+over the last year or two, from which the CUDA version in this repository
+depends on - Phil Tillet for _T_r_i_t_o_n, without which the forward ring flash
+attention CUDA kernel would have taken a magnitude of order more work. ##
+Install ```bash $ pip install ring-attention-pytorch ``` ## Usage ```python
+import torch from ring_attention_pytorch import RingAttention attn =
 RingAttention( dim = 512, dim_head = 64, heads = 8, causal = True,
 auto_shard_seq = True, ring_attn = True, ring_seq_size = 512 ) tokens =
 torch.randn(1, 1024, 512) attended = attn(tokens) assert attended.shape ==
 tokens.shape ``` ## Test First install requirements ```bash $ pip install -
 r requirements.txt ``` Then say testing autoregressive striped ring attention
 on cuda would be ```bash $ python assert.py --use-cuda --causal --striped-ring-
 attn ``` ## Todo - [x] make it work with derived causal mask based on rank and
```

### Comparing `ring-attention-pytorch-0.3.5/ring_attention_pytorch/distributed.py` & `ring-attention-pytorch-0.3.6/ring_attention_pytorch/distributed.py`

 * *Files identical despite different names*

### Comparing `ring-attention-pytorch-0.3.5/ring_attention_pytorch/ring.py` & `ring-attention-pytorch-0.3.6/ring_attention_pytorch/ring.py`

 * *Files identical despite different names*

### Comparing `ring-attention-pytorch-0.3.5/ring_attention_pytorch/ring_attention.py` & `ring-attention-pytorch-0.3.6/ring_attention_pytorch/ring_attention.py`

 * *Files identical despite different names*

### Comparing `ring-attention-pytorch-0.3.5/ring_attention_pytorch/ring_flash_attention.py` & `ring-attention-pytorch-0.3.6/ring_attention_pytorch/ring_flash_attention.py`

 * *Files identical despite different names*

### Comparing `ring-attention-pytorch-0.3.5/ring_attention_pytorch/ring_flash_attention_cuda.py` & `ring-attention-pytorch-0.3.6/ring_attention_pytorch/ring_flash_attention_cuda.py`

 * *Files 2% similar despite different names*

```diff
@@ -553,14 +553,18 @@
         lse = None
 
         # receive buffers, to be alternated with sent buffer
 
         receive_kv = None
         receive_mask = None
 
+        # non-causal and causal striped attention can have final normalization of output fused
+
+        can_fuse_final_output_normalization = not causal or (causal and striped_ring_attn)
+
         for (ring_rank, (is_first, is_last)), ((kv, mask), (receive_kv, receive_mask)) in ring_pass_fn(kv, mask, receive_buffers = (receive_kv, receive_mask), max_iters = max_ring_passes, ring_size = ring_size):
             k, v = kv
 
             # translate key padding mask to bias
 
             bias = None
 
@@ -589,23 +593,25 @@
                 causal = block_causal,
                 o = o,
                 m = m,
                 lse = lse,
                 bias = bias,
                 softmax_scale = softmax_scale,
                 causal_mask_diagonal = causal_mask_diagonal,
-                return_normalized_output = False,
+                return_normalized_output = can_fuse_final_output_normalization and is_last,
                 load_accumulated = not is_first
             )
 
         lse = lse[..., :q_seq_len]
-        m = m[..., :q_seq_len]
 
-        o_scale = torch.exp(m - lse)
-        o.mul_(rearrange(o_scale, 'b h n -> b n h 1'))
+        if not can_fuse_final_output_normalization:
+            m = m[..., :q_seq_len]
+
+            o_scale = torch.exp(m - lse)
+            o.mul_(rearrange(o_scale, 'b h n -> b n h 1'))
 
         ctx.args = (
             causal,
             softmax_scale,
             orig_mask,
             bucket_size,
             ring_reduce_col,
```

### Comparing `ring-attention-pytorch-0.3.5/ring_attention_pytorch.egg-info/PKG-INFO` & `ring-attention-pytorch-0.3.6/ring_attention_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ring-attention-pytorch
-Version: 0.3.5
+Version: 0.3.6
 Summary: Ring Attention - Pytorch
 Home-page: https://github.com/lucidrains/ring-attention-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,distributed attention
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ring-attention-pytorch-0.3.5/setup.py` & `ring-attention-pytorch-0.3.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'ring-attention-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.3.5',
+  version = '0.3.6',
   license='MIT',
   description = 'Ring Attention - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/ring-attention-pytorch',
   keywords = [
```

