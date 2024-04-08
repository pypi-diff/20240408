# Comparing `tmp/bondzai.media-handler-0.0.16.tar.gz` & `tmp/bondzai.media-handler-0.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bondzai.media-handler-0.0.16.tar", last modified: Wed Feb  7 14:05:21 2024, max compression
+gzip compressed data, was "bondzai.media-handler-0.0.17.tar", last modified: Mon Apr  8 11:58:14 2024, max compression
```

## Comparing `bondzai.media-handler-0.0.16.tar` & `bondzai.media-handler-0.0.17.tar`

### file list

```diff
@@ -1,32 +1,51 @@
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2024-02-07 14:05:21.779754 bondzai.media-handler-0.0.16/
--rw-r--r--   0 theo       (501) staff       (20)      547 2024-01-12 11:15:48.000000 bondzai.media-handler-0.0.16/NOTICE
--rw-r--r--   0 theo       (501) staff       (20)     1638 2024-02-07 14:05:21.779834 bondzai.media-handler-0.0.16/PKG-INFO
--rw-r--r--   0 theo       (501) staff       (20)     1246 2023-06-02 23:30:18.000000 bondzai.media-handler-0.0.16/README.rst
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2024-02-07 14:05:21.773444 bondzai.media-handler-0.0.16/bondzai/
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2024-02-07 14:05:21.776920 bondzai.media-handler-0.0.16/bondzai/media_handler/
--rw-r--r--   0 theo       (501) staff       (20)     2503 2024-02-07 14:04:48.000000 bondzai.media-handler-0.0.16/bondzai/media_handler/__init__.py
--rw-r--r--   0 theo       (501) staff       (20)      871 2024-01-12 11:15:48.000000 bondzai.media-handler-0.0.16/bondzai/media_handler/audio.py
--rw-r--r--   0 theo       (501) staff       (20)     1851 2024-01-12 11:15:48.000000 bondzai.media-handler-0.0.16/bondzai/media_handler/base.py
--rw-r--r--   0 theo       (501) staff       (20)     7728 2024-02-07 14:03:00.000000 bondzai.media-handler-0.0.16/bondzai/media_handler/data_packager.py
--rw-r--r--   0 theo       (501) staff       (20)      903 2024-01-12 11:15:48.000000 bondzai.media-handler-0.0.16/bondzai/media_handler/generic.py
--rw-r--r--   0 theo       (501) staff       (20)     1191 2024-01-12 11:15:48.000000 bondzai.media-handler-0.0.16/bondzai/media_handler/image.py
--rw-r--r--   0 theo       (501) staff       (20)      290 2024-01-12 11:15:48.000000 bondzai.media-handler-0.0.16/bondzai/media_handler/registry.py
--rw-r--r--   0 theo       (501) staff       (20)     1171 2024-01-12 11:15:48.000000 bondzai.media-handler-0.0.16/bondzai/media_handler/video.py
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2024-02-07 14:05:21.779527 bondzai.media-handler-0.0.16/bondzai.media_handler.egg-info/
--rw-r--r--   0 theo       (501) staff       (20)     1638 2024-02-07 14:05:21.000000 bondzai.media-handler-0.0.16/bondzai.media_handler.egg-info/PKG-INFO
--rw-r--r--   0 theo       (501) staff       (20)      788 2024-02-07 14:05:21.000000 bondzai.media-handler-0.0.16/bondzai.media_handler.egg-info/SOURCES.txt
--rw-r--r--   0 theo       (501) staff       (20)        1 2024-02-07 14:05:21.000000 bondzai.media-handler-0.0.16/bondzai.media_handler.egg-info/dependency_links.txt
--rw-r--r--   0 theo       (501) staff       (20)        8 2024-02-07 14:05:21.000000 bondzai.media-handler-0.0.16/bondzai.media_handler.egg-info/namespace_packages.txt
--rw-r--r--   0 theo       (501) staff       (20)      121 2024-02-07 14:05:21.000000 bondzai.media-handler-0.0.16/bondzai.media_handler.egg-info/requires.txt
--rw-r--r--   0 theo       (501) staff       (20)       23 2024-02-07 14:05:21.000000 bondzai.media-handler-0.0.16/bondzai.media_handler.egg-info/top_level.txt
--rw-r--r--   0 theo       (501) staff       (20)        1 2024-02-07 14:05:21.000000 bondzai.media-handler-0.0.16/bondzai.media_handler.egg-info/zip-safe
--rw-r--r--   0 theo       (501) staff       (20)       71 2023-05-30 10:20:03.000000 bondzai.media-handler-0.0.16/pyproject.toml
--rw-r--r--   0 theo       (501) staff       (20)      772 2024-02-07 14:05:21.780124 bondzai.media-handler-0.0.16/setup.cfg
--rw-r--r--   0 theo       (501) staff       (20)       36 2024-01-12 11:15:48.000000 bondzai.media-handler-0.0.16/setup.py
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2024-02-07 14:05:21.778231 bondzai.media-handler-0.0.16/tests/
--rw-r--r--   0 theo       (501) staff       (20)        0 2024-01-12 11:15:48.000000 bondzai.media-handler-0.0.16/tests/__init__.py
--rw-r--r--   0 theo       (501) staff       (20)      976 2024-01-12 11:15:48.000000 bondzai.media-handler-0.0.16/tests/test_audio.py
--rw-r--r--   0 theo       (501) staff       (20)     7932 2024-02-07 14:03:00.000000 bondzai.media-handler-0.0.16/tests/test_data_packager.py
--rw-r--r--   0 theo       (501) staff       (20)      840 2024-01-12 11:15:48.000000 bondzai.media-handler-0.0.16/tests/test_generic.py
--rw-r--r--   0 theo       (501) staff       (20)     1172 2024-01-12 11:15:48.000000 bondzai.media-handler-0.0.16/tests/test_image.py
--rw-r--r--   0 theo       (501) staff       (20)     1142 2024-01-12 11:15:48.000000 bondzai.media-handler-0.0.16/tests/test_video.py
+drwxrwxrwx   0        0        0        0 2024-04-08 11:58:14.796821 bondzai.media-handler-0.0.17/
+-rw-rw-rw-   0        0        0      547 2023-10-17 12:30:45.000000 bondzai.media-handler-0.0.17/NOTICE
+-rw-rw-rw-   0        0        0     1728 2024-04-08 11:58:14.796821 bondzai.media-handler-0.0.17/PKG-INFO
+-rw-rw-rw-   0        0        0     1246 2023-10-17 12:30:45.000000 bondzai.media-handler-0.0.17/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-08 11:58:14.720611 bondzai.media-handler-0.0.17/bondzai/
+drwxrwxrwx   0        0        0        0 2024-04-08 11:58:14.734867 bondzai.media-handler-0.0.17/bondzai/media_handler/
+-rw-rw-rw-   0        0        0     2503 2024-04-03 16:19:17.000000 bondzai.media-handler-0.0.17/bondzai/media_handler/__init__.py
+-rw-rw-rw-   0        0        0     1059 2024-04-03 16:19:17.000000 bondzai.media-handler-0.0.17/bondzai/media_handler/audio.py
+-rw-rw-rw-   0        0        0     1851 2023-10-17 12:30:45.000000 bondzai.media-handler-0.0.17/bondzai/media_handler/base.py
+-rw-rw-rw-   0        0        0     8035 2024-04-03 16:19:17.000000 bondzai.media-handler-0.0.17/bondzai/media_handler/data_packager.py
+-rw-rw-rw-   0        0        0      903 2023-10-17 12:30:45.000000 bondzai.media-handler-0.0.17/bondzai/media_handler/generic.py
+-rw-rw-rw-   0        0        0     1191 2023-10-17 12:30:45.000000 bondzai.media-handler-0.0.17/bondzai/media_handler/image.py
+-rw-rw-rw-   0        0        0      290 2023-10-17 12:30:45.000000 bondzai.media-handler-0.0.17/bondzai/media_handler/registry.py
+-rw-rw-rw-   0        0        0     1171 2023-10-17 12:30:45.000000 bondzai.media-handler-0.0.17/bondzai/media_handler/video.py
+drwxrwxrwx   0        0        0        0 2024-04-08 11:58:14.794800 bondzai.media-handler-0.0.17/bondzai.media_handler.egg-info/
+-rw-rw-rw-   0        0        0     1728 2024-04-08 11:58:14.000000 bondzai.media-handler-0.0.17/bondzai.media_handler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1738 2024-04-08 11:58:14.000000 bondzai.media-handler-0.0.17/bondzai.media_handler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 11:58:14.000000 bondzai.media-handler-0.0.17/bondzai.media_handler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-08 11:58:14.000000 bondzai.media-handler-0.0.17/bondzai.media_handler.egg-info/namespace_packages.txt
+-rw-rw-rw-   0        0        0      121 2024-04-08 11:58:14.000000 bondzai.media-handler-0.0.17/bondzai.media_handler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2024-04-08 11:58:14.000000 bondzai.media-handler-0.0.17/bondzai.media_handler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-04-04 15:00:51.000000 bondzai.media-handler-0.0.17/bondzai.media_handler.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2024-04-08 11:58:14.721613 bondzai.media-handler-0.0.17/build/
+drwxrwxrwx   0        0        0        0 2024-04-08 11:58:14.721613 bondzai.media-handler-0.0.17/build/lib/
+drwxrwxrwx   0        0        0        0 2024-04-08 11:58:14.721613 bondzai.media-handler-0.0.17/build/lib/bondzai/
+drwxrwxrwx   0        0        0        0 2024-04-08 11:58:14.740864 bondzai.media-handler-0.0.17/build/lib/bondzai/media_handler/
+-rw-rw-rw-   0        0        0     2503 2024-04-03 16:19:17.000000 bondzai.media-handler-0.0.17/build/lib/bondzai/media_handler/__init__.py
+-rw-rw-rw-   0        0        0     1059 2024-04-03 16:19:17.000000 bondzai.media-handler-0.0.17/build/lib/bondzai/media_handler/audio.py
+-rw-rw-rw-   0        0        0     1851 2023-10-17 12:30:45.000000 bondzai.media-handler-0.0.17/build/lib/bondzai/media_handler/base.py
+-rw-rw-rw-   0        0        0     8035 2024-04-03 16:19:17.000000 bondzai.media-handler-0.0.17/build/lib/bondzai/media_handler/data_packager.py
+-rw-rw-rw-   0        0        0      903 2023-10-17 12:30:45.000000 bondzai.media-handler-0.0.17/build/lib/bondzai/media_handler/generic.py
+-rw-rw-rw-   0        0        0     1191 2023-10-17 12:30:45.000000 bondzai.media-handler-0.0.17/build/lib/bondzai/media_handler/image.py
+-rw-rw-rw-   0        0        0      290 2023-10-17 12:30:45.000000 bondzai.media-handler-0.0.17/build/lib/bondzai/media_handler/registry.py
+-rw-rw-rw-   0        0        0     1171 2023-10-17 12:30:45.000000 bondzai.media-handler-0.0.17/build/lib/bondzai/media_handler/video.py
+drwxrwxrwx   0        0        0        0 2024-04-08 11:58:14.746868 bondzai.media-handler-0.0.17/build/lib/tests/
+-rw-rw-rw-   0        0        0        0 2023-10-17 12:30:45.000000 bondzai.media-handler-0.0.17/build/lib/tests/__init__.py
+-rw-rw-rw-   0        0        0     1446 2024-04-03 16:19:17.000000 bondzai.media-handler-0.0.17/build/lib/tests/test_audio.py
+-rw-rw-rw-   0        0        0     8781 2024-04-03 16:19:17.000000 bondzai.media-handler-0.0.17/build/lib/tests/test_data_packager.py
+-rw-rw-rw-   0        0        0      894 2024-04-03 16:19:17.000000 bondzai.media-handler-0.0.17/build/lib/tests/test_generic.py
+-rw-rw-rw-   0        0        0     1234 2024-04-03 16:19:17.000000 bondzai.media-handler-0.0.17/build/lib/tests/test_image.py
+-rw-rw-rw-   0        0        0     1204 2024-04-03 16:19:17.000000 bondzai.media-handler-0.0.17/build/lib/tests/test_video.py
+-rw-rw-rw-   0        0        0       71 2023-10-17 12:30:45.000000 bondzai.media-handler-0.0.17/pyproject.toml
+-rw-rw-rw-   0        0        0      812 2024-04-08 11:58:14.798891 bondzai.media-handler-0.0.17/setup.cfg
+-rw-rw-rw-   0        0        0       36 2023-10-17 12:30:45.000000 bondzai.media-handler-0.0.17/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 11:58:14.750869 bondzai.media-handler-0.0.17/tests/
+-rw-rw-rw-   0        0        0        0 2023-10-17 12:30:45.000000 bondzai.media-handler-0.0.17/tests/__init__.py
+-rw-rw-rw-   0        0        0     1446 2024-04-03 16:19:17.000000 bondzai.media-handler-0.0.17/tests/test_audio.py
+-rw-rw-rw-   0        0        0     8781 2024-04-03 16:19:17.000000 bondzai.media-handler-0.0.17/tests/test_data_packager.py
+-rw-rw-rw-   0        0        0      894 2024-04-03 16:19:17.000000 bondzai.media-handler-0.0.17/tests/test_generic.py
+-rw-rw-rw-   0        0        0     1234 2024-04-03 16:19:17.000000 bondzai.media-handler-0.0.17/tests/test_image.py
+-rw-rw-rw-   0        0        0     1204 2024-04-03 16:19:17.000000 bondzai.media-handler-0.0.17/tests/test_video.py
```

### Comparing `bondzai.media-handler-0.0.16/NOTICE` & `bondzai.media-handler-0.0.17/NOTICE`

 * *Files identical despite different names*

### Comparing `bondzai.media-handler-0.0.16/README.rst` & `bondzai.media-handler-0.0.17/README.rst`

 * *Files identical despite different names*

### Comparing `bondzai.media-handler-0.0.16/bondzai/media_handler/__init__.py` & `bondzai.media-handler-0.0.17/bondzai/media_handler/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from .base import get_file_mime, load_binary, save_binary, iter_data
 from .audio import AUDIO_ALLOWED_MIME, get_audio_metadata, get_audio_raw_data, save_audio_raw_data
 from .image import IMAGE_ALLOWED_MIME, get_image_metadata, get_image_raw_data, save_image_raw_data
 from .video import VIDEO_ALLOWED_MIME, get_video_metadata, get_video_raw_data, save_video_raw_data
 from .generic import GENERIC_ALLOWED_MIME, get_generic_metadata, get_generic_raw_data, save_generic_raw_data
 
 
