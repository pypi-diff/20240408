# Comparing `tmp/flash_rwkv-0.1.3-py3-none-any.whl.zip` & `tmp/flash_rwkv-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 5379 bytes, number of entries: 9
--rw-r--r--  2.0 unx       76 b- defN 24-Apr-01 03:19 flash_rwkv/__init__.py
--rw-r--r--  2.0 unx       78 b- defN 24-Apr-01 01:36 flash_rwkv/rwkv5/__init__.py
--rw-r--r--  2.0 unx     7101 b- defN 24-Apr-03 14:52 flash_rwkv/rwkv5/wkv5_kernel.cu
+Zip file size: 5450 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      136 b- defN 24-Apr-07 08:57 flash_rwkv/__init__.py
+-rw-r--r--  2.0 unx      138 b- defN 24-Apr-07 08:57 flash_rwkv/rwkv5/__init__.py
+-rw-r--r--  2.0 unx     6969 b- defN 24-Apr-07 09:29 flash_rwkv/rwkv5/wkv5_kernel.cu
 -rw-r--r--  2.0 unx     4814 b- defN 24-Apr-01 01:36 flash_rwkv/rwkv5/wkv5_op.cpp
--rw-r--r--  2.0 unx     7064 b- defN 24-Apr-04 14:48 flash_rwkv/rwkv5/wkv5_op.py
--rw-r--r--  2.0 unx      145 b- defN 24-Apr-05 13:39 flash_rwkv-0.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-05 13:39 flash_rwkv-0.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 24-Apr-05 13:39 flash_rwkv-0.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      726 b- defN 24-Apr-05 13:39 flash_rwkv-0.1.3.dist-info/RECORD
-9 files, 20107 bytes uncompressed, 4121 bytes compressed:  79.5%
+-rw-r--r--  2.0 unx     7196 b- defN 24-Apr-07 09:24 flash_rwkv/rwkv5/wkv5_op.py
+-rw-r--r--  2.0 unx      145 b- defN 24-Apr-08 13:12 flash_rwkv-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-08 13:12 flash_rwkv-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 24-Apr-08 13:12 flash_rwkv-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      728 b- defN 24-Apr-08 13:12 flash_rwkv-0.2.0.dist-info/RECORD
+9 files, 20229 bytes uncompressed, 4192 bytes compressed:  79.3%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: flash_rwkv/rwkv5/wkv5_op.cpp
 Comment: 
 
 Filename: flash_rwkv/rwkv5/wkv5_op.py
 Comment: 
 
-Filename: flash_rwkv-0.1.3.dist-info/METADATA
+Filename: flash_rwkv-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: flash_rwkv-0.1.3.dist-info/WHEEL
+Filename: flash_rwkv-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: flash_rwkv-0.1.3.dist-info/top_level.txt
+Filename: flash_rwkv-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: flash_rwkv-0.1.3.dist-info/RECORD
+Filename: flash_rwkv-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## flash_rwkv/__init__.py

```diff
@@ -1,3 +1,3 @@
-from .rwkv5 import Rwkv5LinearAttention
+from .rwkv5 import Rwkv5LinearAttention, rwkv5_cuda_linear_attention
 
-__all__ = ["Rwkv5LinearAttention"]
+__all__ = ["Rwkv5LinearAttention", "rwkv5_cuda_linear_attention"]
```

## flash_rwkv/rwkv5/__init__.py

```diff
@@ -1,3 +1,3 @@
-from .wkv5_op import Rwkv5LinearAttention
+from .wkv5_op import Rwkv5LinearAttention, rwkv5_cuda_linear_attention
 
-__all__ = ["Rwkv5LinearAttention"]
+__all__ = ["Rwkv5LinearAttention", "rwkv5_cuda_linear_attention"]
```

## flash_rwkv/rwkv5/wkv5_kernel.cu

