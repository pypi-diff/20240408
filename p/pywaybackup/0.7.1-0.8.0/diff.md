# Comparing `tmp/pywaybackup-0.7.1.tar.gz` & `tmp/pywaybackup-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywaybackup-0.7.1.tar", last modified: Wed Apr  3 15:04:35 2024, max compression
+gzip compressed data, was "pywaybackup-0.8.0.tar", last modified: Mon Apr  8 14:35:27 2024, max compression
```

## Comparing `pywaybackup-0.7.1.tar` & `pywaybackup-0.8.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 bitdruid  (1000) bitdruid  (1000)        0 2024-04-03 15:04:35.647937 pywaybackup-0.7.1/
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)       98 2024-04-03 10:05:23.000000 pywaybackup-0.7.1/.gitignore
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)     1065 2024-04-03 10:05:23.000000 pywaybackup-0.7.1/LICENSE
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)     4812 2024-04-03 15:04:35.647937 pywaybackup-0.7.1/PKG-INFO
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)     4459 2024-04-03 15:03:18.000000 pywaybackup-0.7.1/README.md
-drwxr-xr-x   0 bitdruid  (1000) bitdruid  (1000)        0 2024-04-03 15:04:35.644604 pywaybackup-0.7.1/dev/
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)      477 2024-04-03 10:05:23.000000 pywaybackup-0.7.1/dev/pip_build.sh
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)      551 2024-04-03 10:05:23.000000 pywaybackup-0.7.1/dev/venv_create.sh
-drwxr-xr-x   0 bitdruid  (1000) bitdruid  (1000)        0 2024-04-03 15:04:35.644604 pywaybackup-0.7.1/pywaybackup/
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)     3899 2024-04-03 15:00:04.000000 pywaybackup-0.7.1/pywaybackup/SnapshotCollection.py
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)     1569 2024-04-03 11:51:34.000000 pywaybackup-0.7.1/pywaybackup/Verbosity.py
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)        0 2024-04-03 10:05:23.000000 pywaybackup-0.7.1/pywaybackup/__init__.py
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)       21 2024-04-03 15:04:18.000000 pywaybackup-0.7.1/pywaybackup/__version__.py
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)    11506 2024-04-03 15:02:23.000000 pywaybackup-0.7.1/pywaybackup/archive.py
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)     2159 2024-04-03 14:08:39.000000 pywaybackup-0.7.1/pywaybackup/arguments.py
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)      872 2024-04-03 13:50:20.000000 pywaybackup-0.7.1/pywaybackup/main.py
-drwxr-xr-x   0 bitdruid  (1000) bitdruid  (1000)        0 2024-04-03 15:04:35.647937 pywaybackup-0.7.1/pywaybackup.egg-info/
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)     4812 2024-04-03 15:04:35.000000 pywaybackup-0.7.1/pywaybackup.egg-info/PKG-INFO
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)      480 2024-04-03 15:04:35.000000 pywaybackup-0.7.1/pywaybackup.egg-info/SOURCES.txt
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)        1 2024-04-03 15:04:35.000000 pywaybackup-0.7.1/pywaybackup.egg-info/dependency_links.txt
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)       52 2024-04-03 15:04:35.000000 pywaybackup-0.7.1/pywaybackup.egg-info/entry_points.txt
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)       30 2024-04-03 15:04:35.000000 pywaybackup-0.7.1/pywaybackup.egg-info/requires.txt
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)       12 2024-04-03 15:04:35.000000 pywaybackup-0.7.1/pywaybackup.egg-info/top_level.txt
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)       53 2024-04-03 10:05:23.000000 pywaybackup-0.7.1/requirements.txt
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)       38 2024-04-03 15:04:35.647937 pywaybackup-0.7.1/setup.cfg
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)     1091 2024-04-03 10:05:23.000000 pywaybackup-0.7.1/setup.py
+drwxr-xr-x   0 bitdruid  (1000) bitdruid  (1000)        0 2024-04-08 14:35:27.913683 pywaybackup-0.8.0/
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)       98 2024-04-03 10:05:23.000000 pywaybackup-0.8.0/.gitignore
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)     1065 2024-04-03 10:05:23.000000 pywaybackup-0.8.0/LICENSE
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)     4925 2024-04-08 14:35:27.913683 pywaybackup-0.8.0/PKG-INFO
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)     4572 2024-04-08 14:34:18.000000 pywaybackup-0.8.0/README.md
+drwxr-xr-x   0 bitdruid  (1000) bitdruid  (1000)        0 2024-04-08 14:35:27.910350 pywaybackup-0.8.0/dev/
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)      477 2024-04-03 10:05:23.000000 pywaybackup-0.8.0/dev/pip_build.sh
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)      551 2024-04-03 10:05:23.000000 pywaybackup-0.8.0/dev/venv_create.sh
+drwxr-xr-x   0 bitdruid  (1000) bitdruid  (1000)        0 2024-04-08 14:35:27.910350 pywaybackup-0.8.0/pywaybackup/
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)     4606 2024-04-08 14:34:18.000000 pywaybackup-0.8.0/pywaybackup/SnapshotCollection.py
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)     1644 2024-04-08 14:34:18.000000 pywaybackup-0.8.0/pywaybackup/Verbosity.py
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)        0 2024-04-03 10:05:23.000000 pywaybackup-0.8.0/pywaybackup/__init__.py
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)       21 2024-04-08 14:34:18.000000 pywaybackup-0.8.0/pywaybackup/__version__.py
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)    11873 2024-04-08 14:34:18.000000 pywaybackup-0.8.0/pywaybackup/archive.py
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)     2290 2024-04-08 14:34:18.000000 pywaybackup-0.8.0/pywaybackup/arguments.py
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)      815 2024-04-08 14:34:18.000000 pywaybackup-0.8.0/pywaybackup/main.py
+drwxr-xr-x   0 bitdruid  (1000) bitdruid  (1000)        0 2024-04-08 14:35:27.913683 pywaybackup-0.8.0/pywaybackup.egg-info/
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)     4925 2024-04-08 14:35:27.000000 pywaybackup-0.8.0/pywaybackup.egg-info/PKG-INFO
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)      480 2024-04-08 14:35:27.000000 pywaybackup-0.8.0/pywaybackup.egg-info/SOURCES.txt
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)        1 2024-04-08 14:35:27.000000 pywaybackup-0.8.0/pywaybackup.egg-info/dependency_links.txt
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)       52 2024-04-08 14:35:27.000000 pywaybackup-0.8.0/pywaybackup.egg-info/entry_points.txt
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)       30 2024-04-08 14:35:27.000000 pywaybackup-0.8.0/pywaybackup.egg-info/requires.txt
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)       12 2024-04-08 14:35:27.000000 pywaybackup-0.8.0/pywaybackup.egg-info/top_level.txt
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)       53 2024-04-08 14:04:38.000000 pywaybackup-0.8.0/requirements.txt
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)       38 2024-04-08 14:35:27.913683 pywaybackup-0.8.0/setup.cfg
+-rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)     1091 2024-04-03 10:05:23.000000 pywaybackup-0.8.0/setup.py
```

### Comparing `pywaybackup-0.7.1/LICENSE` & `pywaybackup-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pywaybackup-0.7.1/PKG-INFO` & `pywaybackup-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywaybackup
-Version: 0.7.1
+Version: 0.8.0
 Summary: Download snapshots from the Wayback Machine
 Home-page: https://github.com/bitdruid/python-wayback-machine-downloader
 Author: bitdruid
 Author-email: bitdruid@outlook.com
 License: MIT
 Keywords: wayback machine internet archive
 Description-Content-Type: text/markdown
