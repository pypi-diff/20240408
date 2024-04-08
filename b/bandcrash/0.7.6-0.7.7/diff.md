# Comparing `tmp/bandcrash-0.7.6.tar.gz` & `tmp/bandcrash-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bandcrash-0.7.6.tar", max compression
+gzip compressed data, was "bandcrash-0.7.7.tar", max compression
```

## Comparing `bandcrash-0.7.6.tar` & `bandcrash-0.7.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1088 2023-10-06 21:56:05.559363 bandcrash-0.7.6/LICENSE
--rw-r--r--   0        0        0     4579 2023-10-30 22:46:03.382901 bandcrash-0.7.6/README.md
--rw-r--r--   0        0        0    21631 2024-03-06 10:56:20.854978 bandcrash-0.7.6/bandcrash/__init__.py
--rw-r--r--   0        0        0       65 2024-03-07 19:39:33.094972 bandcrash-0.7.6/bandcrash/__version__.py
--rw-r--r--   0        0        0     6282 2024-03-07 19:21:31.655502 bandcrash-0.7.6/bandcrash/cli.py
--rw-r--r--   0        0        0    33390 2024-03-07 19:24:26.963905 bandcrash-0.7.6/bandcrash/gui/__init__.py
--rw-r--r--   0        0        0     1581 2023-10-27 08:22:50.526884 bandcrash-0.7.6/bandcrash/gui/datatypes.py
--rw-r--r--   0        0        0     3939 2024-03-07 19:29:42.161581 bandcrash-0.7.6/bandcrash/gui/encoder.py
--rw-r--r--   0        0        0     2110 2023-11-03 05:44:18.709850 bandcrash-0.7.6/bandcrash/gui/file_utils.py
--rw-r--r--   0        0        0    16819 2023-11-07 02:41:32.977238 bandcrash-0.7.6/bandcrash/gui/track_editor.py
--rw-r--r--   0        0        0     8074 2023-11-18 00:04:06.395471 bandcrash-0.7.6/bandcrash/gui/widgets.py
--rw-r--r--   0        0        0     3892 2023-10-30 22:46:03.384473 bandcrash-0.7.6/bandcrash/images.py
--rw-r--r--   0        0        0     4344 2024-03-07 19:24:16.411177 bandcrash-0.7.6/bandcrash/options.py
--rw-r--r--   0        0        0     2348 2023-11-01 23:47:02.806367 bandcrash-0.7.6/bandcrash/players/camptown.py
--rw-r--r--   0        0        0     7140 2024-03-06 10:20:47.610843 bandcrash-0.7.6/bandcrash/util.py
--rw-r--r--   0        0        0     1443 2024-03-07 19:37:33.489610 bandcrash-0.7.6/pyproject.toml
--rw-r--r--   0        0        0     5693 1970-01-01 00:00:00.000000 bandcrash-0.7.6/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-10-06 21:56:05.559363 bandcrash-0.7.7/LICENSE
+-rw-r--r--   0        0        0     4579 2023-10-30 22:46:03.382901 bandcrash-0.7.7/README.md
+-rw-r--r--   0        0        0    21631 2024-03-06 10:56:20.854978 bandcrash-0.7.7/bandcrash/__init__.py
+-rw-r--r--   0        0        0       65 2024-04-08 20:36:19.659277 bandcrash-0.7.7/bandcrash/__version__.py
+-rw-r--r--   0        0        0     6282 2024-03-07 19:21:31.655502 bandcrash-0.7.7/bandcrash/cli.py
+-rw-r--r--   0        0        0    33655 2024-04-08 20:29:11.529704 bandcrash-0.7.7/bandcrash/gui/__init__.py
+-rw-r--r--   0        0        0     1581 2023-10-27 08:22:50.526884 bandcrash-0.7.7/bandcrash/gui/datatypes.py
+-rw-r--r--   0        0        0     3939 2024-03-07 19:29:42.161581 bandcrash-0.7.7/bandcrash/gui/encoder.py
+-rw-r--r--   0        0        0     2110 2023-11-03 05:44:18.709850 bandcrash-0.7.7/bandcrash/gui/file_utils.py
+-rw-r--r--   0        0        0    17316 2024-04-08 20:29:11.416623 bandcrash-0.7.7/bandcrash/gui/track_editor.py
+-rw-r--r--   0        0        0     8074 2023-11-18 00:04:06.395471 bandcrash-0.7.7/bandcrash/gui/widgets.py
+-rw-r--r--   0        0        0     3846 2024-03-13 07:36:34.589025 bandcrash-0.7.7/bandcrash/images.py
+-rw-r--r--   0        0        0     4344 2024-03-07 19:24:16.411177 bandcrash-0.7.7/bandcrash/options.py
+-rw-r--r--   0        0        0     2348 2023-11-01 23:47:02.806367 bandcrash-0.7.7/bandcrash/players/camptown.py
+-rw-r--r--   0        0        0     7140 2024-03-06 10:20:47.610843 bandcrash-0.7.7/bandcrash/util.py
+-rw-r--r--   0        0        0     1443 2024-04-08 20:30:01.748057 bandcrash-0.7.7/pyproject.toml
+-rw-r--r--   0        0        0     5693 1970-01-01 00:00:00.000000 bandcrash-0.7.7/PKG-INFO
```

### Comparing `bandcrash-0.7.6/LICENSE` & `bandcrash-0.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bandcrash-0.7.6/README.md` & `bandcrash-0.7.7/README.md`

 * *Files identical despite different names*

### Comparing `bandcrash-0.7.6/bandcrash/__init__.py` & `bandcrash-0.7.7/bandcrash/__init__.py`

 * *Files identical despite different names*

### Comparing `bandcrash-0.7.6/bandcrash/cli.py` & `bandcrash-0.7.7/bandcrash/cli.py`

 * *Files identical despite different names*

### Comparing `bandcrash-0.7.6/bandcrash/gui/__init__.py` & `bandcrash-0.7.7/bandcrash/gui/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -382,51 +382,60 @@
                       self.track_listing.select_next, "PgDown")
         add_menu_item(track_menu, "Move &up",
                       self.track_listing.move_up, "Alt+Up")
         add_menu_item(track_menu, "Move &down",
                       self.track_listing.move_down, "Alt+Down")
 
         checkboxes = widgets.FlowLayout()
