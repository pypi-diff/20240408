# Comparing `tmp/pybts-1.3.1.tar.gz` & `tmp/pybts-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybts-1.3.1.tar", max compression
+gzip compressed data, was "pybts-1.3.3.tar", max compression
```

## Comparing `pybts-1.3.1.tar` & `pybts-1.3.3.tar`

### file list

```diff
@@ -1,29 +1,33 @@
--rw-r--r--   0        0        0   157658 2024-04-02 10:08:08.027734 pybts-1.3.1/README.assets/DEMO_Sequence  10-10 _ 100.png
--rw-r--r--   0        0        0   189323 2024-04-02 10:08:08.027734 pybts-1.3.1/README.assets/image-20240329031220580.png
--rw-r--r--   0        0        0   208202 2024-04-02 10:08:08.031734 pybts-1.3.1/README.assets/image-20240329031233459.png
--rw-r--r--   0        0        0   255608 2024-04-02 10:08:08.031734 pybts-1.3.1/README.assets/image-20240401211552611.png
--rw-r--r--   0        0        0   202283 2024-04-02 10:08:08.031734 pybts-1.3.1/README.assets/image-20240401211609525.png
--rw-r--r--   0        0        0     5830 2024-04-02 10:08:08.031734 pybts-1.3.1/README.md
--rw-r--r--   0        0        0      420 2024-04-02 10:08:08.031734 pybts-1.3.1/pybts/__init__.py
--rw-r--r--   0        0        0     2258 2024-04-02 10:08:08.031734 pybts-1.3.1/pybts/board.py
--rw-r--r--   0        0        0     9355 2024-04-02 10:08:08.031734 pybts-1.3.1/pybts/board_server.py
--rw-r--r--   0        0        0     4027 2024-04-02 10:08:08.031734 pybts-1.3.1/pybts/builder.py
--rw-r--r--   0        0        0      473 2024-04-02 10:08:08.035734 pybts-1.3.1/pybts/composites/__init__.py
--rw-r--r--   0        0        0     8709 2024-04-02 10:08:08.035734 pybts-1.3.1/pybts/composites/composite.py
--rw-r--r--   0        0        0     2420 2024-04-02 10:08:08.035734 pybts-1.3.1/pybts/composites/condition_branch.py
--rw-r--r--   0        0        0     5969 2024-04-02 10:08:08.035734 pybts-1.3.1/pybts/composites/parallel.py
--rw-r--r--   0        0        0     2317 2024-04-02 10:08:08.035734 pybts-1.3.1/pybts/composites/selector.py
--rw-r--r--   0        0        0     2541 2024-04-02 10:08:08.035734 pybts-1.3.1/pybts/composites/sequence.py
--rw-r--r--   0        0        0     3220 2024-04-02 10:08:08.035734 pybts-1.3.1/pybts/constants.py
--rw-r--r--   0        0        0      121 2024-04-02 10:08:08.035734 pybts-1.3.1/pybts/decorators/__init__.py
--rw-r--r--   0        0        0    17113 2024-04-02 10:08:08.035734 pybts-1.3.1/pybts/decorators/nodes.py
--rw-r--r--   0        0        0     1533 2024-04-02 10:08:08.035734 pybts-1.3.1/pybts/main.py
--rw-r--r--   0        0        0     5342 2024-04-02 10:08:08.035734 pybts-1.3.1/pybts/node.py
--rw-r--r--   0        0        0    16958 2024-04-02 10:08:08.035734 pybts-1.3.1/pybts/templates/favicon.ico
--rw-r--r--   0        0        0      433 2024-04-02 10:08:08.035734 pybts-1.3.1/pybts/templates/index.html
--rw-r--r--   0        0        0  1966405 2024-04-02 10:08:08.043734 pybts-1.3.1/pybts/templates/static/index-BUWP2os5.js
--rw-r--r--   0        0        0   320362 2024-04-02 10:08:08.047734 pybts-1.3.1/pybts/templates/static/index-BXdrQGHp.css
--rw-r--r--   0        0        0      506 2024-04-02 10:08:08.047734 pybts-1.3.1/pybts/tree.py
--rw-r--r--   0        0        0     8689 2024-04-02 10:08:08.047734 pybts-1.3.1/pybts/utility.py
--rw-r--r--   0        0        0      609 2024-04-02 10:08:08.047734 pybts-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     6550 1970-01-01 00:00:00.000000 pybts-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0   157658 2024-04-08 02:36:46.847127 pybts-1.3.3/README.assets/DEMO_Sequence  10-10 _ 100.png
+-rw-r--r--   0        0        0   189323 2024-04-08 02:36:46.847127 pybts-1.3.3/README.assets/image-20240329031220580.png
+-rw-r--r--   0        0        0   208202 2024-04-08 02:36:46.851127 pybts-1.3.3/README.assets/image-20240329031233459.png
+-rw-r--r--   0        0        0   255608 2024-04-08 02:36:46.851127 pybts-1.3.3/README.assets/image-20240401211552611.png
+-rw-r--r--   0        0        0   202283 2024-04-08 02:36:46.851127 pybts-1.3.3/README.assets/image-20240401211609525.png
+-rw-r--r--   0        0        0     5877 2024-04-08 02:36:46.851127 pybts-1.3.3/README.md
+-rw-r--r--   0        0        0      393 2024-04-08 02:36:46.851127 pybts-1.3.3/pybts/__init__.py
+-rw-r--r--   0        0        0       52 2024-04-08 02:36:46.855127 pybts-1.3.3/pybts/board/__init__.py
+-rw-r--r--   0        0        0     2257 2024-04-08 02:36:46.855127 pybts-1.3.3/pybts/board/board.py
+-rw-r--r--   0        0        0     9681 2024-04-08 02:36:46.855127 pybts-1.3.3/pybts/board/server.py
+-rw-r--r--   0        0        0     4138 2024-04-08 02:36:46.855127 pybts-1.3.3/pybts/builder.py
+-rw-r--r--   0        0        0      473 2024-04-08 02:36:46.855127 pybts-1.3.3/pybts/composites/__init__.py
+-rw-r--r--   0        0        0     8760 2024-04-08 02:36:46.855127 pybts-1.3.3/pybts/composites/composite.py
+-rw-r--r--   0        0        0     2246 2024-04-08 02:36:46.855127 pybts-1.3.3/pybts/composites/condition_branch.py
+-rw-r--r--   0        0        0     5862 2024-04-08 02:36:46.855127 pybts-1.3.3/pybts/composites/parallel.py
+-rw-r--r--   0        0        0     2405 2024-04-08 02:36:46.855127 pybts-1.3.3/pybts/composites/selector.py
+-rw-r--r--   0        0        0     2606 2024-04-08 02:36:46.855127 pybts-1.3.3/pybts/composites/sequence.py
+-rw-r--r--   0        0        0     3242 2024-04-08 02:36:46.855127 pybts-1.3.3/pybts/constants.py
+-rw-r--r--   0        0        0      121 2024-04-08 02:36:46.855127 pybts-1.3.3/pybts/decorators/__init__.py
+-rw-r--r--   0        0        0    16991 2024-04-08 02:36:46.855127 pybts-1.3.3/pybts/decorators/nodes.py
+-rw-r--r--   0        0        0     1521 2024-04-08 02:36:46.855127 pybts-1.3.3/pybts/main.py
+-rw-r--r--   0        0        0     5668 2024-04-08 02:36:46.855127 pybts-1.3.3/pybts/node.py
+-rw-r--r--   0        0        0      115 2024-04-08 02:36:46.855127 pybts-1.3.3/pybts/rl/__init__.py
+-rw-r--r--   0        0        0      459 2024-04-08 02:36:46.855127 pybts-1.3.3/pybts/rl/common.py
+-rw-r--r--   0        0        0    13320 2024-04-08 02:36:46.855127 pybts-1.3.3/pybts/rl/on_policy.py
+-rw-r--r--   0        0        0    16958 2024-04-08 02:36:46.855127 pybts-1.3.3/pybts/templates/favicon.ico
+-rw-r--r--   0        0        0      433 2024-04-08 02:36:46.855127 pybts-1.3.3/pybts/templates/index.html
+-rw-r--r--   0        0        0  1966405 2024-04-08 02:36:46.867127 pybts-1.3.3/pybts/templates/static/index-BUWP2os5.js
+-rw-r--r--   0        0        0   320362 2024-04-08 02:36:46.867127 pybts-1.3.3/pybts/templates/static/index-BXdrQGHp.css
+-rw-r--r--   0        0        0      800 2024-04-08 02:36:46.867127 pybts-1.3.3/pybts/tree.py
+-rw-r--r--   0        0        0     8814 2024-04-08 02:36:46.867127 pybts-1.3.3/pybts/utility.py
+-rw-r--r--   0        0        0      844 2024-04-08 02:36:46.867127 pybts-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0     6796 1970-01-01 00:00:00.000000 pybts-1.3.3/PKG-INFO
```

### Comparing `pybts-1.3.1/README.assets/DEMO_Sequence  10-10 _ 100.png` & `pybts-1.3.3/README.assets/DEMO_Sequence  10-10 _ 100.png`

 * *Files identical despite different names*

### Comparing `pybts-1.3.1/README.assets/image-20240329031220580.png` & `pybts-1.3.3/README.assets/image-20240329031220580.png`

 * *Files identical despite different names*

### Comparing `pybts-1.3.1/README.assets/image-20240329031233459.png` & `pybts-1.3.3/README.assets/image-20240329031233459.png`

 * *Files identical despite different names*

### Comparing `pybts-1.3.1/README.assets/image-20240401211552611.png` & `pybts-1.3.3/README.assets/image-20240401211552611.png`

 * *Files identical despite different names*

### Comparing `pybts-1.3.1/README.assets/image-20240401211609525.png` & `pybts-1.3.3/README.assets/image-20240401211609525.png`

 * *Files identical despite different names*

### Comparing `pybts-1.3.1/README.md` & `pybts-1.3.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,16 @@
   - `BoardServer`: Flask-based web server for visualizing and managing behavior trees. Supports dynamic data updates and visualization through ECharts.
 
 ## Installation
 
 Currently, pybts is not available through package managers and must be installed by cloning the repository:
 
 ```sh
-pip install pybts # not pybts
+pip install pybts
+pip install pybts[rl] # add reinforcement learning support
 # or
 git clone https://github.com/wangtong2015/pybts.git
 cd pybts
 pip install -r requirements.txt
 pip install .
 ```
