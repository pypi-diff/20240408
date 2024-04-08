# Comparing `tmp/productor-0.1.0.tar.gz` & `tmp/productor-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "productor-0.1.0.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `productor-0.1.0.tar` & `productor-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,25 @@
--rw-r--r--   0        0        0     1317 2024-04-07 05:44:59.918350 productor-0.1.0/LICENSE
--rw-r--r--   0        0        0      179 2024-04-07 05:55:54.974862 productor-0.1.0/productor/__init__.py
--rw-r--r--   0        0        0      187 2024-04-07 05:54:13.741770 productor-0.1.0/productor/__version__.py
--rw-r--r--   0        0        0     6025 2024-04-07 07:31:58.204297 productor-0.1.0/productor/productor.py
--rw-r--r--   0        0        0      207 2024-04-07 06:34:30.978945 productor-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      706 1970-01-01 00:00:00.000000 productor-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 productor-0.1.1/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 productor-0.1.1/setup.py
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 productor-0.1.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 productor-0.1.1/.github/workflows/test-release.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 productor-0.1.1/examples/__init__.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 productor-0.1.1/examples/abc/__init__.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 productor-0.1.1/examples/abc/animal.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 productor-0.1.1/examples/abc/cat.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 productor-0.1.1/examples/abc/dog.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 productor-0.1.1/examples/protocol/__init__.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 productor-0.1.1/examples/protocol/animal.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 productor-0.1.1/examples/protocol/cat.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 productor-0.1.1/examples/protocol/dog.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 productor-0.1.1/examples/subclass/__init__.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 productor-0.1.1/examples/subclass/animal.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 productor-0.1.1/examples/subclass/cat.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 productor-0.1.1/examples/subclass/dog.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 productor-0.1.1/productor/__init__.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 productor-0.1.1/productor/__version__.py
+-rw-r--r--   0        0        0     5843 2020-02-02 00:00:00.000000 productor-0.1.1/productor/productor.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 productor-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 productor-0.1.1/LICENSE
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 productor-0.1.1/README.md
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 productor-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 productor-0.1.1/PKG-INFO
```

### Comparing `productor-0.1.0/LICENSE` & `productor-0.1.1/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-BSD 2-Clause License
-
-Copyright (c) 2024, swxs
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-1. Redistributions of source code must retain the above copyright notice, this
-   list of conditions and the following disclaimer.
-
-2. Redistributions in binary form must reproduce the above copyright notice,
-   this list of conditions and the following disclaimer in the documentation
-   and/or other materials provided with the distribution.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+BSD 2-Clause License
+
+Copyright (c) 2024, swxs
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `productor-0.1.0/productor/productor.py` & `productor-0.1.1/productor/productor.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,182 +1,182 @@
-# -*- coding: utf-8 -*-
-# @File    : Helper_productor.py
-# @AUTH    : swxs
-# @Time    : 2019/6/27 16:37
-
-import os
-import sys
-import random
-import logging
-from fnmatch import fnmatch
-from importlib import import_module
-from typing import TypeVar, Optional, Union, Dict, Set, Generic, _ProtocolMeta
-
-logger = logging.getLogger("helper.productor")
-
-T = TypeVar('T', bound=type)
-
-
-class Productor(Generic[T]):
-    def __init__(
-        self,
-        root_dir: str,
-        start_dir: str,
-        base_module: T,
-        temp_module: Optional[T],
-        pattern: str = '*.py',
-    ):
-        """
-        简介
-        ----------
-        通过实例化Productor来初始化工厂(假设为productor)
-        获取子类: productor[name]
-        删除子类: del productor[name]
-
-        参数
-        ----------
-        root_dir :
-            系统根目录
-        start_dir :
-            查询根目录
-        base_module :
-            基础模块，所有查询对象应该是该类的子类
-        temp_module :
-            默认模块，设置为None时， 若没有查询到对象，会报NoModuleException
-        pattern [可选]: 默认为 '*.py'
-            文件匹配规则， 可以减小匹配范围加速匹配
-        """
-        # 所有加载模块的容器
-        self.__productor: Dict[Union[str, int], T] = {}
-        self.__path: Dict[Union[str, int], str] = {}
-        self.__loaded_path: Set[str] = set()
-
-        self.base_module = base_module
-        self.temp_module = temp_module
-
-        self.root_dir = root_dir
-        self.start_dir = os.path.abspath(start_dir)
-        if not os.path.isdir(self.start_dir):
-            raise
-        self.pattern = pattern
-
-    def __getitem__(self, item: Union[str, int]) -> T:
-        """
-        简介
-        ----------
-        尝试匹配指定name、__name__属性的子类或接口实现
-        未匹配成功的情况下返回默认模块或直接报ImportError异常
-
-        参数
-        ----------
-        item :
-        指定的__name__, 可以为数值或者字符串
-
-        返回
-        ----------
-        对应子类
-
-        异常
-        ----------
-
-        """
-        if item not in self.__productor:
-            self.__discover()
-
-        if item in self.__productor:
-            return self.__productor[item]
-
-        if self.temp_module:
-            return self.temp_module
-        else:
-            raise ImportError(f'temp module and {item} not found!')
-
-    def __delitem__(self, item: Union[str, int]) -> None:
-        del sys.modules[self.__path[item]]
-        del self.__productor[item]
-        self.__loaded_path.remove(self.__path[item])
-        del self.__path[item]
-
-    def __contains__(self, item: Union[str, int]) -> bool:
-        return item in self.__productor
-
-    def latest(self) -> T:
-        self.__discover()
-
-        if self.__productor:
-            return self.__productor[max(self.__productor.keys())]
-
-        if self.temp_module:
-            return self.temp_module
-        else:
-            raise ImportError(f'temp module not found!')
-
-    def random(self) -> T:
-        self.__discover()
-
-        if self.__productor:
-            return self.__productor[random.choice(list(self.__productor.keys()))]
-
-        if self.temp_module:
-            return self.temp_module
-        else:
-            raise ImportError(f'temp module not found!')
-
-    def __match_path(self, path, full_path, pattern):
-        # override this method to use alternative matching strategy
-        return fnmatch(path, pattern)
-
-    def __path_2_modulepath(self, path='') -> Optional[str]:
-        if path:
-            path = path.replace('\\', '/').replace(self.root_dir.replace('\\', '/'), '')
-            if path.startswith('/'):
-                path = path[1:]
-            path = path.replace('.py', '').replace('.PY', '')
-            if set('.#~') & set(path):
-                return None
-            path = path.replace('/', '.').strip()
-            if path:
-                return path
-        return None
-
-    def __load_module(self, module: T, module_path: str) -> None:
-        try:
-            name = getattr(module, "name")
-        except Exception:
-            name = getattr(module, "__name__")
-        self.__productor[name] = module
-        self.__path[name] = module_path
-
-    def __discover(self) -> None:
-        # 遍历所有文件, 并尝试匹配name并导入符合条件的子类或实现接口方法的类
-        for root, dirs, files in os.walk(self.start_dir):
-            for file_name in files:
-                full_path = os.path.join(root, file_name)
-                if not self.__match_path(file_name, full_path, self.pattern):
-                    continue
-
-                try:
-                    module_path = self.__path_2_modulepath(full_path)
-                    if module_path is None:
-                        continue
-
-                    if full_path in self.__loaded_path:
-                        continue
-                    else:
-                        self.__loaded_path.add(full_path)
-
-                    module = import_module(module_path)
-
-                    for name in dir(module):
-                        obj: T = getattr(module, name)
-                        if (
-                            isinstance(obj, type)
-                            and getattr(obj, "__module__") == module_path
-                            and issubclass(obj, self.base_module)
-                            and not isinstance(obj, _ProtocolMeta)
-                        ):
-                            try:
-                                self.__load_module(obj, module_path)
-                            except Exception as e:
-                                logger.warning(f'import {full_path} error: {e}')
-                except Exception as e:
-                    logger.warning(f'other error: {e}')
+# -*- coding: utf-8 -*-
+# @File    : Helper_productor.py
+# @AUTH    : swxs
+# @Time    : 2019/6/27 16:37
+
+import os
+import sys
+import random
+import logging
+from fnmatch import fnmatch
+from importlib import import_module
+from typing import TypeVar, Optional, Union, Dict, Set, Generic, _ProtocolMeta
+
+logger = logging.getLogger("helper.productor")
+
+T = TypeVar('T', bound=type)
+
+
+class Productor(Generic[T]):
+    def __init__(
+        self,
+        root_dir: str,
+        start_dir: str,
+        base_module: T,
+        temp_module: Optional[T],
+        pattern: str = '*.py',
+    ):
+        """
+        简介
+        ----------
+        通过实例化Productor来初始化工厂(假设为productor)
+        获取子类: productor[name]
+        删除子类: del productor[name]
+
+        参数
+        ----------
+        root_dir :
+            系统根目录
+        start_dir :
+            查询根目录
+        base_module :
+            基础模块，所有查询对象应该是该类的子类
+        temp_module :
+            默认模块，设置为None时， 若没有查询到对象，会报NoModuleException
+        pattern [可选]: 默认为 '*.py'
+            文件匹配规则， 可以减小匹配范围加速匹配
+        """
+        # 所有加载模块的容器
+        self.__productor: Dict[Union[str, int], T] = {}
+        self.__path: Dict[Union[str, int], str] = {}
+        self.__loaded_path: Set[str] = set()
+
+        self.base_module = base_module
+        self.temp_module = temp_module
+
+        self.root_dir = root_dir
+        self.start_dir = os.path.abspath(start_dir)
+        if not os.path.isdir(self.start_dir):
+            raise
+        self.pattern = pattern
+
+    def __getitem__(self, item: Union[str, int]) -> T:
+        """
+        简介
+        ----------
+        尝试匹配指定name、__name__属性的子类或接口实现
+        未匹配成功的情况下返回默认模块或直接报ImportError异常
+
+        参数
+        ----------
+        item :
+        指定的__name__, 可以为数值或者字符串
+
+        返回
+        ----------
+        对应子类
+
+        异常
+        ----------
+
+        """
+        if item not in self.__productor:
+            self.__discover()
+
+        if item in self.__productor:
+            return self.__productor[item]
+
+        if self.temp_module:
+            return self.temp_module
+        else:
+            raise ImportError(f'temp module and {item} not found!')
+
+    def __delitem__(self, item: Union[str, int]) -> None:
+        del sys.modules[self.__path[item]]
+        del self.__productor[item]
+        self.__loaded_path.remove(self.__path[item])
+        del self.__path[item]
+
+    def __contains__(self, item: Union[str, int]) -> bool:
+        return item in self.__productor
+
+    def latest(self) -> T:
+        self.__discover()
+
+        if self.__productor:
+            return self.__productor[max(self.__productor.keys())]
+
+        if self.temp_module:
+            return self.temp_module
+        else:
+            raise ImportError(f'temp module not found!')
+
+    def random(self) -> T:
+        self.__discover()
+
+        if self.__productor:
+            return self.__productor[random.choice(list(self.__productor.keys()))]
+
+        if self.temp_module:
+            return self.temp_module
+        else:
+            raise ImportError(f'temp module not found!')
+
+    def __match_path(self, path, full_path, pattern):
+        # override this method to use alternative matching strategy
+        return fnmatch(path, pattern)
+
+    def __path_2_modulepath(self, path='') -> Optional[str]:
+        if path:
+            path = path.replace('\\', '/').replace(self.root_dir.replace('\\', '/'), '')
+            if path.startswith('/'):
+                path = path[1:]
+            path = path.replace('.py', '').replace('.PY', '')
+            if set('.#~') & set(path):
+                return None
+            path = path.replace('/', '.').strip()
+            if path:
+                return path
+        return None
+
+    def __load_module(self, module: T, module_path: str) -> None:
+        try:
+            name = getattr(module, "name")
+        except Exception:
+            name = getattr(module, "__name__")
+        self.__productor[name] = module
+        self.__path[name] = module_path
+
+    def __discover(self) -> None:
+        # 遍历所有文件, 并尝试匹配name并导入符合条件的子类或实现接口方法的类
+        for root, dirs, files in os.walk(self.start_dir):
+            for file_name in files:
+                full_path = os.path.join(root, file_name)
+                if not self.__match_path(file_name, full_path, self.pattern):
+                    continue
+
+                try:
+                    module_path = self.__path_2_modulepath(full_path)
+                    if module_path is None:
+                        continue
+
+                    if full_path in self.__loaded_path:
+                        continue
+                    else:
+                        self.__loaded_path.add(full_path)
+
+                    module = import_module(module_path)
+
+                    for name in dir(module):
+                        obj: T = getattr(module, name)
+                        if (
+                            isinstance(obj, type)
+                            and getattr(obj, "__module__") == module_path
+                            and issubclass(obj, self.base_module)
+                            and not isinstance(obj, _ProtocolMeta)
+                        ):
+                            try:
+                                self.__load_module(obj, module_path)
+                            except Exception as e:
+                                logger.warning(f'import {full_path} error: {e}')
+                except Exception as e:
+                    logger.warning(f'other error: {e}')
```

