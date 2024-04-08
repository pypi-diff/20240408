# Comparing `tmp/ppatch-0.0.1.tar.gz` & `tmp/ppatch-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ppatch-0.0.1.tar", last modified: Tue Mar 12 10:05:11 2024, max compression
+gzip compressed data, was "ppatch-0.0.3.tar", last modified: Mon Apr  8 09:16:57 2024, max compression
```

## Comparing `ppatch-0.0.1.tar` & `ppatch-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,15 @@
--rw-r--r--   0        0        0     1066 2024-01-25 10:42:24.584919 ppatch-0.0.1/LICENSE
--rw-r--r--   0        0        0     5031 2024-03-12 10:00:50.281699 ppatch-0.0.1/README.md
--rw-r--r--   0        0        0      499 2024-03-12 10:05:11.723110 ppatch-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       27 2024-01-25 10:42:24.593919 ppatch-0.0.1/src/ppatch/__init__.py
--rw-r--r--   0        0        0     7497 2024-03-07 07:41:26.163480 ppatch-0.0.1/src/ppatch/app.py
--rw-r--r--   0        0        0      931 2024-03-06 10:31:54.994336 ppatch-0.0.1/src/ppatch/model.py
--rw-r--r--   0        0        0     1572 2024-03-06 11:08:26.125703 ppatch-0.0.1/src/ppatch/utils/common.py
--rw-r--r--   0        0        0     2802 2024-03-12 09:59:06.670493 ppatch-0.0.1/src/ppatch/utils/parse.py
--rw-r--r--   0        0        0     5511 2024-03-12 08:41:06.286229 ppatch-0.0.1/src/ppatch/utils/resolve.py
--rw-r--r--   0        0        0     5343 1970-01-01 00:00:00.000000 ppatch-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-01-25 10:42:24.584919 ppatch-0.0.3/LICENSE
+-rw-r--r--   0        0        0    11981 2024-04-08 08:34:31.003741 ppatch-0.0.3/README.md
+-rw-r--r--   0        0        0      499 2024-04-08 09:16:57.991465 ppatch-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       21 2024-03-13 07:54:26.926711 ppatch-0.0.3/src/ppatch/__init__.py
+-rw-r--r--   0        0        0      335 2024-04-03 09:07:58.028939 ppatch-0.0.3/src/ppatch/app.py
+-rw-r--r--   0        0        0     1622 2024-04-03 12:39:04.843779 ppatch-0.0.3/src/ppatch/commands/apply.py
+-rw-r--r--   0        0        0     3003 2024-03-25 11:47:38.380836 ppatch-0.0.3/src/ppatch/commands/auto.py
+-rw-r--r--   0        0        0     1590 2024-03-25 06:28:43.676959 ppatch-0.0.3/src/ppatch/commands/get.py
+-rw-r--r--   0        0        0      870 2024-03-25 06:28:43.239945 ppatch-0.0.3/src/ppatch/commands/show.py
+-rw-r--r--   0        0        0     5020 2024-04-03 12:27:11.745378 ppatch-0.0.3/src/ppatch/commands/trace.py
+-rw-r--r--   0        0        0     1535 2024-04-03 12:14:16.362389 ppatch-0.0.3/src/ppatch/model.py
+-rw-r--r--   0        0        0     2290 2024-04-03 09:44:38.712738 ppatch-0.0.3/src/ppatch/utils/common.py
+-rw-r--r--   0        0        0     2802 2024-03-12 09:59:06.670493 ppatch-0.0.3/src/ppatch/utils/parse.py
+-rw-r--r--   0        0        0     7293 2024-04-03 11:22:08.504525 ppatch-0.0.3/src/ppatch/utils/resolve.py
+-rw-r--r--   0        0        0    12293 1970-01-01 00:00:00.000000 ppatch-0.0.3/PKG-INFO
```

### Comparing `ppatch-0.0.1/LICENSE` & `ppatch-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ppatch-0.0.1/src/ppatch/utils/common.py` & `ppatch-0.0.3/src/ppatch/utils/common.py`

 * *Files 20% similar despite different names*

```diff
@@ -50,7 +50,31 @@
     positions = []
 
     for i in range(len(main_list) - sublist_length + 1):
         if main_list[i : i + sublist_length] == sublist:
             positions.append(i)
 
     return positions
+
+
+def isnamedtupleinstance(x):
+    _type = type(x)
+    bases = _type.__bases__
+    if len(bases) != 1 or bases[0] != tuple:
+        return False
+    fields = getattr(_type, "_fields", None)
+    if not isinstance(fields, tuple):
+        return False
+    return all(type(i) == str for i in fields)
+
+
+def unpack(obj):
+    if isinstance(obj, dict):
+        return {key: unpack(value) for key, value in obj.items()}
+    elif isinstance(obj, list):
+        return [unpack(value) for value in obj]
+    elif isnamedtupleinstance(obj):
+        return {key: unpack(value) for key, value in obj._asdict().items()}
+    elif isinstance(obj, tuple):
+        return tuple(unpack(value) for value in obj)
+    else:
+        return obj
```

### Comparing `ppatch-0.0.1/src/ppatch/utils/parse.py` & `ppatch-0.0.3/src/ppatch/utils/parse.py`

 * *Files identical despite different names*

### Comparing `ppatch-0.0.1/src/ppatch/utils/resolve.py` & `ppatch-0.0.3/src/ppatch/utils/resolve.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,40 @@
-from whatthepatch.patch import Change
-
-from ppatch.model import Hunk, Line
+from ppatch.app import MAX_DIFF_LINES
+from ppatch.model import ApplyResult, Change, Hunk, Line
 from ppatch.utils.common import find_list_positions
 
 
 def apply_change(
-    changes: list[Change], target: list[Line], flag: bool = False
-) -> tuple[list[Line], list[Line]]:
+    changes: list[Change],
+    target: list[Line],
+    reverse: bool = False,
+    flag: bool = False,
+    flag_hunk: int = -1,
+) -> ApplyResult:
     """Apply a diff to a target string."""
 
