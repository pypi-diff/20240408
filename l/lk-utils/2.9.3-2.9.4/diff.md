# Comparing `tmp/lk_utils-2.9.3-py3-none-any.whl.zip` & `tmp/lk_utils-2.9.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,26 +1,28 @@
-Zip file size: 23468 bytes, number of entries: 24
--rw-r--r--  2.0 unx     1543 b- defN 80-Jan-01 00:00 lk_utils/__init__.py
+Zip file size: 25181 bytes, number of entries: 26
+-rw-r--r--  2.0 unx     1750 b- defN 80-Jan-01 00:00 lk_utils/__init__.py
 -rw-r--r--  2.0 unx      847 b- defN 80-Jan-01 00:00 lk_utils/__main__.py
--rw-r--r--  2.0 unx      116 b- defN 80-Jan-01 00:00 lk_utils/binding/__init__.py
+-rw-r--r--  2.0 unx      185 b- defN 80-Jan-01 00:00 lk_utils/binding/__init__.py
 -rw-r--r--  2.0 unx     2016 b- defN 80-Jan-01 00:00 lk_utils/binding/binding.py
--rw-r--r--  2.0 unx     4420 b- defN 80-Jan-01 00:00 lk_utils/binding/signal.py
+-rw-r--r--  2.0 unx      696 b- defN 80-Jan-01 00:00 lk_utils/binding/defer.py
+-rw-r--r--  2.0 unx     6350 b- defN 80-Jan-01 00:00 lk_utils/binding/signal.py
 -rw-r--r--  2.0 unx      410 b- defN 80-Jan-01 00:00 lk_utils/common_typing.py
 -rw-r--r--  2.0 unx      141 b- defN 80-Jan-01 00:00 lk_utils/filesniff/__init__.py
 -rw-r--r--  2.0 unx     9735 b- defN 80-Jan-01 00:00 lk_utils/filesniff/finder.py
 -rw-r--r--  2.0 unx     6772 b- defN 80-Jan-01 00:00 lk_utils/filesniff/main.py
 -rw-r--r--  2.0 unx     3753 b- defN 80-Jan-01 00:00 lk_utils/filesniff/shutil.py
 -rw-r--r--  2.0 unx      582 b- defN 80-Jan-01 00:00 lk_utils/filesniff/traceback.py
+-rw-r--r--  2.0 unx     1056 b- defN 80-Jan-01 00:00 lk_utils/importer.py
 -rw-r--r--  2.0 unx     6455 b- defN 80-Jan-01 00:00 lk_utils/read_and_write.py
 -rw-r--r--  2.0 unx      495 b- defN 80-Jan-01 00:00 lk_utils/subproc/__init__.py
 -rw-r--r--  2.0 unx      606 b- defN 80-Jan-01 00:00 lk_utils/subproc/multiprocess.py
 -rw-r--r--  2.0 unx     1816 b- defN 80-Jan-01 00:00 lk_utils/subproc/promise.py
 -rw-r--r--  2.0 unx     5381 b- defN 80-Jan-01 00:00 lk_utils/subproc/subprocess.py
 -rw-r--r--  2.0 unx     8592 b- defN 80-Jan-01 00:00 lk_utils/subproc/threading.py
--rw-r--r--  2.0 unx      981 b- defN 80-Jan-01 00:00 lk_utils/textwrap.py
+-rw-r--r--  2.0 unx     1018 b- defN 80-Jan-01 00:00 lk_utils/textwrap.py
 -rw-r--r--  2.0 unx      203 b- defN 80-Jan-01 00:00 lk_utils/time_utils/__init__.py
 -rw-r--r--  2.0 unx     1533 b- defN 80-Jan-01 00:00 lk_utils/time_utils/time.py
 -rw-r--r--  2.0 unx     5207 b- defN 80-Jan-01 00:00 lk_utils/time_utils/timeit.py
