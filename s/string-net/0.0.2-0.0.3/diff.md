# Comparing `tmp/string_net-0.0.2.tar.gz` & `tmp/string_net-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "string_net-0.0.2.tar", last modified: Thu Apr  4 15:14:39 2024, max compression
+gzip compressed data, was "string_net-0.0.3.tar", last modified: Mon Apr  8 07:34:37 2024, max compression
```

## Comparing `string_net-0.0.2.tar` & `string_net-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 leonardonossa   (501) staff       (20)        0 2024-04-04 15:14:39.107301 string_net-0.0.2/
--rw-r--r--   0 leonardonossa   (501) staff       (20)     1071 2024-04-03 18:50:00.000000 string_net-0.0.2/LICENSE
--rw-r--r--   0 leonardonossa   (501) staff       (20)     1472 2024-04-04 15:14:39.107360 string_net-0.0.2/PKG-INFO
--rw-r--r--   0 leonardonossa   (501) staff       (20)      977 2024-04-03 21:25:08.000000 string_net-0.0.2/README.rst
--rw-r--r--   0 leonardonossa   (501) staff       (20)      750 2024-04-04 15:14:39.107593 string_net-0.0.2/setup.cfg
--rw-r--r--   0 leonardonossa   (501) staff       (20)       72 2024-04-03 20:18:58.000000 string_net-0.0.2/setup.py
-drwxr-xr-x   0 leonardonossa   (501) staff       (20)        0 2024-04-04 15:14:39.105590 string_net-0.0.2/src/
-drwxr-xr-x   0 leonardonossa   (501) staff       (20)        0 2024-04-04 15:14:39.106566 string_net-0.0.2/src/string_net/
--rw-r--r--   0 leonardonossa   (501) staff       (20)       76 2024-04-03 21:07:39.000000 string_net-0.0.2/src/string_net/__init__.py
--rw-r--r--   0 leonardonossa   (501) staff       (20)     1747 2024-04-04 15:10:05.000000 string_net-0.0.2/src/string_net/string_net.py
-drwxr-xr-x   0 leonardonossa   (501) staff       (20)        0 2024-04-04 15:14:39.107207 string_net-0.0.2/src/string_net.egg-info/
--rw-r--r--   0 leonardonossa   (501) staff       (20)     1472 2024-04-04 15:14:39.000000 string_net-0.0.2/src/string_net.egg-info/PKG-INFO
--rw-r--r--   0 leonardonossa   (501) staff       (20)      282 2024-04-04 15:14:39.000000 string_net-0.0.2/src/string_net.egg-info/SOURCES.txt
--rw-r--r--   0 leonardonossa   (501) staff       (20)        1 2024-04-04 15:14:39.000000 string_net-0.0.2/src/string_net.egg-info/dependency_links.txt
--rw-r--r--   0 leonardonossa   (501) staff       (20)       46 2024-04-04 15:14:39.000000 string_net-0.0.2/src/string_net.egg-info/requires.txt
--rw-r--r--   0 leonardonossa   (501) staff       (20)       11 2024-04-04 15:14:39.000000 string_net-0.0.2/src/string_net.egg-info/top_level.txt
+drwxr-xr-x   0 leonardonossa   (501) staff       (20)        0 2024-04-08 07:34:37.414787 string_net-0.0.3/
+-rw-r--r--   0 leonardonossa   (501) staff       (20)     1071 2024-04-03 18:50:00.000000 string_net-0.0.3/LICENSE
+-rw-r--r--   0 leonardonossa   (501) staff       (20)     1472 2024-04-08 07:34:37.414860 string_net-0.0.3/PKG-INFO
+-rw-r--r--   0 leonardonossa   (501) staff       (20)      977 2024-04-03 21:25:08.000000 string_net-0.0.3/README.rst
+-rw-r--r--   0 leonardonossa   (501) staff       (20)      765 2024-04-08 07:34:37.415093 string_net-0.0.3/setup.cfg
+-rw-r--r--   0 leonardonossa   (501) staff       (20)       72 2024-04-03 20:18:58.000000 string_net-0.0.3/setup.py
+drwxr-xr-x   0 leonardonossa   (501) staff       (20)        0 2024-04-08 07:34:37.413002 string_net-0.0.3/src/
+drwxr-xr-x   0 leonardonossa   (501) staff       (20)        0 2024-04-08 07:34:37.414026 string_net-0.0.3/src/string_net/
+-rw-r--r--   0 leonardonossa   (501) staff       (20)       90 2024-04-08 07:08:01.000000 string_net-0.0.3/src/string_net/__init__.py
+-rw-r--r--   0 leonardonossa   (501) staff       (20)     2394 2024-04-08 06:59:38.000000 string_net-0.0.3/src/string_net/string_net.py
+drwxr-xr-x   0 leonardonossa   (501) staff       (20)        0 2024-04-08 07:34:37.414689 string_net-0.0.3/src/string_net.egg-info/
+-rw-r--r--   0 leonardonossa   (501) staff       (20)     1472 2024-04-08 07:34:37.000000 string_net-0.0.3/src/string_net.egg-info/PKG-INFO
+-rw-r--r--   0 leonardonossa   (501) staff       (20)      282 2024-04-08 07:34:37.000000 string_net-0.0.3/src/string_net.egg-info/SOURCES.txt
+-rw-r--r--   0 leonardonossa   (501) staff       (20)        1 2024-04-08 07:34:37.000000 string_net-0.0.3/src/string_net.egg-info/dependency_links.txt
+-rw-r--r--   0 leonardonossa   (501) staff       (20)       46 2024-04-08 07:34:37.000000 string_net-0.0.3/src/string_net.egg-info/requires.txt
+-rw-r--r--   0 leonardonossa   (501) staff       (20)       11 2024-04-08 07:34:37.000000 string_net-0.0.3/src/string_net.egg-info/top_level.txt
```

### Comparing `string_net-0.0.2/LICENSE` & `string_net-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `string_net-0.0.2/PKG-INFO` & `string_net-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: string_net
-Version: 0.0.2
+Version: 0.0.3
 Summary: Observe the ppi network from STRING db.
 Home-page: https://github.com/LeonardoNossa/STRING-package.git
 Author: Leonardo Nossa
 License: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Operating System :: POSIX
```