-__version__ = "0.0.16"
+__version__ = "0.0.17"
 
 
 def get_raw_data(file_path: Path) -> list[float]:
     """
     Get raw data as list from file
     Args:
         file_path: path of the file
```

### Comparing `bondzai.media-handler-0.0.16/bondzai/media_handler/audio.py` & `bondzai.media-handler-0.0.17/bondzai/media_handler/audio.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,31 +5,35 @@
 import soundfile as sf
 from .base import check_mime
 
 
 AUDIO_ALLOWED_MIME = [
     "audio/x-wav",
     "audio/wav",
+    "audio/x-flac",
+    "audio/flac",
     "audio/mpeg"
 ]
 
 
 def get_audio_metadata(file_path: Path) -> dict:
     mime = check_mime(file_path, AUDIO_ALLOWED_MIME)
     audio = audio_metadata.load(file_path)
 
     return {
         "mime": mime,
         "sample_rate": audio["streaminfo"].sample_rate,
         "channels": audio["streaminfo"].channels,
+        "bit_depth": audio["streaminfo"].bit_depth
     }
 
 
 def get_audio_raw_data(file_path: Path) -> list[float]:
-    data, _ = sf.read(file_path)
-    return data.flatten().tolist()
+    data, _ = sf.read(file_path, dtype=np.float32)
+    return data.ravel().tolist()
 
 
 def save_audio_raw_data(raw_data: list, metadata: dict, file_path: Path):
     nb_channels = metadata["channels"]
-    data = np.reshape(raw_data, (int(len(raw_data) / nb_channels), nb_channels))
-    sf.write(file_path, data, metadata["sample_rate"])
+    sub_type = f"PCM_{metadata['bit_depth']}"
+    data = np.reshape(raw_data, (int(len(raw_data) / nb_channels), nb_channels)).astype(np.float32)
+    sf.write(file_path, data, metadata["sample_rate"], subtype=sub_type)
```

### Comparing `bondzai.media-handler-0.0.16/bondzai/media_handler/base.py` & `bondzai.media-handler-0.0.17/bondzai/media_handler/base.py`

 * *Files identical despite different names*

### Comparing `bondzai.media-handler-0.0.16/bondzai/media_handler/data_packager.py` & `bondzai.media-handler-0.0.17/bondzai/media_handler/data_packager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
 from pathlib import Path
 import tempfile
 import yaml
 import shutil
 import tarfile
+
 from . import get_raw_data, get_metadata, save_binary, iter_data, save_raw_data
 
 
 UNKNOWN = "unknown"
 LABEL_LIST_FILE_NAME = "LABEL_LIST.json"
 
 
@@ -164,56 +165,59 @@
         init_output_dict: If given, initialise output_dict by that one
     Returns:
         output_dict: "outputs" section of the dataset.yml
     """
     output_dict = init_output_dict.copy()
     data_dict = {"dataset": [], "outputs": {}}
     compress = None
