# Comparing `tmp/kfish-99.0.202404061955-py3-none-any.whl.zip` & `tmp/kfish-99.0.202404080617-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 8021 bytes, number of entries: 6
--rw-r--r--  2.0 unx    12858 b- defN 24-Apr-06 19:49 kfish/__init__.py
--rw-r--r--  2.0 unx    11358 b- defN 24-Apr-06 19:55 kfish-99.0.202404061955.dist-info/LICENSE
--rw-r--r--  2.0 unx      302 b- defN 24-Apr-06 19:55 kfish-99.0.202404061955.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-06 19:55 kfish-99.0.202404061955.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 24-Apr-06 19:55 kfish-99.0.202404061955.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      510 b- defN 24-Apr-06 19:55 kfish-99.0.202404061955.dist-info/RECORD
-6 files, 25126 bytes uncompressed, 7091 bytes compressed:  71.8%
+Zip file size: 8067 bytes, number of entries: 6
+-rw-r--r--  2.0 unx    13060 b- defN 24-Apr-08 06:09 kfish/__init__.py
+-rw-r--r--  2.0 unx    11358 b- defN 24-Apr-08 06:17 kfish-99.0.202404080617.dist-info/LICENSE
+-rw-r--r--  2.0 unx      302 b- defN 24-Apr-08 06:17 kfish-99.0.202404080617.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-08 06:17 kfish-99.0.202404080617.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 24-Apr-08 06:17 kfish-99.0.202404080617.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      510 b- defN 24-Apr-08 06:17 kfish-99.0.202404080617.dist-info/RECORD
+6 files, 25328 bytes uncompressed, 7137 bytes compressed:  71.8%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: kfish/__init__.py
 Comment: 
 
-Filename: kfish-99.0.202404061955.dist-info/LICENSE
+Filename: kfish-99.0.202404080617.dist-info/LICENSE
 Comment: 
 
-Filename: kfish-99.0.202404061955.dist-info/METADATA
+Filename: kfish-99.0.202404080617.dist-info/METADATA
 Comment: 
 
-Filename: kfish-99.0.202404061955.dist-info/WHEEL
+Filename: kfish-99.0.202404080617.dist-info/WHEEL
 Comment: 
 
-Filename: kfish-99.0.202404061955.dist-info/top_level.txt
+Filename: kfish-99.0.202404080617.dist-info/top_level.txt
 Comment: 
 
-Filename: kfish-99.0.202404061955.dist-info/RECORD
+Filename: kfish-99.0.202404080617.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kfish/__init__.py

```diff
@@ -100,15 +100,19 @@
         else:
             virtual_media_url = results['Status']['VirtualMedia']['@odata.id']
         request = Request(f'{self.baseurl}{virtual_media_url}', headers=self.headers)
         results = json.loads(urlopen(request).read())
         if 'Oem' in results:
             odata = results['Oem']['Supermicro']['VirtualMediaConfig']['@odata.id']
         else:
-            for member in results['Members']:
+            member_list = results['Members']
+            if not member_list:
+                print(f"Error: VirtualMedia Member list in {self.baseurl}{virtual_media_url} is empty")
+                sys.exit(1)
+            for member in member_list:
                 odata = member['@odata.id']
                 if odata.endswith('CD') or odata.endswith('Cd') or odata.endswith('2'):
                     break
         ret_data = f'{self.baseurl}{odata}'
         if self.debug:
             print(f"ISO URL is {ret_data}")
         return ret_data
```

## Comparing `kfish-99.0.202404061955.dist-info/LICENSE` & `kfish-99.0.202404080617.dist-info/LICENSE`

 * *Files identical despite different names*