### Comparing `string_net-0.0.2/README.rst` & `string_net-0.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `string_net-0.0.2/setup.cfg` & `string_net-0.0.3/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = string_net
-version = 0.0.2
+version = 0.0.3
 description = Observe the ppi network from STRING db.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/LeonardoNossa/STRING-package.git
 author = Leonardo Nossa
 author_mail = leonardo.nossa@icloud.com
 license = LICENSE
@@ -20,14 +20,15 @@
 package_dir = 
 	=src
 python_requires = >=3.11
 install requires = 
 	requests >= 2.31.0
 	Pillow >= 10.3.0
 	Pandas >= 1.5.3
+	Bs4 >= 4.12.3
 
 [options.extras_require]
 dev = 
 	twine >= 5.0.0
 	flake8 >= 7.0.0
 	tox >= 4.14.2
```

### Comparing `string_net-0.0.2/src/string_net/string_net.py` & `string_net-0.0.3/src/string_net/string_net.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,65 +1,88 @@
 import requests
 from PIL import Image
 from io import BytesIO
 import os
 import pandas as pd
 import io
+from bs4 import BeautifulSoup
+import warnings
 
 species = 9606
 
 
 def net(protein_name):
 
     STRING_network = "https://string-db.org/api/image/network"
 
     parameters = {
         "identifiers": protein_name,
         "species": species,
-        "networ k_flavor": "physical interactions"
+        "network_flavor": "physical interactions"
     }
 
     http_response_1 = requests.get(STRING_network, params=parameters)
 
     if http_response_1.status_code == 200:
 
         network = Image.open(BytesIO(http_response_1.content))
         new_network = Image.new("RGB", network.size, "white")
         new_network.paste(network, (0, 0), network)
-        
+
         directory = 'img_cache'
         if not os.path.exists(directory):
             os.makedirs(directory)
 
         img_path = os.path.join(directory, f"{protein_name}_network_image.png")
         new_network.save(img_path)
     else:
         print(f"Error > Status code: {http_response_1.status_code}")
 
 
 def get_partners(protein_name):
+
     STRING_partner = "https://string-db.org/api/tsv/interaction_partners"
 
     parameters_partners = {
         "identifiers": protein_name,
         "species": species
     }
 
     http_response_2 = requests.get(STRING_partner, params=parameters_partners)
 
     if http_response_2.status_code == 200:
         df = pd.read_csv(io.StringIO(http_response_2.text), sep='\t')
-        print(df)  
+        print(df)
 
         directory_csv = 'interaction_partner_data'
         if not os.path.exists(directory_csv):
             os.makedirs(directory_csv)
-        
-        csv_file_path = os.path.join(directory_csv, f"{protein_name}_interaction_partners.csv")
+
+        csv_file_path = os.path.join(directory_csv, f"{protein_name}.csv")
         df.to_csv(csv_file_path, index=False)
 
     else:
         print(f"Error > Status code: {http_response_2.status_code}")
 
+def info(protein_name):
+
+    UNIPROT_info = f"https://www.uniprot.org/uniprot/{protein_name}.xml"
+
+    http_response_3 = requests.get(UNIPROT_info)
+
+    if http_response_3.status_code == 200:
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore")
+            info = BeautifulSoup(http_response_3.content, "html5lib")
+        tag = info.find("comment", type = "function")
+    
+        if tag is not None:
+            return tag.text.strip()
+        else:
+            return f"The description of {protein_name} is not avaible."
+    
+    else:
+        print(f"Error > Status code: {http_response_3.status_code}")
+
```

### Comparing `string_net-0.0.2/src/string_net.egg-info/PKG-INFO` & `string_net-0.0.3/src/string_net.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: string-net
-Version: 0.0.2
+Version: 0.0.3
 Summary: Observe the ppi network from STRING db.
 Home-page: https://github.com/LeonardoNossa/STRING-package.git
 Author: Leonardo Nossa
 License: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Operating System :: POSIX
```