-    if data_folder.suffixes == [".tar", ".gz"]:
-        temp_dir = Path(tempfile.mkdtemp())
-        with tarfile.open(data_folder, "r") as tar_file:
-            tar_file.extractall(temp_dir)
-        data_folder = temp_dir
-    if save_folder.suffixes == [".tar", ".gz"]:
-        compress = save_folder
-        save_folder = Path(tempfile.mkdtemp())
-    else:
-        if save_folder.exists():
-            shutil.rmtree(save_folder)
-        save_folder.mkdir(parents=True)
-    
-    with open(data_folder / LABEL_LIST_FILE_NAME, "r") as f:
-        output_list = json.load(f)
-
-    file_list = _parse_folder_recursive(data_folder, output_list)
-    file_list = sorted(file_list, key=lambda _file: _file["data"])
-    for file in file_list:
-        file_path = file["data"]
-        file["metadata"] = get_metadata(file_path)
-        new_file_name = get_maestro_file_name(file_path, file["output"])
-        new_file_path = save_folder / new_file_name
-        shutil.copy(file_path, new_file_path)
-        if convert_to_bin:
-            new_file_path = convert_to_binary(new_file_path)
-        file["data"] = new_file_path.name
-        file["source_id"] = source_name
-        data_dict["dataset"].append(file)
-        for key, value in file["output"].items():
-            if key not in output_dict:
-                output_dict[key] = {}
-            if value not in output_dict[key].keys():
-                if value.lower() == UNKNOWN:
-                    index = 0
-                else:
-                    index = 1
-                    existing_index_list = list(output_dict[key].values())
-                    while index in existing_index_list:
-                        index += 1
-                output_dict[key][value] = index
-    data_dict["outputs"] = output_dict
-    with open(save_folder / "dataset.yml", "w") as y:
-        yaml.safe_dump(data_dict, y, sort_keys=False)
+    with tempfile.TemporaryDirectory() as temp_dir:
+        if data_folder.suffixes == [".tar", ".gz"]:
+            temp_folder = Path(temp_dir) / "extract"
+            temp_folder.mkdir()
+            with tarfile.open(data_folder, "r") as tar_file:
+                tar_file.extractall(temp_folder)
+            data_folder = temp_folder
+        if save_folder.suffixes == [".tar", ".gz"]:
+            compress = save_folder
+            save_folder = Path(temp_dir) / "save"
+            save_folder.mkdir()
+        else:
+            if save_folder.exists():
+                shutil.rmtree(save_folder)
+            save_folder.mkdir(parents=True)
+        
+        with open(data_folder / LABEL_LIST_FILE_NAME, "r") as f:
+            output_list = json.load(f)
+
+        file_list = _parse_folder_recursive(data_folder, output_list)
+        file_list = sorted(file_list, key=lambda _file: _file["data"])
+        for file in file_list:
+            file_path = file["data"]
+            file["metadata"] = get_metadata(file_path)
+            new_file_name = get_maestro_file_name(file_path, file["output"])
+            new_file_path = save_folder / new_file_name
+            shutil.copy(file_path, new_file_path)
+            if convert_to_bin:
+                new_file_path = convert_to_binary(new_file_path)
+            file["data"] = new_file_path.name
+            file["source_id"] = source_name
+            data_dict["dataset"].append(file)
+            for key, value in file["output"].items():
+                if key not in output_dict:
+                    output_dict[key] = {}
+                if value not in output_dict[key].keys():
+                    if value.lower() == UNKNOWN:
+                        index = 0
+                    else:
+                        index = 1
+                        existing_index_list = list(output_dict[key].values())
+                        while index in existing_index_list:
+                            index += 1
+                    output_dict[key][value] = index
+        data_dict["outputs"] = output_dict
+        with open(save_folder / "dataset.yml", "w") as y:
+            yaml.safe_dump(data_dict, y, sort_keys=False)
 
