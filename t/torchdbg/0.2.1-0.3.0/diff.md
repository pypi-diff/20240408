# Comparing `tmp/torchdbg-0.2.1.tar.gz` & `tmp/torchdbg-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchdbg-0.2.1.tar", max compression
+gzip compressed data, was "torchdbg-0.3.0.tar", max compression
```

## Comparing `torchdbg-0.2.1.tar` & `torchdbg-0.3.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       53 2024-04-06 16:55:02.300964 torchdbg-0.2.1/README.md
--rw-r--r--   0        0        0      325 2024-04-07 17:01:12.388473 torchdbg-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     6044 2024-04-07 17:01:08.561012 torchdbg-0.2.1/torchdbg/__init__.py
--rw-r--r--   0        0        0      645 1970-01-01 00:00:00.000000 torchdbg-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       53 2024-04-06 16:55:02.300964 torchdbg-0.3.0/README.md
+-rw-r--r--   0        0        0      325 2024-04-08 21:34:17.842723 torchdbg-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6083 2024-04-08 21:33:41.932831 torchdbg-0.3.0/torchdbg/__init__.py
+-rw-r--r--   0        0        0      645 1970-01-01 00:00:00.000000 torchdbg-0.3.0/PKG-INFO
```

### Comparing `torchdbg-0.2.1/torchdbg/__init__.py` & `torchdbg-0.3.0/torchdbg/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,15 +61,14 @@
 class LoggingMode(TorchFunctionMode):
     next_id: int
 
     def __init__(self, skip=0):
         self.memo = WeakTensorKeyDictionary()
         self.next_id = 0
         self.skip = skip
-        self.lines_traversed = defaultdict(set)
 
     def __enter__(self):
         frame = inspect.currentframe()
         for _ in range(self.skip + 1):
             frame = frame.f_back
         self.frame = frame
         super().__enter__()
@@ -108,14 +107,19 @@
             else:
                 return res
 
     def __torch_function__(self, func, tys, args=(), kwargs=None):
         if kwargs is None:
             kwargs = {}
 
+        # Don't bother with accessors
+        func_name = resolve_name(func)
+        if func_name is not None and func_name.endswith('.__get__'):
+            return func(*args, **kwargs)
+
         # The more complicated user frame plan
         #
         # We would like to record multiple levels of frames, so that we can implement
         # both step and next functionality in the debugger.  However, we don't want to
         # unconditionally dump all the frames, as it's pretty common to be dozens of
         # frame deep from top level launcher code that doesn't matter from the
         # perspective of debugging.
@@ -146,31 +150,29 @@
                 del lcls['self']
             stack.append({
                 'name': frame.f_code.co_name,
                 'line': frame.f_lineno,
                 'filename': file_id,
                 'locals': self._json(lcls),
             })
-            self.lines_traversed[file_id].add(frame.f_lineno)
-            if len(self.lines_traversed[file_id]) > 1:
-                dump_source(filename)
+            dump_source(filename)
 
         while frame:
             if not frame.f_code.co_filename.startswith(uninteresting_dirs):
                 handle_frame(frame, frame.f_locals if frame.f_back is not None else {})
 
             # Stop traversing once we've hit the context manager frame
             if frame is self.frame:
                 break
 
             inner_frame = frame
             frame = frame.f_back
 
         rs = func(*args, **kwargs)
         trace_structured("eager_dispatch", metadata_fn=lambda: {
-            "target": resolve_name(func),
-            "stack": stack,
+            "target": func_name or str(func),
+            "stack": list(reversed(stack)),
             "args": self._json(args),
             "kwargs": self._json(kwargs),
             "ret": self._json(rs),
         })
         return rs
```

### Comparing `torchdbg-0.2.1/PKG-INFO` & `torchdbg-0.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchdbg
-Version: 0.2.1
+Version: 0.3.0
 Summary: PyTorch centric eager mode debugger/tracer
 License: BSD-3
 Author: Edward Z. Yang
 Author-email: ezyang@meta.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

