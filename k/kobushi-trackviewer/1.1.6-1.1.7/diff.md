# Comparing `tmp/kobushi_trackviewer-1.1.6-py3-none-any.whl.zip` & `tmp/kobushi_trackviewer-1.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 42490 bytes, number of entries: 19
+Zip file size: 42850 bytes, number of entries: 19
 -rw-r--r--  2.0 unx      634 b- defN 21-Aug-15 09:07 kobushi/__init__.py
 -rw-r--r--  2.0 unx      649 b- defN 21-Aug-14 12:53 kobushi/__main__.py
--rw-r--r--  2.0 unx       22 b- defN 23-Jul-22 01:57 kobushi/_version.py
+-rw-r--r--  2.0 unx       22 b- defN 24-Apr-08 14:07 kobushi/_version.py
 -rw-r--r--  2.0 unx     3482 b- defN 21-Aug-20 14:15 kobushi/dialog_multifields.py
--rw-r--r--  2.0 unx    35123 b- defN 23-Jun-24 15:41 kobushi/gui_interface.py
+-rw-r--r--  2.0 unx    35123 b- defN 24-Apr-08 14:07 kobushi/gui_interface.py
 -rw-r--r--  2.0 unx     2999 b- defN 21-Aug-14 12:53 kobushi/loadheader.py
 -rw-r--r--  2.0 unx      761 b- defN 22-Oct-15 12:32 kobushi/loadmapgrammer.py
--rw-r--r--  2.0 unx     1665 b- defN 22-Apr-18 12:51 kobushi/map-grammer.lark
--rw-r--r--  2.0 unx     9929 b- defN 23-Jul-22 02:36 kobushi/mapinterpreter.py
--rw-r--r--  2.0 unx    11659 b- defN 23-Jul-22 02:37 kobushi/mapobj.py
--rw-r--r--  2.0 unx    17242 b- defN 23-Jun-24 15:41 kobushi/mapplot.py
--rw-r--r--  2.0 unx     6306 b- defN 21-Aug-20 14:15 kobushi/othertrack_window.py
+-rw-r--r--  2.0 unx     1781 b- defN 24-Apr-08 14:07 kobushi/map-grammer.lark
+-rw-r--r--  2.0 unx     9929 b- defN 23-Jul-22 03:03 kobushi/mapinterpreter.py
+-rw-r--r--  2.0 unx    11659 b- defN 23-Jul-22 03:03 kobushi/mapobj.py
+-rw-r--r--  2.0 unx    17464 b- defN 24-Apr-08 14:07 kobushi/mapplot.py
+-rw-r--r--  2.0 unx     6733 b- defN 24-Apr-08 14:07 kobushi/othertrack_window.py
 -rw-r--r--  2.0 unx    17540 b- defN 23-Mar-18 15:38 kobushi/trackcoordinate.py
 -rw-r--r--  2.0 unx    35622 b- defN 23-Jun-24 15:41 kobushi/trackgenerator.py
--rw-r--r--  2.0 unx     9724 b- defN 23-Jul-22 02:59 kobushi_trackviewer-1.1.6.dist-info/LICENSE
--rw-r--r--  2.0 unx     2749 b- defN 23-Jul-22 02:59 kobushi_trackviewer-1.1.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-22 02:59 kobushi_trackviewer-1.1.6.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Jul-22 02:59 kobushi_trackviewer-1.1.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1562 b- defN 23-Jul-22 02:59 kobushi_trackviewer-1.1.6.dist-info/RECORD
-19 files, 157768 bytes uncompressed, 39948 bytes compressed:  74.7%
+-rw-r--r--  2.0 unx     9724 b- defN 24-Apr-08 14:08 kobushi_trackviewer-1.1.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2749 b- defN 24-Apr-08 14:08 kobushi_trackviewer-1.1.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-08 14:08 kobushi_trackviewer-1.1.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 24-Apr-08 14:08 kobushi_trackviewer-1.1.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1562 b- defN 24-Apr-08 14:08 kobushi_trackviewer-1.1.7.dist-info/RECORD
+19 files, 158533 bytes uncompressed, 40308 bytes compressed:  74.6%
```

## zipnote {}

```diff
@@ -36,23 +36,23 @@
 
 Filename: kobushi/trackcoordinate.py
 Comment: 
 
 Filename: kobushi/trackgenerator.py
 Comment: 
 
