# Comparing `tmp/selenium-network-intercept-0.0.2.tar.gz` & `tmp/selenium-network-intercept-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenium-network-intercept-0.0.2.tar", last modified: Mon Apr  8 17:27:49 2024, max compression
+gzip compressed data, was "selenium-network-intercept-0.0.3.tar", last modified: Mon Apr  8 18:24:31 2024, max compression
```

## Comparing `selenium-network-intercept-0.0.2.tar` & `selenium-network-intercept-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 17:27:49.285391 selenium-network-intercept-0.0.2/
--rw-rw-rw-   0        0        0     1093 2024-04-08 16:39:54.000000 selenium-network-intercept-0.0.2/LICENCE
--rw-rw-rw-   0        0        0     6353 2024-04-08 17:27:49.284392 selenium-network-intercept-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     5944 2024-04-08 17:26:13.000000 selenium-network-intercept-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-08 17:27:49.278392 selenium-network-intercept-0.0.2/selenium_network_intercept/
--rw-rw-rw-   0        0        0       37 2024-04-08 16:34:11.000000 selenium-network-intercept-0.0.2/selenium_network_intercept/__init__.py
--rw-rw-rw-   0        0        0     3747 2024-04-08 17:26:28.000000 selenium-network-intercept-0.0.2/selenium_network_intercept/intercept.py
--rw-rw-rw-   0        0        0     3237 2024-03-04 14:19:54.000000 selenium-network-intercept-0.0.2/selenium_network_intercept/objected.py
--rw-rw-rw-   0        0        0     1807 2024-04-08 17:26:28.000000 selenium-network-intercept-0.0.2/selenium_network_intercept/request.py
--rw-rw-rw-   0        0        0     1580 2024-04-08 17:26:28.000000 selenium-network-intercept-0.0.2/selenium_network_intercept/response.py
-drwxrwxrwx   0        0        0        0 2024-04-08 17:27:49.283391 selenium-network-intercept-0.0.2/selenium_network_intercept.egg-info/
--rw-rw-rw-   0        0        0     6353 2024-04-08 17:27:49.000000 selenium-network-intercept-0.0.2/selenium_network_intercept.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      421 2024-04-08 17:27:49.000000 selenium-network-intercept-0.0.2/selenium_network_intercept.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 17:27:49.000000 selenium-network-intercept-0.0.2/selenium_network_intercept.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2024-04-08 17:27:49.000000 selenium-network-intercept-0.0.2/selenium_network_intercept.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-08 17:27:49.285391 selenium-network-intercept-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      664 2024-04-08 17:27:46.000000 selenium-network-intercept-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:24:31.126279 selenium-network-intercept-0.0.3/
+-rw-rw-rw-   0        0        0     1093 2024-04-08 16:39:54.000000 selenium-network-intercept-0.0.3/LICENCE
+-rw-rw-rw-   0        0        0     6353 2024-04-08 18:24:31.125279 selenium-network-intercept-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5944 2024-04-08 17:26:13.000000 selenium-network-intercept-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-08 18:24:31.118824 selenium-network-intercept-0.0.3/selenium_network_intercept/
+-rw-rw-rw-   0        0        0       37 2024-04-08 16:34:11.000000 selenium-network-intercept-0.0.3/selenium_network_intercept/__init__.py
+-rw-rw-rw-   0        0        0       39 2024-04-08 18:15:43.000000 selenium-network-intercept-0.0.3/selenium_network_intercept/exceptions.py
+-rw-rw-rw-   0        0        0     4446 2024-04-08 18:23:51.000000 selenium-network-intercept-0.0.3/selenium_network_intercept/intercept.py
+-rw-rw-rw-   0        0        0     3237 2024-03-04 14:19:54.000000 selenium-network-intercept-0.0.3/selenium_network_intercept/objected.py
+-rw-rw-rw-   0        0        0     1807 2024-04-08 18:23:16.000000 selenium-network-intercept-0.0.3/selenium_network_intercept/request.py
+-rw-rw-rw-   0        0        0     1580 2024-04-08 18:22:50.000000 selenium-network-intercept-0.0.3/selenium_network_intercept/response.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:24:31.124275 selenium-network-intercept-0.0.3/selenium_network_intercept.egg-info/
+-rw-rw-rw-   0        0        0     6353 2024-04-08 18:24:31.000000 selenium-network-intercept-0.0.3/selenium_network_intercept.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      462 2024-04-08 18:24:31.000000 selenium-network-intercept-0.0.3/selenium_network_intercept.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 18:24:31.000000 selenium-network-intercept-0.0.3/selenium_network_intercept.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-04-08 18:24:31.000000 selenium-network-intercept-0.0.3/selenium_network_intercept.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 18:24:31.126279 selenium-network-intercept-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      664 2024-04-08 18:24:25.000000 selenium-network-intercept-0.0.3/setup.py
```

### Comparing `selenium-network-intercept-0.0.2/LICENCE` & `selenium-network-intercept-0.0.3/LICENCE`

 * *Files identical despite different names*

### Comparing `selenium-network-intercept-0.0.2/PKG-INFO` & `selenium-network-intercept-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium-network-intercept
-Version: 0.0.2
+Version: 0.0.3
 Summary: Interceptador de requisições http não oficial do selenium 4
 Author: Alexandre Mariano
 Author-email: alexandre_mariano@hotmail.com.br
 License: MIT License
 Keywords: selenium,network,intercept,http,requests,selenium network intercept,selenium intercept
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `selenium-network-intercept-0.0.2/README.md` & `selenium-network-intercept-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `selenium-network-intercept-0.0.2/selenium_network_intercept/intercept.py` & `selenium-network-intercept-0.0.3/selenium_network_intercept/intercept.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import time
 import json