@@ -71,18 +71,19 @@
 (year 2019, year+month 201901, year+month+day 20190101, year+month+day+hour 2019010112)
    - `-r RANGE`, `--range RANGE`: Specify the range in years for which to search and download snapshots.
    - `--start`: Timestamp to start searching.
    - `--end`: Timestamp to end searching.
 
 #### Additional
 
+- `--csv`: Save a csv file with the list of snapshots inside the output folder.
 - `--no-redirect`: Do not follow redirects of snapshots. Archive.org sometimes redirects to a different snapshot for several reasons. Downloading redirects may lead to timestamp-folders which contain some files with a different timestamp. This does not matter if you only want to download the latest version (`-c`).
 - `--verbosity [LEVEL]`: Set the verbosity: json (print json response), progress (show progress bar) or standard (default).
 - `--retry [RETRY_FAILED]`: Retry failed downloads. You can specify the number of retry attempts as an integer.
-- `--worker [AMOUNT]`: The number of worker to use for downloading (simultaneous downloads). Default is 1. Beware: Using too many worker will lead into refused connections from the Wayback Machine. Duration about 1.5 minutes.
+- `--worker [AMOUNT]`: The number of worker to use for downloading (simultaneous downloads). Default is 1. A safe spot is about 10 workers. Beware: Using too many worker will lead into refused connections from the Wayback Machine. Duration about 1.5 minutes.
 
 ### Examples
 
 Download latest snapshot of all files:<br>
 `waybackup -u http://example.com -c`
 
 Download latest snapshot of all files with retries:<br>
