# Comparing `tmp/unitlab-2.1.5.tar.gz` & `tmp/unitlab-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitlab-2.1.5.tar", last modified: Fri Apr  5 12:20:50 2024, max compression
+gzip compressed data, was "unitlab-2.1.6.tar", last modified: Mon Apr  8 13:29:09 2024, max compression
```

## Comparing `unitlab-2.1.5.tar` & `unitlab-2.1.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2024-04-05 12:20:50.913275 unitlab-2.1.5/
--rw-rw-r--   0 me        (1000) me        (1000)     1069 2024-02-13 07:39:37.000000 unitlab-2.1.5/LICENSE.md
--rw-r--r--   0 me        (1000) me        (1000)      793 2024-04-05 12:20:50.913275 unitlab-2.1.5/PKG-INFO
--rw-rw-r--   0 me        (1000) me        (1000)     1434 2023-09-24 12:59:00.000000 unitlab-2.1.5/README.md
--rw-rw-r--   0 me        (1000) me        (1000)      106 2024-04-05 12:20:50.913275 unitlab-2.1.5/setup.cfg
--rw-rw-r--   0 me        (1000) me        (1000)     1092 2024-04-05 12:19:12.000000 unitlab-2.1.5/setup.py
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2024-04-05 12:20:50.913275 unitlab-2.1.5/src/
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2024-04-05 12:20:50.913275 unitlab-2.1.5/src/unitlab/
--rw-rw-r--   0 me        (1000) me        (1000)      214 2024-04-05 11:53:23.000000 unitlab-2.1.5/src/unitlab/__init__.py
--rw-rw-r--   0 me        (1000) me        (1000)       29 2024-03-06 15:43:31.000000 unitlab-2.1.5/src/unitlab/__main__.py
--rw-rw-r--   0 me        (1000) me        (1000)    12057 2024-04-05 09:59:24.000000 unitlab-2.1.5/src/unitlab/client.py
--rw-rw-r--   0 me        (1000) me        (1000)    12386 2024-04-05 09:59:30.000000 unitlab-2.1.5/src/unitlab/dataset.py
--rw-rw-r--   0 me        (1000) me        (1000)      950 2024-04-05 12:19:27.000000 unitlab-2.1.5/src/unitlab/exceptions.py
--rw-rw-r--   0 me        (1000) me        (1000)     4513 2024-04-05 12:20:03.000000 unitlab-2.1.5/src/unitlab/main.py
--rw-rw-r--   0 me        (1000) me        (1000)     1852 2024-04-05 12:20:07.000000 unitlab-2.1.5/src/unitlab/utils.py
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2024-04-05 12:20:50.913275 unitlab-2.1.5/src/unitlab.egg-info/
--rw-r--r--   0 me        (1000) me        (1000)      793 2024-04-05 12:20:50.000000 unitlab-2.1.5/src/unitlab.egg-info/PKG-INFO
--rw-rw-r--   0 me        (1000) me        (1000)      411 2024-04-05 12:20:50.000000 unitlab-2.1.5/src/unitlab.egg-info/SOURCES.txt
--rw-rw-r--   0 me        (1000) me        (1000)        1 2024-04-05 12:20:50.000000 unitlab-2.1.5/src/unitlab.egg-info/dependency_links.txt
--rw-rw-r--   0 me        (1000) me        (1000)       45 2024-04-05 12:20:50.000000 unitlab-2.1.5/src/unitlab.egg-info/entry_points.txt
--rw-rw-r--   0 me        (1000) me        (1000)       48 2024-04-05 12:20:50.000000 unitlab-2.1.5/src/unitlab.egg-info/requires.txt
--rw-rw-r--   0 me        (1000) me        (1000)        8 2024-04-05 12:20:50.000000 unitlab-2.1.5/src/unitlab.egg-info/top_level.txt
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2024-04-08 13:29:09.347086 unitlab-2.1.6/
+-rw-rw-r--   0 me        (1000) me        (1000)     1069 2024-02-13 07:39:37.000000 unitlab-2.1.6/LICENSE.md
+-rw-r--r--   0 me        (1000) me        (1000)      793 2024-04-08 13:29:09.347086 unitlab-2.1.6/PKG-INFO
+-rw-rw-r--   0 me        (1000) me        (1000)     1434 2023-09-24 12:59:00.000000 unitlab-2.1.6/README.md
+-rw-rw-r--   0 me        (1000) me        (1000)      106 2024-04-08 13:29:09.347086 unitlab-2.1.6/setup.cfg
+-rw-rw-r--   0 me        (1000) me        (1000)     1092 2024-04-08 13:28:42.000000 unitlab-2.1.6/setup.py
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2024-04-08 13:29:09.347086 unitlab-2.1.6/src/
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2024-04-08 13:29:09.347086 unitlab-2.1.6/src/unitlab/
+-rw-rw-r--   0 me        (1000) me        (1000)      214 2024-04-05 11:53:23.000000 unitlab-2.1.6/src/unitlab/__init__.py
+-rw-rw-r--   0 me        (1000) me        (1000)       29 2024-03-06 15:43:31.000000 unitlab-2.1.6/src/unitlab/__main__.py
+-rw-rw-r--   0 me        (1000) me        (1000)    12065 2024-04-08 12:17:22.000000 unitlab-2.1.6/src/unitlab/client.py
+-rw-rw-r--   0 me        (1000) me        (1000)    12386 2024-04-05 09:59:30.000000 unitlab-2.1.6/src/unitlab/dataset.py
+-rw-rw-r--   0 me        (1000) me        (1000)      950 2024-04-05 12:19:27.000000 unitlab-2.1.6/src/unitlab/exceptions.py
+-rw-rw-r--   0 me        (1000) me        (1000)     4553 2024-04-08 12:17:26.000000 unitlab-2.1.6/src/unitlab/main.py
+-rw-rw-r--   0 me        (1000) me        (1000)     1852 2024-04-05 12:20:07.000000 unitlab-2.1.6/src/unitlab/utils.py
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2024-04-08 13:29:09.347086 unitlab-2.1.6/src/unitlab.egg-info/
+-rw-r--r--   0 me        (1000) me        (1000)      793 2024-04-08 13:29:09.000000 unitlab-2.1.6/src/unitlab.egg-info/PKG-INFO
+-rw-rw-r--   0 me        (1000) me        (1000)      411 2024-04-08 13:29:09.000000 unitlab-2.1.6/src/unitlab.egg-info/SOURCES.txt
+-rw-rw-r--   0 me        (1000) me        (1000)        1 2024-04-08 13:29:09.000000 unitlab-2.1.6/src/unitlab.egg-info/dependency_links.txt
+-rw-rw-r--   0 me        (1000) me        (1000)       45 2024-04-08 13:29:09.000000 unitlab-2.1.6/src/unitlab.egg-info/entry_points.txt
+-rw-rw-r--   0 me        (1000) me        (1000)       48 2024-04-08 13:29:09.000000 unitlab-2.1.6/src/unitlab.egg-info/requires.txt
+-rw-rw-r--   0 me        (1000) me        (1000)        8 2024-04-08 13:29:09.000000 unitlab-2.1.6/src/unitlab.egg-info/top_level.txt
```

### Comparing `unitlab-2.1.5/LICENSE.md` & `unitlab-2.1.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `unitlab-2.1.5/PKG-INFO` & `unitlab-2.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitlab
-Version: 2.1.5
+Version: 2.1.6
 Home-page: https://github.com/teamunitlab/unitlab-sdk
 Author: Unitlab Inc.
 Author-email: team@unitlab.ai
 License: MIT
 Keywords: unitlab-sdk
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `unitlab-2.1.5/README.md` & `unitlab-2.1.6/README.md`

 * *Files identical despite different names*

### Comparing `unitlab-2.1.5/setup.py` & `unitlab-2.1.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="unitlab",
-    version="2.1.5",
+    version="2.1.6",
     license="MIT",
     author="Unitlab Inc.",
     author_email="team@unitlab.ai",
     packages=find_packages("src"),
     include_package_data=True,
     package_data={"static": ["*"], "Potato": ["*.so"]},
     classifiers=[
```

### Comparing `unitlab-2.1.5/src/unitlab/client.py` & `unitlab-2.1.6/src/unitlab/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
 
     def project(self, project_id, pretty=0):
         return self._get(f"/api/sdk/projects/{project_id}/?pretty={pretty}")
 
     def project_members(self, project_id, pretty=0):
         return self._get(f"/api/sdk/projects/{project_id}/members/?pretty={pretty}")
 
-    def upload_data(self, project_id, directory, batch_size=100):
+    def project_upload_data(self, project_id, directory, batch_size=100):
         if not os.path.isdir(directory):
             raise ValueError(f"Directory {directory} does not exist")
 
         files = [
             file
             for files_list in (
                 glob.glob(os.path.join(directory, "") + extension)
@@ -200,15 +200,15 @@
             filename = f"dataset-{dataset_id}.json"
             with open(filename, "wb") as f:
                 for chunk in r.iter_content(chunk_size=1024 * 1024):
                     f.write(chunk)
             logger.info(f"File: {os.path.abspath(filename)}")
             return os.path.abspath(filename)
 
-    def download_dataset_files(self, dataset_id):
+    def dataset_download_files(self, dataset_id):
         response = self._post(
             f"/api/sdk/datasets/{dataset_id}/", data={"download_type": "files"}
         )
         folder = f"dataset-files-{dataset_id}"
         os.makedirs(folder, exist_ok=True)
         dataset_files = [
             dataset_file
```

### Comparing `unitlab-2.1.5/src/unitlab/dataset.py` & `unitlab-2.1.6/src/unitlab/dataset.py`

 * *Files identical despite different names*

### Comparing `unitlab-2.1.5/src/unitlab/exceptions.py` & `unitlab-2.1.6/src/unitlab/exceptions.py`

 * *Files identical despite different names*

### Comparing `unitlab-2.1.5/src/unitlab/main.py` & `unitlab-2.1.6/src/unitlab/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     IMG_SEMANTIC_SEGMENTATION = "img_semantic_segmentation"
     IMG_INSTANCE_SEGMENTATION = "img_instance_segmentation"
     IMG_POLYGON = "img_polygon"
     IMG_LINE = "img_line"
     IMG_POINT = "img_point"
 
 
-@app.command()
+@app.command(help="Configure the credentials")
 def configure(
     api_key: Annotated[str, typer.Option(help="The api-key obtained from unitlab.ai")],
     api_url: Annotated[str, typer.Option()] = "https://api.unitlab.ai",
 ):
     if not validators.url(api_url, simple_host=True):
         raise typer.BadParameter("Invalid api url")
     write_config(api_key=api_key, api_url=api_url)
@@ -72,15 +72,15 @@
 def upload(
     pk: UUID,
     api_key: API_KEY,
     directory: Annotated[
         Path, typer.Option(help="Directory containing the data to be uploaded")
     ],
 ):
-    get_client(api_key).upload_data(str(pk), directory=directory)
+    get_client(api_key).project_upload_data(str(pk), directory=directory)
 
 
 @dataset_app.command(name="list", help="List datasets")
 def dataset_list(api_key: API_KEY):
     print(get_client(api_key).datasets(pretty=1))
 
 
@@ -141,12 +141,12 @@
 ):
     if download_type == DownloadType.annotation:
         if not export_type:
             raise typer.BadParameter(
                 "Export type is required when download type is annotation"
             )
         get_client(api_key).dataset_download(pk, export_type)
-    get_client(api_key).download_dataset_files(pk)
+    get_client(api_key).dataset_download_files(pk)
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `unitlab-2.1.5/src/unitlab/utils.py` & `unitlab-2.1.6/src/unitlab/utils.py`

 * *Files identical despite different names*

### Comparing `unitlab-2.1.5/src/unitlab.egg-info/PKG-INFO` & `unitlab-2.1.6/src/unitlab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitlab
-Version: 2.1.5
+Version: 2.1.6
 Home-page: https://github.com/teamunitlab/unitlab-sdk
 Author: Unitlab Inc.
 Author-email: team@unitlab.ai
 License: MIT
 Keywords: unitlab-sdk
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