-    if compress is not None:
-        create_tar_from_folder(compress, save_folder)
+        if compress is not None:
+            create_tar_from_folder(compress, save_folder)
 
     return output_dict
```

### Comparing `bondzai.media-handler-0.0.16/bondzai/media_handler/generic.py` & `bondzai.media-handler-0.0.17/bondzai/media_handler/generic.py`

 * *Files identical despite different names*

### Comparing `bondzai.media-handler-0.0.16/bondzai/media_handler/image.py` & `bondzai.media-handler-0.0.17/bondzai/media_handler/image.py`

 * *Files identical despite different names*

### Comparing `bondzai.media-handler-0.0.16/bondzai/media_handler/video.py` & `bondzai.media-handler-0.0.17/bondzai/media_handler/video.py`

 * *Files identical despite different names*

### Comparing `bondzai.media-handler-0.0.16/bondzai.media_handler.egg-info/SOURCES.txt` & `bondzai.media-handler-0.0.17/bondzai.media_handler.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -7,20 +7,48 @@
 ./bondzai/media_handler/audio.py
 ./bondzai/media_handler/base.py
 ./bondzai/media_handler/data_packager.py
 ./bondzai/media_handler/generic.py
 ./bondzai/media_handler/image.py
 ./bondzai/media_handler/registry.py
 ./bondzai/media_handler/video.py
+./build/lib/bondzai/media_handler/__init__.py
+./build/lib/bondzai/media_handler/audio.py
+./build/lib/bondzai/media_handler/base.py
+./build/lib/bondzai/media_handler/data_packager.py
+./build/lib/bondzai/media_handler/generic.py
+./build/lib/bondzai/media_handler/image.py
+./build/lib/bondzai/media_handler/registry.py
+./build/lib/bondzai/media_handler/video.py
+./build/lib/tests/__init__.py
+./build/lib/tests/test_audio.py
+./build/lib/tests/test_data_packager.py
+./build/lib/tests/test_generic.py
+./build/lib/tests/test_image.py
+./build/lib/tests/test_video.py
 ./tests/__init__.py
 ./tests/test_audio.py
 ./tests/test_data_packager.py
 ./tests/test_generic.py
 ./tests/test_image.py
 ./tests/test_video.py
 bondzai.media_handler.egg-info/PKG-INFO
 bondzai.media_handler.egg-info/SOURCES.txt
 bondzai.media_handler.egg-info/dependency_links.txt
 bondzai.media_handler.egg-info/namespace_packages.txt
 bondzai.media_handler.egg-info/requires.txt
 bondzai.media_handler.egg-info/top_level.txt