+from selenium_network_intercept.exceptions import CapabilityNotFound
 from selenium_network_intercept.response import network_response
 from selenium_network_intercept.request import network_request
 from time import sleep
 from selenium_network_intercept.objected import ObjectIntercepted
 
 
 def  _get_url(params,req_or_res): #falta teste unitario
@@ -31,14 +32,30 @@
     try:
         treated_url = url.split('?')[0]
         return treated_url
     except:
         return url
 
 
+def verify_capabilities(driver):
+    """
+    Verifica se o driver contém a capacidade "performance" para interceptar requisições.
+    """
+    if 'performance' in driver.log_types:
+        return None
+    raise CapabilityNotFound(
+        """O driver não contém a capacidade "performance" para interceptar requisições.
+Verifique a documentação ou tente adicionar em sua instância do webdriver:
+
+from selenium.webdriver import ChromeOptions
+options = ChromeOptions()
+options.set_capability('goog:loggingPrefs', {'performance': 'ALL'})
+driver = webdriver.Chrome(options=options)"""
+    )
+
 def intercept_http(
     driver,
     route,
     delay=5
     ) -> ObjectIntercepted:
     
     """
@@ -54,24 +71,23 @@
     Nota:
         Esta função intercepta solicitações HTTP feitas pela instância fornecida de WebDriver. Ela busca
         solicitações cujas URLs terminam com o sufixo especificado (`url_endswith`). Não sendo necessário enviar 
         informações como query na URL, somente a rota necessária.
         Para cada solicitação interceptada, ela recupera informações relevantes, como o corpo da solicitação, 
         código de status, URL e método HTTP, e as encapsula em uma instância de ObjectIntercepted.
     """
-    initial_time = time.time()
+    verify_capabilities(driver)
     
+    initial_time = time.time()
     logs1 = driver.get_log('performance') 
-    
+
     sleep(delay)
     
     object_intercepted = ObjectIntercepted(route)
-    
     logs2 = driver.get_log('performance')
-    
     logs = logs1 + logs2
     
     
     for log in logs:
         message = json.loads(log.get('message')).get('message')
         params  = json.loads(log.get('message')).get('message').get('params')
         method  = json.loads(log.get('message')).get('message').get('method')
```

### Comparing `selenium-network-intercept-0.0.2/selenium_network_intercept/objected.py` & `selenium-network-intercept-0.0.3/selenium_network_intercept/objected.py`

 * *Files identical despite different names*

### Comparing `selenium-network-intercept-0.0.2/selenium_network_intercept/request.py` & `selenium-network-intercept-0.0.3/selenium_network_intercept/request.py`

 * *Files identical despite different names*

### Comparing `selenium-network-intercept-0.0.2/selenium_network_intercept/response.py` & `selenium-network-intercept-0.0.3/selenium_network_intercept/response.py`

 * *Files identical despite different names*

### Comparing `selenium-network-intercept-0.0.2/selenium_network_intercept.egg-info/PKG-INFO` & `selenium-network-intercept-0.0.3/selenium_network_intercept.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium-network-intercept
-Version: 0.0.2
+Version: 0.0.3
 Summary: Interceptador de requisições http não oficial do selenium 4
 Author: Alexandre Mariano
 Author-email: alexandre_mariano@hotmail.com.br
 License: MIT License
 Keywords: selenium,network,intercept,http,requests,selenium network intercept,selenium intercept
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `selenium-network-intercept-0.0.2/setup.py` & `selenium-network-intercept-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 file = open('README.md', 'r',encoding='utf-8')
 readme = file.read()
 
 
 setup(
     name='selenium-network-intercept',
-    version='0.0.2',
+    version='0.0.3',
     license='MIT License',
     author='Alexandre Mariano',
     long_description=readme,
     long_description_content_type='text/markdown',
     author_email='alexandre_mariano@hotmail.com.br',
     keywords=['selenium', 'network', 'intercept','http','requests','selenium network intercept','selenium intercept'],
     description='Interceptador de requisições http não oficial do selenium 4',
```