-        self.do_preview = QCheckBox("Web preview")
+        self.do_preview = QCheckBox("Web player")
         self.do_mp3 = QCheckBox("MP3")
         self.do_ogg = QCheckBox("Ogg Vorbis")
         self.do_flac = QCheckBox("FLAC")
-        self.do_zip = QCheckBox("Build .zip files")
         self.do_cleanup = QCheckBox("Clean extra files")
+        self.do_zip = QCheckBox("Build .zip files")
         checkboxes.addWidget(self.do_preview)
         checkboxes.addWidget(self.do_mp3)
         checkboxes.addWidget(self.do_ogg)
         checkboxes.addWidget(self.do_flac)
-        checkboxes.addWidget(self.do_zip)
         checkboxes.addWidget(self.do_cleanup)
+        checkboxes.addWidget(self.do_zip)
         layout.addRow("Build options", checkboxes)
 
         butler_opts = QHBoxLayout()
         self.do_butler = QCheckBox()
         self.butler_target = QLineEdit()
         self.butler_target.setPlaceholderText("username/my-album-name")
         self.butler_prefix = QLineEdit()
         self.butler_prefix.setPlaceholderText("prefix")
         butler_opts.addWidget(self.do_butler)
         butler_opts.addWidget(self.butler_target, 50)
         butler_opts.addWidget(self.butler_prefix, 10)
-        layout.addRow("itch.io", butler_opts)
+        layout.addRow("itch.io butler", butler_opts)
 
         buttons = QHBoxLayout()
 
         start_button = QPushButton("Encode")
         start_button.clicked.connect(self.encode_album)
 
         buttons.addWidget(start_button)
 
         layout.addRow(buttons)
 
         self.setWindowTitle(self.filename or 'New Album')
 
         self.reset()
+
+        for widget in (
+            self.artist,
+            self.title,
+            self.genre,
+            self.composer
+        ):
+            widget.textChanged.connect(self.apply)
+
         self.apply()
         self.update_hash()
 
     @property
     def filename(self):
         """ The current filename of the album """
         return self.path_delegate.filename
@@ -579,14 +588,16 @@
         }
 
         # update whether the itch.io checkbox is enabled
         butler_path = get_encode_options().butler_path
         self.do_butler.setEnabled(
             bool(butler_path and shutil.which(butler_path)))
 
+        self.track_listing.track_editor.update_placeholders(self.data)
+
     @property
     def history_state(self):
         """ Get the current edit history state """
         return self.track_listing.current_row, copy.deepcopy(self.data)
 
     @history_state.setter
     def history_state(self, state):