--rw-r--r--  2.0 unx     3897 b- defN 80-Jan-01 00:00 lk_utils-2.9.3.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 lk_utils-2.9.3.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1965 b- defN 16-Jan-01 00:00 lk_utils-2.9.3.dist-info/RECORD
-24 files, 67554 bytes uncompressed, 20298 bytes compressed:  70.0%
+-rw-r--r--  2.0 unx     3897 b- defN 80-Jan-01 00:00 lk_utils-2.9.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 lk_utils-2.9.4.dist-info/WHEEL
+?rw-r--r--  2.0 unx     2124 b- defN 16-Jan-01 00:00 lk_utils-2.9.4.dist-info/RECORD
+26 files, 71708 bytes uncompressed, 21769 bytes compressed:  69.6%
```

## zipnote {}

```diff
@@ -6,14 +6,17 @@
 
 Filename: lk_utils/binding/__init__.py
 Comment: 
 
 Filename: lk_utils/binding/binding.py
 Comment: 
 
+Filename: lk_utils/binding/defer.py
+Comment: 
+
 Filename: lk_utils/binding/signal.py
 Comment: 
 
 Filename: lk_utils/common_typing.py
 Comment: 
 
 Filename: lk_utils/filesniff/__init__.py
@@ -27,14 +30,17 @@
 
 Filename: lk_utils/filesniff/shutil.py
 Comment: 
 
 Filename: lk_utils/filesniff/traceback.py
 Comment: 
 
+Filename: lk_utils/importer.py
+Comment: 
+
 Filename: lk_utils/read_and_write.py
 Comment: 
 
 Filename: lk_utils/subproc/__init__.py
 Comment: 
 
 Filename: lk_utils/subproc/multiprocess.py
@@ -57,17 +63,17 @@
 
 Filename: lk_utils/time_utils/time.py
 Comment: 
 
 Filename: lk_utils/time_utils/timeit.py
 Comment: 
 
-Filename: lk_utils-2.9.3.dist-info/METADATA
+Filename: lk_utils-2.9.4.dist-info/METADATA
 Comment: 
 
-Filename: lk_utils-2.9.3.dist-info/WHEEL
+Filename: lk_utils-2.9.4.dist-info/WHEEL
 Comment: 
 
-Filename: lk_utils-2.9.3.dist-info/RECORD
+Filename: lk_utils-2.9.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## lk_utils/__init__.py

```diff
@@ -1,11 +1,12 @@
 if 1:
     import lk_logger
-    lk_logger.setup(quiet=True)
+    lk_logger.setup(quiet=True, show_funcname=False, show_varnames=True)
 
+from . import binding
 from . import common_typing as t
 from . import common_typing as typing
 from . import filesniff
 from . import filesniff as fs
 from . import read_and_write
 from . import read_and_write as rw
 from . import subproc
@@ -29,19 +30,23 @@
 from .filesniff import findall_files
 from .filesniff import get_current_dir
 from .filesniff import make_link as mklink
 from .filesniff import make_links as mklinks
 from .filesniff import normpath
 from .filesniff import xpath
 from .filesniff import xpath as relpath  # backward compatible
+# from .importer import get_module
+# from .importer import get_package
+# from .importer import load_module
+# from .importer import load_package
 from .read_and_write import dumps
 from .read_and_write import loads
 from .read_and_write import ropen
 from .read_and_write import wopen
 from .subproc import new_thread
 from .subproc import run_cmd_args
 from .subproc import run_cmd_line
 from .subproc import run_new_thread
 from .time_utils import timestamp
 from .time_utils import wait
 
-__version__ = '2.9.3'
+__version__ = '2.9.4'
```

## lk_utils/binding/__init__.py

```diff
@@ -1,4 +1,6 @@
 from .binding import bind_with
 from .binding import call_once
+# from .defer import define_later
+# from .defer import iterate_later
 from .signal import Signal
 from .signal import config
```

## lk_utils/binding/signal.py