```diff
@@ -76,128 +76,117 @@
 __global__ void kernel_backward(const int B, const int T, const int C, const int H,
                                 const F *__restrict__ const _r, const F *__restrict__ const _k, const F *__restrict__ const _v, const float *__restrict__ _w, const float *__restrict__ __w, const F *__restrict__ _u, const F *__restrict__ const _gy,
                                 F *__restrict__ const _gr, F *__restrict__ const _gk, F *__restrict__ const _gv, F *__restrict__ const _gw, F *__restrict__ const _gu)
 {
     const int b = blockIdx.x / H;
     const int h = blockIdx.x % H;
     const int i = threadIdx.x;
-    _w += h * _N_;
-    _u += h * _N_;
-    __w += h * _N_;
-
-    __shared__ float w_[_N_], u_[_N_];
-    __shared__ float r[_N_], k[_N_], v[_N_], gy[_N_];
-    __syncthreads();
-    w_[i] = _w[i];
-    u_[i] = float(_u[i]);
-    __syncthreads();
-
-    const float w = w_[i];
+    _w += h*_N_;
+    _u += h*_N_;
+    __w += h*_N_;
+    const float w = _w[i];
+    const float u = float(_u[i]);
     const float ww = __w[i];
-    const float u = u_[i];
 
-    float state[_N_] = {0}, saaaa[_N_] = {0}, sbbbb[_N_] = {0}, scccc[_N_] = {0}, sdddd[_N_] = {0};
+    __shared__ float v[_N_], r[_N_], k[_N_], gy[_N_], w_[_N_], u_[_N_];
+    float state[_N_] = {0}, saaaa[_N_] = {0}, sbbbb[_N_] = {0};
 
     float gw = 0, gu = 0;
-    const int t000 = b * T * C + h * _N_ + i;
-    const int t111 = (b + 1) * T * C + h * _N_ + i;
-    const int t222 = t111 - 2 * C;
+    const int t000 = b*T*C + h*_N_ + i;
+    const int t111 = (b+1)*T*C + h*_N_ + i;
+    const int t222 = t111 - 2*C;
 
     for (int t = t000; t < t111; t += C)
     {
         __syncthreads();
         v[i] = float(_v[t]);
         gy[i] = float(_gy[t]);
         __syncthreads();
 
         const float k = float(_k[t]);
-        float gr = 0, gu_ = 0;
+        float gr = 0, _gu_ = 0;
 
-#pragma unroll
+        #pragma unroll
         for (int j = 0; j < _N_; j++)
         {
-            float &s = state[j];
+            float& s = state[j];
             float x = k * v[j];
 
             gr += (u * x + s) * gy[j];
-            gu_ += x * gy[j];
+            _gu_ += x * gy[j];
             s = s * w + x;
         }
         _gr[t] = F(gr);
-        gu += float(_r[t]) * gu_;
+        gu += float(_r[t]) * _gu_;
     }
-    _gu[b * C + h * _N_ + i] = F(gu);
-
+    _gu[b*C + h*_N_ + i] = F(gu);
+    
     for (int t = t000; t < t222; t += C)
     {
         __syncthreads();
         v[i] = float(_v[t]);
-        gy[i] = float(_gy[t + 2 * C]);
+        gy[i] = float(_gy[t + 2*C]);
         __syncthreads();
 
         const float k = float(_k[t]);
-        float gw_ = 0;
-
-#pragma unroll
+        const float r = float(_r[t + 2*C]);
+        
+        #pragma unroll
         for (int j = 0; j < _N_; j++)
         {
-            float &s = saaaa[j];
-            float &s2 = sbbbb[j];
+            float& s = saaaa[j];
+            float& s2 = sbbbb[j];
             float x = k * v[j];
-
+            
             float tmp = w * (x + s);
             s = tmp;
             s2 = tmp + w * s2;
-            gw_ += s2 * gy[j];
+            gw += r * s2 * gy[j];
         }
-        gw += float(_r[t + 2 * C]) * gw_;
+    }    
+    _gw[b*C + h*_N_ + i] = F(ww * gw);
+
+    #pragma unroll
+    for (int j = 0; j < _N_; ++j) {
+        saaaa[j] = 0;
+        sbbbb[j] = 0;
     }
-    _gw[b * C + h * _N_ + i] = F(ww * gw);
 
+    __syncthreads();
+    w_[i] = _w[i];
+    u_[i] = float(_u[i]);
+    __syncthreads();
+    
     for (int t = t111 - C; t >= t000; t -= C)
     {
         __syncthreads();
+        r[i] = float(_r[t]);
+        k[i] = float(_k[t]);
         v[i] = float(_v[t]);
         gy[i] = float(_gy[t]);
         __syncthreads();
 
-        const float rr = float(_r[t]);
-        float gk = 0;
+        const float rr = r[i];
+        const float gyy = gy[i];
+        float gk = 0, gv = 0;
 
-#pragma unroll
+        #pragma unroll
         for (int j = 0; j < _N_; j++)
         {
-            float &s = scccc[j];
+            float& s = saaaa[j];
+            float& s2 = sbbbb[j];
             float x = rr * gy[j];
-
+            float x2 = gyy * r[j];
+            
             gk += (u * x + s) * v[j];
+            gv += (u_[j] * x2 + s2) * k[j];
             s = x + s * w;
+            s2 = x2 + s2 * w_[j];
         }
         _gk[t] = F(gk);
-    }
-
-    for (int t = t111 - C; t >= t000; t -= C)
-    {
-        __syncthreads();
-        r[i] = float(_r[t]);
-        k[i] = float(_k[t]);
-        __syncthreads();
-
-        const float gyy = float(_gy[t]);
-        float gv = 0;
-
-#pragma unroll
-        for (int j = 0; j < _N_; j++)
-        {
-            float &s = sdddd[j];
-            float x = gyy * r[j];
-
-            gv += (u_[j] * x + s) * k[j];
-            s = x + s * w_[j];
-        }
         _gv[t] = F(gv);
     }
 }
 
 void cuda_forward_bf16(int B, int T, int C, int H, float *state, bf16 *r, bf16 *k, bf16 *v, float *w, bf16 *u, bf16 *y)
 {
     assert(H * _N_ == C);
```