```

### Comparing `bandcrash-0.7.6/bandcrash/gui/datatypes.py` & `bandcrash-0.7.7/bandcrash/gui/datatypes.py`

 * *Files identical despite different names*

### Comparing `bandcrash-0.7.6/bandcrash/gui/encoder.py` & `bandcrash-0.7.7/bandcrash/gui/encoder.py`

 * *Files identical despite different names*

### Comparing `bandcrash-0.7.6/bandcrash/gui/file_utils.py` & `bandcrash-0.7.7/bandcrash/gui/file_utils.py`

 * *Files identical despite different names*

### Comparing `bandcrash-0.7.6/bandcrash/gui/track_editor.py` & `bandcrash-0.7.7/bandcrash/gui/track_editor.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,14 +174,26 @@
 
         datatypes.apply_checkbox_fields(self.data, (
             ('explicit', self.explicit, False),
         ))
 
         LOGGER.debug("applied: %s", self.data)
 
+    def update_placeholders(self, album_data):
+        """ Update the placeholder text in the track editor widgets """
+        if album_data:
+            for field, widget in (
+                ('genre', self.genre),
+                ('artist', self.artist),
+                ('composer', self.composer),
+            ):
+                LOGGER.debug("updated placeholder for %s", field)
+                widget.setPlaceholderText(album_data.get(
+                    field, 'If different than album'))
+
 
 class TrackListEditor(QSplitter):
     """ The track listing panel and editor """
     # pylint:disable=too-many-instance-attributes
 
     class TrackItem(QListWidgetItem):
         """ an item in the track listing """
```

### Comparing `bandcrash-0.7.6/bandcrash/gui/widgets.py` & `bandcrash-0.7.7/bandcrash/gui/widgets.py`

 * *Files identical despite different names*

### Comparing `bandcrash-0.7.6/bandcrash/images.py` & `bandcrash-0.7.7/bandcrash/images.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 def load_image(in_path: str) -> PIL.Image:
     """ Load an image into memory, pooling it """
     if not os.path.isfile(in_path):
         raise FileNotFoundError(f"Couldn't find image {in_path}")
     return PIL.Image.open(in_path)
 
 
-@functools.lru_cache()
 def generate_image(in_path: str, size: int) -> PIL.Image:
     """ Given an image path, generate a rendition that fits within the size constraint
 
     :param str in_path: Path to the file
     :param int size: Maximum size (both width and height)
     """
     image = load_image(in_path)
@@ -59,15 +58,14 @@
     out_file = slugify_filename(f'{basename}.{size}.{ext}')
     image.convert(mode).save(os.path.join(out_dir, out_file))
     LOGGER.info("Wrote image %s", out_file)
 
     return out_file, image.width, image.height
 
 
-@functools.lru_cache()
 def generate_blob(in_path: str, size: int, ext: str = "jpeg") -> bytes:
     """ Generate a data blob for a compressed image
 
     :param str in_path: Path to the file
     :param int size: Maximum rendition size
     :param str format: Output file format
```

### Comparing `bandcrash-0.7.6/bandcrash/options.py` & `bandcrash-0.7.7/bandcrash/options.py`

 * *Files identical despite different names*

### Comparing `bandcrash-0.7.6/bandcrash/players/camptown.py` & `bandcrash-0.7.7/bandcrash/players/camptown.py`

 * *Files identical despite different names*

### Comparing `bandcrash-0.7.6/bandcrash/util.py` & `bandcrash-0.7.7/bandcrash/util.py`

 * *Files identical despite different names*

### Comparing `bandcrash-0.7.6/pyproject.toml` & `bandcrash-0.7.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bandcrash"
-version = "0.7.6"
+version = "0.7.7"
 description = "Tools for publishing albums to the web and digital stores"
 authors = ["fluffy <fluffy@beesbuzz.biz>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/fluffy-critter/bandcrash"
 documentation = "https://bandcrash.readthedocs.io/"
 include = [
```

### Comparing `bandcrash-0.7.6/PKG-INFO` & `bandcrash-0.7.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bandcrash
-Version: 0.7.6
+Version: 0.7.7
 Summary: Tools for publishing albums to the web and digital stores
 Home-page: https://github.com/fluffy-critter/bandcrash
 License: MIT
 Author: fluffy
 Author-email: fluffy@beesbuzz.biz
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