-bondzai.media_handler.egg-info/zip-safe
+bondzai.media_handler.egg-info/zip-safe
+bondzai/media_handler/__init__.py
+bondzai/media_handler/audio.py
+bondzai/media_handler/base.py
+bondzai/media_handler/data_packager.py
+bondzai/media_handler/generic.py
+bondzai/media_handler/image.py
+bondzai/media_handler/registry.py
+bondzai/media_handler/video.py
+tests/__init__.py
+tests/test_audio.py
+tests/test_data_packager.py
+tests/test_generic.py
+tests/test_image.py
+tests/test_video.py
```

### Comparing `bondzai.media-handler-0.0.16/setup.cfg` & `bondzai.media-handler-0.0.17/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,51 @@
-00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
-00000010: 3d20 626f 6e64 7a61 692e 6d65 6469 612d  = bondzai.media-
-00000020: 6861 6e64 6c65 720a 7665 7273 696f 6e20  handler.version 
-00000030: 3d20 6174 7472 3a20 626f 6e64 7a61 692e  = attr: bondzai.
-00000040: 6d65 6469 615f 6861 6e64 6c65 722e 5f5f  media_handler.__
-00000050: 7665 7273 696f 6e5f 5f0a 6175 7468 6f72  version__.author
-00000060: 203d 2042 6f6e 647a 6169 0a64 6573 6372   = Bondzai.descr
-00000070: 6970 7469 6f6e 203d 2042 6f6e 647a 6169  iption = Bondzai
-00000080: 204d 6564 6961 2048 616e 646c 6572 0a6c   Media Handler.l
-00000090: 6f6e 675f 6465 7363 7269 7074 696f 6e20  ong_description 
-000000a0: 3d20 6669 6c65 3a20 5245 4144 4d45 2e72  = file: README.r
-000000b0: 7374 0a6b 6579 776f 7264 7320 3d20 6461  st.keywords = da
-000000c0: 7669 6e73 792c 2062 6f6e 647a 6169 2c20  vinsy, bondzai, 
-000000d0: 6d65 6469 610a 6c69 6365 6e73 6520 3d20  media.license = 
-000000e0: 4170 6163 6865 204c 6963 656e 7365 2032  Apache License 2
-000000f0: 2e30 0a6c 6963 656e 7365 5f66 696c 6573  .0.license_files
-00000100: 203d 200a 094c 4943 454e 5345 0a09 4e4f   = ..LICENSE..NO
-00000110: 5449 4345 0a63 6c61 7373 6966 6965 7273  TICE.classifiers
-00000120: 203d 200a 0950 726f 6772 616d 6d69 6e67   = ..Programming
-00000130: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000140: 686f 6e20 3a3a 2033 0a09 4c69 6365 6e73  hon :: 3..Licens
-00000150: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
-00000160: 6420 3a3a 2041 7061 6368 6520 536f 6674  d :: Apache Soft
-00000170: 7761 7265 204c 6963 656e 7365 0a09 4f70  ware License..Op
-00000180: 6572 6174 696e 6720 5379 7374 656d 203a  erating System :
-00000190: 3a20 4f53 2049 6e64 6570 656e 6465 6e74  : OS Independent
-000001a0: 0a0a 5b6f 7074 696f 6e73 5d0a 7061 636b  ..[options].pack
-000001b0: 6167 6573 203d 2066 696e 645f 6e61 6d65  ages = find_name
-000001c0: 7370 6163 653a 0a70 6163 6b61 6765 5f64  space:.package_d
-000001d0: 6972 203d 200a 093d 202e 0a7a 6970 5f73  ir = ..= ..zip_s
-000001e0: 6166 6520 3d20 5472 7565 0a69 6e63 6c75  afe = True.inclu
-000001f0: 6465 5f70 6163 6b61 6765 5f64 6174 6120  de_package_data 
-00000200: 3d20 5472 7565 0a6e 616d 6573 7061 6365  = True.namespace
-00000210: 5f70 6163 6b61 6765 7320 3d20 0a09 626f  _packages = ..bo
-00000220: 6e64 7a61 690a 696e 7374 616c 6c5f 7265  ndzai.install_re
-00000230: 7175 6972 6573 203d 200a 0970 7974 6573  quires = ..pytes
-00000240: 743d 3d37 2e32 2e30 0a09 5079 5941 4d4c  t==7.2.0..PyYAML
-00000250: 3d3d 362e 302e 300a 096e 756d 7079 3d3d  ==6.0.0..numpy==
-00000260: 312e 3235 2e30 0a09 736f 756e 6466 696c  1.25.0..soundfil
-00000270: 653d 3d30 2e31 322e 310a 0961 7564 696f  e==0.12.1..audio
-00000280: 2d6d 6574 6164 6174 613d 3d30 2e31 312e  -metadata==0.11.
-00000290: 310a 0969 6d61 6765 696f 3d3d 322e 3330  1..imageio==2.30
-000002a0: 2e30 0a09 696d 6167 6569 6f2d 6666 6d70  .0..imageio-ffmp
-000002b0: 6567 3d3d 302e 342e 380a 0a5b 6f70 7469  eg==0.4.8..[opti
-000002c0: 6f6e 732e 7061 636b 6167 6573 2e66 696e  ons.packages.fin
-000002d0: 645d 0a77 6865 7265 203d 202e 0a0a 5b65  d].where = ...[e
-000002e0: 6767 5f69 6e66 6f5d 0a74 6167 5f62 7569  gg_info].tag_bui
-000002f0: 6c64 203d 200a 7461 675f 6461 7465 203d  ld = .tag_date =
-00000300: 2030 0a0a                                 0..
+00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
+00000010: 203d 2062 6f6e 647a 6169 2e6d 6564 6961   = bondzai.media
+00000020: 2d68 616e 646c 6572 0d0a 7665 7273 696f  -handler..versio
+00000030: 6e20 3d20 6174 7472 3a20 626f 6e64 7a61  n = attr: bondza
+00000040: 692e 6d65 6469 615f 6861 6e64 6c65 722e  i.media_handler.
+00000050: 5f5f 7665 7273 696f 6e5f 5f0d 0a61 7574  __version__..aut
+00000060: 686f 7220 3d20 426f 6e64 7a61 690d 0a64  hor = Bondzai..d
+00000070: 6573 6372 6970 7469 6f6e 203d 2042 6f6e  escription = Bon
+00000080: 647a 6169 204d 6564 6961 2048 616e 646c  dzai Media Handl
+00000090: 6572 0d0a 6c6f 6e67 5f64 6573 6372 6970  er..long_descrip
+000000a0: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
+000000b0: 444d 452e 7273 740d 0a6b 6579 776f 7264  DME.rst..keyword
+000000c0: 7320 3d20 6461 7669 6e73 792c 2062 6f6e  s = davinsy, bon
+000000d0: 647a 6169 2c20 6d65 6469 610d 0a6c 6963  dzai, media..lic
+000000e0: 656e 7365 203d 2041 7061 6368 6520 4c69  ense = Apache Li
+000000f0: 6365 6e73 6520 322e 300d 0a6c 6963 656e  cense 2.0..licen
+00000100: 7365 5f66 696c 6573 203d 200d 0a09 4c49  se_files = ...LI
+00000110: 4345 4e53 450d 0a09 4e4f 5449 4345 0d0a  CENSE...NOTICE..
+00000120: 636c 6173 7369 6669 6572 7320 3d20 0d0a  classifiers = ..
+00000130: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
+00000140: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000150: 3a3a 2033 0d0a 094c 6963 656e 7365 203a  :: 3...License :
+00000160: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
+00000170: 3a20 4170 6163 6865 2053 6f66 7477 6172  : Apache Softwar
+00000180: 6520 4c69 6365 6e73 650d 0a09 4f70 6572  e License...Oper
+00000190: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
+000001a0: 4f53 2049 6e64 6570 656e 6465 6e74 0d0a  OS Independent..
+000001b0: 0d0a 5b6f 7074 696f 6e73 5d0d 0a70 6163  ..[options]..pac
+000001c0: 6b61 6765 7320 3d20 6669 6e64 5f6e 616d  kages = find_nam
+000001d0: 6573 7061 6365 3a0d 0a70 6163 6b61 6765  espace:..package
+000001e0: 5f64 6972 203d 200d 0a09 3d20 2e0d 0a7a  _dir = ...= ...z
+000001f0: 6970 5f73 6166 6520 3d20 5472 7565 0d0a  ip_safe = True..
+00000200: 696e 636c 7564 655f 7061 636b 6167 655f  include_package_
+00000210: 6461 7461 203d 2054 7275 650d 0a6e 616d  data = True..nam
+00000220: 6573 7061 6365 5f70 6163 6b61 6765 7320  espace_packages 
+00000230: 3d20 0d0a 0962 6f6e 647a 6169 0d0a 696e  = ...bondzai..in
+00000240: 7374 616c 6c5f 7265 7175 6972 6573 203d  stall_requires =
+00000250: 200d 0a09 7079 7465 7374 3d3d 372e 322e   ...pytest==7.2.
+00000260: 300d 0a09 5079 5941 4d4c 3d3d 362e 302e  0...PyYAML==6.0.
+00000270: 300d 0a09 6e75 6d70 793d 3d31 2e32 352e  0...numpy==1.25.
+00000280: 300d 0a09 736f 756e 6466 696c 653d 3d30  0...soundfile==0
+00000290: 2e31 322e 310d 0a09 6175 6469 6f2d 6d65  .12.1...audio-me
+000002a0: 7461 6461 7461 3d3d 302e 3131 2e31 0d0a  tadata==0.11.1..
+000002b0: 0969 6d61 6765 696f 3d3d 322e 3330 2e30  .imageio==2.30.0
+000002c0: 0d0a 0969 6d61 6765 696f 2d66 666d 7065  ...imageio-ffmpe
+000002d0: 673d 3d30 2e34 2e38 0d0a 0d0a 5b6f 7074  g==0.4.8....[opt
+000002e0: 696f 6e73 2e70 6163 6b61 6765 732e 6669  ions.packages.fi
+000002f0: 6e64 5d0d 0a77 6865 7265 203d 202e 0d0a  nd]..where = ...
+00000300: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
+00000310: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
+00000320: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
```

### Comparing `bondzai.media-handler-0.0.16/tests/test_audio.py` & `bondzai.media-handler-0.0.17/build/lib/tests/test_image.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,29 @@
-from bondzai.media_handler import save_audio_raw_data, get_audio_raw_data, get_audio_metadata
+from bondzai.media_handler import save_image_raw_data, get_image_raw_data, get_image_metadata
+from bondzai.media_handler.image import GREYSCALE_8BIT_MODE, RGB_8BIT_MODE
 import tempfile
 import pytest
 from pathlib import Path
 import numpy as np
 
 