```diff
@@ -1,7 +1,9 @@
+import re
+import textwrap
 import typing as t
 from contextlib import contextmanager
 from functools import partial
 from types import FunctionType
 
 
 class T:
@@ -9,57 +11,67 @@
     Func = t.Union[FunctionType, t.Callable]
     # Func = FunctionType
     # Func = t.Callable
     FuncId = str
     Funcs = t.Dict[FuncId, Func]
 
 
-class _Config:
+class _Config:  # DELETE
     duplicate_locals_scheme: T.DuplicateLocalsScheme = 'override'
     # use_thread_pool: bool = False
 
 
 config = _Config()
 
 
-class _Signal:
+class Signal:
     _funcs: T.Funcs
+
+    def __class_getitem__(cls, *_: t.Any) -> t.Type['Signal']:
+        """
+        use square brackets to annotate a signal type.
+        https://stackoverflow.com/a/68982326
+        usage:
+            some_signal: Signal[int, str]
+        """
+        return cls
     
-    def __init__(self):
+    def __init__(self, *_) -> None:
         self._funcs = {}
     
     def __bool__(self) -> bool:
         return bool(self._funcs)
     
     def __len__(self) -> int:
         return len(self._funcs)
     
     # decorator
     def __call__(self, func: T.Func) -> T.Func:
         self.bind(func)
         return func
     
-    def emit(self, *_args, **_kwargs) -> None:
+    def emit(self, *_args, error_level: int = 1, **_kwargs) -> None:
+        """
+        error_level: see `_PropagationChain._error_level:comment`
+        """
         if not self._funcs: return
+
         # print(self._funcs, ':l')
-        with _propagation_chain.locking(self):
+        with _prop_chain.locking(self, error_level):
             f: T.Func
             for f in tuple(self._funcs.values()):
-                if _propagation_chain.check(f):
+                if _prop_chain.check(f):
                     try:
                         f(*_args, **_kwargs)
                     except Exception as e:
                         print(':e', e)
-                else:
-                    print(
-                        'function prevented because '
-                        'out of propagation chain', f
-                    )
+                # else:  # TODO: should we break here or use `config` to decide?
+                #     break
     
-    # DELETE: we don't want to use `name` param in future.
+    # DELETE: param `name` may be removed in future.
     def bind(self, func: T.Func, name: str = None) -> T.FuncId:
         id = name or get_func_id(func)
         if (
             id in self._funcs and
             config.duplicate_locals_scheme == 'ignore'
         ):
             return id
@@ -75,77 +87,111 @@
     
     def unbind_all(self) -> None:
         self._funcs.clear()
     
     clear = unbind_all
 
 
-class SignalFactory:
-    
-    def __getitem__(self, *types: t.Type) -> t.Type[_Signal]:
-        return _Signal
-    
-    def __call__(self, *types: t.Type) -> _Signal:
-        return _Signal()
-
-
-Signal = SignalFactory()
-
-
 class _PropagationChain:
     """
-    a chain to check and avoid infinite loop, which may be caused by mutual
+    a chain to check and avoid infinite loop, which may be caused by mutual -
     signal binding.
     """
     
-    _chain: t.Set[T.FuncId]
+    _chain: t.List[T.FuncId]
+    _error_level: int
+    #   0: no error print
+    #   1: brief error print
+    #   2: detailed error print
+    #   3: detailed error print and raise error
     _is_locked: bool
-    _lock_owner: t.Optional[_Signal]
+    _lock_owner: t.Optional[Signal]
     
-    def __init__(self):
-        self._chain = set()
+    def __init__(self) -> None:
+        self._chain = []
+        self._error_level = 0
         self._is_locked = False
         self._lock_owner = None
     
+    # @property
+    # def chain(self) -> t.List[T.FuncId]:
+    #     return self._chain
+
     @property
-    def lock_owner(self) -> t.Optional[_Signal]:
+    def lock_owner(self) -> t.Optional[Signal]:
         return self._lock_owner
     
     @contextmanager
-    def locking(self, owner: _Signal) -> None:
-        self.lock(owner)
+    def locking(self, owner: Signal, error_level: int = 1) -> t.Iterator[None]:
+        self.lock(owner, error_level)
         yield
         self.unlock(owner)
     
     def check(self, func: T.Func) -> bool:
         """
         check if function already triggered in this propagation chain.
         """
         if (id := get_func_id(func)) not in self._chain:
-            self._chain.add(id)
+            self._chain.append(id)
             return True
-        else:
-            return False
+        
+        def print_error_details() -> None:
+            chain = tuple(map(_pretty_id, self._chain))
+            if len(chain) == 1:
+                diagram = (
+                    '╭─▶ 1. {}'.format(chain[0]),
+                    '╰─x 2. {}'.format(chain[0]),
+                )
+            else:
+                diagram = (
+                    '╭─▶ 1. {}'.format(chain[0]),
+                    *(
+                        '│   {}. {}'.format(i, x) 
+                        for i, x in enumerate(chain[1:], 2)
+                    ),
+                    '╰─x {}. {}'.format(len(chain) + 1, chain[0]),
+                )
+
+            print(textwrap.dedent('''
+                signal prevented because of circular emissions:
+                    {}
+            ''').format(
+                textwrap.indent('\n'.join(diagram), '    ').lstrip()
+            ), ':p3v4s')
+
+        def _pretty_id(func_id: T.FuncId) -> str:
+            a, b, c = re.fullmatch(r'(.+)\((.+):(.+)\)', func_id).groups()
+            b = re.split(r'[/\\]', b)[-1]
+            return f'{a} ({b}:{c})'
+
+        if self._error_level == 1:
+            print('signal prevented because of circular emissions', ':p2vs')
+        elif self._error_level == 2:
+            print_error_details()
+        elif self._error_level == 3:
+            print_error_details()
+            raise RecursionError('circular signal emissions')
+        return False
     
-    def lock(self, owner: _Signal) -> bool:
+    def lock(self, owner: Signal, error_level: int = 1) -> bool:
         if self._lock_owner:
             return False
+        # assert not self._chain
+        self._error_level = error_level
         self._is_locked = True
         self._lock_owner = owner
-        # assert not self._chain
-        # # self._chain.clear()
-        # print(f'locked by {owner}', ':pv')
         return True
     
-    def unlock(self, controller: _Signal) -> bool:
-        if self._lock_owner != controller:
+    def unlock(self, controller: Signal) -> bool:
+        if controller is not self._lock_owner:
             return False
+        self._chain.clear()
+        self._error_level = 0
         self._is_locked = False
         self._lock_owner = None
-        self._chain.clear()
         return True
 
 
 # def get_func_args_count(func: FunctionType) -> int:
 #     cnt = func.__code__.co_argcount - len(func.__defaults__ or ())
 #     if 'method' in str(func.__class__): cnt -= 1
 #     return cnt
@@ -154,14 +200,17 @@
 def get_func_id(func: T.Func) -> T.FuncId:
     # related test: tests/duplicate_locals.py
     if config.duplicate_locals_scheme == 'exclusive':
         return str(id(func))
     else:
         # https://stackoverflow.com/a/46479810
         if isinstance(func, partial):
-            # fix: `functools.partial` has no `__qualname__`.
-            return func.func.__qualname__
-        else:
-            return func.__qualname__
+            func = func.func
+        # # return func.__qualname__
+        return '{}({}:{})'.format(
+            func.__qualname__,
+            func.__code__.co_filename, 
+            func.__code__.co_firstlineno,
+        )
 
 
-_propagation_chain = _PropagationChain()
+_prop_chain = _PropagationChain()
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## lk_utils/textwrap.py

```diff
@@ -7,17 +7,18 @@
 def dedent(text: str, lstrip: bool = True, join_sep: str = None) -> str:
     """
     params:
         join_sep: suggest: '-', '|' or '\\'.
     """
     out = textwrap.dedent(text).rstrip()
     if join_sep:
