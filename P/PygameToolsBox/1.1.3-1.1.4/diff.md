# Comparing `tmp/PygameToolsBox-1.1.3.tar.gz` & `tmp/PygameToolsBox-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PygameToolsBox-1.1.3.tar", last modified: Sun Apr  7 03:41:25 2024, max compression
+gzip compressed data, was "PygameToolsBox-1.1.4.tar", last modified: Sun Apr  7 04:03:42 2024, max compression
```

## Comparing `PygameToolsBox-1.1.3.tar` & `PygameToolsBox-1.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 03:41:25.644772 PygameToolsBox-1.1.3/
--rw-rw-rw-   0        0        0     1091 2024-03-26 20:21:58.000000 PygameToolsBox-1.1.3/LICENSE
--rw-rw-rw-   0        0        0     3681 2024-04-07 03:41:25.642779 PygameToolsBox-1.1.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-07 03:41:25.613781 PygameToolsBox-1.1.3/PygameToolsBox/
--rw-rw-rw-   0        0        0       21 2024-04-07 03:41:01.000000 PygameToolsBox-1.1.3/PygameToolsBox/__init__.py
--rw-rw-rw-   0        0        0     4609 2024-04-07 03:40:18.000000 PygameToolsBox-1.1.3/PygameToolsBox/animated_object.py
--rw-rw-rw-   0        0        0      517 2024-04-07 01:29:10.000000 PygameToolsBox-1.1.3/PygameToolsBox/mask_image.py
--rw-rw-rw-   0        0        0     2838 2024-04-07 02:00:30.000000 PygameToolsBox-1.1.3/PygameToolsBox/parallax_bg.py
--rw-rw-rw-   0        0        0     3696 2024-04-06 19:08:25.000000 PygameToolsBox-1.1.3/PygameToolsBox/spritesheet.py
-drwxrwxrwx   0        0        0        0 2024-04-07 03:41:25.631774 PygameToolsBox-1.1.3/PygameToolsBox.egg-info/
--rw-rw-rw-   0        0        0     3681 2024-04-07 03:41:25.000000 PygameToolsBox-1.1.3/PygameToolsBox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      371 2024-04-07 03:41:25.000000 PygameToolsBox-1.1.3/PygameToolsBox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 03:41:25.000000 PygameToolsBox-1.1.3/PygameToolsBox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-04-07 03:41:25.000000 PygameToolsBox-1.1.3/PygameToolsBox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-07 03:41:25.000000 PygameToolsBox-1.1.3/PygameToolsBox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3075 2024-04-07 02:29:42.000000 PygameToolsBox-1.1.3/README.md
--rw-rw-rw-   0        0        0      773 2024-03-26 20:57:41.000000 PygameToolsBox-1.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-07 03:41:25.644772 PygameToolsBox-1.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-07 04:03:42.420729 PygameToolsBox-1.1.4/
+-rw-rw-rw-   0        0        0     1091 2024-03-26 20:21:58.000000 PygameToolsBox-1.1.4/LICENSE
+-rw-rw-rw-   0        0        0     3681 2024-04-07 04:03:42.419445 PygameToolsBox-1.1.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-07 04:03:42.394435 PygameToolsBox-1.1.4/PygameToolsBox/
+-rw-rw-rw-   0        0        0       21 2024-04-07 04:03:27.000000 PygameToolsBox-1.1.4/PygameToolsBox/__init__.py
+-rw-rw-rw-   0        0        0     4636 2024-04-07 04:03:04.000000 PygameToolsBox-1.1.4/PygameToolsBox/animated_object.py
+-rw-rw-rw-   0        0        0      517 2024-04-07 01:29:10.000000 PygameToolsBox-1.1.4/PygameToolsBox/mask_image.py
+-rw-rw-rw-   0        0        0     2838 2024-04-07 02:00:30.000000 PygameToolsBox-1.1.4/PygameToolsBox/parallax_bg.py
+-rw-rw-rw-   0        0        0     3696 2024-04-06 19:08:25.000000 PygameToolsBox-1.1.4/PygameToolsBox/spritesheet.py
+drwxrwxrwx   0        0        0        0 2024-04-07 04:03:42.409438 PygameToolsBox-1.1.4/PygameToolsBox.egg-info/
+-rw-rw-rw-   0        0        0     3681 2024-04-07 04:03:42.000000 PygameToolsBox-1.1.4/PygameToolsBox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      371 2024-04-07 04:03:42.000000 PygameToolsBox-1.1.4/PygameToolsBox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 04:03:42.000000 PygameToolsBox-1.1.4/PygameToolsBox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-04-07 04:03:42.000000 PygameToolsBox-1.1.4/PygameToolsBox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-07 04:03:42.000000 PygameToolsBox-1.1.4/PygameToolsBox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3075 2024-04-07 02:29:42.000000 PygameToolsBox-1.1.4/README.md
+-rw-rw-rw-   0        0        0      773 2024-03-26 20:57:41.000000 PygameToolsBox-1.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-07 04:03:42.420729 PygameToolsBox-1.1.4/setup.cfg
```

### Comparing `PygameToolsBox-1.1.3/LICENSE` & `PygameToolsBox-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `PygameToolsBox-1.1.3/PKG-INFO` & `PygameToolsBox-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PygameToolsBox
-Version: 1.1.3
+Version: 1.1.4
 Summary: Library for manage sprite sheet, and pallax background
 Author-email: FranckSix <francksix@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/FranckSix/PygameSpriteTools
 Project-URL: Issues, https://github.com/FranckSix/PygameSpriteTools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PygameToolsBox-1.1.3/PygameToolsBox/animated_object.py` & `PygameToolsBox-1.1.4/PygameToolsBox/animated_object.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,23 +61,23 @@
         super().__init__()
         self._images = [MaskImage(i) for i in images]
         self._actions = dict[str, ActionSequence]()
         self._current_action: ActionSequence | None = None
         self._cooling = cooling
         self._cool_down = cooling
         self._image_index = 0
-        self._rect = Rect(0,0,0,0)
+        self._rect = Rect(0, 0, 0, 0)
 
     @property
     def image(self) -> Surface:
-        return self._images[self._image_index].image if self._image_index else None
+        return self._images[self._image_index].image if self._image_index is not None else None
 
     @property
     def mask(self) -> Surface:
-        return self._images[self._image_index].mask if self._image_index else None
+        return self._images[self._image_index].mask if self._image_index is not None else None
 
     @property
     def rect(self) -> Rect:
         return self._rect
 
     @rect.setter
     def rect(self, value: Rect):
```