## flash_rwkv/rwkv5/wkv5_op.py

```diff
@@ -92,28 +92,28 @@
                     receptance,
                     key,
                     value,
                     ee_time_decay,
                     time_first,
                     out,
                 )
-            return out, state
+            return out
 
     @staticmethod
     def backward(ctx, gout):
         with torch.no_grad():
             batch = ctx.batch
             seq_length = ctx.seq_length
             hidden_size = ctx.hidden_size
             num_heads = ctx.num_heads
             receptance, key, value, ee_time_decay, e_time_decay, time_first = ctx.saved_tensors
 
             global_shape = (batch, seq_length, hidden_size)
 
-            greceptance = torch.empty(
+            g_receptance = torch.empty(
                 global_shape,
                 device=gout.device,
                 requires_grad=False,
                 dtype=receptance.dtype,
                 memory_format=torch.contiguous_format,
             )
             g_key = torch.empty(
@@ -130,22 +130,22 @@
                 dtype=receptance.dtype,
                 memory_format=torch.contiguous_format,
             )
             g_time_decay = torch.empty(
                 (batch, hidden_size),
                 device=gout.device,
                 requires_grad=False,
-                dtype=torch.bfloat16,
+                dtype=receptance.dtype,
                 memory_format=torch.contiguous_format,
             )
             g_time_first = torch.empty(
                 (batch, hidden_size),
                 device=gout.device,
                 requires_grad=False,
-                dtype=torch.bfloat16,
+                dtype=receptance.dtype,
                 memory_format=torch.contiguous_format,
             )
             if receptance.dtype == torch.bfloat16:
                 rwkv5_cuda_kernel.backward_bf16(
                     batch,
                     seq_length,
                     hidden_size,
@@ -153,15 +153,15 @@
                     receptance,
                     key,
                     value,
                     ee_time_decay,
                     e_time_decay,
                     time_first,
                     gout,
-                    greceptance,
+                    g_receptance,
                     g_key,
                     g_value,
                     g_time_decay,
                     g_time_first,
                 )
             elif receptance.dtype == torch.float16:
                 rwkv5_cuda_kernel.backward_fp16(
@@ -172,15 +172,15 @@
                     receptance,
                     key,
                     value,
                     ee_time_decay,
                     e_time_decay,
                     time_first,
                     gout,
-                    greceptance,
+                    g_receptance,
                     g_key,
                     g_value,
                     g_time_decay,
                     g_time_first,
                 )
             elif receptance.dtype == torch.float32:
                 rwkv5_cuda_kernel.backward_fp32(
@@ -191,19 +191,22 @@
                     receptance,
                     key,
                     value,
                     ee_time_decay,
                     e_time_decay,
                     time_first,
                     gout,
-                    greceptance,
+                    g_receptance,
                     g_key,
                     g_value,
                     g_time_decay,
                     g_time_first,
                 )
             head_size = hidden_size // num_heads
-            g_time_decay = torch.sum(g_time_decay, 0).view(num_heads, head_size)
-            g_time_first = torch.sum(g_time_first, 0).view(num_heads, head_size)
-            return (None, None, None, None, greceptance, g_key, g_value, g_time_decay, g_time_first)
+            g_time_decay = torch.sum(g_time_decay, 0).flatten()
+            g_time_first = torch.sum(g_time_first, 0).flatten()
+            return (g_receptance, g_key, g_value, g_time_decay, g_time_first, None)
 
 load_wkv5_cuda_kernel()
+
+def rwkv5_cuda_linear_attention(receptance, key, value, time_decay, time_first, state):
+    return Rwkv5LinearAttention.apply(receptance, key, value, time_decay, time_first, state)
```