-        if join_sep == '\\':
-            join_sep = '\\\\'  # escape for regular expression
-        out = re.sub(rf' +{join_sep} *\n', ' ', out)
+        if '\\' in join_sep:
+            # escape for regular expression
+            join_sep = join_sep.replace('\\', '\\\\')
+        out = re.sub(rf' +{join_sep} *\n *', ' ', out)
     return out.lstrip() if lstrip else out
 
 
 def indent(text: str, spaces: int = 4, rstrip: bool = True) -> str:
     out = textwrap.indent(text, ' ' * spaces)
     return out.rstrip() if rstrip else out
```

## Comparing `lk_utils-2.9.3.dist-info/METADATA` & `lk_utils-2.9.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lk-utils
-Version: 2.9.3
+Version: 2.9.4
 Summary: LK Utils is a set of utility wrappers made for data processing.
 License: MIT
 Author: Likianta
 Author-email: likianta@foxmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `lk_utils-2.9.3.dist-info/RECORD` & `lk_utils-2.9.4.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,26 @@
-lk_utils/__init__.py,sha256=qVakJ0J5hKCAjKMiP6vFjlEIVRgwN1LkME3pKpM4XLs,1543
+lk_utils/__init__.py,sha256=CImGoWF30TAjKXTVtcpBkfscEEubGWrViVUr8l7stAY,1750
 lk_utils/__main__.py,sha256=KA4dDZb-xAV20iKRTg_YijCSOGepJG_j8h0O6VMYuu8,847
-lk_utils/binding/__init__.py,sha256=O-A9LpGPWVeczBdoz8vbul3o0WdUgk4khjAGjQg34aA,116
+lk_utils/binding/__init__.py,sha256=Jk4aZkU0EA5dT8r6RUKjKQ1qAdJpHG9c3GwnuWawHww,185
 lk_utils/binding/binding.py,sha256=pATcRkfHMAwWAk7GsYS8xXx4B1w004mj1GG8PTCg2Vc,2016
-lk_utils/binding/signal.py,sha256=GQOjB08r_wnpGVhaxDr0nfa5R6UcM_QcICfrBTgFIio,4420
+lk_utils/binding/defer.py,sha256=tskWv8YveJAWNhAjEY1o7ME_L6ubwMcAJ0jNO1eCZOo,696
+lk_utils/binding/signal.py,sha256=cB8hjMW4OOUkCuHKafVlR7SjySDnvrqWyvSvl57R-jE,6350
 lk_utils/common_typing.py,sha256=k-bc-wizItD81mIlTPhzSJmtaoFXKjCP4HrZJhJJUx8,410
 lk_utils/filesniff/__init__.py,sha256=rtggL_f0-XRZga_t8jWg8sbIwDFsJUIYz-PFcHE0daM,141
 lk_utils/filesniff/finder.py,sha256=6RCryziJqByUPCUBk7ugSeITKaoO_SPBX9z9TObQY-o,9735
 lk_utils/filesniff/main.py,sha256=QK_yxep5KUu9JiDqCnPFAq4ZhGVWiqW_fxIc9Qk_4jo,6772
 lk_utils/filesniff/shutil.py,sha256=qMVWopIGW_TRxGXY_qpEgEMLh9tIyQ2jJeHuYVbT8HU,3753
 lk_utils/filesniff/traceback.py,sha256=SoJjnT2ArSrgR3NGOtQ_awCyMQga-e7W6ij7jp0zfdA,582
+lk_utils/importer.py,sha256=SoJciwW2pUahqdWn_HtNSV2x9sAkpmkghFeqsMHmXlc,1056
 lk_utils/read_and_write.py,sha256=oLmGlyFCrOogTWXm-_IyMnmidzSA4gRlh1abE5OGSz0,6455
 lk_utils/subproc/__init__.py,sha256=unuknQy_ylsVHNjWexRlBXIqWX4rPSJvQmD1_1WdSWE,495
 lk_utils/subproc/multiprocess.py,sha256=rWLUB9y-_WtVq63E20fQUG4KLGr-I1vhrBopJ5yms0M,606
 lk_utils/subproc/promise.py,sha256=MKH1oUHYxxq-65yyDcJxsI-v_QOVPOIbJJAqVOrS9v0,1816
 lk_utils/subproc/subprocess.py,sha256=DZ8wgwoyae2GLG-KqFASQY_0ZcJZSpfhRT-0JefxlVk,5381
 lk_utils/subproc/threading.py,sha256=m9pWtcMkwlGqL4w5_rPazUVM96tDUEhb5UNB6qQTxMg,8592
-lk_utils/textwrap.py,sha256=t5KJkdWmmHLCgBbHIKZwbJEOeRAVUvIr0lsYkwVLMww,981
+lk_utils/textwrap.py,sha256=LHNz-HcijyLJFjhSwGRnq7SUsSWktiJ-Sp6hRLSMnCA,1018
 lk_utils/time_utils/__init__.py,sha256=IUPhGSeyiDdNfJpEFAhNd0rMb2CaxIqZo8yKfAUmK5g,203
 lk_utils/time_utils/time.py,sha256=orUzrsQ81fvLIQShEeam-2QfF8IRHITZN--KMbmRO4I,1533
 lk_utils/time_utils/timeit.py,sha256=3QtXEelzxWpUG8LKayn6jkITXPSuSdD7hVbyYXvK8dA,5207
-lk_utils-2.9.3.dist-info/METADATA,sha256=yIWZJBk8eVVzwrI3xMKmYaIDR4gtuGUnZFTmRx6iwXw,3897
-lk_utils-2.9.3.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-lk_utils-2.9.3.dist-info/RECORD,,
+lk_utils-2.9.4.dist-info/METADATA,sha256=My9Y6xCcDRB5m4pxbWSInvSY7ASEueFvfUQsHmuNF-Q,3897
+lk_utils-2.9.4.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+lk_utils-2.9.4.dist-info/RECORD,,
```