### Comparing `PygameToolsBox-1.1.3/PygameToolsBox/mask_image.py` & `PygameToolsBox-1.1.4/PygameToolsBox/mask_image.py`

 * *Files identical despite different names*

### Comparing `PygameToolsBox-1.1.3/PygameToolsBox/parallax_bg.py` & `PygameToolsBox-1.1.4/PygameToolsBox/parallax_bg.py`

 * *Files identical despite different names*

### Comparing `PygameToolsBox-1.1.3/PygameToolsBox/spritesheet.py` & `PygameToolsBox-1.1.4/PygameToolsBox/spritesheet.py`

 * *Files identical despite different names*

### Comparing `PygameToolsBox-1.1.3/PygameToolsBox.egg-info/PKG-INFO` & `PygameToolsBox-1.1.4/PygameToolsBox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PygameToolsBox
-Version: 1.1.3
+Version: 1.1.4
 Summary: Library for manage sprite sheet, and pallax background
 Author-email: FranckSix <francksix@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/FranckSix/PygameSpriteTools
 Project-URL: Issues, https://github.com/FranckSix/PygameSpriteTools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PygameToolsBox-1.1.3/README.md` & `PygameToolsBox-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `PygameToolsBox-1.1.3/pyproject.toml` & `PygameToolsBox-1.1.4/pyproject.toml`

 * *Files identical despite different names*