-Filename: kobushi_trackviewer-1.1.6.dist-info/LICENSE
+Filename: kobushi_trackviewer-1.1.7.dist-info/LICENSE
 Comment: 
 
-Filename: kobushi_trackviewer-1.1.6.dist-info/METADATA
+Filename: kobushi_trackviewer-1.1.7.dist-info/METADATA
 Comment: 
 
-Filename: kobushi_trackviewer-1.1.6.dist-info/WHEEL
+Filename: kobushi_trackviewer-1.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: kobushi_trackviewer-1.1.6.dist-info/top_level.txt
+Filename: kobushi_trackviewer-1.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: kobushi_trackviewer-1.1.6.dist-info/RECORD
+Filename: kobushi_trackviewer-1.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kobushi/_version.py

```diff
@@ -1 +1 @@
-__version__ = '1.1.6'
+__version__ = '1.1.7'
```

## kobushi/gui_interface.py

```diff
@@ -1,9 +1,9 @@
 '''
-    Copyright 2021-2022 konawasabi
+    Copyright 2021-2024 konawasabi
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -582,15 +582,15 @@
                     self.profYlim = [float(dialog.variables['min'].get()),float(dialog.variables['max'].get())]
                 else:
                     self.profYlim = None
                 self.plot_all()
     def aboutwindow(self, event=None):
         msg  = 'Kobushi trackviewer\n'
         msg += 'Version '+__version__+'\n\n'
-        msg += 'Copyright © 2021-2023 konawasabi\n'
+        msg += 'Copyright © 2021-2024 konawasabi\n'
         msg += 'Released under the Apache License, Version 2.0 .\n'
         msg += 'https://www.apache.org/licenses/LICENSE-2.0'
         tk.messagebox.showinfo(message=msg)
     def customdialog_test(self, event=None):
         dialog_obj = dialog_multifields.dialog_multifields(self,\
                                         [{'name':'A', 'type':'str', 'label':'test A', 'default':'alpha'},\
                                         {'name':'B', 'type':'Double', 'label':'test B', 'default':100}],\
```

## kobushi/map-grammer.lark

```diff
@@ -27,18 +27,20 @@
        | label "(" [expression ("," expression)*] ")" -> call_function
           
 ?mapfunc: label "(" [expression] ("," [expression])* ")"
         
 ?mapobject: label ["[" parameter "]"] // [key]が指定されていない場合もNoneを返す
 
 ?label: CNAME
-VALNAME: ("_"|LETTER|DIGIT) ("_"|LETTER|DIGIT)*
+VALNAME: ("_"|LETTER|SIMCH_LETTER|DIGIT) ("_"|LETTER|SIMCH_LETTER|DIGIT)*
 
 string: /'[^']*'/ -> remquote
 
+SIMCH_LETTER: ("\u0080".."\u07ff") | ("\u0800".."\uffff") | ("\U00010000".."\U0010ffff")
+
 %import common.CNAME
 %import common.LETTER
 %import common.DIGIT
 %import common.SIGNED_NUMBER
 
 %import common.WS_INLINE
 %import common.SH_COMMENT
```

## kobushi/mapplot.py

```diff
@@ -1,9 +1,9 @@
 '''
-    Copyright 2021 konawasabi
+    Copyright 2021-2024 konawasabi
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -62,14 +62,17 @@
         owntrack = self.rotate_track(owntrack,-self.origin_angle)
         
         ax_pl.plot(owntrack[:,1],owntrack[:,2],color='black') # 自軌道描画
         
         # 他軌道描画
         if othertrack_list != None:
             for key in othertrack_list:
+                if key == '\\':
+                    key = ''
+                    # 渡された他軌道リストの要素がバックスラッシュなら''に置き換える。othertrack_window.py参照のこと。
                 othertrack = self.environment.othertrack_pos[key]
                 othertrack = othertrack[othertrack[:,0] >= self.environment.othertrack.cp_range[key]['min']]
                 othertrack = othertrack[othertrack[:,0] <= self.environment.othertrack.cp_range[key]['max']]
                 othertrack = othertrack[othertrack[:,0] >= self.distrange['plane'][0]]
                 othertrack = othertrack[othertrack[:,0] <= self.distrange['plane'][1]]
                 othertrack = self.rotate_track(othertrack,-self.origin_angle)
                 ax_pl.plot(othertrack[:,1],othertrack[:,2],color=self.environment.othertrack_linecolor[key]['current'])
```