-@pytest.mark.parametrize("format", [(".wav", "audio/wav")])  # Not test for (".mp3", "audio/mpeg") because lossy
-def test_audio(format):
+@pytest.mark.parametrize("mode", [GREYSCALE_8BIT_MODE, RGB_8BIT_MODE])
+@pytest.mark.parametrize("format", [(".png", "image/png")])  # Not test for (".jpg", "image/jpeg") because lossy
+def test_image(format, mode):
     TOLERANCE = 1e-4
 
-    nb_channels = 2
-    length = 1024
-    fs = 16000
+    width = 24
+    height = 32
+    depth = len(mode)
 
-    save_dir = Path(tempfile.mkdtemp())
-    data = 2 * np.random.random(length * nb_channels) - 1
-    data = data.astype("float32").tolist()
-    file_path = save_dir / ("test" + format[0])
-    save_audio_raw_data(data, {"mime": format[1], "sample_rate": fs, "channels": nb_channels}, file_path)
-    raw_data = get_audio_raw_data(file_path)
-    metadata = get_audio_metadata(file_path)
-    assert np.max(np.abs(np.asarray(raw_data) - np.asarray(data))) < TOLERANCE
-    assert metadata["channels"] == nb_channels
-    assert metadata["sample_rate"] == fs
-    assert metadata["mime"] == format[1]
+    with tempfile.TemporaryDirectory() as save_dir:
+        data = np.random.randint(0, 255, width * height * depth)
+        data = (data.astype("float32") / 2 ** 8).tolist()
+        file_path = Path(save_dir) / ("test" + format[0])
+        save_image_raw_data(data, {"mime": format[1], "width": width, "height": height, "mode": mode}, file_path)
+        raw_data = get_image_raw_data(file_path)
+        metadata = get_image_metadata(file_path)
+        assert np.max(np.abs(np.asarray(raw_data) - np.asarray(data))) < TOLERANCE
+        assert metadata["width"] == width
+        assert metadata["height"] == height
+        assert metadata["mode"] == mode
+        assert metadata["mime"] == format[1]
```

### Comparing `bondzai.media-handler-0.0.16/tests/test_data_packager.py` & `bondzai.media-handler-0.0.17/build/lib/tests/test_data_packager.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import json
-from re import S
 import tarfile
 from uuid import uuid4
 
 import yaml
 from bondzai.media_handler import get_raw_data, save_raw_data
 from bondzai.media_handler.base import load_binary
 from bondzai.media_handler.data_packager import generate_dataset, create_tar_from_folder, convert_to_binary, create_chunks, get_maestro_file_name
@@ -14,15 +13,15 @@
 
 
 UNKNOWN = "unknown"
 LABEL_LIST_FILE_NAME = "LABEL_LIST.json"
 TOLERANCE = 1e-4
 
 DATA_GENERATION_DICT = {
-    "audio": {"ext": ".wav", "metadata": {"mime": "audio/wav", "sample_rate": 48000, "channels": 16}},
+    "audio": {"ext": ".wav", "metadata": {"mime": "audio/wav", "sample_rate": 48000, "channels": 16, "bit_depth": 16}},
     "image": {"ext": ".png", "metadata": {"mime": "image/png", "width": 128, "height": 64, "mode": "RGB"}},
     "video": {"ext": ".mp4", "metadata": {"mime": "video/mp4", "width": 32, "height": 16, "fps": 20}},
     "generic": {"ext": ".json", "metadata": {"mime": "application/json", "dim": [16]}},
     }
 
 def generate_random_file(data_type: str, save_folder: Path) -> (Path, list[float]):
     save_folder.mkdir(parents=True, exist_ok=True)
@@ -37,57 +36,65 @@
 
 def test_get_files_from_tar():
     # TODO : keep function?
     assert True
 
 @pytest.mark.parametrize("data_type", ["audio", "generic", "video", "image"]) 
 def test_create_tar_from_folder(data_type):
-    save_folder = Path(tempfile.mkdtemp())
-    file_list = [generate_random_file(data_type, save_folder) for _ in range(5)]
-    tar_path = Path(tempfile.mkdtemp()) / "save.tar.gz"
-    create_tar_from_folder(tar_path, save_folder)
-    assert tar_path.exists()
-    retrieve_folder = tar_path.parent / "retrieved"
-    retrieve_folder.mkdir()
-    with tarfile.open(tar_path, "w") as tar:
-        tar.extractall(retrieve_folder)
-    for index, file in enumerate(retrieve_folder.iterdir()):
-        tar_data = get_raw_data(file)
-        assert file_list[index][1]  
-        assert np.max(np.abs(np.asarray(file_list[index][1]) - np.asarray(tar_data))) < TOLERANCE
+    with tempfile.TemporaryDirectory() as temp_dir:
+        save_folder = Path(temp_dir) / "save"
+        save_folder.mkdir()
+        file_path_list = []
+        file_data_list = []
+        for _ in range(5):
+            path, data = generate_random_file(data_type, save_folder)
+            file_path_list.append(path)
+            file_data_list.append(data)
+        tar_path = Path(temp_dir) / "save.tar.gz"
+        create_tar_from_folder(tar_path, save_folder)
+        assert tar_path.exists()
+        retrieve_folder = Path(temp_dir) / "retrieved"
+        retrieve_folder.mkdir()
+        with tarfile.open(tar_path, "r:gz") as tar:
+            tar.extractall(retrieve_folder)
+        for file in retrieve_folder.iterdir():
+            tar_data = get_raw_data(file)
+            expected_file = save_folder / file.name
+            index = file_path_list.index(expected_file)
+            assert np.max(np.abs(np.asarray(file_data_list[index]) - np.asarray(tar_data))) < TOLERANCE
 
 
 @pytest.mark.parametrize("data_type", ["audio", "generic", "video", "image"]) 
 def test_convert_to_binary(data_type):
-    save_folder = Path(tempfile.mkdtemp())
-    save_file, data = generate_random_file(data_type, save_folder)
-    bin_file = convert_to_binary(save_file)
-    assert bin_file.exists()
-    bin_data = list(load_binary(bin_file))
-    assert data == bin_data
-    bin_file_2 = convert_to_binary(bin_file)
-    assert bin_file_2 == bin_file
-    bin_data_2 = list(load_binary(bin_file_2))
-    assert data == bin_data_2
+    with tempfile.TemporaryDirectory() as save_folder:
+        save_file, data = generate_random_file(data_type, Path(save_folder))
+        bin_file = convert_to_binary(save_file)
+        assert bin_file.exists()
+        bin_data = list(load_binary(bin_file))
+        assert data == bin_data
+        bin_file_2 = convert_to_binary(bin_file)
+        assert bin_file_2 == bin_file
+        bin_data_2 = list(load_binary(bin_file_2))
+        assert data == bin_data_2
 
 
 @pytest.mark.parametrize("data_type", ["audio", "generic", "video"]) 
 def test_create_chunks(data_type):
     unit_size = 16 * 32 * 3
     chunk_size = 5 * unit_size
     hop_len = 3 * unit_size
 