```

### Comparing `pybts-1.3.1/pybts/board.py` & `pybts-1.3.3/pybts/board/board.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import os
 import time
 import typing
 
 from pybts import utility
 from pybts.tree import Tree
 
-
 class Board:
     def __init__(self, tree: Tree, log_dir: str = '.'):
         self.tree = tree
         self.project = tree.name
         self.log_dir = os.path.join(log_dir, self.project)
         self.history_dir = os.path.join(self.log_dir, 'pybts-history')
         self.current_path = os.path.join(self.log_dir, 'pybts.json')
```

### Comparing `pybts-1.3.1/pybts/board_server.py` & `pybts-1.3.3/pybts/board/server.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,28 +6,32 @@
 )
 from pybts import utility
 import os
 import argparse
 import yaml
 import datetime
 
-BASE_DIR = os.path.dirname(os.path.abspath(__file__))
+BASE_DIR = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 TEMPLATES_DIR = os.path.join(BASE_DIR, 'templates')
 STATIC_DIR = os.path.join(TEMPLATES_DIR, 'static')
 
 
 # TODO: 正在运行的项目要有UI展示
 # TODO: 项目名称过长的话要有相应的处理（加tooltip）
 
-class BoardServer:
+class Server:
 
-    def __init__(self, title: str = 'PYBT', log_dir: str = '', update_interval: int = 0.5, debug: bool = False,
+    def __init__(self,
+                 title: str = 'PYBT',
+                 log_dir: str = '',
+                 update_interval: int = 1,
+                 debug: bool = False,
                  host: str = '0.0.0.0', port: int = 10000):
         self.title = title
-        self.update_interval = update_interval  # 每隔0.5s刷新一次
+        self.update_interval = update_interval  # 每隔1s刷新一次
         self.log_dir = log_dir
         self.app = Flask(__name__, static_folder=STATIC_DIR, template_folder=TEMPLATES_DIR)
         self.debug = debug
         self.host = host
         self.port = port
 
         # 注册路由
@@ -93,21 +97,26 @@
                     "roam"                   : True,
                     "label"                  : {
                         "backgroundColor": "#fff",
                         "position"       : "bottom",
                         'distance'       : 10,
                         "verticalAlign"  : "middle",
                         "align"          : "center",
-                        "fontSize"       : 15
+                        "fontSize"       : 14,
+                        'overflow'       : 'breakAll'
                     },
                     "leaves"                 : {
                         "label": {
-                            "position"     : "right",
-                            "verticalAlign": "middle",
-                            "align"        : "left",
+                            "backgroundColor": "#fff",
+                            "position"       : "bottom",
+                            'distance'       : 10,
+                            "verticalAlign"  : "middle",
+                            "align"          : "center",
+                            "fontSize"       : 14,
+                            'overflow'       : 'breakAll'
                         },
                     },
                     "emphasis"               : {
                         "focus": "descendant",
                     },
                     "expandAndCollapse"      : False,
                     "animationDuration"      : 100,
@@ -122,15 +131,14 @@
             ],
         }
 
     def run(self):
         self.app.run(host=self.host, port=self.port, debug=self.debug)
 
     def index(self, path):