## kobushi/othertrack_window.py

```diff
@@ -1,9 +1,9 @@
 '''
-    Copyright 2021 konawasabi
+    Copyright 2021-2024 konawasabi
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -67,14 +67,17 @@
         '''他軌道リストをクリックしたときのイベント処理
         '''
         columnlabel = {'#0':'Check','#1':'From', '#2':'To', '#3':'Color'}
         if event != None:
             if getattr(event, 'widget').identify("element", event.x, event.y) == 'text': #パラメータ部分クリックかどうか。チェックボックスだとimage
                 clicked_column = self.othertrack_tree.identify_column(event.x)
                 clicked_track = self.othertrack_tree.identify_row(event.y)
+                if clicked_track == '\\':
+                    clicked_track = ''
+                    # クリックされた要素のidがバックスラッシュなら軌道キーを''に置き換える。通常は要素id = 軌道キー
                 #print(clicked_track,columnlabel[clicked_column])
                 if clicked_column in ['#1','#2','#3'] and clicked_track != 'root':
                     if clicked_column == '#3': # ラインカラーかどうか？
                         inputdata = colorchooser.askcolor(color=self.mainwindow.result.othertrack_linecolor[clicked_track]['current'],title=clicked_track+' ,default: '+self.mainwindow.result.othertrack_linecolor[clicked_track]['default'])
                         if inputdata[1] != None:
                             self.mainwindow.result.othertrack_linecolor[clicked_track]['current'] = inputdata[1]
                             self.othertrack_tree.tag_configure(clicked_track,foreground=self.mainwindow.result.othertrack_linecolor[clicked_track]['current'])
@@ -94,11 +97,12 @@
         self.mainwindow.plot_all()
     def set_ottree_value(self):
         if self.othertrack_tree.exists('root'):
             self.othertrack_tree.delete('root')
         self.othertrack_tree.insert("", "end", 'root', text='root', open=True)
         colorix = 0
         for i in self.mainwindow.result.othertrack.data.keys():
-            self.othertrack_tree.insert("root", "end", i, text=i, values=(min(self.mainwindow.result.othertrack.data[i], key=lambda x: x['distance'])['distance'],max(self.mainwindow.result.othertrack.data[i], key=lambda x: x['distance'])['distance'], '■■■'),tags=(i,))
+            self.othertrack_tree.insert("root", "end", '\\' if i=='' else i, text=i, values=(min(self.mainwindow.result.othertrack.data[i], key=lambda x: x['distance'])['distance'],max(self.mainwindow.result.othertrack.data[i], key=lambda x: x['distance'])['distance'], '■■■'),tags=(i,))
+            # trackkey == '' (空文字列)の場合はidをバックスラッシュに置き換える。（他軌道ツリーのroot要素と重複するため）
             self.othertrack_tree.tag_configure(i,foreground=self.mainwindow.result.othertrack_linecolor[i]['current'])
         #self.subwindow.othertrack_tree.see('root')
         #self.othertrack_tree.configure(yscrollcommand=self.ottree_scrollbar.set)
```

## Comparing `kobushi_trackviewer-1.1.6.dist-info/LICENSE` & `kobushi_trackviewer-1.1.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `kobushi_trackviewer-1.1.6.dist-info/METADATA` & `kobushi_trackviewer-1.1.7.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kobushi-trackviewer
-Version: 1.1.6
+Version: 1.1.7
 Summary: Trackviewer for BVE trainsim 5/6
 Home-page: https://github.com/konawasabi/kobushi-trackviewer/
 Author: Konawasabi
 Author-email: webmaster@konawasabi.riceball.jp
 License: Apache License 2.0
 Keywords: BVE trainsim
 Description-Content-Type: text/markdown
```