-    save_folder = Path(tempfile.mkdtemp())
-    save_file, random_data = generate_random_file(data_type, save_folder)
-    chunk_folder = save_file.parent / "chunks"
-    create_chunks(save_file, chunk_size, hop_len, chunk_folder)
-    for index, file in enumerate(chunk_folder.iterdir()):
-        chunk_data = get_raw_data(file)
-        chopped_data = random_data[hop_len * index: hop_len * index + chunk_size]
-        assert np.max(np.abs(np.asarray(chunk_data) - np.asarray(chopped_data))) < TOLERANCE
+    with tempfile.TemporaryDirectory() as save_folder:
+        save_file, random_data = generate_random_file(data_type, Path(save_folder))
+        chunk_folder = save_file.parent / "chunks"
+        create_chunks(save_file, chunk_size, hop_len, chunk_folder)
+        for index, file in enumerate(chunk_folder.iterdir()):
+            chunk_data = get_raw_data(file)
+            chopped_data = random_data[hop_len * index: hop_len * index + chunk_size]
+            assert np.max(np.abs(np.asarray(chunk_data) - np.asarray(chopped_data))) < TOLERANCE
 
 
 def test_get_maestro_file_name():
     file_name = get_maestro_file_name(Path("a/b/c/file.txt"), {"key_1": "value_1", "key_2": "value_2"})
     assert file_name == 'file[key_1;value_1][key_2;value_2].txt'
 
 
@@ -117,59 +124,66 @@
                 new_file_path = new_file_path.with_suffix(".bin")
             assert new_file_path.exists()
             new_data = load_binary(new_file_path) if convert_to_bin else get_raw_data(new_file_path)
             assert np.max(np.abs(np.asarray(new_data) - np.asarray(file_data))) < TOLERANCE
     
     file_list = []
     
-    dataset_folder = Path(tempfile.mkdtemp())
-    LABELS = {"number": ["1", "2", "3"], "letter": ["a", "b"]}
-    output_dict_ref = {}
-    for key, value_list in LABELS.items():
-        output_dict_ref[key] = {v: idx + 1 for idx, v in enumerate(value_list)}
-    label_list = list(LABELS.keys())
-    for label_1 in LABELS[label_list[0]]:
-        for label_2 in LABELS[label_list[1]]:
-            file, file_data = generate_random_file(data_type, dataset_folder / label_1 / label_2)
-            file_name = f"{file.stem}[{label_list[1]};{label_2}][{label_list[0]};{label_1}]{file.suffix}"
-            file_list.append((file, file_data, file_name))
-    
-    with open(dataset_folder / LABEL_LIST_FILE_NAME, "w")  as f:
-        json.dump(label_list, f)
-
-
-    save_folder = Path(tempfile.mkdtemp())
-    output_dict = generate_dataset(dataset_folder, save_folder, "src_1")
-    check_dataset(save_folder, file_list, source_name="src_1", convert_to_bin=True)
-    compare_output_dicts(output_dict, output_dict_ref)
-
-    save_folder = Path(tempfile.mkdtemp())
-    output_dict = generate_dataset(dataset_folder, save_folder, "src_2", convert_to_bin=False)
-    check_dataset(save_folder, file_list, source_name="src_2", convert_to_bin=False)
-    compare_output_dicts(output_dict, output_dict_ref)
-
-    save_folder = Path(tempfile.mkdtemp())
-    tar_path = Path(tempfile.mkdtemp()) / "dataset.tar.gz"
-    create_tar_from_folder(tar_path, dataset_folder)
-    output_dict = generate_dataset(tar_path, save_folder, "src_3")
-    check_dataset(save_folder, file_list, source_name="src_3", convert_to_bin=True)
-    compare_output_dicts(output_dict, output_dict_ref)
-
-    tar_save_path = Path(tempfile.mkdtemp()) / "save.tar.gz"
-    output_dict = generate_dataset(dataset_folder, tar_save_path, "src_4")
-    save_folder = Path(tempfile.mkdtemp())
-    with tarfile.open(tar_save_path, "r") as tar:
-        tar.extractall(save_folder)
-    check_dataset(save_folder, file_list, source_name="src_4", convert_to_bin=True)
-    compare_output_dicts(output_dict, output_dict_ref)
-
-    init_output_dict = {"bool": {"true": 1, "false": 2}, "number": {"0": 2}}
-    new_output_dict_ref = output_dict_ref.copy()
-    new_output_dict_ref["bool"] = init_output_dict["bool"]
-    new_output_dict_ref["number"]["0"] = 2
-    new_output_dict_ref["number"]["1"] = 1
-    new_output_dict_ref["number"]["2"] = 3
-    new_output_dict_ref["number"]["3"] = 4
-    save_folder = Path(tempfile.mkdtemp())
-    output_dict = generate_dataset(dataset_folder, save_folder, "src_5", init_output_dict=init_output_dict)
-    check_dataset(save_folder, file_list, source_name="src_5", convert_to_bin=True)
-    compare_output_dicts(output_dict, new_output_dict_ref)
+    with tempfile.TemporaryDirectory() as temp_dir:
+        dataset_folder = Path(temp_dir) / "dataset"
+        dataset_folder.mkdir()
+        LABELS = {"number": ["1", "2", "3"], "letter": ["a", "b"]}
+        output_dict_ref = {}
+        for key, value_list in LABELS.items():
+            output_dict_ref[key] = {v: idx + 1 for idx, v in enumerate(value_list)}
+        label_list = list(LABELS.keys())
+        for label_1 in LABELS[label_list[0]]:
+            for label_2 in LABELS[label_list[1]]:
+                file, file_data = generate_random_file(data_type, dataset_folder / label_1 / label_2)
+                file_name = f"{file.stem}[{label_list[1]};{label_2}][{label_list[0]};{label_1}]{file.suffix}"
+                file_list.append((file, file_data, file_name))
+        
+        with open(dataset_folder / LABEL_LIST_FILE_NAME, "w")  as f:
+            json.dump(label_list, f)
+
+
+        save_folder = Path(temp_dir) / "save_1"
+        save_folder.mkdir()
+        output_dict = generate_dataset(dataset_folder, save_folder, "src_1")
+        check_dataset(save_folder, file_list, source_name="src_1", convert_to_bin=True)
+        compare_output_dicts(output_dict, output_dict_ref)
+
+        save_folder = Path(temp_dir) / "save_2"
+        save_folder.mkdir()
+        output_dict = generate_dataset(dataset_folder, save_folder, "src_2", convert_to_bin=False)
+        check_dataset(save_folder, file_list, source_name="src_2", convert_to_bin=False)
+        compare_output_dicts(output_dict, output_dict_ref)
+
+        save_folder = Path(temp_dir) / "save_3"
+        save_folder.mkdir()
+        tar_path = Path(temp_dir) / "dataset.tar.gz"
+        create_tar_from_folder(tar_path, dataset_folder)
+        output_dict = generate_dataset(tar_path, save_folder, "src_3")
+        check_dataset(save_folder, file_list, source_name="src_3", convert_to_bin=True)
+        compare_output_dicts(output_dict, output_dict_ref)
+
+        tar_save_path = Path(temp_dir) / "save.tar.gz"
+        output_dict = generate_dataset(dataset_folder, tar_save_path, "src_4")
+        save_folder = Path(temp_dir) / "save_4"
+        save_folder.mkdir()
+        with tarfile.open(tar_save_path, "r") as tar:
+            tar.extractall(save_folder)
+        check_dataset(save_folder, file_list, source_name="src_4", convert_to_bin=True)
+        compare_output_dicts(output_dict, output_dict_ref)
+
+        init_output_dict = {"bool": {"true": 1, "false": 2}, "number": {"0": 2}}
+        new_output_dict_ref = output_dict_ref.copy()
+        new_output_dict_ref["bool"] = init_output_dict["bool"]
+        new_output_dict_ref["number"]["0"] = 2
+        new_output_dict_ref["number"]["1"] = 1
+        new_output_dict_ref["number"]["2"] = 3
+        new_output_dict_ref["number"]["3"] = 4
+        with tempfile.TemporaryDirectory() as temp_dir:
+            save_folder = Path(temp_dir)
+            output_dict = generate_dataset(dataset_folder, save_folder, "src_5", init_output_dict=init_output_dict)
+            check_dataset(save_folder, file_list, source_name="src_5", convert_to_bin=True)
+            compare_output_dicts(output_dict, new_output_dict_ref)
```

### Comparing `bondzai.media-handler-0.0.16/tests/test_generic.py` & `bondzai.media-handler-0.0.17/build/lib/tests/test_generic.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 
 @pytest.mark.parametrize("format", [(".json", "application/json")])
 def test_generic(format):
     TOLERANCE = 1e-4
     dim = [24, 3]
     length = 18
 