-    # TODO: 这里有个巨大的问题：diff 信息中的行号与实际行号不一致
+    # 如果反向，则交换所有的 old 和 new
+    if reverse:
+        for change in changes:
+            change.old, change.new = change.new, change.old
+
+    # 这里有个巨大的问题：diff 信息中的行号与实际行号不一致
     # 一种修复方式：搜索 diff 每个 hunk 的上下文行，然后修改标记
 
     # 首先统计 Hunk 数
     hunk_indexes = []
     for change in changes:
         if change.hunk not in hunk_indexes:
             hunk_indexes.append(change.hunk)
 
     # TODO: 支持 -F 参数
     # 将changes按照hunk分组，注意同一个 hunk 中的 change 要进行分类，前三行要放入前置上下文，中间的要放入中间上下文，后三行要放入后置上下文
     hunk_list: list[Hunk] = []
+    conflict_hunk_num_list: list[int] = []
+    failed_hunk_list: list[Hunk] = []
     for hunk_index in hunk_indexes:
         hunk_changes = [change for change in changes if change.hunk == hunk_index]
 
         # 这里遍历的顺序已经是正确的顺序
         hunk_context = []
         hunk_middle = []
         hunk_post = []
@@ -41,15 +51,18 @@
                 hunk_post.append(change)
             else:
                 break
 
         # 注意把后置上下文反转回来
         hunk_post = list(reversed(hunk_post))
 
-        # 最后获取中间上下文
+        assert len(hunk_context) <= MAX_DIFF_LINES
+        assert len(hunk_post) <= MAX_DIFF_LINES
+
+        # 最后获取中间代码
         for change in hunk_changes:
             if change not in hunk_context and change not in hunk_post:
                 hunk_middle.append(change)
 
         hunk_list.append(
             Hunk(
                 index=hunk_index,
@@ -66,15 +79,16 @@
 
         def cal_offsets(target: list[Line], changes: list[Change]) -> list[int]:
             pos_list = find_list_positions(
                 [line.content for line in target],
                 [change.line for change in changes],
             )
             if len(pos_list) == 0:
-                raise Exception(f"context lines do not exist in source")
+                return []  # 这样使得下面计算交集时一定为空
+                # raise Exception(f"context lines do not exist in source")
 
             offset_list = []
             if len(changes) == 0:
                 offset_list = pos_list
             else:
                 for position in pos_list:
                     offset = position + 1 - changes[0].old
@@ -83,23 +97,26 @@
             return offset_list
 
         offset_context = cal_offsets(target, hunk.context)
         offset_post = cal_offsets(target, hunk.post)
 
         offset_list = list(set(offset_context) & set(offset_post))
         if len(offset_list) == 0:
-            raise Exception("offsets do not intersect")
+            failed_hunk_list.append(hunk)
+            hunk_list.remove(hunk)
+            continue
+            # raise Exception("offsets do not intersect")
 
         # 计算最小 offset
         min_offset = None
         for offset in offset_list:
             if min_offset is None or abs(offset) < abs(min_offset):
                 min_offset = offset
 
-        for change in hunk.all_:
+        for change in hunk.middle:
             changes.append(
                 Change(
                     hunk=change.hunk,
                     old=change.old + min_offset if change.old is not None else None,
                     new=change.new + min_offset if change.new is not None else None,
                     line=change.line,
                 )
@@ -127,31 +144,63 @@
             target.insert(
                 change.new - 1,
                 Line(
                     index=change.new - 1,
                     content=change.line,
                     changed=True,
                     status=True,
-                    flag=flag,
+                    flag=True
+                    if flag and (change.hunk == flag_hunk or flag_hunk == -1)
+                    else False,
+                    hunk=change.hunk,
                 ),
             )
             add_count += 1
 
         elif change.new is None and change.old is not None:
             index = change.old - 1 - del_count + add_count
 
             # 如果被修改行有标记，则将其添加进标记列表
             if target[index].flag:
                 flag_line_list.append(target[index])
 
             del target[index]
             del_count += 1
 
+            conflict_hunk_num_list.append(change.hunk)
+
+        else:
+            # 对其他行也要标记 flag
+            index = change.old - 1 - del_count + add_count
+            assert index == change.new - 1
+            target[index].flag = (
+                True
+                if flag and (change.hunk == flag_hunk or flag_hunk == -1)
+                else target[index].flag
+            )
+
     new_line_list = []
     for index, line in enumerate(target):
+        # 判断是否在 Flag 行附近进行了修改
+        # 如果该行为 changed，且前后行为flag，则也加入标记列表
+        if line.changed and not line.flag:
+            if index > 0 and target[index - 1].flag:
+                line.flag = True
+            if index < len(target) - 1 and target[index + 1].flag:
+                line.flag = True
+
+            if line.flag:
+                flag_line_list.append(line)
+                conflict_hunk_num_list.append(line.hunk)
+
         new_line_list.append(
             Line(
                 index=index, content=line.content, changed=line.changed, flag=line.flag
             )
         )
 
-    return new_line_list, flag_line_list
+    return ApplyResult(
+        new_line_list=new_line_list,
+        flag_line_list=flag_line_list,
+        conflict_hunk_num_list=conflict_hunk_num_list,
+        failed_hunk_list=failed_hunk_list,
+    )
```

