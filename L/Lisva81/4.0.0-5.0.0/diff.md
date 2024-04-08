# Comparing `tmp/Lisva81-4.0.0.tar.gz` & `tmp/Lisva81-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Lisva81-4.0.0.tar", last modified: Sat Apr  6 06:05:13 2024, max compression
+gzip compressed data, was "Lisva81-5.0.0.tar", last modified: Mon Apr  8 01:33:57 2024, max compression
```

## Comparing `Lisva81-4.0.0.tar` & `Lisva81-5.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 06:05:13.696079 Lisva81-4.0.0/
--rw-rw-rw-   0        0        0     1235 2023-04-13 20:26:37.000000 Lisva81-4.0.0/LICENSE
-drwxrwxrwx   0        0        0        0 2024-04-06 06:05:13.649076 Lisva81-4.0.0/Lisva81/
--rw-rw-rw-   0        0        0     7083 2024-04-06 06:00:05.000000 Lisva81-4.0.0/Lisva81/__init__.py
--rw-rw-rw-   0        0        0       75 2024-04-06 06:03:57.000000 Lisva81-4.0.0/Lisva81/version.py
-drwxrwxrwx   0        0        0        0 2024-04-06 06:05:13.686078 Lisva81-4.0.0/Lisva81.egg-info/
--rw-rw-rw-   0        0        0      992 2024-04-06 06:05:12.000000 Lisva81-4.0.0/Lisva81.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2024-04-06 06:05:12.000000 Lisva81-4.0.0/Lisva81.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 06:05:12.000000 Lisva81-4.0.0/Lisva81.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2024-04-06 06:05:12.000000 Lisva81-4.0.0/Lisva81.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-06 06:05:12.000000 Lisva81-4.0.0/Lisva81.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-04-06 06:05:12.000000 Lisva81-4.0.0/Lisva81.egg-info/zip-safe
--rw-rw-rw-   0        0        0      992 2024-04-06 06:05:13.693079 Lisva81-4.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      638 2023-04-25 04:32:36.000000 Lisva81-4.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-06 06:05:13.698079 Lisva81-4.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1605 2024-02-24 05:09:28.000000 Lisva81-4.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 01:33:57.673784 Lisva81-5.0.0/
+-rw-rw-rw-   0        0        0     1235 2023-04-13 20:26:37.000000 Lisva81-5.0.0/LICENSE
+drwxrwxrwx   0        0        0        0 2024-04-08 01:33:57.489774 Lisva81-5.0.0/Lisva81/
+-rw-rw-rw-   0        0        0     8335 2024-04-08 01:32:48.000000 Lisva81-5.0.0/Lisva81/__init__.py
+-rw-rw-rw-   0        0        0       75 2024-04-08 01:32:57.000000 Lisva81-5.0.0/Lisva81/version.py
+drwxrwxrwx   0        0        0        0 2024-04-08 01:33:57.656783 Lisva81-5.0.0/Lisva81.egg-info/
+-rw-rw-rw-   0        0        0      992 2024-04-08 01:33:55.000000 Lisva81-5.0.0/Lisva81.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2024-04-08 01:33:55.000000 Lisva81-5.0.0/Lisva81.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 01:33:55.000000 Lisva81-5.0.0/Lisva81.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-04-08 01:33:55.000000 Lisva81-5.0.0/Lisva81.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-08 01:33:55.000000 Lisva81-5.0.0/Lisva81.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-04-08 01:33:55.000000 Lisva81-5.0.0/Lisva81.egg-info/zip-safe
+-rw-rw-rw-   0        0        0      992 2024-04-08 01:33:57.662783 Lisva81-5.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      638 2023-04-25 04:32:36.000000 Lisva81-5.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-08 01:33:57.674784 Lisva81-5.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1605 2024-02-24 05:09:28.000000 Lisva81-5.0.0/setup.py
```

### Comparing `Lisva81-4.0.0/LICENSE` & `Lisva81-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Lisva81-4.0.0/Lisva81/__init__.py` & `Lisva81-5.0.0/Lisva81/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -44,16 +44,21 @@
 
 def printl(text):
     init()
     print(Fore.GREEN + text,end='\r')
 
 def make_session(type,id):
     session = requests.Session()
+    headers = {"User-Agent":"Mozilla/5.0 (Windows NT 6.1; Win64; x64; rv:109.0) Gecko/20100101 Firefox/115.0","Upgrade-Insecure-Requests":"1"}
     if type=="rv":
         return session
+    elif type=="rme":
+    	host = "https://revmedicaelectronica.sld.cu/index.php/rme"
+    	payload = {"source": "","username": "raydel0307","password": "R@ydel2022*","remember": "1"}
+    	resp = session.post(f"{host}/login/signIn", data=payload, headers=headers)
     elif type=="apye":
         host = "https://apye.esceg.cu/index.php/apye/"
         resp = session.get(host + "login")
         soup = BeautifulSoup(resp.text, "html.parser")
         csrfToken = soup.find("input",attrs={"name":"csrfToken"})['value']
         url_post = host + 'login/signIn'
         payload = {}