```

### Comparing `pywaybackup-0.7.1/README.md` & `pywaybackup-0.8.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -59,18 +59,19 @@
 (year 2019, year+month 201901, year+month+day 20190101, year+month+day+hour 2019010112)
    - `-r RANGE`, `--range RANGE`: Specify the range in years for which to search and download snapshots.
    - `--start`: Timestamp to start searching.
    - `--end`: Timestamp to end searching.
 
 #### Additional
 
+- `--csv`: Save a csv file with the list of snapshots inside the output folder.
 - `--no-redirect`: Do not follow redirects of snapshots. Archive.org sometimes redirects to a different snapshot for several reasons. Downloading redirects may lead to timestamp-folders which contain some files with a different timestamp. This does not matter if you only want to download the latest version (`-c`).
 - `--verbosity [LEVEL]`: Set the verbosity: json (print json response), progress (show progress bar) or standard (default).
 - `--retry [RETRY_FAILED]`: Retry failed downloads. You can specify the number of retry attempts as an integer.
-- `--worker [AMOUNT]`: The number of worker to use for downloading (simultaneous downloads). Default is 1. Beware: Using too many worker will lead into refused connections from the Wayback Machine. Duration about 1.5 minutes.
+- `--worker [AMOUNT]`: The number of worker to use for downloading (simultaneous downloads). Default is 1. A safe spot is about 10 workers. Beware: Using too many worker will lead into refused connections from the Wayback Machine. Duration about 1.5 minutes.
 
 ### Examples
 
 Download latest snapshot of all files:<br>
 `waybackup -u http://example.com -c`
 
 Download latest snapshot of all files with retries:<br>
```

### Comparing `pywaybackup-0.7.1/dev/venv_create.sh` & `pywaybackup-0.8.0/dev/venv_create.sh`

 * *Files identical despite different names*

### Comparing `pywaybackup-0.7.1/pywaybackup/SnapshotCollection.py` & `pywaybackup-0.8.0/pywaybackup/SnapshotCollection.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,60 @@
 from urllib.parse import urlparse
 import os
 
 class SnapshotCollection:
 
-    CDX_LIST = []
     SNAPSHOT_COLLECTION = []
     MODE_CURRENT = 0
 
     @classmethod
