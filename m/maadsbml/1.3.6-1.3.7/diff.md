# Comparing `tmp/maadsbml-1.3.6.tar.gz` & `tmp/maadsbml-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maadsbml-1.3.6.tar", last modified: Tue Apr  2 21:55:39 2024, max compression
+gzip compressed data, was "maadsbml-1.3.7.tar", last modified: Mon Apr  8 14:45:13 2024, max compression
```

## Comparing `maadsbml-1.3.6.tar` & `maadsbml-1.3.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 21:55:39.011206 maadsbml-1.3.6/
--rw-rw-rw-   0        0        0     1067 2021-04-28 21:31:09.000000 maadsbml-1.3.6/LICENSE.txt
--rw-rw-rw-   0        0        0       65 2021-01-25 23:03:44.000000 maadsbml-1.3.6/MANIFEST.in
--rw-rw-rw-   0        0        0     8814 2024-04-02 21:55:39.010196 maadsbml-1.3.6/PKG-INFO
--rw-rw-rw-   0        0        0     8277 2024-04-01 04:08:00.000000 maadsbml-1.3.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 21:55:38.979146 maadsbml-1.3.6/maadsbml/
--rw-rw-rw-   0        0        0      204 2024-03-29 17:59:02.000000 maadsbml-1.3.6/maadsbml/__init__.py
--rw-rw-rw-   0        0        0     8841 2020-10-18 21:34:32.000000 maadsbml-1.3.6/maadsbml/balancedata.py
--rw-rw-rw-   0        0        0     5395 2020-06-27 20:48:48.000000 maadsbml-1.3.6/maadsbml/callmas.py
--rw-rw-rw-   0        0        0     7453 2024-04-02 21:55:05.000000 maadsbml-1.3.6/maadsbml/sendfiles.py
-drwxrwxrwx   0        0        0        0 2024-04-02 21:55:39.007140 maadsbml-1.3.6/maadsbml.egg-info/
--rw-rw-rw-   0        0        0     8814 2024-04-02 21:55:38.000000 maadsbml-1.3.6/maadsbml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      317 2024-04-02 21:55:38.000000 maadsbml-1.3.6/maadsbml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 21:55:38.000000 maadsbml-1.3.6/maadsbml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      115 2024-04-02 21:55:38.000000 maadsbml-1.3.6/maadsbml.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-02 21:55:38.000000 maadsbml-1.3.6/maadsbml.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      122 2021-02-05 16:13:30.000000 maadsbml-1.3.6/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-04-02 21:55:39.011206 maadsbml-1.3.6/setup.cfg
--rw-rw-rw-   0        0        0     1026 2024-04-02 21:55:19.000000 maadsbml-1.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 14:45:13.101379 maadsbml-1.3.7/
+-rw-rw-rw-   0        0        0     1067 2021-04-28 21:31:09.000000 maadsbml-1.3.7/LICENSE.txt
+-rw-rw-rw-   0        0        0       65 2021-01-25 23:03:44.000000 maadsbml-1.3.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     8825 2024-04-08 14:45:13.100170 maadsbml-1.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0     8277 2024-04-01 04:08:00.000000 maadsbml-1.3.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-08 14:45:13.069717 maadsbml-1.3.7/maadsbml/
+-rw-rw-rw-   0        0        0      204 2024-03-29 17:59:02.000000 maadsbml-1.3.7/maadsbml/__init__.py
+-rw-rw-rw-   0        0        0     8841 2020-10-18 21:34:32.000000 maadsbml-1.3.7/maadsbml/balancedata.py
+-rw-rw-rw-   0        0        0     5395 2020-06-27 20:48:48.000000 maadsbml-1.3.7/maadsbml/callmas.py
+-rw-rw-rw-   0        0        0     7793 2024-04-08 14:44:16.000000 maadsbml-1.3.7/maadsbml/sendfiles.py
+drwxrwxrwx   0        0        0        0 2024-04-08 14:45:13.098197 maadsbml-1.3.7/maadsbml.egg-info/
+-rw-rw-rw-   0        0        0     8825 2024-04-08 14:45:12.000000 maadsbml-1.3.7/maadsbml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2024-04-08 14:45:12.000000 maadsbml-1.3.7/maadsbml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 14:45:12.000000 maadsbml-1.3.7/maadsbml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      115 2024-04-08 14:45:12.000000 maadsbml-1.3.7/maadsbml.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-08 14:45:12.000000 maadsbml-1.3.7/maadsbml.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      122 2021-02-05 16:13:30.000000 maadsbml-1.3.7/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 14:45:13.101379 maadsbml-1.3.7/setup.cfg
+-rw-rw-rw-   0        0        0     1037 2024-04-08 14:40:47.000000 maadsbml-1.3.7/setup.py
```

### Comparing `maadsbml-1.3.6/LICENSE.txt` & `maadsbml-1.3.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `maadsbml-1.3.6/PKG-INFO` & `maadsbml-1.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: maadsbml
-Version: 1.3.6
-Summary: Multi-Agent Accelerator for Data Science (MAADS) Batch AutoML
+Version: 1.3.7
+Summary: Multi-Agent Accelerator for Data Science (MAADS) Batch AutoML (MAADSBML)
 Home-page: https://github.com/smaurice101/acnsmauricedsmas
 Author: Sebastian Maurice
 Author-email: sebastian.maurice@otics.ca
 License: MIT License
 Keywords: multi-agent, data science, batch automl, optimization, prescriptive analytics, machine learning, automl,auto-ml,artificial intelligence,predictive analytics,advanced analytics
 Description-Content-Type: text/markdown
 License-File: license.txt
```