-        print('index', path)
         if path not in ['', '/', 'index.html']:
             target_paths = [
                 path,
                 path + '.html'
             ]
             for target_path in target_paths:
                 if os.path.exists(os.path.join(TEMPLATES_DIR, target_path)):
```

### Comparing `pybts-1.3.1/pybts/builder.py` & `pybts-1.3.3/pybts/builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,14 +88,20 @@
                 Selector,
                 ReactiveSelector,
                 SelectorWithMemory,
                 ConditionBranch,
         )
 
         self.register_bt(
+                Failure,
+                Success,
+                Running
+        )
+
+        self.register_bt(
                 Inverter,
                 RunningUntilCondition,
                 OneShot,
                 Count,
                 RunningIsFailure,
                 RunningIsSuccess,
                 FailureIsSuccess,
```

### Comparing `pybts-1.3.1/pybts/composites/composite.py` & `pybts-1.3.3/pybts/composites/composite.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,28 +11,28 @@
 class Composite(Node, ABC):
     """
     组合节点
     """
 
     def __init__(
             self,
-            name: str = '',
             children: typing.Optional[typing.List[py_trees.behaviour.Behaviour]] = None,
+            **kwargs
     ):
-        super().__init__(name=name)
+        super().__init__(**kwargs)
         if children is not None:
             for child in children:
                 self.add_child(child)
         else:
             self.children = []
         self.current_child: typing.Optional[behaviour.Behaviour] = None
 
     @classmethod
     def creator(cls, d: dict, c: list):
-        return cls(name=d['name'], children=c)
+        return cls(children=c, **d)
 
     def stop(self, new_status: Status = Status.INVALID) -> None:
         """
         Provide common stop-level functionality for all composites.
 
          * Retain the current child on :data:`~py_trees.common.Status.SUCCESS` or
            :data:`~py_trees.common.Status.FAILURE` (for introspection), lose it on
@@ -221,27 +221,32 @@
             uuid.UUID: unique id of the child
         """
         self.children.insert(index, child)
         child.parent = self
         return child.id
 
 
-def _SEQ_SEL_tick(self: Composite, tick_again_status: list[Status], continue_status: list[Status],
-                  no_child_status: Status):
+def SEQ_SEL_tick(
+        self: Composite,
+        tick_again_status: list[Status],
+        continue_status: list[Status],
+        no_child_status: Status,
+        start_index: int = 0
+):
     """Sequence/Selector的tick逻辑"""
     self.debug_info['tick_count'] += 1
     self.logger.debug("%s.tick()" % (self.__class__.__name__))
 
     if self.status in tick_again_status:
         # 重新执行上次执行的子节点
         assert self.current_child is not None
         index = self.children.index(self.current_child)
     else:
-        self.current_child = None
-        index = 0
+        self.current_child = None  # 从头执行
+        index = start_index
 
     for child in itertools.islice(self.children, index, None):
         self.current_child = child
         yield from child.tick()
         if child.status not in continue_status:
             break
 
@@ -259,8 +264,7 @@
 
     # TODO: 这里要不要加这个是存疑的（组合节点invalid stop会停止所有子节点，所以某个子节点返回invalid是否要将所有的其他节点都停止？）
     # if new_status != Status.RUNNING:
     #     self.stop(new_status)
 
     self.status = new_status
     yield self
-
```

### Comparing `pybts-1.3.1/pybts/composites/condition_branch.py` & `pybts-1.3.3/pybts/composites/condition_branch.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from pybts.node import Node
 from abc import ABC
 import typing
 from py_trees.common import Status
 from py_trees import behaviour
 import itertools
-from pybts.composites.composite import Composite, _SEQ_SEL_tick
+from pybts.composites.composite import Composite, SEQ_SEL_tick
 
 
 class ConditionBranch(Composite):
     """
     条件分支节点
     只能有2或3个子节点
 
@@ -34,17 +34,14 @@
         <ReactiveSelector>
             <Children[0]/>
             <Children[2]/>
         </ReactiveSelector>
     <Parallel>
     """
 
-    def __init__(self, name: str = '', children: typing.Optional[typing.List[py_trees.behaviour.Behaviour]] = None):
-        super().__init__(name=name, children=children)
-
     def tick(self) -> typing.Iterator[Behaviour]:
         assert len(self.children) in [2, 3]
         condition = self.children[0]
         yield from condition.tick()
 
         exec_child = None  # 准备执行的节点
         if condition.status == Status.SUCCESS:
```

### Comparing `pybts-1.3.1/pybts/composites/parallel.py` & `pybts-1.3.3/pybts/composites/parallel.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,26 +21,27 @@
     - 如果未达到成功阈值，即使所有子节点都已完成执行，也返回 FAILURE
     - RUNNING 状态的子节点在下一次tick时会继续执行，非RUNNING状态的子节点在下一次tick时会重置并重新开始
     - success_threshold 设置为 -1 表示所有子节点都必须成功才算总体成功
     """
 
     def __init__(
             self,
-            name: str = '',
             success_threshold: int = 1,
-            children: typing.Optional[typing.List[py_trees.behaviour.Behaviour]] = None,
+            **kwargs
     ):
-        super().__init__(name=name, children=children)
+        super().__init__(**kwargs)
         self.success_threshold = success_threshold
 
     @classmethod
     def creator(cls, d: dict, c: list):
-        return cls(name=d['name'],
-                   success_threshold=int(d.get('success_threshold', 1)),
-                   children=c)
+        return cls(
+                success_threshold=int(d.get('success_threshold', 1)),
+                children=c,
+                **d
+        )
 
     def tick(self) -> typing.Iterator[py_trees.behaviour.Behaviour]:
         """
             同时执行所有子节点，并根据成功阈值来决定返回状态
             - 如果有子节点返回 RUNNING 状态，节点本身返回 RUNNING
             - 子节点的执行不依赖于其它子节点的状态；每个子节点独立执行
             - 如果达到或超过指定的成功阈值（success_threshold），则返回 SUCCESS
```

### Comparing `pybts-1.3.1/pybts/composites/selector.py` & `pybts-1.3.3/pybts/composites/selector.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,58 +1,60 @@
 import py_trees
 import typing
 from py_trees.common import Status
 from py_trees import behaviour
-from pybts.composites.composite import Composite, _SEQ_SEL_tick
+from pybts.composites.composite import Composite, SEQ_SEL_tick
 
 
 class Selector(Composite):
     """
     组合节点：选择节点
     依次顺序执行子节点
     - 当前执行节点返回 FAILURE/INVALID，继续执行后续节点
     - 当前执行节点返回 RUNNING，停止执行后续节点，下次执行还是从这个节点开始
     - 当前执行节点返回 SUCCESS，停止执行后续节点，下次执行从第一个节点开始
     返回最后一个执行节点的状态，如果没有孩子，则返回FAILURE
     """
 
     def tick(self) -> typing.Iterator[behaviour.Behaviour]:
-        return _SEQ_SEL_tick(
+        return SEQ_SEL_tick(
                 self,
                 tick_again_status=[Status.RUNNING],
                 continue_status=[Status.FAILURE, Status.INVALID],
-                no_child_status=Status.FAILURE)
+                no_child_status=Status.FAILURE,
+                start_index=0)
 
 
 class SelectorWithMemory(Selector):
     """
     记忆选择节点
     - 当前执行节点返回 FAILURE/INVALID，继续执行后续节点
     - 当前执行节点返回 SUCCESS/RUNNING，停止执行后续节点，下次执行还是从这个节点开始
     - 当前执行节点返回 SUCCESS，停止执行后续节点，下次执行从第一个节点开始
     返回最后一个执行节点的状态，如果没有孩子，则返回FAILURE
     """
 
     def tick(self) -> typing.Iterator[behaviour.Behaviour]:
-        return _SEQ_SEL_tick(
+        return SEQ_SEL_tick(
                 self,
                 tick_again_status=[Status.SUCCESS, Status.RUNNING],
                 continue_status=[Status.FAILURE, Status.INVALID],
-                no_child_status=Status.FAILURE)
+                no_child_status=Status.FAILURE,
+                start_index=0)
 
 
 class ReactiveSelector(Selector):
     """
     反应式选择节点
     依次顺序执行子节点
     - 当前执行节点返回 FAILURE/INVALID，继续执行后续节点
     - 当前执行节点返回 SUCCESS/RUNNING，停止执行后续节点，下次执行从第一个节点开始
     返回最后一个执行节点的状态，如果没有孩子，则返回FAILURE
     """
 
     def tick(self) -> typing.Iterator[behaviour.Behaviour]:
-        return _SEQ_SEL_tick(
+        return SEQ_SEL_tick(
                 self,
                 tick_again_status=[],
                 continue_status=[Status.FAILURE, Status.INVALID],
-                no_child_status=Status.FAILURE)
-
+                no_child_status=Status.FAILURE,
+                start_index=0)
```

### Comparing `pybts-1.3.1/pybts/composites/sequence.py` & `pybts-1.3.3/pybts/composites/sequence.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,50 +1,53 @@
 import py_trees
 from pybts.node import Node
 from abc import ABC
 import typing
 from py_trees.common import Status
 from py_trees import behaviour
 import itertools
-from pybts.composites.composite import Composite, _SEQ_SEL_tick
+from pybts.composites.composite import Composite, SEQ_SEL_tick
 
 
 class Sequence(Composite):
     """
     组合节点：顺序节点
     依次顺序执行子节点
     - 当前执行节点返回 SUCCESS，继续执行后续节点
     - 当前执行节点返回 RUNNING，停止执行后续节点，下次执行还是从这个节点开始
     - 当前执行节点返回 FAILURE/INVALID，停止执行后续节点，下次执行从第一个节点开始
     返回最后一个执行节点的状态，如果没有孩子，则返回SUCCESS
     """
 
     def tick(self) -> typing.Iterator[behaviour.Behaviour]:
-        return _SEQ_SEL_tick(self,
-                             tick_again_status=[Status.RUNNING],
-                             continue_status=[Status.SUCCESS],
-                             no_child_status=Status.SUCCESS)
+        return SEQ_SEL_tick(
+                self,
+                tick_again_status=[Status.RUNNING],
+                continue_status=[Status.SUCCESS],
+                no_child_status=Status.SUCCESS,
+                start_index=0)
 
 
 class SequenceWithMemory(Sequence):
     """
     记忆顺序节点
     依次顺序执行子节点
     - 当前执行节点返回 SUCCESS，继续执行后续节点
     - 当前执行节点返回 FAILURE/RUNNING，停止执行后续节点，下次执行还是从这个节点开始
     - 当前执行节点返回 INVALID，停止执行后续节点，下次执行从第一个节点开始
     返回最后一个执行节点的状态，如果没有孩子，则返回SUCCESS
     """
 
     def tick(self) -> typing.Iterator[behaviour.Behaviour]:
-        return _SEQ_SEL_tick(
+        return SEQ_SEL_tick(
                 self,
                 tick_again_status=[Status.RUNNING, Status.FAILURE],
                 continue_status=[Status.SUCCESS],
-                no_child_status=Status.SUCCESS)
+                no_child_status=Status.SUCCESS,
+                start_index=0)
 
 
 class ReactiveSequence(Sequence):
     """
     反应式顺序节点
     依次顺序执行子节点
     - 当前执行节点返回 SUCCESS，继续执行后续节点
@@ -52,14 +55,13 @@
     返回最后一个执行节点的状态，如果没有孩子，则返回SUCCESS
 
     可以起到打断后续RUNNING节点的效果
     - 如果前面的节点返回SUCCESS，则后续的RUNNING节点会继续运行，否则就会打断掉
     """
 
     def tick(self) -> typing.Iterator[behaviour.Behaviour]:
-        return _SEQ_SEL_tick(
+        return SEQ_SEL_tick(
                 self,
                 tick_again_status=[],
                 continue_status=[Status.SUCCESS],
-                no_child_status=Status.SUCCESS)
-
-
+                no_child_status=Status.SUCCESS,
+                start_index=0)
```

### Comparing `pybts-1.3.1/pybts/constants.py` & `pybts-1.3.3/pybts/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from py_trees.common import Status, Access
+from enum import Enum
 
 
 def _hex_color(color: str) -> tuple[int, int, int]:
     # 将十六进制颜色代码转换为RGB值
     r = int(color[0:2], 16)  # 转换红色分量
     g = int(color[2:4], 16)  # 转换绿色分量
     b = int(color[4:6], 16)  # 转换蓝色分量
```

### Comparing `pybts-1.3.1/pybts/decorators/nodes.py` & `pybts-1.3.3/pybts/decorators/nodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,31 +8,31 @@
 
 class Decorator(Node, ABC):
     """
     装饰节点
     只有一个子节点
     """
 
-    @classmethod
-    def creator(cls, d: dict, c: list):
-        return cls(name=d['name'], child=c[0])
-
-    def __init__(self, child: py_trees.behaviour.Behaviour, name: str = ''):
+    def __init__(self, child: py_trees.behaviour.Behaviour, **kwargs):
         # Checks
         if not isinstance(child, py_trees.behaviour.Behaviour):
             raise TypeError(
                     "A decorator's child must be an instance of py_trees.behaviours.Behaviour"
             )
         # Initialise
-        super().__init__(name=name)
+        super().__init__(**kwargs)
         self.children.append(child)
         # Give a convenient alias
         self.decorated = self.children[0]
         self.decorated.parent = self
 
+    @classmethod
+    def creator(cls, d: dict, c: list):
+        return cls(child=c[0], **d)
+
     def tick(self) -> typing.Iterator[py_trees.behaviour.Behaviour]:
         """
         Manage the decorated child through the tick.
 
         Yields:
             a reference to itself or one of its children
         """
@@ -120,34 +120,33 @@
 
     Encapsulates a behaviour and wait for it's status to flip to the
     desired state. This behaviour will tick with
     :data:`~py_trees.Status.RUNNING` while waiting and
     :data:`~py_trees.Status.SUCCESS` when the flip occurs.
     """
 
-    def __init__(self, child: py_trees.behaviour.Behaviour, status: str | Status, name: str = '', ):
+    def __init__(self, child: py_trees.behaviour.Behaviour, status: str | Status, **kwargs):
         """
         Initialise with child and optional name, status variables.
 
         Args:
             name: the decorator name
             child: the child to be decorated
             status: the desired status to watch for
         """
-        super().__init__(name=name, child=child)
+        super().__init__(child=child, **kwargs)
         if isinstance(status, str):
             status = Status(status)
         self.succeed_status = status
 
     @classmethod
     def creator(cls, d: dict, c: list):
         return cls(
-                name=d.get('name'),
                 child=c[0],
-                status=d['status']
+                **d
         )
 
     def to_data(self):
         return {
             **super().to_data(),
             'succeed_status': self.succeed_status
         }
@@ -189,39 +188,38 @@
     * With policy :data:`~py_trees.common.OneShotPolicy.ON_COMPLETION`, the oneshot will activate when the child
       returns :data:`~py_trees.Status.SUCCESS` || :data:`~py_trees.Status.FAILURE`.
 
     .. seealso:: :meth:`py_trees.idioms.oneshot`
     """
 
     def __init__(
-            self, name: str, child: py_trees.behaviour.Behaviour, policy: str | list[Status] = 'SUCCESS'
+            self, child: py_trees.behaviour.Behaviour, policy: str | list[Status] = 'SUCCESS', **kwargs
     ):
         """
         Init with the decorated child.
 
         Args:
             child: behaviour to shoot
             name: the decorator name
             policy: policy determining when the oneshot should activate
             - SUCCESS
             - SUCCESS|FAILURE
         """
-        super(OneShot, self).__init__(name=name, child=child)
+        super(OneShot, self).__init__(child=child, **kwargs)
         self.final_status: typing.Optional[Status] = None
         if isinstance(policy, str):
             self.policy = list(map(lambda x: Status(x), policy.split('|')))
         else:
             self.policy = policy
 
     @classmethod
     def creator(cls, d: dict, c: list):
         return cls(
-                name=d['name'],
                 child=c[0],
-                policy=d.get('policy', 'SUCCESS')
+                **d
         )
 
     def to_data(self):
         return {
             **super().to_data(),
             'policy'      : self.policy,
             'final_status': self.final_status
@@ -292,23 +290,23 @@
         total_tick_count: number of ticks in total
         running_count: number of ticks resulting in this state
         success_count: number of ticks resulting in this state
         failure_count: number of ticks resulting in this state
         interrupt_count: number of times a higher priority has interrupted
     """
 
-    def __init__(self, child: py_trees.behaviour.Behaviour, name: str = ''):
+    def __init__(self, child: py_trees.behaviour.Behaviour, name: str = '', **kwargs):
         """
         Init the counter.
 
         Args:
             name: the decorator name
             child: the child behaviour or subtree
         """
-        super(Count, self).__init__(name=name, child=child)
+        super(Count, self).__init__(name=name, child=child, **kwargs)
         self.total_tick_count = 0
         self.failure_count = 0
         self.success_count = 0
         self.running_count = 0
         self.interrupt_count = 0
 
     def to_data(self):
```

### Comparing `pybts-1.3.1/pybts/main.py` & `pybts-1.3.3/pybts/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import shutil
 
-import pybts
 import argparse
 import os
+import pybts
 
 
 def directory_type(path):
     if not os.path.isdir(path):
         raise argparse.ArgumentTypeError(f"{path} is not a valid directory")
     return path
 
@@ -36,13 +36,13 @@
         from pybts import utility
         import tqdm
         for project in tqdm.tqdm(utility.extract_project_path_list(args.dir)):
             utility.clear_project(args.dir, project)
             print(f'Successful cleared {args.dir}: {project}')
         return
 
-    server = pybts.board_server.BoardServer(log_dir=args.dir, debug=args.debug, host=args.host, port=args.port)
+    server = pybts.board.Server(log_dir=args.dir, debug=args.debug, host=args.host, port=args.port)
     server.run()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `pybts-1.3.1/pybts/node.py` & `pybts-1.3.3/pybts/node.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     - stop
 
     下一次tick的时候状态一开始是RUNNING，则直接调用
     update
 
     """
 
-    def __init__(self, name: str = ''):
+    def __init__(self, name: str = '', **kwargs):
         super().__init__(name=name or self.__class__.__name__)
         self._updater_iter = None
         self.debug_info = {
             'tick_count'      : 0,
             'update_count'    : 0,
             'reset_count'     : 0,
             'terminate_count' : 0,
@@ -46,15 +46,15 @@
         self.debug_info['reset_count'] += 1
         self._updater_iter = None
         if self.status != Status.INVALID:
             self.stop(Status.INVALID)
 
     @classmethod
     def creator(cls, d: dict, c: list):
-        return cls(name=d['name'])
+        return cls(**d)
 
     def to_data(self):
         # 在board上查看的信息
         return {
             'debug_info': self.debug_info,
         }
 
@@ -136,62 +136,71 @@
         self.debug_info['terminate_count'] += 1
 
     def initialise(self) -> None:
         super().initialise()
         self.logger.debug("%s.initialise()" % (self.__class__.__name__))
         self.debug_info['initialise_count'] += 1
 
+    def __str__(self):
+        if len(self.children) == 0:
+            return f'<{self.name} id="{self.id.hex}"/>'
+        else:
+            return f'<{self.name} id="{self.id.hex}"> {len(self.children)} </{self.name}>'
+
+    def __repr__(self):
+        return self.__str__()
+
 
 class Action(Node, ABC):
     """
     行为节点
     """
 
-    def __init__(self, name: str = ''):
-        super().__init__(name=name)
+    def __init__(self, name: str = '', **kwargs):
+        super().__init__(name=name, **kwargs)
         self.actions = Queue()
 
     def to_data(self):
         from pybts.utility import read_queue_without_destroying
         actions = read_queue_without_destroying(self.actions)
         return {
             **super().to_data(),
             'actions': [str(act) for act in actions]
         }
 
 
-class Condition(Node, ABC):
+class Condition:
     """
-    条件节点
+    条件节点，只能多继承使用
     """
     pass
 
 
-class Success(Condition):
+class Success(Node, Condition):
     """
     成功节点
     """
 
     def update(self) -> Status:
         super().update()
         return Status.SUCCESS
 
     def stop(self, new_status: common.Status) -> None:
         super().stop(new_status)
 
 
-class Failure(Condition):
+class Failure(Node, Condition):
     """
     失败节点
     """
 
     def update(self) -> Status:
         super().update()
         return Status.FAILURE
 
 
-class Running(Condition):
+class Running(Node, Condition):
     """Running Node"""
 
     def update(self) -> Status:
         super().update()
         return Status.RUNNING
```

### Comparing `pybts-1.3.1/pybts/templates/favicon.ico` & `pybts-1.3.3/pybts/templates/favicon.ico`

 * *Files identical despite different names*

### Comparing `pybts-1.3.1/pybts/templates/static/index-BUWP2os5.js` & `pybts-1.3.3/pybts/templates/static/index-BUWP2os5.js`

 * *Files identical despite different names*

### Comparing `pybts-1.3.1/pybts/templates/static/index-BXdrQGHp.css` & `pybts-1.3.3/pybts/templates/static/index-BXdrQGHp.css`

 * *Files identical despite different names*

### Comparing `pybts-1.3.1/pybts/utility.py` & `pybts-1.3.3/pybts/utility.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from pybts.constants import *
 import yaml
 from queue import Queue
 import xml.etree.ElementTree as ET
 from xml.dom import minidom
 import os
 import json
+import jinja2
 
 
 def read_queue_without_destroying(q: Queue):
     # 创建一个空列表来存储队列中的元素
     temp_list = []
 
     # 遍历队列，复制元素到列表和临时队列
@@ -240,7 +241,11 @@
 def clear_project(log_dir: str, project: str):
     current_path = os.path.join(log_dir, project, 'pybts.json')
     if os.path.exists(current_path):
         os.remove(current_path)
     history_dir = os.path.join(log_dir, project, 'history')
     if os.path.exists(history_dir):
         delete_folder_contents(history_dir)
+
+
+def jinja2_render(template: str, context: dict) -> str:
+    return jinja2.Template(template).render(context)
```

### Comparing `pybts-1.3.1/PKG-INFO` & `pybts-1.3.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
 Name: pybts
-Version: 1.3.1
+Version: 1.3.3
 Summary: 
 Home-page: https://github.com/wangtong2015/pybts
 Keywords: BehaviorTree,AI
 Author: 王童
 Author-email: 785271992@qq.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Provides-Extra: rl
 Requires-Dist: flask (>=3.0.2,<4.0.0)
+Requires-Dist: gymnasium (>=0.29.1,<0.30.0) ; extra == "rl"
 Requires-Dist: jinja2 (>=3.1.3,<4.0.0)
 Requires-Dist: py-trees (>=2.2.3,<3.0.0)
+Requires-Dist: stable-baselines3 (>=2.3.0,<3.0.0) ; extra == "rl"
+Requires-Dist: torch (>=2.2.2,<3.0.0) ; extra == "rl"
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Project-URL: Repository, https://github.com/wangtong2015/pybts
 Description-Content-Type: text/markdown
 
 # PYBTS - Python Behavior Tree
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/pybts.svg)](https://pypi.org/project/pybts/)
@@ -51,15 +55,16 @@
   - `BoardServer`: Flask-based web server for visualizing and managing behavior trees. Supports dynamic data updates and visualization through ECharts.
 
 ## Installation
 
 Currently, pybts is not available through package managers and must be installed by cloning the repository:
 
 ```sh
-pip install pybts # not pybts
+pip install pybts
+pip install pybts[rl] # add reinforcement learning support
 # or
 git clone https://github.com/wangtong2015/pybts.git
 cd pybts
 pip install -r requirements.txt
 pip install .
 ```
```