-    save_dir = Path(tempfile.mkdtemp())
-    data = 2 * np.random.random(length * np.prod(dim)) - 1
-    data = data.astype("float32").tolist()
-    file_path = save_dir / ("test" + format[0])
-    save_generic_raw_data(data, {"mime": format[1], "dim": dim}, file_path)
-    raw_data = get_generic_raw_data(file_path)
-    metadata = get_generic_metadata(file_path)
-    assert np.max(np.abs(np.asarray(raw_data) - np.asarray(data))) < TOLERANCE
-    assert metadata["mime"] == format[1]
-    assert metadata["dim"] == dim
+    with tempfile.TemporaryDirectory() as save_dir:
+        data = 2 * np.random.random(length * np.prod(dim)) - 1
+        data = data.astype("float32").tolist()
+        file_path = Path(save_dir) / ("test" + format[0])
+        save_generic_raw_data(data, {"mime": format[1], "dim": dim}, file_path)
+        raw_data = get_generic_raw_data(file_path)
+        metadata = get_generic_metadata(file_path)
+        assert np.max(np.abs(np.asarray(raw_data) - np.asarray(data))) < TOLERANCE
+        assert metadata["mime"] == format[1]
+        assert metadata["dim"] == dim
```

### Comparing `bondzai.media-handler-0.0.16/tests/test_image.py` & `bondzai.media-handler-0.0.17/tests/test_image.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 def test_image(format, mode):
     TOLERANCE = 1e-4
 
     width = 24
     height = 32
     depth = len(mode)
 
-    save_dir = Path(tempfile.mkdtemp())
-    data = np.random.randint(0, 255, width * height * depth)
-    data = (data.astype("float32") / 2 ** 8).tolist()
-    file_path = save_dir / ("test" + format[0])
-    save_image_raw_data(data, {"mime": format[1], "width": width, "height": height, "mode": mode}, file_path)
-    raw_data = get_image_raw_data(file_path)
-    metadata = get_image_metadata(file_path)
-    assert np.max(np.abs(np.asarray(raw_data) - np.asarray(data))) < TOLERANCE
-    assert metadata["width"] == width
-    assert metadata["height"] == height
-    assert metadata["mode"] == mode
-    assert metadata["mime"] == format[1]
+    with tempfile.TemporaryDirectory() as save_dir:
+        data = np.random.randint(0, 255, width * height * depth)
+        data = (data.astype("float32") / 2 ** 8).tolist()
+        file_path = Path(save_dir) / ("test" + format[0])
+        save_image_raw_data(data, {"mime": format[1], "width": width, "height": height, "mode": mode}, file_path)
+        raw_data = get_image_raw_data(file_path)
+        metadata = get_image_metadata(file_path)
+        assert np.max(np.abs(np.asarray(raw_data) - np.asarray(data))) < TOLERANCE
+        assert metadata["width"] == width
+        assert metadata["height"] == height
+        assert metadata["mode"] == mode
+        assert metadata["mime"] == format[1]
```

### Comparing `bondzai.media-handler-0.0.16/tests/test_video.py` & `bondzai.media-handler-0.0.17/build/lib/tests/test_video.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 
     width = 48 # Must be a multiple of 16
     height = 32 # Must be a multiple of 16
     depth = 3
     frame_nb = 7
     fps = 20
 
-    save_dir = Path(tempfile.mkdtemp())
-    data = np.random.randint(0, 255, width * height * depth * frame_nb).astype(np.float32) / 256
-    data = data.tolist()
-    file_path = save_dir / ("test" + format[0])
-    save_video_raw_data(data, {"mime": format[1], "width": width, "height": height, "fps": fps}, file_path)
-    raw_data = get_video_raw_data(file_path)
-    metadata = get_video_metadata(file_path)
-    assert metadata["fps"] == fps
-    assert metadata["width"] == width
-    assert metadata["height"] == height
-    assert metadata["mime"] == format[1]
-    assert np.max(np.abs(np.asarray(raw_data) - np.asarray(data))) < TOLERANCE
+    with tempfile.TemporaryDirectory() as save_dir:
+        data = np.random.randint(0, 255, width * height * depth * frame_nb).astype(np.float32) / 256
+        data = data.tolist()
+        file_path = Path(save_dir) / ("test" + format[0])
+        save_video_raw_data(data, {"mime": format[1], "width": width, "height": height, "fps": fps}, file_path)
+        raw_data = get_video_raw_data(file_path)
+        metadata = get_video_metadata(file_path)
+        assert metadata["fps"] == fps
+        assert metadata["width"] == width
+        assert metadata["height"] == height
+        assert metadata["mime"] == format[1]
+        assert np.max(np.abs(np.asarray(raw_data) - np.asarray(data))) < TOLERANCE
```