### Comparing `maadsbml-1.3.6/README.md` & `maadsbml-1.3.7/README.md`

 * *Files identical despite different names*

### Comparing `maadsbml-1.3.6/maadsbml/balancedata.py` & `maadsbml-1.3.7/maadsbml/balancedata.py`

 * *Files identical despite different names*

### Comparing `maadsbml-1.3.6/maadsbml/callmas.py` & `maadsbml-1.3.7/maadsbml/callmas.py`

 * *Files identical despite different names*

### Comparing `maadsbml-1.3.6/maadsbml/sendfiles.py` & `maadsbml-1.3.7/maadsbml/sendfiles.py`

 * *Files 14% similar despite different names*

```diff
@@ -106,14 +106,30 @@
       async with ClientSession() as session:
         html = await fetch(session,message)
         await session.close()
         return html
     except Exception as e:
      pass   
 
+def genpkey(username,filename):
+     pkey = ""
+     chars_to_remove= [" ", "(", ")","%","$","&","#","+","=","\\","@",".","/",":","*","?","\"","|","<",">"]
+     
+     if username != "" and filename != "":
+         sc = set(chars_to_remove)
+         for i in sc:
+           filename = filename.replace(i, '_')
+
+     pkey = username + "_" + filename
+
+     return pkey
+
+#pkey=genpkey('admin','aesopowerdemand.csv')
+#print(pkey)
+    
 def hypertraining(host,port,filename,dependentvariable,removeoutliers=0,hasseasonality=0,summer='6,7,8',winter='11,12,1,2',shoulder='3,4,5,9,10',trainingpercentage=70,shuffle=0,deepanalysis=0,username='admin',timeout=1200,company='otics',password='123',email='support@otics.ca',usereverseproxy=0,microserviceid='',maadstoken='123',mode=0):
 
 # curl "http://localhost:5595?hypertraining=1&mode=0&username=admin&company=otics&email=support@otics.ca&filename=aesopowerdemand.csv&removeoutliers=0&
 #hasseasonality=0&dependentvariable=AESO_Power_Demand&summer=6,7,8&winter=11,12,1,2&shoulder=3,4,5,9,10&trainingpercentage=70&shuffle=0&deepanalysis=0"
 #maads.hypertraining(maadstoken,host,port,filename,dependentvariable,username='admin',mode=0,timeout=180,company='otics',removeoutliers=0,hasseasonality=0,summer='6,7,8',winter='11,12,1,2',shoulder='3,4,5,9,10',trainingpercentage=70,shuffle=0,deepanalysis=0,password='123',email='support@otics.ca',usereverseproxy=0,microserviceid='')
 
     if host=='' or port=='' or filename=='' or dependentvariable == '':
@@ -132,15 +148,16 @@
       loop = asyncio.get_event_loop()
       val=loop.run_until_complete(tcp_echo_clienttrain(value, loop,host,port,microserviceid,timeout))
     except IOError as e: 
       if e.errno == errno.EPIPE: 
         pass
 
     if val == None:
-       val="INFO: Broken pipe exception was caught - this may happen due to network issues or low algorithm accuracy.  The system did finish - check the 'exception' folder for your algorithm JSON, and check PDFREPORTS folder for your pdf. The broken pipe may be beacause you selected seasonality and some of the algorithms' accuracy are very low.  You should turn off seasonality or set the months with low accuracy to -1." 
+       pkey=genpkey(username,filename)
+       val="{\"AlgoKey\":\"" + pkey + "\", \"BrokenPipe\":\"Broken pipe exception was caught - this may happen due to network issues. The system will finish - use the AlgoKey and check the 'exception' folder for your algorithm JSON, and check PDFREPORTS folder for your pdf.\"}" 
        return val
     
   #  loop.close()
     return val
 
 def algodescription(host,port,pkey,timeout=300,usereverseproxy=0,microserviceid=''):
     if host=='' or port=='' or pkey=='':
```

### Comparing `maadsbml-1.3.6/maadsbml.egg-info/PKG-INFO` & `maadsbml-1.3.7/maadsbml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: maadsbml
-Version: 1.3.6
-Summary: Multi-Agent Accelerator for Data Science (MAADS) Batch AutoML
+Version: 1.3.7
+Summary: Multi-Agent Accelerator for Data Science (MAADS) Batch AutoML (MAADSBML)
 Home-page: https://github.com/smaurice101/acnsmauricedsmas
 Author: Sebastian Maurice
 Author-email: sebastian.maurice@otics.ca
 License: MIT License
 Keywords: multi-agent, data science, batch automl, optimization, prescriptive analytics, machine learning, automl,auto-ml,artificial intelligence,predictive analytics,advanced analytics
 Description-Content-Type: text/markdown
 License-File: license.txt
```

### Comparing `maadsbml-1.3.6/setup.py` & `maadsbml-1.3.7/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 	
 
 with open("requirements.txt","r") as f:
     required = f.read().splitlines()
     
 setuptools.setup(
     name='maadsbml',
-    version='1.3.6',
-    description='Multi-Agent Accelerator for Data Science (MAADS) Batch AutoML',
+    version='1.3.7',
+    description='Multi-Agent Accelerator for Data Science (MAADS) Batch AutoML (MAADSBML)',
     license='MIT License',
     packages=['maadsbml'],
     author='Sebastian Maurice',
     author_email='sebastian.maurice@otics.ca',
     keywords=['multi-agent, data science, batch automl, optimization, prescriptive analytics, machine learning, automl,auto-ml,artificial intelligence', 'predictive analytics', 'advanced analytics'],
     long_description=long_description,
     install_requires=required,
```