-    def create_list_full(cls, cdxResult):
-        cls.CDX_LIST = sorted([{"timestamp": snapshot[0], "url": snapshot[1], "status": snapshot[2], "mimetype": snapshot[3], "digest": snapshot[4]} for i, snapshot in enumerate(cdxResult.json()[1:])], key=lambda k: k['timestamp'], reverse=True)
-
-    @classmethod
-    def create_list_current(cls):
-        cls.MODE_CURRENT = 1
-        cdxResult_list_filtered = []
-        url_set = set()
-        for snapshot in cls.CDX_LIST:
-            if snapshot["url"] not in url_set:
-                cdxResult_list_filtered.append(snapshot)
-                url_set.add(snapshot["url"])
-        cls.CDX_LIST = cdxResult_list_filtered
+    def create_list(cls, cdxResult, mode):
+        """
+        Create the snapshot collection list from a cdx result.
 
+        - mode `full`: All snapshots are included.
+        - mode `current`: Only the latest snapshot of each file is included.
+        """
+        # creates a list of dictionaries for each snapshot entry
+        cls.SNAPSHOT_COLLECTION = sorted([{"timestamp": snapshot[0], "digest": snapshot[1], "mimetype": snapshot[2], "status": snapshot[3], "url": snapshot[4]} for snapshot in cdxResult.json()[1:]], key=lambda k: k['timestamp'], reverse=True)
+        if mode == "current": 
+            cls.MODE_CURRENT = 1
+            cdxResult_list_filtered = []
+            url_set = set()
+            # filters the list to only include the latest snapshot of each file
+            for snapshot in cls.SNAPSHOT_COLLECTION:
+                if snapshot["url"] not in url_set:
+                    cdxResult_list_filtered.append(snapshot)
+                    url_set.add(snapshot["url"])
+            cls.SNAPSHOT_COLLECTION = cdxResult_list_filtered
+        # writes the index for each snapshot entry
+        cls.SNAPSHOT_COLLECTION = [{"id": idx, **entry} for idx, entry in enumerate(cls.SNAPSHOT_COLLECTION)]
+    
     @classmethod
     def count_list(cls):
-        return len(cls.CDX_LIST)
+        return len(cls.SNAPSHOT_COLLECTION)
 
     @classmethod
     def create_collection(cls):
-        for cdx_entry in cls.CDX_LIST:
+        new_collection = []
+        for cdx_entry in cls.SNAPSHOT_COLLECTION:
             timestamp, url = cdx_entry["timestamp"], cdx_entry["url"]
             url_archive = f"http://web.archive.org/web/{timestamp}{cls._url_get_filetype(url)}/{url}"
             collection_entry = {
-                "id": len(cls.SNAPSHOT_COLLECTION),
+                "id": cls.SNAPSHOT_COLLECTION.index(cdx_entry),
                 "timestamp": timestamp,
                 "url_archive": url_archive,
                 "url_origin": url,
-                "file": False,
-                "redirect": False,
-                "response": False
+                "redirect_url": False,
+                "redirect_timestamp": False,
+                "response": False,
+                "file": False
             }
-            cls.SNAPSHOT_COLLECTION.append(collection_entry)
+            new_collection.append(collection_entry)
+        cls.SNAPSHOT_COLLECTION = new_collection
     
     @classmethod
     def snapshot_entry_create_output(cls, collection_entry: dict, output: str) -> str:
         """
         Create the output path for a snapshot entry of the collection according to the mode.
 
         Input:
@@ -56,15 +66,15 @@
         """
         timestamp, url = collection_entry["timestamp"], collection_entry["url_origin"]
         domain, subdir, filename = cls._url_split(url)
         if cls.MODE_CURRENT:
             download_dir = os.path.join(output, domain, subdir)
         else:
             download_dir = os.path.join(output, domain, timestamp, subdir)