@@ -92,20 +97,30 @@
     elif "apye.esceg.cu" in dl:
         value = dl.split("apye/")[1].split("/")
         filename = value[3]
         total_size = int(value[1])
         type = "apye"
         id = value[2]
         url = f"https://apye.esceg.cu/index.php/apye/$$$call$$$/api/file/file-api/download-file?submissionFileId=^&submissionId={value[0]}&stageId=1"
-    else:
+    elif "revmedicaelectronica" in dl:
+        value = dl.split("rme/")[1].split("/")
+        filename = value[3]
+        total_size = int(value[1])
+        type = "rme"
+        id = value[2]
+        url = f"https://revmedicaelectronica.sld.cu/index.php/rme/author/download/{value[0]}/^"
+    elif "nube.uo.edu.cu" in dl:
         url = dl.split("{")[0]+".file"
         filename = dl.split("/")[-1]
         id = dl.split("{")[1].split("}")[0]
         total_size = int(dl.split("}/")[1].split("/")[0])
         type = "uo"
+    else:
+    	printl(Fore.BLUE + 'URL no permitida ... !!!')
+    	return
 
     if not session:
         session = make_session(type,id)
     if session:
         init()
         os.system(cmd)
         printl(Fore.BLUE + 'Sesion Iniciada ... !!!')
@@ -133,14 +148,23 @@
         for v in values:
             url = url.replace("^",v)
             resp = session.get(url,headers=headers,stream=True,verify=False)
             for chunk in resp.iter_content(chunk_size=8192):
                 chunk_por += len(chunk)
                 f.write(chunk)
                 progress(f'{filet} ',chunk_por,total_size)
+    elif "revmedicaelectronica" in dl:
+        values = id.split("-")
+        for v in values:
+            url = url.replace("^",v)
+            resp = session.get(url,headers=headers,stream=True,verify=False)
+            for chunk in resp.iter_content(chunk_size=1024*1024):
+                chunk_por += len(chunk)
+                f.write(chunk)
+                progress(f'{filet} ',chunk_por,total_size)
     elif "api.download.cu" in dl:
         for v in values:
             url = host.replace("*",v)
             resp = session.get(url,headers=headers,stream=True,verify=False)
             for chunk in resp.iter_content(chunk_size=8192):
                 chunk_por += len(chunk)
                 f.write(chunk)
@@ -156,15 +180,15 @@
             i+=1
             if parte==totals:
                 total_size = chunk_por
     f.close()
     if os.path.exists('Lisva81/' + filename):
         os.unlink('Lisva81/' + filename)
     shutil.move(filename,'Lisva81/'+filename)
-    if "revgacetaestudiantil.sld" in dl:
+    if "revgacetaestudiantil.sld" in dl or "revmedicaelectronica" in dl:
         with open('Lisva81/dwnl' + filename, "wb") as filet:
             filet.write(open(f, "rb").read().replace(b"\x89PNG\r\n\x1a\n\x00\x00\x00\rIHDR\x00\x00\x00\x01\x00\x00\x00\x01\x08\x02\x00\x00\x00\x90wS\xde\x00\x00\x00\x0cIDATx\x9cc```\x00\x00\x00\x04\x00\x01\xf6\x178U\x00\x00\x00\x00IEND\xaeB`\x82",b''))
         os.unlink(f)
     os.system(cmd)
     printl('Descarga Finalizada !!! Archivos Guardados en ./Downloads. Envie 0 y luego Enter para salir o pulse solo Enter para continuar')
     state = 'finish'
     a = input()
```

### Comparing `Lisva81-4.0.0/Lisva81.egg-info/PKG-INFO` & `Lisva81-5.0.0/Lisva81.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Lisva81
-Version: 4.0.0
+Version: 5.0.0
 Summary: Python 3 library for short text
 Home-page: https://github.com/fenixinvitado2021/downfree
 Author: RayServer
 Author-email: susej.mabel2009@gmail.com
 License: The Unlicense (Unlicense)
 Keywords: telegram,download,stream,bots
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `Lisva81-4.0.0/PKG-INFO` & `Lisva81-5.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Lisva81
-Version: 4.0.0
+Version: 5.0.0
 Summary: Python 3 library for short text
 Home-page: https://github.com/fenixinvitado2021/downfree
 Author: RayServer
 Author-email: susej.mabel2009@gmail.com
 License: The Unlicense (Unlicense)
 Keywords: telegram,download,stream,bots
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `Lisva81-4.0.0/README.md` & `Lisva81-5.0.0/README.md`

 * *Files identical despite different names*

### Comparing `Lisva81-4.0.0/setup.py` & `Lisva81-5.0.0/setup.py`

 * *Files identical despite different names*