-        download_file = os.path.join(download_dir, filename)
+        download_file = os.path.abspath(os.path.join(download_dir, filename))
         return download_file
 
     @classmethod
     def snapshot_entry_modify(cls, collection_entry: dict, key: str, value: str):
         """
         Modify a key-value pair in a snapshot entry of the collection (dict).
```

### Comparing `pywaybackup-0.7.1/pywaybackup/Verbosity.py` & `pywaybackup-0.8.0/pywaybackup/Verbosity.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import tqdm
 import json
 from pywaybackup.SnapshotCollection import SnapshotCollection as sc
 
 class Verbosity:
 
-    snapshots = None
     mode = None
     args = None
     pbar = None
 
     @classmethod
     def open(cls, args: list):
         cls.args = args
@@ -18,32 +17,32 @@
             cls.mode = "json"
         else:
             cls.mode = "standard"
 
     @classmethod
     def close(cls):
         if cls.mode == "progress":
-            cls.pbar.close()
+            if cls.pbar is not None: cls.pbar.close()
         if cls.mode == "progress" or cls.mode == "standard":
-            successed = len([snapshot for snapshot in sc.SNAPSHOT_COLLECTION if snapshot["file"]])
-            failed = len([snapshot for snapshot in sc.SNAPSHOT_COLLECTION if not snapshot["file"]])
+            successed = len([snapshot for snapshot in sc.SNAPSHOT_COLLECTION if "file" in snapshot and snapshot["file"]])
+            failed = len([snapshot for snapshot in sc.SNAPSHOT_COLLECTION if "file" in snapshot and not snapshot["file"]])
             print(f"\nFiles downloaded: {successed}")
             print(f"Files missing: {failed}")
             print("")
         if cls.mode == "json":
             print(json.dumps(sc.SNAPSHOT_COLLECTION, indent=4, sort_keys=True))
 
     @classmethod
     def write(cls, message: str = None, progress: int = None):
         if cls.mode == "progress":
             if progress == 0:
                 print("")
                 maxval = sc.count_list()
                 cls.pbar = tqdm.tqdm(total=maxval, desc="Downloading", unit=" snapshot", ascii="░▒█")
-            elif progress == 1:
+            elif cls.pbar is not None and progress == 1:
                 cls.pbar.update(1)
                 cls.pbar.refresh()
         elif cls.mode == "json":
             pass
         else:
             if message:
                 print(message)
```

### Comparing `pywaybackup-0.7.1/pywaybackup/archive.py` & `pywaybackup-0.8.0/pywaybackup/archive.py`

 * *Files 14% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
 def print_list():
     v.write("")
     count = sc.count_list()
     if count == 0:
         v.write("\nNo snapshots found")
     else:
-        __import__('pprint').pprint(sc.CDX_LIST)
+        __import__('pprint').pprint(sc.SNAPSHOT_COLLECTION)
         v.write(f"\n-----> {count} snapshots listed")
 
 
 
 
 
 # create filelist
@@ -91,18 +91,17 @@
         query_range = ""
         if not range:
             if start: query_range = query_range + f"&from={start}"
             if end: query_range = query_range + f"&to={end}"
         else: 
             query_range = "&from=" + str(datetime.now().year - range)
         cdx_url = f"*.{url}/*" if not explicit else f"{url}"
-        cdxQuery = f"https://web.archive.org/cdx/search/xd?output=json&url={cdx_url}{query_range}&fl=timestamp,original,statuscode,mimetype,digest&filter!=statuscode:200"
+        cdxQuery = f"https://web.archive.org/cdx/search/xd?output=json&url={cdx_url}{query_range}&fl=timestamp,digest,mimetype,statuscode,original&filter!=statuscode:200"
         cdxResult = requests.get(cdxQuery)
-        sc.create_list_full(cdxResult)
-        sc.create_list_current() if mode == "current" else None
+        sc.create_list(cdxResult, mode)
         v.write(f"\n-----> {sc.count_list()} snapshots found")
     except requests.exceptions.ConnectionError as e:
         v.write(f"\n-----> ERROR: could not query snapshots:\n{e}"); exit()
 
 
 
 
@@ -191,15 +190,14 @@
                         response_status = response.status
                         location = response.getheader("Location")
                         if location:
                             status_message = f"{status_message}\n" + \
                                 f"           -> URL: {location}"
                             location = urljoin(download_url, location)
                             download_url = location
-                            sc.snapshot_entry_modify(snapshot_entry, "redirect", True)
                             sc.snapshot_entry_modify(snapshot_entry, "redirect_timestamp", sc.url_get_timestamp(location))
                             sc.snapshot_entry_modify(snapshot_entry, "redirect_url", location)
                         else:
                             break
             if response_status == 200:
                 sc.snapshot_entry_modify(snapshot_entry, "file", sc.snapshot_entry_create_output(snapshot_entry, output))
                 download_file = snapshot_entry["file"]
@@ -252,8 +250,22 @@
 }
 def parse_response_code(response_code: int):
     """
     Parse the response code of the Wayback Machine and return a human-readable message.
     """
     if response_code in RESPONSE_CODE_DICT:
         return RESPONSE_CODE_DICT[response_code]
-    return "Unknown response code"
+    return "Unknown response code"
+
+def save_csv(output: str):
+    """
+    Write a CSV file with the list of snapshots.
+    """
+    import csv
+    if sc.count_list() > 0:
+        v.write("\nSaving CSV file...")
+        os.makedirs(os.path.abspath(output), exist_ok=True)
+        with open(os.path.join(output, "waybackup.csv"), mode='w') as file:
+            row = csv.DictWriter(file, sc.SNAPSHOT_COLLECTION[0].keys())
+            row.writeheader()
+            for snapshot in sc.SNAPSHOT_COLLECTION:
+                row.writerow(snapshot)
```

### Comparing `pywaybackup-0.7.1/pywaybackup/arguments.py` & `pywaybackup-0.8.0/pywaybackup/arguments.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     optional.add_argument('-e', '--explicit', action='store_true', help='Search only for the explicit given url')
     optional.add_argument('-o', '--output', type=str, help='Output folder')
     optional.add_argument('-r', '--range', type=int, help='Range in years to search')
     optional.add_argument('--start', type=int, help='Start timestamp format: YYYYMMDDhhmmss')
     optional.add_argument('--end', type=int, help='End timestamp format: YYYYMMDDhhmmss')
 
     special = parser.add_argument_group('special')
+    special.add_argument('--csv', action='store_true', help='Save a csv file with the list of snapshots inside the output folder')
     special.add_argument('--no-redirect', action='store_true', help='Do not follow redirects by archive.org')
     special.add_argument('--verbosity', type=str, default="standard", choices=["standard", "progress", "json"], help='Verbosity level')
     special.add_argument('--retry', type=int, default=0, metavar="X-TIMES", help='Retry failed downloads (opt tries as int, else infinite)')
     special.add_argument('--worker', type=int, default=1, metavar="AMOUNT", help='Number of worker (simultaneous downloads)')
 
     args = parser.parse_args()
```

### Comparing `pywaybackup-0.7.1/pywaybackup.egg-info/PKG-INFO` & `pywaybackup-0.8.0/pywaybackup.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywaybackup
-Version: 0.7.1
+Version: 0.8.0
 Summary: Download snapshots from the Wayback Machine
 Home-page: https://github.com/bitdruid/python-wayback-machine-downloader
 Author: bitdruid
 Author-email: bitdruid@outlook.com
 License: MIT
 Keywords: wayback machine internet archive
 Description-Content-Type: text/markdown
@@ -71,18 +71,19 @@
 (year 2019, year+month 201901, year+month+day 20190101, year+month+day+hour 2019010112)
    - `-r RANGE`, `--range RANGE`: Specify the range in years for which to search and download snapshots.
    - `--start`: Timestamp to start searching.
    - `--end`: Timestamp to end searching.
 
 #### Additional
 
+- `--csv`: Save a csv file with the list of snapshots inside the output folder.
 - `--no-redirect`: Do not follow redirects of snapshots. Archive.org sometimes redirects to a different snapshot for several reasons. Downloading redirects may lead to timestamp-folders which contain some files with a different timestamp. This does not matter if you only want to download the latest version (`-c`).
 - `--verbosity [LEVEL]`: Set the verbosity: json (print json response), progress (show progress bar) or standard (default).
 - `--retry [RETRY_FAILED]`: Retry failed downloads. You can specify the number of retry attempts as an integer.
-- `--worker [AMOUNT]`: The number of worker to use for downloading (simultaneous downloads). Default is 1. Beware: Using too many worker will lead into refused connections from the Wayback Machine. Duration about 1.5 minutes.
+- `--worker [AMOUNT]`: The number of worker to use for downloading (simultaneous downloads). Default is 1. A safe spot is about 10 workers. Beware: Using too many worker will lead into refused connections from the Wayback Machine. Duration about 1.5 minutes.
 
 ### Examples
 
 Download latest snapshot of all files:<br>
 `waybackup -u http://example.com -c`
 
 Download latest snapshot of all files with retries:<br>
```

### Comparing `pywaybackup-0.7.1/setup.py` & `pywaybackup-0.8.0/setup.py`

 * *Files identical despite different names*

